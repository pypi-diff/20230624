# Comparing `tmp/avocado-framework-98.0.tar.gz` & `tmp/avocado-framework-99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocado-framework-98.0.tar", last modified: Thu Jul 14 20:53:43 2022, max compression
+gzip compressed data, was "avocado-framework-99.0.tar", last modified: Thu Nov 10 19:12:41 2022, max compression
```

## Comparing `avocado-framework-98.0.tar` & `avocado-framework-99.0.tar`

### file list

```diff
@@ -1,877 +1,887 @@
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.981576 avocado-framework-98.0/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    18542 2016-04-28 15:01:56.000000 avocado-framework-98.0/LICENSE
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      195 2021-11-01 18:09:57.000000 avocado-framework-98.0/MANIFEST.in
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2883 2022-05-13 17:48:04.000000 avocado-framework-98.0/Makefile
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    11627 2022-07-14 20:53:43.981576 avocado-framework-98.0/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10679 2022-05-13 17:48:04.000000 avocado-framework-98.0/README
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10679 2022-05-13 17:48:04.000000 avocado-framework-98.0/README.rst
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        5 2022-07-14 20:50:57.000000 avocado-framework-98.0/VERSION
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.867576 avocado-framework-98.0/avocado/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1174 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      150 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/__main__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.870576 avocado-framework-98.0/avocado/core/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9039 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4018 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/app.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12144 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/data_dir.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5250 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/decorators.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.871576 avocado-framework-98.0/avocado/core/dependencies/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-05-13 17:48:04.000000 avocado-framework-98.0/avocado/core/dependencies/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.871576 avocado-framework-98.0/avocado/core/dependencies/requirements/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-05-13 17:48:04.000000 avocado-framework-98.0/avocado/core/dependencies/requirements/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.871576 avocado-framework-98.0/avocado/core/dependencies/requirements/cache/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      356 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/dependencies/requirements/cache/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.871576 avocado-framework-98.0/avocado/core/dependencies/requirements/cache/backends/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-05-13 17:48:04.000000 avocado-framework-98.0/avocado/core/dependencies/requirements/cache/backends/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10799 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/dependencies/requirements/cache/backends/sqlite.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4125 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/dispatcher.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1720 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/enabled_extension_manager.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4318 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/exceptions.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1644 2022-05-13 17:48:04.000000 avocado-framework-98.0/avocado/core/exit_codes.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7637 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/extension_manager.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    25414 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/job.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      895 2021-03-04 22:57:12.000000 avocado-framework-98.0/avocado/core/job_id.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5959 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/jobdata.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    24151 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/loader.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)     2934 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/main.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    15697 2022-07-14 20:25:14.000000 avocado-framework-98.0/avocado/core/messages.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.872576 avocado-framework-98.0/avocado/core/nrunner/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-05-13 17:48:04.000000 avocado-framework-98.0/avocado/core/nrunner/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      504 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/nrunner/__main__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10238 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/nrunner/app.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      981 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/nrunner/config.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    19098 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/nrunner/runnable.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2439 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/nrunner/runner.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7498 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/nrunner/task.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    24592 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/output.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9317 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/parameters.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9207 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/parser.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2005 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/parser_common_args.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    15429 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/plugin_interfaces.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1149 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/references.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8592 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/resolver.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3801 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/result.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9830 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/runner.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.872576 avocado-framework-98.0/avocado/core/safeloader/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      798 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/safeloader/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    16391 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/safeloader/core.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2483 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/safeloader/docstring.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10240 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/safeloader/imported.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6260 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/safeloader/module.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      775 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/safeloader/utils.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    26268 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/settings.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1216 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/settings_dispatcher.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.873576 avocado-framework-98.0/avocado/core/spawners/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-98.0/avocado/core/spawners/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3051 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/spawners/common.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       44 2021-03-04 22:57:12.000000 avocado-framework-98.0/avocado/core/spawners/exceptions.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2104 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/spawners/mock.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.873576 avocado-framework-98.0/avocado/core/status/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-98.0/avocado/core/status/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6589 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/status/repo.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1779 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/status/server.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      826 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/status/utils.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      442 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/streams.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12215 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/suite.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9971 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/sysinfo.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5877 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/tags.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6360 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/tapparser.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.873576 avocado-framework-98.0/avocado/core/task/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-98.0/avocado/core/task/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10438 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/task/runtime.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12844 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/task/statemachine.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    31367 2022-07-14 20:25:14.000000 avocado-framework-98.0/avocado/core/test.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3881 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/test_id.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1237 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/teststatus.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    17680 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/tree.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.874576 avocado-framework-98.0/avocado/core/utils/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-05-13 17:48:04.000000 avocado-framework-98.0/avocado/core/utils/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2211 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/utils/loader.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8312 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/utils/messages.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1446 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/utils/path.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      812 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/utils/version.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12651 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/varianter.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      813 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/core/version.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.861576 avocado-framework-98.0/avocado/etc/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.861576 avocado-framework-98.0/avocado/etc/avocado/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.861576 avocado-framework-98.0/avocado/etc/avocado/scripts/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.861576 avocado-framework-98.0/avocado/etc/avocado/scripts/job/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.874576 avocado-framework-98.0/avocado/etc/avocado/scripts/job/post.d/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      244 2019-07-19 21:00:45.000000 avocado-framework-98.0/avocado/etc/avocado/scripts/job/post.d/README
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.874576 avocado-framework-98.0/avocado/etc/avocado/scripts/job/pre.d/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      243 2019-07-19 21:00:45.000000 avocado-framework-98.0/avocado/etc/avocado/scripts/job/pre.d/README
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.874576 avocado-framework-98.0/avocado/etc/avocado/sysinfo/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      157 2020-09-09 00:55:30.000000 avocado-framework-98.0/avocado/etc/avocado/sysinfo/commands
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      294 2019-07-19 21:00:45.000000 avocado-framework-98.0/avocado/etc/avocado/sysinfo/files
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       23 2019-07-19 21:00:45.000000 avocado-framework-98.0/avocado/etc/avocado/sysinfo/profilers
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.875576 avocado-framework-98.0/avocado/libexec/
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      634 2019-07-19 21:00:45.000000 avocado-framework-98.0/avocado/libexec/avocado-bash-utils
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)       53 2019-07-19 21:00:45.000000 avocado-framework-98.0/avocado/libexec/avocado_debug
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)       53 2019-07-19 21:00:45.000000 avocado-framework-98.0/avocado/libexec/avocado_error
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)       52 2019-07-19 21:00:45.000000 avocado-framework-98.0/avocado/libexec/avocado_info
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)       52 2019-07-19 21:00:45.000000 avocado-framework-98.0/avocado/libexec/avocado_warn
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.878576 avocado-framework-98.0/avocado/plugins/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      545 2022-01-26 18:48:01.000000 avocado-framework-98.0/avocado/plugins/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1638 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/archive.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    22329 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/assets.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4249 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/beaker_result.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1242 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/bystatus.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4076 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/config.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1691 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/dependency.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3496 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/dict_variants.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    15736 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/diff.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    14480 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/distro.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1206 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/exec_path.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5370 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/human.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10294 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/jobs.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3559 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/jobscripts.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4875 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/journal.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5201 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/json_variants.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5063 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/jsonresult.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8227 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/list.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3984 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/plugins.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3029 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/replay.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4262 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/resolvers.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9299 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/run.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12081 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/runner_nrunner.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.878576 avocado-framework-98.0/avocado/plugins/runners/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-05-13 17:48:04.000000 avocado-framework-98.0/avocado/plugins/runners/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4007 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/runners/asset.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6219 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/runners/avocado_instrumented.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      903 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/runners/dry_run.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6780 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/runners/exec_test.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      834 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/runners/noop.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5845 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/runners/package.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5729 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/runners/python_unittest.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7241 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/runners/sysinfo.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2495 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/runners/tap.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.879576 avocado-framework-98.0/avocado/plugins/spawners/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-98.0/avocado/plugins/spawners/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    14571 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/spawners/podman.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3573 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/spawners/process.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6762 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/sysinfo.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6886 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/tap.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4377 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/testlogs.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1449 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/teststmpdir.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6202 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/variants.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6119 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/vmimage.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10037 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/plugins/xunit.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.883576 avocado-framework-98.0/avocado/utils/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      560 2022-01-26 18:48:01.000000 avocado-framework-98.0/avocado/utils/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3201 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/ar.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9118 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/archive.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    23777 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/asset.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10725 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/astring.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      976 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/aurl.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3798 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/build.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8062 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/cloudinit.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    16231 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/cpu.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2056 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/crypto.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2598 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/data_factory.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10155 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/data_structures.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5663 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/datadrainer.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2938 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/debug.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10836 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/diff_validator.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7621 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/disk.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    15985 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/distro.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5978 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/dmesg.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6671 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/download.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      795 2021-11-01 18:09:57.000000 avocado-framework-98.0/avocado/utils/exit_codes.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.884576 avocado-framework-98.0/avocado/utils/external/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      545 2022-01-26 18:48:01.000000 avocado-framework-98.0/avocado/utils/external/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12579 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/external/gdbmi_parser.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    27100 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/external/spark.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2999 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/file_utils.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3261 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/filelock.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    26030 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/gdb.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5351 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/genio.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6707 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/git.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    13854 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/iso9660.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7240 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/kernel.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1900 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/linux.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8024 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/linux_modules.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    25520 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/lv_utils.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    14904 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/memory.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    11228 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/multipath.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.884576 avocado-framework-98.0/avocado/utils/network/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-05-13 17:48:04.000000 avocado-framework-98.0/avocado/utils/network/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      406 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/network/common.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       90 2021-02-11 22:50:38.000000 avocado-framework-98.0/avocado/utils/network/exceptions.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4388 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/network/hosts.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    21769 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/network/interfaces.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5630 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/network/ports.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4178 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/output.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    11470 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/partition.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7550 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/path.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12641 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/pci.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    18321 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/pmem.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5964 2022-07-14 20:25:14.000000 avocado-framework-98.0/avocado/utils/podman.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    43647 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/process.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4726 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/script.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    27439 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/service.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.885576 avocado-framework-98.0/avocado/utils/software_manager/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-05-13 17:48:04.000000 avocado-framework-98.0/avocado/utils/software_manager/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.885576 avocado-framework-98.0/avocado/utils/software_manager/backends/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-98.0/avocado/utils/software_manager/backends/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9421 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/backends/apt.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1323 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/backends/base.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      943 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/backends/dnf.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3751 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/backends/dpkg.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10093 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/backends/rpm.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9874 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/backends/yum.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5986 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/backends/zypper.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2768 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/distro_packages.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2978 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/inspector.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5073 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/main.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2677 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/software_manager/manager.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5381 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/softwareraid.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9182 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/ssh.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3513 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/stacktrace.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    11756 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/sysinfo.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    21991 2022-07-11 13:32:25.000000 avocado-framework-98.0/avocado/utils/vmimage.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1065 2022-05-13 17:48:04.000000 avocado-framework-98.0/avocado/utils/wait.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.886576 avocado-framework-98.0/avocado_framework.egg-info/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    11627 2022-07-14 20:53:43.000000 avocado-framework-98.0/avocado_framework.egg-info/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    31325 2022-07-14 20:53:43.000000 avocado-framework-98.0/avocado_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2022-07-14 20:53:43.000000 avocado-framework-98.0/avocado_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4426 2022-07-14 20:53:43.000000 avocado-framework-98.0/avocado_framework.egg-info/entry_points.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2022-07-14 13:07:39.000000 avocado-framework-98.0/avocado_framework.egg-info/not-zip-safe
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       11 2022-07-14 20:53:43.000000 avocado-framework-98.0/avocado_framework.egg-info/requires.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        8 2022-07-14 20:53:43.000000 avocado-framework-98.0/avocado_framework.egg-info/top_level.txt
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.863576 avocado-framework-98.0/examples/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.861576 avocado-framework-98.0/examples/apis/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.886576 avocado-framework-98.0/examples/apis/utils/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      603 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/apis/utils/ssh.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.887576 avocado-framework-98.0/examples/gdb-prerun-scripts/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      174 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/gdb-prerun-scripts/README
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       42 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/gdb-prerun-scripts/pass-sigusr1
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.887576 avocado-framework-98.0/examples/hint-files/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       85 2021-02-11 22:50:38.000000 avocado-framework-98.0/examples/hint-files/.avocado.hint.example
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      463 2021-02-11 22:50:38.000000 avocado-framework-98.0/examples/hint-files/README.rst
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.889576 avocado-framework-98.0/examples/jobs/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      286 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/jobs/README.rst
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)     1052 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/custom_exec_test.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      195 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/failjob.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      675 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/multiple_suites_from_config.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      466 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/passjob.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      358 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/passjob_cit_varianter.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      708 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/passjob_custom.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      331 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/passjob_html.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      377 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/passjob_html_browser.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      494 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/passjob_with_test.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      369 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/sleepjob_dict_varianter.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      369 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/sleepjob_json_varianter.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      370 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/sleepjob_yaml_to_mux.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      785 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/jobs/unix_status_server.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.862576 avocado-framework-98.0/examples/nrunner/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.862576 avocado-framework-98.0/examples/nrunner/recipes/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.891576 avocado-framework-98.0/examples/nrunner/recipes/runnables/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      121 2022-05-13 17:48:04.000000 avocado-framework-98.0/examples/nrunner/recipes/runnables/asset.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       69 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/nrunner/recipes/runnables/exec_test_echo_no_newline.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      117 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/nrunner/recipes/runnables/exec_test_sh_echo_env_var.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       58 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/nrunner/recipes/runnables/exec_test_sleep_3.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       17 2021-02-11 22:50:38.000000 avocado-framework-98.0/examples/nrunner/recipes/runnables/noop.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       66 2022-05-13 17:48:04.000000 avocado-framework-98.0/examples/nrunner/recipes/runnables/package_check_foo.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       99 2022-05-13 17:48:04.000000 avocado-framework-98.0/examples/nrunner/recipes/runnables/python_unittest.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      274 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/nrunner/recipes/runnables/sysinfo.json
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.862576 avocado-framework-98.0/examples/nrunner/recipes/tasks/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.891576 avocado-framework-98.0/examples/nrunner/recipes/tasks/exec-status/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      112 2021-02-11 22:50:38.000000 avocado-framework-98.0/examples/nrunner/recipes/tasks/exec-status/1-uname-result.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      145 2021-02-11 22:50:38.000000 avocado-framework-98.0/examples/nrunner/recipes/tasks/exec-status/2-dd-result.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      114 2021-02-11 22:50:38.000000 avocado-framework-98.0/examples/nrunner/recipes/tasks/exec-status/3-sleep-result.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      111 2021-02-11 22:50:38.000000 avocado-framework-98.0/examples/nrunner/recipes/tasks/exec-status/4-sleep-long-result.json
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.892576 avocado-framework-98.0/examples/nrunner/recipes/tasks/exec-test/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       82 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/nrunner/recipes/tasks/exec-test/1-uname.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       92 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/nrunner/recipes/tasks/exec-test/2-echo.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       84 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/nrunner/recipes/tasks/exec-test/3-sleep.json
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.892576 avocado-framework-98.0/examples/nrunner/recipes/tasks/unittest-result/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      111 2021-02-11 22:50:38.000000 avocado-framework-98.0/examples/nrunner/recipes/tasks/unittest-result/1-unittest-testcase-localhost.json
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.892576 avocado-framework-98.0/examples/nrunner/runners/
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      543 2022-05-13 17:48:04.000000 avocado-framework-98.0/examples/nrunner/runners/avocado-runner-foo
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.892576 avocado-framework-98.0/examples/plugins/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      411 2016-10-06 13:45:36.000000 avocado-framework-98.0/examples/plugins/README.rst
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.862576 avocado-framework-98.0/examples/plugins/cli-cmd/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.892576 avocado-framework-98.0/examples/plugins/cli-cmd/hello/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      266 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/cli-cmd/hello/hello.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      321 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/cli-cmd/hello/setup.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.892576 avocado-framework-98.0/examples/plugins/cli-cmd/hello_option/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      592 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/cli-cmd/hello_option/hello_option.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      368 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/cli-cmd/hello_option/setup.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.893576 avocado-framework-98.0/examples/plugins/cli-cmd/hello_parser/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      710 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/cli-cmd/hello_parser/hello_parser.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      368 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/cli-cmd/hello_parser/setup.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.893576 avocado-framework-98.0/examples/plugins/cli-cmd/hello_priority/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      359 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/cli-cmd/hello_priority/hello_priority.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      363 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/cli-cmd/hello_priority/setup.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.862576 avocado-framework-98.0/examples/plugins/job-pre-post/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.893576 avocado-framework-98.0/examples/plugins/job-pre-post/mail/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2273 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/job-pre-post/mail/avocado_job_mail.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      511 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/job-pre-post/mail/setup.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.894576 avocado-framework-98.0/examples/plugins/job-pre-post/sleep/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      835 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/job-pre-post/sleep/avocado_job_sleep.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      502 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/job-pre-post/sleep/setup.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.894576 avocado-framework-98.0/examples/plugins/tests/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      733 2022-05-13 17:48:04.000000 avocado-framework-98.0/examples/plugins/tests/README.rst
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.894576 avocado-framework-98.0/examples/plugins/tests/magic/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.894576 avocado-framework-98.0/examples/plugins/tests/magic/avocado_magic/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-98.0/examples/plugins/tests/magic/avocado_magic/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1730 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/tests/magic/avocado_magic/resolver.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1037 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/tests/magic/avocado_magic/runner.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      728 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/plugins/tests/magic/setup.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.862576 avocado-framework-98.0/examples/testplans/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.894576 avocado-framework-98.0/examples/testplans/release/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1855 2022-07-14 20:35:15.000000 avocado-framework-98.0/examples/testplans/release/pre.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2054 2022-07-14 20:35:15.000000 avocado-framework-98.0/examples/testplans/release/release.json
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.902576 avocado-framework-98.0/examples/tests/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.907576 avocado-framework-98.0/examples/tests/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1015 2022-07-14 13:13:22.000000 avocado-framework-98.0/examples/tests/__pycache__/assert.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1048 2022-07-14 13:13:22.000000 avocado-framework-98.0/examples/tests/__pycache__/cancel_on_exception.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      853 2022-07-14 13:13:33.000000 avocado-framework-98.0/examples/tests/__pycache__/cancelonsetup.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      599 2022-07-14 13:14:21.000000 avocado-framework-98.0/examples/tests/__pycache__/canceltest.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      714 2022-07-14 13:15:32.000000 avocado-framework-98.0/examples/tests/__pycache__/cit_parameters.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      838 2022-07-14 13:13:19.000000 avocado-framework-98.0/examples/tests/__pycache__/doublefail.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      648 2022-07-14 13:13:02.000000 avocado-framework-98.0/examples/tests/__pycache__/errortest.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      986 2022-07-14 13:13:20.000000 avocado-framework-98.0/examples/tests/__pycache__/fail_on_exception.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      649 2022-07-14 13:08:08.000000 avocado-framework-98.0/examples/tests/__pycache__/failtest.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      707 2022-07-14 13:13:18.000000 avocado-framework-98.0/examples/tests/__pycache__/failtest_with_warning.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      831 2022-07-14 13:12:59.000000 avocado-framework-98.0/examples/tests/__pycache__/gendata.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1119 2022-07-14 13:13:23.000000 avocado-framework-98.0/examples/tests/__pycache__/logging_streams.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      622 2022-07-14 13:15:44.000000 avocado-framework-98.0/examples/tests/__pycache__/params.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      605 2022-07-14 13:08:08.000000 avocado-framework-98.0/examples/tests/__pycache__/passtest.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      794 2022-07-14 13:13:11.000000 avocado-framework-98.0/examples/tests/__pycache__/phases.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      774 2022-07-14 13:12:07.000000 avocado-framework-98.0/examples/tests/__pycache__/sleeptest.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      803 2022-07-14 13:12:25.000000 avocado-framework-98.0/examples/tests/__pycache__/sleeptest_async.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      858 2022-07-14 13:13:23.000000 avocado-framework-98.0/examples/tests/__pycache__/timeouttest.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      679 2022-07-14 13:13:19.000000 avocado-framework-98.0/examples/tests/__pycache__/uncaught_exception.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      624 2022-07-14 13:13:02.000000 avocado-framework-98.0/examples/tests/__pycache__/warntest.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      699 2022-07-14 13:12:58.000000 avocado-framework-98.0/examples/tests/__pycache__/whiteboard.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      236 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/tests/abort.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      344 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/assert.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2055 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/assets.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.907576 avocado-framework-98.0/examples/tests/assets.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5223 2019-07-23 15:43:52.000000 avocado-framework-98.0/examples/tests/assets.py.data/gnu_hello_signer.gpg
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1036 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/cabort.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.907576 avocado-framework-98.0/examples/tests/cabort.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       50 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/cabort.py.data/abort.c
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      583 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/cancel_on_exception.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      869 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/cancel_test.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      352 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/cancelonsetup.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      210 2021-03-04 22:57:12.000000 avocado-framework-98.0/examples/tests/canceltest.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      363 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/cit_parameters.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      166 2022-05-13 17:48:04.000000 avocado-framework-98.0/examples/tests/custom_env_variable.sh
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.907576 avocado-framework-98.0/examples/tests/custom_env_variable.sh.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      138 2022-05-13 17:48:04.000000 avocado-framework-98.0/examples/tests/custom_env_variable.sh.data/variants.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      914 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/datadir.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.907576 avocado-framework-98.0/examples/tests/datadir.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/datadir.py.data/datadir.c
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      422 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/doublefail.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      661 2019-07-23 15:43:52.000000 avocado-framework-98.0/examples/tests/env_variables.sh
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.907576 avocado-framework-98.0/examples/tests/env_variables.sh.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      138 2018-02-12 01:59:15.000000 avocado-framework-98.0/examples/tests/env_variables.sh.data/env_variables.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      274 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/errortest.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      519 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/errortest_nasty.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      565 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/errortest_nasty2.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      541 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/errortest_nasty3.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      655 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/fail_on_exception.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      277 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/failtest.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)       17 2016-10-06 13:45:36.000000 avocado-framework-98.0/examples/tests/failtest.sh
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      331 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/failtest_ugly.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      321 2022-07-14 20:25:14.000000 avocado-framework-98.0/examples/tests/failtest_with_warning.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    11698 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/gdbtest.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.908576 avocado-framework-98.0/examples/tests/gdbtest.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      589 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/gdbtest.py.data/return99.c
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       80 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/gdbtest.py.data/segfault.c
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      450 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/gendata.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1339 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/linuxbuild.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.908576 avocado-framework-98.0/examples/tests/linuxbuild.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      150 2020-02-19 20:37:17.000000 avocado-framework-98.0/examples/tests/linuxbuild.py.data/linuxbuild.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1007 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/logging_streams.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1483 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/modify_variable.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.908576 avocado-framework-98.0/examples/tests/modify_variable.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      129 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/modify_variable.py.data/print_variable.c
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      769 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/multiple_tests.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2503 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/multiplextest.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.908576 avocado-framework-98.0/examples/tests/multiplextest.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1699 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/multiplextest.py.data/multiplextest.yaml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.908576 avocado-framework-98.0/examples/tests/output_check.sh.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2017-08-24 03:23:42.000000 avocado-framework-98.0/examples/tests/output_check.sh.data/stderr.expected
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       14 2017-08-24 03:23:42.000000 avocado-framework-98.0/examples/tests/output_check.sh.data/stdout.expected
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      275 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/params.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      226 2022-06-09 19:17:14.000000 avocado-framework-98.0/examples/tests/passtest.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)       16 2016-10-06 13:45:36.000000 avocado-framework-98.0/examples/tests/passtest.sh
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      265 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/tests/passtest_with_requirement.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      327 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/phases.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      499 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/property.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1486 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/raise.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.909576 avocado-framework-98.0/examples/tests/raise.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      649 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/raise.py.data/raise.c
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      292 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/raise.py.data/raise.yaml
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      340 2016-06-01 19:09:56.000000 avocado-framework-98.0/examples/tests/simplewarning.sh
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1039 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/skip_conditional.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      863 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/sleeptenmin.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.909576 avocado-framework-98.0/examples/tests/sleeptenmin.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      394 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/sleeptenmin.py.data/sleeptenmin.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      411 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/sleeptest.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.909576 avocado-framework-98.0/examples/tests/sleeptest.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      493 2021-03-04 22:57:12.000000 avocado-framework-98.0/examples/tests/sleeptest.py.data/sleeptest.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      118 2020-07-21 15:22:36.000000 avocado-framework-98.0/examples/tests/sleeptest.py.data/sleeptest.yaml
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      115 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/tests/sleeptest.sh
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.909576 avocado-framework-98.0/examples/tests/sleeptest.sh.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      118 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/tests/sleeptest.sh.data/sleeptest.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      434 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/sleeptest_async.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1451 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/synctest.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.910576 avocado-framework-98.0/examples/tests/synctest.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2017-11-27 16:06:12.000000 avocado-framework-98.0/examples/tests/synctest.py.data/stderr.expected
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       39 2017-11-27 16:06:06.000000 avocado-framework-98.0/examples/tests/synctest.py.data/stdout.expected
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1666 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/synctest.py.data/synctest.tar.bz2
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      265 2016-04-28 15:01:56.000000 avocado-framework-98.0/examples/tests/synctest.py.data/synctest.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2142 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/test_env.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      486 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/timeouttest.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      301 2021-11-01 18:09:57.000000 avocado-framework-98.0/examples/tests/uncaught_exception.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      249 2021-03-04 22:57:12.000000 avocado-framework-98.0/examples/tests/warntest.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      356 2022-07-11 13:32:25.000000 avocado-framework-98.0/examples/tests/whiteboard.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.910576 avocado-framework-98.0/examples/varianter_cit/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      380 2021-02-11 22:50:38.000000 avocado-framework-98.0/examples/varianter_cit/params.cit
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      224 2021-02-11 22:50:38.000000 avocado-framework-98.0/examples/varianter_cit/test_params.cit
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.910576 avocado-framework-98.0/examples/varianter_pict/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      132 2019-07-19 21:00:45.000000 avocado-framework-98.0/examples/varianter_pict/params.pict
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.911576 avocado-framework-98.0/examples/yaml_to_mux/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      330 2019-07-19 21:00:45.000000 avocado-framework-98.0/examples/yaml_to_mux/complex.yaml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.911576 avocado-framework-98.0/examples/yaml_to_mux/hw/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      344 2019-07-19 21:00:45.000000 avocado-framework-98.0/examples/yaml_to_mux/hw/hw.yaml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.911576 avocado-framework-98.0/examples/yaml_to_mux/os/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      298 2019-07-19 21:00:45.000000 avocado-framework-98.0/examples/yaml_to_mux/os/linux.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      111 2019-07-19 21:00:45.000000 avocado-framework-98.0/examples/yaml_to_mux/os/windows.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       80 2019-07-19 21:00:45.000000 avocado-framework-98.0/examples/yaml_to_mux/simple.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      108 2019-07-19 21:00:45.000000 avocado-framework-98.0/examples/yaml_to_mux/simple_vars.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      602 2019-07-19 21:00:45.000000 avocado-framework-98.0/examples/yaml_to_mux/types.yaml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.914576 avocado-framework-98.0/selftests/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.917576 avocado-framework-98.0/selftests/.data/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.918576 avocado-framework-98.0/selftests/.data/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2004 2022-07-14 13:12:24.000000 avocado-framework-98.0/selftests/.data/__pycache__/get_data.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8587 2022-07-14 13:12:47.000000 avocado-framework-98.0/selftests/.data/__pycache__/test_statuses.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1126 2022-07-14 13:12:36.000000 avocado-framework-98.0/selftests/.data/__pycache__/unittests.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       36 2019-07-23 15:43:52.000000 avocado-framework-98.0/selftests/.data/avocado.gz
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       64 2021-02-11 22:50:38.000000 avocado-framework-98.0/selftests/.data/avocado.xz
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       46 2019-07-23 15:43:52.000000 avocado-framework-98.0/selftests/.data/empty.tar.bz2
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3376 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/.data/get_data.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.918576 avocado-framework-98.0/selftests/.data/get_data.py.data/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.919576 avocado-framework-98.0/selftests/.data/get_data.py.data/GetData.test_a/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.919576 avocado-framework-98.0/selftests/.data/get_data.py.data/GetData.test_a/long-cbbd/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       12 2019-07-19 21:00:45.000000 avocado-framework-98.0/selftests/.data/get_data.py.data/GetData.test_a/long-cbbd/variant_data
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.919576 avocado-framework-98.0/selftests/.data/get_data.py.data/GetData.test_a/medium-1a7a/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       12 2019-07-19 21:00:45.000000 avocado-framework-98.0/selftests/.data/get_data.py.data/GetData.test_a/medium-1a7a/variant_data
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.919576 avocado-framework-98.0/selftests/.data/get_data.py.data/GetData.test_a/short-475e/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       12 2019-07-19 21:00:45.000000 avocado-framework-98.0/selftests/.data/get_data.py.data/GetData.test_a/short-475e/variant_data
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2019-07-19 21:00:45.000000 avocado-framework-98.0/selftests/.data/get_data.py.data/GetData.test_a/test_data
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.919576 avocado-framework-98.0/selftests/.data/get_data.py.data/GetData.test_b/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2019-07-19 21:00:45.000000 avocado-framework-98.0/selftests/.data/get_data.py.data/GetData.test_b/test_data
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       11 2019-07-19 21:00:45.000000 avocado-framework-98.0/selftests/.data/get_data.py.data/file_data
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      354 2021-02-11 22:50:38.000000 avocado-framework-98.0/selftests/.data/get_data.py.data/get_data.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       83 2019-07-19 21:00:45.000000 avocado-framework-98.0/selftests/.data/get_data.py.data/get_data.yaml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      150 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/guaca.a
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    56132 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/hello.deb
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    71999 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/hello.rpm
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6108 2019-07-19 21:00:45.000000 avocado-framework-98.0/selftests/.data/jenkins-junit.xsd
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.864576 avocado-framework-98.0/selftests/.data/safeloader/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.920576 avocado-framework-98.0/selftests/.data/safeloader/caveat_multilevel/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       82 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/caveat_multilevel/failure.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.920576 avocado-framework-98.0/selftests/.data/safeloader/caveat_multilevel/l1/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/caveat_multilevel/l1/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.920576 avocado-framework-98.0/selftests/.data/safeloader/caveat_multilevel/l1/l2/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/caveat_multilevel/l1/l2/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.920576 avocado-framework-98.0/selftests/.data/safeloader/caveat_multilevel/l1/l2/l3/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       90 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/caveat_multilevel/l1/l2/l3/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       87 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/caveat_multilevel/success.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.921576 avocado-framework-98.0/selftests/.data/safeloader/data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1236 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/.data/safeloader/data/dont_crash.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      713 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/.data/safeloader/data/dont_detect_non_avocado.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      385 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/.data/safeloader/data/double_import.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1579 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/.data/safeloader/data/imports.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      156 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/infinite_recurse.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/parent1.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/parent4.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/parent7.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/parent9.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.922576 avocado-framework-98.0/selftests/.data/safeloader/data/path/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/path/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       79 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/path/parent10.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/path/parent2.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/path/parent3.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/path/parent5.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/path/parent6.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/safeloader/data/path/parent8.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)   378880 2019-07-19 21:00:45.000000 avocado-framework-98.0/selftests/.data/sample.iso
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1313 2017-06-27 20:18:38.000000 avocado-framework-98.0/selftests/.data/test_archive__symlinks.zip
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7200 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/.data/test_statuses.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      438 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/.data/unittests.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)     1383 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/.data/whiteboard.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.923576 avocado-framework-98.0/selftests/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      147 2022-07-14 13:07:44.000000 avocado-framework-98.0/selftests/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    15333 2022-07-14 13:07:56.000000 avocado-framework-98.0/selftests/__pycache__/check.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5050 2022-07-14 13:07:44.000000 avocado-framework-98.0/selftests/__pycache__/utils.cpython-310.pyc
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)    28628 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/check.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      909 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/check_tmp_dirs
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.924576 avocado-framework-98.0/selftests/deployment/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3056 2021-02-11 22:50:38.000000 avocado-framework-98.0/selftests/deployment/README.rst
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       74 2019-11-19 20:03:57.000000 avocado-framework-98.0/selftests/deployment/ansible.cfg
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      161 2021-02-11 22:50:38.000000 avocado-framework-98.0/selftests/deployment/deployment.yml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.924576 avocado-framework-98.0/selftests/deployment/group_vars/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       45 2021-02-11 22:50:38.000000 avocado-framework-98.0/selftests/deployment/group_vars/all
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       18 2021-08-18 18:06:49.000000 avocado-framework-98.0/selftests/deployment/inventory
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.865576 avocado-framework-98.0/selftests/deployment/roles/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.864576 avocado-framework-98.0/selftests/deployment/roles/avocado/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.924576 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.925576 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/copr/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      161 2021-03-04 22:57:12.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/copr/avocado.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      292 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/copr/examples.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      849 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/copr/plugins.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      456 2021-03-04 22:57:12.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/main.yml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.925576 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/official/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      161 2021-03-04 22:57:12.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/official/avocado.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      292 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/official/examples.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      849 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/official/plugins.yml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.925576 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/pip/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      219 2021-03-04 22:57:12.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/pip/avocado.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      144 2021-03-04 22:57:12.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/pip/examples.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2016 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/pip/plugins.yml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.926576 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/rpm/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      161 2021-03-04 22:57:12.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/rpm/avocado.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      292 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/rpm/examples.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      849 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/rpm/plugins.yml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.864576 avocado-framework-98.0/selftests/deployment/roles/common/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.926576 avocado-framework-98.0/selftests/deployment/roles/common/tasks/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      204 2021-03-04 22:57:12.000000 avocado-framework-98.0/selftests/deployment/roles/common/tasks/aexpect.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      695 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/deployment/roles/common/tasks/dependencies.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       76 2021-02-11 22:50:38.000000 avocado-framework-98.0/selftests/deployment/roles/common/tasks/main.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2500 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/deployment/roles/common/tasks/repos.yml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.865576 avocado-framework-98.0/selftests/deployment/roles/tests/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.926576 avocado-framework-98.0/selftests/deployment/roles/tests/tasks/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1932 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/deployment/roles/tests/tasks/main.yml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.865576 avocado-framework-98.0/selftests/deployment/roles/virtualenv/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.927576 avocado-framework-98.0/selftests/deployment/roles/virtualenv/tasks/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      266 2021-02-11 22:50:38.000000 avocado-framework-98.0/selftests/deployment/roles/virtualenv/tasks/main.yml
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      301 2021-02-11 22:50:38.000000 avocado-framework-98.0/selftests/deployment/vars.yml
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.933576 avocado-framework-98.0/selftests/functional/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2021-10-16 20:28:12.000000 avocado-framework-98.0/selftests/functional/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.940576 avocado-framework-98.0/selftests/functional/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      158 2022-07-14 13:10:29.000000 avocado-framework-98.0/selftests/functional/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3103 2022-07-14 13:12:20.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_argument_parsing.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    42614 2022-07-14 13:13:06.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_basic.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1063 2022-07-14 13:12:20.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_coroutine.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1901 2022-07-14 13:12:20.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_export_variables.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4421 2022-07-14 13:12:20.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_fetch_asset.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1372 2022-07-14 13:12:20.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_getdata.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7653 2022-07-14 13:12:23.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_interrupt.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1817 2022-07-14 13:12:25.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_job_api_features.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6005 2022-07-14 13:12:26.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_job_timeout.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2345 2022-07-14 13:12:27.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_journal.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2579 2022-07-14 13:12:27.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_json_variants.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8980 2022-07-14 13:12:28.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_list.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4877 2022-07-14 13:12:33.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_lv_utils.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7487 2022-07-14 13:13:39.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_nrunner.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4597 2022-07-14 13:08:26.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_nrunner_interface.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    18745 2022-07-14 13:12:44.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_output.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    13479 2022-07-14 13:12:33.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_output_check.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3201 2022-07-14 13:12:36.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_replay.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2758 2022-07-14 13:12:37.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_requirements_cache.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4351 2022-07-14 13:13:50.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_resolver.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2518 2022-07-14 13:13:54.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_runner_asset.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2630 2022-07-14 13:13:55.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_runner_package.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    11149 2022-07-14 13:13:56.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_skiptests.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1827 2022-07-14 13:13:59.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_software_manager.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3640 2022-07-14 13:12:38.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_statuses.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4750 2022-07-14 13:12:58.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_streams.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4084 2022-07-14 13:13:03.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_sysinfo.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1551 2022-07-14 13:12:38.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_task_statemachine.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1611 2022-07-14 13:12:38.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_task_timeout.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3169 2022-07-14 13:13:05.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_teststmpdir.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1909 2022-07-14 13:12:40.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_thirdparty_bugs.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3630 2022-07-14 13:12:40.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_unittest_compat.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6789 2022-07-14 13:12:41.000000 avocado-framework-98.0/selftests/functional/__pycache__/test_utils.cpython-310.pyc
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.942576 avocado-framework-98.0/selftests/functional/plugin/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.943576 avocado-framework-98.0/selftests/functional/plugin/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      165 2022-07-14 13:10:29.000000 avocado-framework-98.0/selftests/functional/plugin/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9540 2022-07-14 13:14:08.000000 avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_assets.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1069 2022-07-14 13:14:11.000000 avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_bystatus.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2525 2022-07-14 13:14:12.000000 avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_diff.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3731 2022-07-14 13:14:13.000000 avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_jobscripts.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1965 2022-07-14 13:14:14.000000 avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_jsonresult.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3874 2022-07-14 13:14:16.000000 avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_logs.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3286 2022-07-14 13:10:29.000000 avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_vmimage.cpython-310.pyc
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.944576 avocado-framework-98.0/selftests/functional/plugin/spawners/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/spawners/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.944576 avocado-framework-98.0/selftests/functional/plugin/spawners/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2768 2022-07-14 13:14:21.000000 avocado-framework-98.0/selftests/functional/plugin/spawners/__pycache__/test_podman.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1325 2022-07-14 13:14:22.000000 avocado-framework-98.0/selftests/functional/plugin/spawners/__pycache__/test_process.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2594 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/spawners/test_podman.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      951 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/spawners/test_process.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12450 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/test_assets.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      788 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/test_bystatus.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2458 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/test_diff.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4426 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/test_jobscripts.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1858 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/test_jsonresult.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3474 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/test_logs.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2935 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/plugin/test_vmimage.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.944576 avocado-framework-98.0/selftests/functional/serial/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.945576 avocado-framework-98.0/selftests/functional/serial/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5014 2022-07-14 13:08:52.000000 avocado-framework-98.0/selftests/functional/serial/__pycache__/test_requirements.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5839 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/serial/test_requirements.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2951 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_argument_parsing.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    48414 2022-07-14 20:25:14.000000 avocado-framework-98.0/selftests/functional/test_basic.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      731 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_coroutine.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1323 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_export_variables.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5442 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_fetch_asset.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1154 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_getdata.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10204 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_interrupt.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1321 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_job_api_features.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7129 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_job_timeout.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2049 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_journal.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2404 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_json_variants.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10228 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_list.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5927 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_lv_utils.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8680 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_nrunner.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4458 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.947576 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1130 2022-07-08 19:26:31.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/capabilities.schema.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       17 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       84 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_avocado_instrumented.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       20 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_dry_run.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       72 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_exec_test.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       17 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_noop.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       99 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_python_unittest.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       87 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_robot.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       58 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_tap.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       42 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_task.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      109 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_avocado_instrumented.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       45 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_dry_run.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       97 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_exec_test.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       42 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_noop.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      124 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_python_unittest.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      112 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_robot.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       83 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_tap.json
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    22884 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_output.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    17925 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_output_check.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2870 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_replay.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3731 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_requirements_cache.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4436 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_resolver.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2304 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_runner_asset.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2565 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_runner_package.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10472 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_skiptests.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1379 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_software_manager.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6472 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_statuses.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5273 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_streams.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5422 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_sysinfo.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1267 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_task_statemachine.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1102 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_task_timeout.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3114 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_teststmpdir.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2105 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_thirdparty_bugs.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3714 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_unittest_compat.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6435 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/test_utils.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.948576 avocado-framework-98.0/selftests/functional/utils/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/utils/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.948576 avocado-framework-98.0/selftests/functional/utils/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      164 2022-07-14 13:14:34.000000 avocado-framework-98.0/selftests/functional/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6448 2022-07-14 13:14:01.000000 avocado-framework-98.0/selftests/functional/utils/__pycache__/test_asset.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1222 2022-07-14 13:14:08.000000 avocado-framework-98.0/selftests/functional/utils/__pycache__/test_podman.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7895 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/utils/test_asset.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1019 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/functional/utils/test_podman.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      282 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/isort.sh
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.949576 avocado-framework-98.0/selftests/jobs/
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      466 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/jobs/example_passjob
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      358 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/jobs/example_passjob_cit_varianter
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      331 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/jobs/example_passjob_html
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      369 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/jobs/example_sleepjob_dict_varianter
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      369 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/jobs/example_sleepjob_json_varianter
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      785 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/jobs/example_unix_status_server
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      465 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/jobs/pass
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.949576 avocado-framework-98.0/selftests/jobs/tests/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.950576 avocado-framework-98.0/selftests/jobs/tests/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      611 2022-07-14 13:12:05.000000 avocado-framework-98.0/selftests/jobs/tests/__pycache__/passtest.cpython-310.pyc
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)       17 2021-03-04 22:57:12.000000 avocado-framework-98.0/selftests/jobs/tests/pass
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      226 2022-06-09 19:17:14.000000 avocado-framework-98.0/selftests/jobs/tests/passtest.py
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)     1550 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/lint.sh
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)     1265 2022-05-13 17:48:04.000000 avocado-framework-98.0/selftests/modules-boundaries.sh
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.865576 avocado-framework-98.0/selftests/pre_release/
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.950576 avocado-framework-98.0/selftests/pre_release/jobs/
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)     1057 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/pre_release/jobs/pre_release.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.951576 avocado-framework-98.0/selftests/pre_release/tests/
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)     1103 2022-07-11 17:58:40.000000 avocado-framework-98.0/selftests/pre_release/tests/check-copr-rpm-version.sh
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      462 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/pre_release/tests/cirrusci.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1082 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/pre_release/tests/readthedocs.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2938 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/pre_release/tests/vmimage.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.951576 avocado-framework-98.0/selftests/pre_release/tests/vmimage.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2514 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/pre_release/tests/vmimage.py.data/variants.yml
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      424 2022-07-08 19:26:31.000000 avocado-framework-98.0/selftests/run
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      926 2022-06-21 20:03:32.000000 avocado-framework-98.0/selftests/run_coverage
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)     1068 2022-06-23 14:48:31.000000 avocado-framework-98.0/selftests/safeloader.sh
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      318 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/signedoff-check.sh
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)      228 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/spell.sh
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)       57 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/style.sh
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.957576 avocado-framework-98.0/selftests/unit/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-06-21 14:31:52.000000 avocado-framework-98.0/selftests/unit/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.964576 avocado-framework-98.0/selftests/unit/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      152 2022-07-14 13:09:50.000000 avocado-framework-98.0/selftests/unit/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7183 2022-07-14 13:09:04.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_datadir.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1152 2022-07-14 13:09:04.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_dependencies_resolver.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1473 2022-07-14 13:09:04.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_dispatcher.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2199 2022-07-14 13:09:04.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_hintfiles.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12750 2022-07-14 13:09:04.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_job.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8715 2022-07-14 13:09:10.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_loader.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    17550 2022-07-14 13:09:13.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_nrunner.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1411 2022-07-14 13:09:25.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_output.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1547 2022-07-14 13:09:25.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_parameters.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1898 2022-07-14 13:09:26.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_parser.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2490 2022-07-14 13:09:27.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_plugin_interfaces.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1230 2022-07-14 13:09:29.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_references.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2324 2022-07-14 13:09:29.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_result.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3241 2022-07-14 13:09:31.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_runner_asset.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5734 2022-07-14 13:09:31.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_runner_package.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1944 2022-07-14 13:09:35.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_runner_sysinfo.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1060 2022-07-14 13:09:35.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_caveats.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9089 2022-07-14 13:09:36.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_core.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6658 2022-07-14 13:09:39.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_docstring.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9634 2022-07-14 13:09:43.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_imported.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3950 2022-07-14 13:09:50.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_module.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1901 2022-07-14 13:09:52.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_utils.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6294 2022-07-14 13:09:53.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_settings.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6215 2022-07-14 13:09:56.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_status_repo.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1239 2022-07-14 13:10:00.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_status_utils.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3086 2022-07-14 13:10:01.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_suite.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2941 2022-07-14 13:10:01.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_sysinfo.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    11446 2022-07-14 13:10:03.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_tags.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10077 2022-07-14 13:10:09.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_tap.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3716 2022-07-14 13:10:14.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_task_runtime.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7200 2022-07-14 13:08:41.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_test.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3951 2022-07-14 13:10:19.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_test_id.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2988 2022-07-14 13:10:20.000000 avocado-framework-98.0/selftests/unit/__pycache__/test_tree.cpython-310.pyc
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.965576 avocado-framework-98.0/selftests/unit/plugin/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/plugin/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.967576 avocado-framework-98.0/selftests/unit/plugin/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7521 2022-07-14 13:10:21.000000 avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_assets.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4293 2022-07-14 13:10:24.000000 avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_jsonresult.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6783 2022-07-14 13:10:24.000000 avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_resolver.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2365 2022-07-14 13:10:26.000000 avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_spawner.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7473 2022-07-14 13:10:29.000000 avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_vmimage.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7483 2022-07-14 13:10:29.000000 avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_xunit.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10006 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/plugin/test_assets.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4168 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/plugin/test_jsonresult.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6830 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/plugin/test_resolver.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2089 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/plugin/test_spawner.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8483 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/plugin/test_vmimage.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5858 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/plugin/test_xunit.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9281 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_datadir.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1037 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_dependencies_resolver.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1158 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_dispatcher.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1844 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_hintfiles.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    14519 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_job.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10967 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_loader.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    17616 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_nrunner.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      911 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_output.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2285 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_parameters.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1015 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_parser.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2036 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_plugin_interfaces.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      832 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_references.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1908 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_result.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2828 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_runner_asset.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6966 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_runner_package.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2204 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_runner_sysinfo.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      741 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_safeloader_caveats.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10254 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_safeloader_core.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6611 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_safeloader_docstring.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8371 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_safeloader_imported.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3106 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_safeloader_module.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1293 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_safeloader_utils.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6537 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_settings.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7883 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_status_repo.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      617 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_status_utils.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2882 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_suite.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3248 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_sysinfo.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    13253 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_tags.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12312 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_tap.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3740 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_task_runtime.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6667 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_test.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3605 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_test_id.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2638 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/test_tree.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.972576 avocado-framework-98.0/selftests/unit/utils/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.979576 avocado-framework-98.0/selftests/unit/utils/__pycache__/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1896 2022-07-14 13:10:30.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_ar.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8834 2022-07-14 13:10:31.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_archive.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5324 2022-07-14 13:10:36.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_astring.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3945 2022-07-14 13:10:38.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_cloudinit.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9295 2022-07-14 13:10:39.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_cpu.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5633 2022-07-14 13:10:45.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_data_structures.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4109 2022-07-14 13:10:47.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_datadrainer.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4303 2022-07-14 13:10:48.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_diff_validator.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3278 2022-07-14 13:10:49.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_disk.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3538 2022-07-14 13:10:50.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_distro.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2075 2022-07-14 13:10:51.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_filelock.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1574 2022-07-14 13:10:52.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_gdb.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2197 2022-07-14 13:10:53.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_genio.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6616 2022-07-14 13:10:53.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_iso9660.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1348 2022-07-14 13:10:56.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_kernel.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2624 2022-07-14 13:10:56.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_linux_modules.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3905 2022-07-14 13:10:58.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_memory.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2976 2022-07-14 13:11:00.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_network.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1328 2022-07-14 13:11:01.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_output.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7998 2022-07-14 13:11:02.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_partition.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1926 2022-07-14 13:11:03.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_path.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1609 2022-07-14 13:11:04.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_pci.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      814 2022-07-14 13:11:05.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_pmem.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    25651 2022-07-14 13:11:05.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_process.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      942 2022-07-14 13:11:16.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_script.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10086 2022-07-14 13:11:17.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_service.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1872 2022-07-14 13:11:20.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_software_manager.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2924 2022-07-14 13:11:21.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_ssh.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3030 2022-07-14 13:11:23.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_stacktrace.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    31717 2022-07-14 13:11:23.000000 avocado-framework-98.0/selftests/unit/utils/__pycache__/test_vmimage.cpython-310.pyc
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1398 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_ar.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8992 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_archive.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6348 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_astring.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2827 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_cloudinit.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    10232 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.980576 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      335 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/armv7
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      221 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/armv8
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      852 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/i386
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      286 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/power8
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      251 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/power9
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       72 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/risc_v
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1182 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/s390x
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1494 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/s390x_2
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3144 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/s390x_3
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8991 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/x86_64
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5193 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_data_structures.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2448 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_datadrainer.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5752 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_diff_validator.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2870 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_disk.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2261 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_distro.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1185 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_filelock.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1220 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_gdb.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1732 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_genio.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6328 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_iso9660.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      866 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_kernel.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2143 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_linux_modules.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:43.981576 avocado-framework-98.0/selftests/unit/utils/test_linux_modules.py.data/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      752 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_linux_modules.py.data/lsmod
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7153 2021-11-01 18:09:57.000000 avocado-framework-98.0/selftests/unit/utils/test_linux_modules.py.data/proc_modules
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3956 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_memory.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2201 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_network.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1170 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_output.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     8324 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_partition.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1338 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_path.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1476 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_pci.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      340 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_pmem.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    31526 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_process.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      541 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_script.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12716 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_service.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1215 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_software_manager.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2408 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_ssh.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2932 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_stacktrace.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    32272 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/unit/utils/test_vmimage.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5138 2022-07-11 13:32:25.000000 avocado-framework-98.0/selftests/utils.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       38 2022-07-14 20:53:43.981576 avocado-framework-98.0/setup.cfg
--rwxrwxr-x   0 cleber    (1000) cleber    (1000)    17502 2022-07-11 13:32:25.000000 avocado-framework-98.0/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.323128 avocado-framework-99.0/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)    18542 2016-04-28 15:01:56.000000 avocado-framework-99.0/LICENSE
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      195 2022-10-07 18:12:16.000000 avocado-framework-99.0/MANIFEST.in
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2883 2022-10-27 20:58:37.000000 avocado-framework-99.0/Makefile
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    11627 2022-11-10 19:12:41.323128 avocado-framework-99.0/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10679 2022-10-27 20:58:37.000000 avocado-framework-99.0/README
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10679 2022-10-27 20:58:37.000000 avocado-framework-99.0/README.rst
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        5 2022-11-10 19:09:51.000000 avocado-framework-99.0/VERSION
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.253127 avocado-framework-99.0/avocado/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1174 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      150 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/__main__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.256127 avocado-framework-99.0/avocado/core/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9172 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4018 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/app.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    12144 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/data_dir.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5250 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/decorators.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.257127 avocado-framework-99.0/avocado/core/dependencies/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-27 20:58:37.000000 avocado-framework-99.0/avocado/core/dependencies/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.257127 avocado-framework-99.0/avocado/core/dependencies/requirements/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-27 20:58:37.000000 avocado-framework-99.0/avocado/core/dependencies/requirements/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.257127 avocado-framework-99.0/avocado/core/dependencies/requirements/cache/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      356 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/dependencies/requirements/cache/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.257127 avocado-framework-99.0/avocado/core/dependencies/requirements/cache/backends/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-27 20:58:37.000000 avocado-framework-99.0/avocado/core/dependencies/requirements/cache/backends/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    11704 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/dependencies/requirements/cache/backends/sqlite.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4249 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/dispatcher.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1720 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/enabled_extension_manager.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4318 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/exceptions.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1644 2022-10-27 20:58:37.000000 avocado-framework-99.0/avocado/core/exit_codes.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7637 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/extension_manager.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    25414 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/job.py
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      895 2021-03-04 22:57:12.000000 avocado-framework-99.0/avocado/core/job_id.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5959 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/jobdata.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    24151 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/loader.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)     2934 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/main.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    15697 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/messages.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.258127 avocado-framework-99.0/avocado/core/nrunner/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-27 20:58:37.000000 avocado-framework-99.0/avocado/core/nrunner/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      504 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/nrunner/__main__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10238 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/nrunner/app.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      981 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/nrunner/config.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    19712 2022-11-08 16:49:59.000000 avocado-framework-99.0/avocado/core/nrunner/runnable.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3315 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/nrunner/runner.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7501 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/nrunner/task.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    24592 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/output.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9317 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/parameters.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9207 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/parser.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2005 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/parser_common_args.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    15778 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/plugin_interfaces.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1149 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/references.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8592 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/resolver.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3801 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/result.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9830 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/runner.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.258127 avocado-framework-99.0/avocado/core/safeloader/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      798 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/safeloader/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    16391 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/safeloader/core.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2483 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/safeloader/docstring.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10240 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/safeloader/imported.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6260 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/safeloader/module.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      775 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/safeloader/utils.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    26268 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/settings.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1216 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/settings_dispatcher.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.258127 avocado-framework-99.0/avocado/core/spawners/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-99.0/avocado/core/spawners/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3051 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/spawners/common.py
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       44 2021-03-04 22:57:12.000000 avocado-framework-99.0/avocado/core/spawners/exceptions.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2104 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/spawners/mock.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.259127 avocado-framework-99.0/avocado/core/status/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-99.0/avocado/core/status/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6589 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/status/repo.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1779 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/status/server.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      826 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/status/utils.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      442 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/streams.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    12215 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/suite.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9971 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/sysinfo.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5877 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/tags.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6360 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/tapparser.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.259127 avocado-framework-99.0/avocado/core/task/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-99.0/avocado/core/task/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10464 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/task/runtime.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    13026 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/task/statemachine.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    31367 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/test.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3881 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/test_id.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1237 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/teststatus.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    17680 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/tree.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.260127 avocado-framework-99.0/avocado/core/utils/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-27 20:58:37.000000 avocado-framework-99.0/avocado/core/utils/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2211 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/utils/loader.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8312 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/utils/messages.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1446 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/utils/path.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      812 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/utils/version.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    12651 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/varianter.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      813 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/core/version.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.246127 avocado-framework-99.0/avocado/etc/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.246127 avocado-framework-99.0/avocado/etc/avocado/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.246127 avocado-framework-99.0/avocado/etc/avocado/scripts/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.246127 avocado-framework-99.0/avocado/etc/avocado/scripts/job/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.260127 avocado-framework-99.0/avocado/etc/avocado/scripts/job/post.d/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      244 2019-07-19 21:00:45.000000 avocado-framework-99.0/avocado/etc/avocado/scripts/job/post.d/README
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.260127 avocado-framework-99.0/avocado/etc/avocado/scripts/job/pre.d/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      243 2019-07-19 21:00:45.000000 avocado-framework-99.0/avocado/etc/avocado/scripts/job/pre.d/README
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.260127 avocado-framework-99.0/avocado/etc/avocado/sysinfo/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      157 2020-09-09 00:55:30.000000 avocado-framework-99.0/avocado/etc/avocado/sysinfo/commands
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      294 2019-07-19 21:00:45.000000 avocado-framework-99.0/avocado/etc/avocado/sysinfo/files
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       23 2019-07-19 21:00:45.000000 avocado-framework-99.0/avocado/etc/avocado/sysinfo/profilers
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.260127 avocado-framework-99.0/avocado/libexec/
+-rwxrwxr-x   0 cleber    (1000) cleber    (1000)      634 2019-07-19 21:00:45.000000 avocado-framework-99.0/avocado/libexec/avocado-bash-utils
+-rwxrwxr-x   0 cleber    (1000) cleber    (1000)       53 2019-07-19 21:00:45.000000 avocado-framework-99.0/avocado/libexec/avocado_debug
+-rwxrwxr-x   0 cleber    (1000) cleber    (1000)       53 2019-07-19 21:00:45.000000 avocado-framework-99.0/avocado/libexec/avocado_error
+-rwxrwxr-x   0 cleber    (1000) cleber    (1000)       52 2019-07-19 21:00:45.000000 avocado-framework-99.0/avocado/libexec/avocado_info
+-rwxrwxr-x   0 cleber    (1000) cleber    (1000)       52 2019-07-19 21:00:45.000000 avocado-framework-99.0/avocado/libexec/avocado_warn
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.264127 avocado-framework-99.0/avocado/plugins/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      545 2022-01-26 18:48:01.000000 avocado-framework-99.0/avocado/plugins/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1638 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/archive.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    22329 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/assets.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4249 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/beaker_result.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1242 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/bystatus.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2575 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/cache.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4076 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/config.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1799 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/dependency.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3496 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/dict_variants.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    15736 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/diff.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    14480 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/distro.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1206 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/exec_path.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5370 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/human.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10294 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/jobs.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3559 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/jobscripts.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4875 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/journal.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5201 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/json_variants.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5063 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/jsonresult.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8181 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/list.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4124 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/plugins.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3029 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/replay.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1869 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/requirement_cache.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4262 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/resolvers.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10225 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/run.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    15247 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runner_nrunner.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.265127 avocado-framework-99.0/avocado/plugins/runners/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-27 20:58:37.000000 avocado-framework-99.0/avocado/plugins/runners/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4007 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runners/asset.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6219 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runners/avocado_instrumented.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      903 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runners/dry_run.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6032 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runners/exec_test.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      834 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runners/noop.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5845 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runners/package.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2383 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runners/podman_image.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5729 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runners/python_unittest.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7241 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runners/sysinfo.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2505 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/runners/tap.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.265127 avocado-framework-99.0/avocado/plugins/spawners/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-99.0/avocado/plugins/spawners/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    14571 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/spawners/podman.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3578 2022-11-07 18:55:58.000000 avocado-framework-99.0/avocado/plugins/spawners/process.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6762 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/sysinfo.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6886 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/tap.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4377 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/testlogs.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1449 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/teststmpdir.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6202 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/variants.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6348 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/vmimage.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10037 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/plugins/xunit.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.270127 avocado-framework-99.0/avocado/utils/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      560 2022-01-26 18:48:01.000000 avocado-framework-99.0/avocado/utils/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3201 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/ar.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9118 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/archive.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    23777 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/asset.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10725 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/astring.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      976 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/aurl.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3798 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/build.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8062 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/cloudinit.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    16231 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/cpu.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2056 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/crypto.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2607 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/data_factory.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10155 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/data_structures.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5663 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/datadrainer.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2938 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/debug.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10836 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/diff_validator.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7621 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/disk.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    15985 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/distro.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5978 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/dmesg.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6671 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/download.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      795 2022-10-07 18:12:16.000000 avocado-framework-99.0/avocado/utils/exit_codes.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.270127 avocado-framework-99.0/avocado/utils/external/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      545 2022-01-26 18:48:01.000000 avocado-framework-99.0/avocado/utils/external/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    12579 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/external/gdbmi_parser.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    27100 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/external/spark.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2999 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/file_utils.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3261 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/filelock.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    26030 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/gdb.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5351 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/genio.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6707 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/git.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    13854 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/iso9660.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7240 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/kernel.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1900 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/linux.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8024 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/linux_modules.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    25505 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/lv_utils.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    14904 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/memory.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    11228 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/multipath.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.270127 avocado-framework-99.0/avocado/utils/network/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-27 20:58:37.000000 avocado-framework-99.0/avocado/utils/network/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      406 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/network/common.py
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       90 2021-02-11 22:50:38.000000 avocado-framework-99.0/avocado/utils/network/exceptions.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4388 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/network/hosts.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    22200 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/network/interfaces.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5630 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/network/ports.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4178 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/output.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    11470 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/partition.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7550 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/path.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    13650 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/pci.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    18321 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/pmem.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6057 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/podman.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    43647 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/process.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4726 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/script.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    27530 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/service.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.271127 avocado-framework-99.0/avocado/utils/software_manager/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-27 20:58:37.000000 avocado-framework-99.0/avocado/utils/software_manager/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.272127 avocado-framework-99.0/avocado/utils/software_manager/backends/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-01-26 18:48:01.000000 avocado-framework-99.0/avocado/utils/software_manager/backends/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9421 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/backends/apt.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1323 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/backends/base.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      943 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/backends/dnf.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3760 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/backends/dpkg.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10093 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/backends/rpm.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9874 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/backends/yum.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5986 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/backends/zypper.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2768 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/distro_packages.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2978 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/inspector.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5073 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/main.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2677 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/software_manager/manager.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5381 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/softwareraid.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9182 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/ssh.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3513 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/stacktrace.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    11756 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/sysinfo.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    23551 2022-11-04 17:27:10.000000 avocado-framework-99.0/avocado/utils/vmimage.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1065 2022-10-27 20:58:37.000000 avocado-framework-99.0/avocado/utils/wait.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.272127 avocado-framework-99.0/avocado_framework.egg-info/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    11627 2022-11-10 19:12:41.000000 avocado-framework-99.0/avocado_framework.egg-info/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    31814 2022-11-10 19:12:41.000000 avocado-framework-99.0/avocado_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2022-11-10 19:12:41.000000 avocado-framework-99.0/avocado_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4741 2022-11-10 19:12:41.000000 avocado-framework-99.0/avocado_framework.egg-info/entry_points.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2022-11-07 21:15:48.000000 avocado-framework-99.0/avocado_framework.egg-info/not-zip-safe
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       11 2022-11-10 19:12:41.000000 avocado-framework-99.0/avocado_framework.egg-info/requires.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        8 2022-11-10 19:12:41.000000 avocado-framework-99.0/avocado_framework.egg-info/top_level.txt
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.249127 avocado-framework-99.0/examples/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.247127 avocado-framework-99.0/examples/apis/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.272127 avocado-framework-99.0/examples/apis/utils/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      603 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/apis/utils/ssh.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.272127 avocado-framework-99.0/examples/gdb-prerun-scripts/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      174 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/gdb-prerun-scripts/README
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       42 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/gdb-prerun-scripts/pass-sigusr1
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.273127 avocado-framework-99.0/examples/hint-files/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       85 2021-02-11 22:50:38.000000 avocado-framework-99.0/examples/hint-files/.avocado.hint.example
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      463 2021-02-11 22:50:38.000000 avocado-framework-99.0/examples/hint-files/README.rst
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.274127 avocado-framework-99.0/examples/jobs/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      286 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/jobs/README.rst
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)     1052 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/custom_exec_test.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      195 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/failjob.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      675 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/multiple_suites_from_config.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      466 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/passjob.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      358 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/passjob_cit_varianter.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      708 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/passjob_custom.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      331 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/passjob_html.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      377 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/passjob_html_browser.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      494 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/passjob_with_test.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      369 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/sleepjob_dict_varianter.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      369 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/sleepjob_json_varianter.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      370 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/sleepjob_yaml_to_mux.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      785 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/jobs/unix_status_server.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.247127 avocado-framework-99.0/examples/nrunner/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.247127 avocado-framework-99.0/examples/nrunner/recipes/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.274127 avocado-framework-99.0/examples/nrunner/recipes/runnables/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      121 2022-10-27 20:58:37.000000 avocado-framework-99.0/examples/nrunner/recipes/runnables/asset.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       69 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/nrunner/recipes/runnables/exec_test_echo_no_newline.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      117 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/nrunner/recipes/runnables/exec_test_sh_echo_env_var.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       58 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/nrunner/recipes/runnables/exec_test_sleep_3.json
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       17 2021-02-11 22:50:38.000000 avocado-framework-99.0/examples/nrunner/recipes/runnables/noop.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       66 2022-10-27 20:58:37.000000 avocado-framework-99.0/examples/nrunner/recipes/runnables/package_check_foo.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       99 2022-10-27 20:58:37.000000 avocado-framework-99.0/examples/nrunner/recipes/runnables/python_unittest.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      274 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/nrunner/recipes/runnables/sysinfo.json
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.247127 avocado-framework-99.0/examples/nrunner/recipes/tasks/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.275128 avocado-framework-99.0/examples/nrunner/recipes/tasks/exec-status/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      112 2021-02-11 22:50:38.000000 avocado-framework-99.0/examples/nrunner/recipes/tasks/exec-status/1-uname-result.json
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      145 2021-02-11 22:50:38.000000 avocado-framework-99.0/examples/nrunner/recipes/tasks/exec-status/2-dd-result.json
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      114 2021-02-11 22:50:38.000000 avocado-framework-99.0/examples/nrunner/recipes/tasks/exec-status/3-sleep-result.json
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      111 2021-02-11 22:50:38.000000 avocado-framework-99.0/examples/nrunner/recipes/tasks/exec-status/4-sleep-long-result.json
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.275128 avocado-framework-99.0/examples/nrunner/recipes/tasks/exec-test/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       82 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/nrunner/recipes/tasks/exec-test/1-uname.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       92 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/nrunner/recipes/tasks/exec-test/2-echo.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       84 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/nrunner/recipes/tasks/exec-test/3-sleep.json
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.275128 avocado-framework-99.0/examples/nrunner/recipes/tasks/unittest-result/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      111 2021-02-11 22:50:38.000000 avocado-framework-99.0/examples/nrunner/recipes/tasks/unittest-result/1-unittest-testcase-localhost.json
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.275128 avocado-framework-99.0/examples/plugins/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      411 2016-10-06 13:45:36.000000 avocado-framework-99.0/examples/plugins/README.rst
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.247127 avocado-framework-99.0/examples/plugins/cli-cmd/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.275128 avocado-framework-99.0/examples/plugins/cli-cmd/hello/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      266 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/cli-cmd/hello/hello.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      321 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/cli-cmd/hello/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.276127 avocado-framework-99.0/examples/plugins/cli-cmd/hello_option/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      592 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/cli-cmd/hello_option/hello_option.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      368 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/cli-cmd/hello_option/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.276127 avocado-framework-99.0/examples/plugins/cli-cmd/hello_parser/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      710 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/cli-cmd/hello_parser/hello_parser.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      368 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/cli-cmd/hello_parser/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.276127 avocado-framework-99.0/examples/plugins/cli-cmd/hello_priority/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      359 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/cli-cmd/hello_priority/hello_priority.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      363 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/cli-cmd/hello_priority/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.247127 avocado-framework-99.0/examples/plugins/job-pre-post/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.276127 avocado-framework-99.0/examples/plugins/job-pre-post/mail/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2273 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/job-pre-post/mail/avocado_job_mail.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      511 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/job-pre-post/mail/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.276127 avocado-framework-99.0/examples/plugins/job-pre-post/sleep/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      835 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/job-pre-post/sleep/avocado_job_sleep.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      502 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/job-pre-post/sleep/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.276127 avocado-framework-99.0/examples/plugins/tests/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      733 2022-10-27 20:58:37.000000 avocado-framework-99.0/examples/plugins/tests/README.rst
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.276127 avocado-framework-99.0/examples/plugins/tests/magic/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.277127 avocado-framework-99.0/examples/plugins/tests/magic/avocado_magic/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/plugins/tests/magic/avocado_magic/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1730 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/tests/magic/avocado_magic/resolver.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1037 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/tests/magic/avocado_magic/runner.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      728 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/plugins/tests/magic/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.248127 avocado-framework-99.0/examples/testplans/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.277127 avocado-framework-99.0/examples/testplans/release/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1855 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/testplans/release/pre.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2054 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/testplans/release/release.json
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.281127 avocado-framework-99.0/examples/tests/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.283127 avocado-framework-99.0/examples/tests/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1015 2022-11-07 21:19:53.000000 avocado-framework-99.0/examples/tests/__pycache__/assert.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1048 2022-11-07 21:19:53.000000 avocado-framework-99.0/examples/tests/__pycache__/cancel_on_exception.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      853 2022-11-07 21:20:02.000000 avocado-framework-99.0/examples/tests/__pycache__/cancelonsetup.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      599 2022-11-07 21:20:45.000000 avocado-framework-99.0/examples/tests/__pycache__/canceltest.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      714 2022-11-07 21:21:52.000000 avocado-framework-99.0/examples/tests/__pycache__/cit_parameters.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      838 2022-11-07 21:19:51.000000 avocado-framework-99.0/examples/tests/__pycache__/doublefail.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      648 2022-11-07 21:19:30.000000 avocado-framework-99.0/examples/tests/__pycache__/errortest.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      986 2022-11-07 21:19:52.000000 avocado-framework-99.0/examples/tests/__pycache__/fail_on_exception.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      649 2022-11-07 21:16:17.000000 avocado-framework-99.0/examples/tests/__pycache__/failtest.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      707 2022-11-07 21:19:48.000000 avocado-framework-99.0/examples/tests/__pycache__/failtest_with_warning.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      831 2022-11-07 21:19:29.000000 avocado-framework-99.0/examples/tests/__pycache__/gendata.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1119 2022-11-07 21:19:54.000000 avocado-framework-99.0/examples/tests/__pycache__/logging_streams.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      622 2022-11-07 21:22:02.000000 avocado-framework-99.0/examples/tests/__pycache__/params.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      605 2022-11-07 21:16:17.000000 avocado-framework-99.0/examples/tests/__pycache__/passtest.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      794 2022-11-07 21:19:45.000000 avocado-framework-99.0/examples/tests/__pycache__/phases.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1158 2022-11-07 21:16:17.000000 avocado-framework-99.0/examples/tests/__pycache__/sleeptenmin.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      774 2022-11-07 21:19:02.000000 avocado-framework-99.0/examples/tests/__pycache__/sleeptest.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      803 2022-11-07 21:20:27.000000 avocado-framework-99.0/examples/tests/__pycache__/sleeptest_async.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      858 2022-11-07 21:19:53.000000 avocado-framework-99.0/examples/tests/__pycache__/timeouttest.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      679 2022-11-07 21:19:51.000000 avocado-framework-99.0/examples/tests/__pycache__/uncaught_exception.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      624 2022-11-07 21:19:30.000000 avocado-framework-99.0/examples/tests/__pycache__/warntest.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      699 2022-11-07 21:19:29.000000 avocado-framework-99.0/examples/tests/__pycache__/whiteboard.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      236 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/tests/abort.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      344 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/assert.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2055 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/assets.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.284127 avocado-framework-99.0/examples/tests/assets.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)     5223 2019-07-23 15:43:52.000000 avocado-framework-99.0/examples/tests/assets.py.data/gnu_hello_signer.gpg
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1036 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/cabort.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.284127 avocado-framework-99.0/examples/tests/cabort.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       50 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/cabort.py.data/abort.c
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      583 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/cancel_on_exception.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      869 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/cancel_test.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      352 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/cancelonsetup.py
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      210 2021-03-04 22:57:12.000000 avocado-framework-99.0/examples/tests/canceltest.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      363 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/cit_parameters.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      166 2022-10-27 20:58:37.000000 avocado-framework-99.0/examples/tests/custom_env_variable.sh
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.284127 avocado-framework-99.0/examples/tests/custom_env_variable.sh.data/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      138 2022-10-27 20:58:37.000000 avocado-framework-99.0/examples/tests/custom_env_variable.sh.data/variants.yaml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      914 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/datadir.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.284127 avocado-framework-99.0/examples/tests/datadir.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       78 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/datadir.py.data/datadir.c
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      757 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/dependency_ansible.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      422 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/doublefail.py
+-rwxrwxr-x   0 cleber    (1000) cleber    (1000)      661 2019-07-23 15:43:52.000000 avocado-framework-99.0/examples/tests/env_variables.sh
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.284127 avocado-framework-99.0/examples/tests/env_variables.sh.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      138 2018-02-12 01:59:15.000000 avocado-framework-99.0/examples/tests/env_variables.sh.data/env_variables.yaml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      274 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/errortest.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      519 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/errortest_nasty.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      565 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/errortest_nasty2.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      541 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/errortest_nasty3.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      655 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/fail_on_exception.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      277 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/failtest.py
+-rwxrwxr-x   0 cleber    (1000) cleber    (1000)       17 2016-10-06 13:45:36.000000 avocado-framework-99.0/examples/tests/failtest.sh
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      331 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/failtest_ugly.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      321 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/failtest_with_warning.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    11698 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/gdbtest.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.284127 avocado-framework-99.0/examples/tests/gdbtest.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      589 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/gdbtest.py.data/return99.c
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       80 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/gdbtest.py.data/segfault.c
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      450 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/gendata.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1339 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/linuxbuild.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.284127 avocado-framework-99.0/examples/tests/linuxbuild.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      150 2020-02-19 20:37:17.000000 avocado-framework-99.0/examples/tests/linuxbuild.py.data/linuxbuild.yaml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1007 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/logging_streams.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1483 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/modify_variable.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.284127 avocado-framework-99.0/examples/tests/modify_variable.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      129 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/modify_variable.py.data/print_variable.c
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      769 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/multiple_tests.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2503 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/multiplextest.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.284127 avocado-framework-99.0/examples/tests/multiplextest.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)     1699 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/multiplextest.py.data/multiplextest.yaml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.285127 avocado-framework-99.0/examples/tests/output_check.sh.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2017-08-24 03:23:42.000000 avocado-framework-99.0/examples/tests/output_check.sh.data/stderr.expected
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       14 2017-08-24 03:23:42.000000 avocado-framework-99.0/examples/tests/output_check.sh.data/stdout.expected
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      275 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/params.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      226 2022-08-11 17:38:14.000000 avocado-framework-99.0/examples/tests/passtest.py
+-rwxrwxr-x   0 cleber    (1000) cleber    (1000)       16 2016-10-06 13:45:36.000000 avocado-framework-99.0/examples/tests/passtest.sh
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      264 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/passtest_with_dependency.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      327 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/phases.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      499 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/property.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1486 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/raise.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.285127 avocado-framework-99.0/examples/tests/raise.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      649 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/raise.py.data/raise.c
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      292 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/raise.py.data/raise.yaml
+-rwxrwxr-x   0 cleber    (1000) cleber    (1000)      340 2016-06-01 19:09:56.000000 avocado-framework-99.0/examples/tests/simplewarning.sh
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1039 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/skip_conditional.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      863 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/sleeptenmin.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.285127 avocado-framework-99.0/examples/tests/sleeptenmin.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      394 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/sleeptenmin.py.data/sleeptenmin.yaml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      411 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/sleeptest.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.285127 avocado-framework-99.0/examples/tests/sleeptest.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      493 2021-03-04 22:57:12.000000 avocado-framework-99.0/examples/tests/sleeptest.py.data/sleeptest.json
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      118 2020-07-21 15:22:36.000000 avocado-framework-99.0/examples/tests/sleeptest.py.data/sleeptest.yaml
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      115 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/tests/sleeptest.sh
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.285127 avocado-framework-99.0/examples/tests/sleeptest.sh.data/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      118 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/tests/sleeptest.sh.data/sleeptest.yaml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      434 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/sleeptest_async.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1451 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/synctest.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.285127 avocado-framework-99.0/examples/tests/synctest.py.data/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2017-11-27 16:06:12.000000 avocado-framework-99.0/examples/tests/synctest.py.data/stderr.expected
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       39 2017-11-27 16:06:06.000000 avocado-framework-99.0/examples/tests/synctest.py.data/stdout.expected
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)     1666 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/synctest.py.data/synctest.tar.bz2
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      265 2016-04-28 15:01:56.000000 avocado-framework-99.0/examples/tests/synctest.py.data/synctest.yaml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2142 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/test_env.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      486 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/timeouttest.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      301 2022-10-07 18:12:16.000000 avocado-framework-99.0/examples/tests/uncaught_exception.py
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      249 2021-03-04 22:57:12.000000 avocado-framework-99.0/examples/tests/warntest.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      356 2022-11-04 17:27:10.000000 avocado-framework-99.0/examples/tests/whiteboard.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.286127 avocado-framework-99.0/examples/varianter_cit/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      380 2021-02-11 22:50:38.000000 avocado-framework-99.0/examples/varianter_cit/params.cit
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      224 2021-02-11 22:50:38.000000 avocado-framework-99.0/examples/varianter_cit/test_params.cit
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.286127 avocado-framework-99.0/examples/varianter_pict/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      132 2019-07-19 21:00:45.000000 avocado-framework-99.0/examples/varianter_pict/params.pict
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.286127 avocado-framework-99.0/examples/yaml_to_mux/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      330 2019-07-19 21:00:45.000000 avocado-framework-99.0/examples/yaml_to_mux/complex.yaml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.286127 avocado-framework-99.0/examples/yaml_to_mux/hw/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      344 2019-07-19 21:00:45.000000 avocado-framework-99.0/examples/yaml_to_mux/hw/hw.yaml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.286127 avocado-framework-99.0/examples/yaml_to_mux/os/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      298 2019-07-19 21:00:45.000000 avocado-framework-99.0/examples/yaml_to_mux/os/linux.yaml
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      111 2019-07-19 21:00:45.000000 avocado-framework-99.0/examples/yaml_to_mux/os/windows.yaml
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       80 2019-07-19 21:00:45.000000 avocado-framework-99.0/examples/yaml_to_mux/simple.yaml
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      108 2019-07-19 21:00:45.000000 avocado-framework-99.0/examples/yaml_to_mux/simple_vars.yaml
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      602 2019-07-19 21:00:45.000000 avocado-framework-99.0/examples/yaml_to_mux/types.yaml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.287127 avocado-framework-99.0/selftests/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.289127 avocado-framework-99.0/selftests/.data/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.289127 avocado-framework-99.0/selftests/.data/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2004 2022-11-07 21:20:26.000000 avocado-framework-99.0/selftests/.data/__pycache__/get_data.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8587 2022-11-07 21:20:20.000000 avocado-framework-99.0/selftests/.data/__pycache__/test_statuses.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1126 2022-11-07 21:17:06.000000 avocado-framework-99.0/selftests/.data/__pycache__/unittests.cpython-310.pyc
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       36 2019-07-23 15:43:52.000000 avocado-framework-99.0/selftests/.data/avocado.gz
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       64 2021-02-11 22:50:38.000000 avocado-framework-99.0/selftests/.data/avocado.xz
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       46 2019-07-23 15:43:52.000000 avocado-framework-99.0/selftests/.data/empty.tar.bz2
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3376 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/.data/get_data.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.289127 avocado-framework-99.0/selftests/.data/get_data.py.data/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.289127 avocado-framework-99.0/selftests/.data/get_data.py.data/GetData.test_a/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.290127 avocado-framework-99.0/selftests/.data/get_data.py.data/GetData.test_a/long-cbbd/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       12 2019-07-19 21:00:45.000000 avocado-framework-99.0/selftests/.data/get_data.py.data/GetData.test_a/long-cbbd/variant_data
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.290127 avocado-framework-99.0/selftests/.data/get_data.py.data/GetData.test_a/medium-1a7a/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       12 2019-07-19 21:00:45.000000 avocado-framework-99.0/selftests/.data/get_data.py.data/GetData.test_a/medium-1a7a/variant_data
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.290127 avocado-framework-99.0/selftests/.data/get_data.py.data/GetData.test_a/short-475e/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       12 2019-07-19 21:00:45.000000 avocado-framework-99.0/selftests/.data/get_data.py.data/GetData.test_a/short-475e/variant_data
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2019-07-19 21:00:45.000000 avocado-framework-99.0/selftests/.data/get_data.py.data/GetData.test_a/test_data
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.290127 avocado-framework-99.0/selftests/.data/get_data.py.data/GetData.test_b/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2019-07-19 21:00:45.000000 avocado-framework-99.0/selftests/.data/get_data.py.data/GetData.test_b/test_data
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       11 2019-07-19 21:00:45.000000 avocado-framework-99.0/selftests/.data/get_data.py.data/file_data
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      354 2021-02-11 22:50:38.000000 avocado-framework-99.0/selftests/.data/get_data.py.data/get_data.json
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       83 2019-07-19 21:00:45.000000 avocado-framework-99.0/selftests/.data/get_data.py.data/get_data.yaml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      150 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/guaca.a
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    56132 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/hello.deb
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    71999 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/hello.rpm
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)     6108 2019-07-19 21:00:45.000000 avocado-framework-99.0/selftests/.data/jenkins-junit.xsd
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.250127 avocado-framework-99.0/selftests/.data/safeloader/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.290127 avocado-framework-99.0/selftests/.data/safeloader/caveat_multilevel/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       82 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/caveat_multilevel/failure.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.290127 avocado-framework-99.0/selftests/.data/safeloader/caveat_multilevel/l1/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/caveat_multilevel/l1/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.290127 avocado-framework-99.0/selftests/.data/safeloader/caveat_multilevel/l1/l2/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/caveat_multilevel/l1/l2/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.290127 avocado-framework-99.0/selftests/.data/safeloader/caveat_multilevel/l1/l2/l3/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       90 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/caveat_multilevel/l1/l2/l3/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       87 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/caveat_multilevel/success.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.291128 avocado-framework-99.0/selftests/.data/safeloader/data/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1236 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/.data/safeloader/data/dont_crash.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      713 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/.data/safeloader/data/dont_detect_non_avocado.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      385 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/.data/safeloader/data/double_import.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1579 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/.data/safeloader/data/imports.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      156 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/infinite_recurse.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       78 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/parent1.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       78 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/parent4.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       78 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/parent7.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       78 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/parent9.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.292127 avocado-framework-99.0/selftests/.data/safeloader/data/path/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/path/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       79 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/path/parent10.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       78 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/path/parent2.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       78 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/path/parent3.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       78 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/path/parent5.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       78 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/path/parent6.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       78 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/safeloader/data/path/parent8.py
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)   378880 2019-07-19 21:00:45.000000 avocado-framework-99.0/selftests/.data/sample.iso
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)     1313 2017-06-27 20:18:38.000000 avocado-framework-99.0/selftests/.data/test_archive__symlinks.zip
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7200 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/.data/test_statuses.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      438 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/.data/unittests.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)     1383 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/.data/whiteboard.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.292127 avocado-framework-99.0/selftests/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      147 2022-11-07 21:15:56.000000 avocado-framework-99.0/selftests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    15522 2022-11-07 21:16:07.000000 avocado-framework-99.0/selftests/__pycache__/check.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5050 2022-11-07 21:15:56.000000 avocado-framework-99.0/selftests/__pycache__/utils.cpython-310.pyc
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)    29326 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/check.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      909 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/check_tmp_dirs
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.292127 avocado-framework-99.0/selftests/deployment/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3056 2022-10-26 14:58:28.000000 avocado-framework-99.0/selftests/deployment/README.rst
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       74 2019-11-19 20:03:57.000000 avocado-framework-99.0/selftests/deployment/ansible.cfg
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      161 2021-02-11 22:50:38.000000 avocado-framework-99.0/selftests/deployment/deployment.yml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.292127 avocado-framework-99.0/selftests/deployment/group_vars/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       45 2021-02-11 22:50:38.000000 avocado-framework-99.0/selftests/deployment/group_vars/all
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       18 2021-08-18 18:06:49.000000 avocado-framework-99.0/selftests/deployment/inventory
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.250127 avocado-framework-99.0/selftests/deployment/roles/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.250127 avocado-framework-99.0/selftests/deployment/roles/avocado/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.293127 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.293127 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/copr/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      161 2021-03-04 22:57:12.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/copr/avocado.yml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      292 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/copr/examples.yml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      849 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/copr/plugins.yml
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      456 2021-03-04 22:57:12.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/main.yml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.293127 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/official/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      161 2021-03-04 22:57:12.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/official/avocado.yml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      292 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/official/examples.yml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      849 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/official/plugins.yml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.293127 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/pip/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      219 2021-03-04 22:57:12.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/pip/avocado.yml
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      144 2021-03-04 22:57:12.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/pip/examples.yml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2016 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/pip/plugins.yml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.294128 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/rpm/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      161 2021-03-04 22:57:12.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/rpm/avocado.yml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      292 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/rpm/examples.yml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      849 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/rpm/plugins.yml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.250127 avocado-framework-99.0/selftests/deployment/roles/common/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.294128 avocado-framework-99.0/selftests/deployment/roles/common/tasks/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      204 2021-03-04 22:57:12.000000 avocado-framework-99.0/selftests/deployment/roles/common/tasks/aexpect.yml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      695 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/deployment/roles/common/tasks/dependencies.yml
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       76 2021-02-11 22:50:38.000000 avocado-framework-99.0/selftests/deployment/roles/common/tasks/main.yml
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2500 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/deployment/roles/common/tasks/repos.yml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.250127 avocado-framework-99.0/selftests/deployment/roles/tests/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.294128 avocado-framework-99.0/selftests/deployment/roles/tests/tasks/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1932 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/deployment/roles/tests/tasks/main.yml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.250127 avocado-framework-99.0/selftests/deployment/roles/virtualenv/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.294128 avocado-framework-99.0/selftests/deployment/roles/virtualenv/tasks/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      266 2021-02-11 22:50:38.000000 avocado-framework-99.0/selftests/deployment/roles/virtualenv/tasks/main.yml
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)      301 2021-02-11 22:50:38.000000 avocado-framework-99.0/selftests/deployment/vars.yml
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.297128 avocado-framework-99.0/selftests/functional/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2021-10-16 20:28:12.000000 avocado-framework-99.0/selftests/functional/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.301128 avocado-framework-99.0/selftests/functional/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      158 2022-11-07 21:17:38.000000 avocado-framework-99.0/selftests/functional/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3103 2022-11-07 21:20:19.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_argument_parsing.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    42614 2022-11-07 21:19:40.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_basic.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1063 2022-11-07 21:20:21.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_coroutine.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1901 2022-11-07 21:19:13.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_export_variables.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4421 2022-11-07 21:19:14.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_fetch_asset.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1372 2022-11-07 21:20:21.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_getdata.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7653 2022-11-07 21:19:13.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_interrupt.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1817 2022-11-07 21:19:15.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_job_api_features.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6005 2022-11-07 21:20:22.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_job_timeout.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2345 2022-11-07 21:19:20.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_journal.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2579 2022-11-07 21:19:13.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_json_variants.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8980 2022-11-07 21:19:15.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_list.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4877 2022-11-07 21:19:20.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_lv_utils.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7487 2022-11-07 21:20:24.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_nrunner.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4597 2022-11-07 21:16:28.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_nrunner_interface.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    18745 2022-11-07 21:19:23.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_output.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    13479 2022-11-07 21:19:29.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_output_check.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3201 2022-11-07 21:19:32.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_replay.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2758 2022-11-07 21:19:33.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_requirements_cache.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4351 2022-11-07 21:19:33.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_resolver.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2518 2022-11-07 21:19:19.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_runner_asset.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2630 2022-11-07 21:19:35.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_runner_package.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    11149 2022-11-07 21:20:10.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_skiptests.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1827 2022-11-07 21:19:13.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_software_manager.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3640 2022-11-07 21:20:10.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_statuses.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4750 2022-11-07 21:19:37.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_streams.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4084 2022-11-07 21:20:12.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_sysinfo.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1551 2022-11-07 21:19:39.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_task_statemachine.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1611 2022-11-07 21:20:18.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_task_timeout.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3169 2022-11-07 21:19:13.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_teststmpdir.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1909 2022-11-07 21:19:14.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_thirdparty_bugs.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3630 2022-11-07 21:19:39.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_unittest_compat.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6789 2022-11-08 22:10:38.000000 avocado-framework-99.0/selftests/functional/__pycache__/test_utils.cpython-310.pyc
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.302127 avocado-framework-99.0/selftests/functional/plugin/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.302127 avocado-framework-99.0/selftests/functional/plugin/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      165 2022-11-07 21:17:38.000000 avocado-framework-99.0/selftests/functional/plugin/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9540 2022-11-07 21:20:33.000000 avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_assets.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1069 2022-11-07 21:20:36.000000 avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_bystatus.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2525 2022-11-07 21:20:36.000000 avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_diff.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3731 2022-11-07 21:20:37.000000 avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_jobscripts.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1965 2022-11-07 21:20:38.000000 avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_jsonresult.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3874 2022-11-07 21:20:41.000000 avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_logs.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1076 2022-11-07 21:20:45.000000 avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_podman_image.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3286 2022-11-07 21:17:38.000000 avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_vmimage.cpython-310.pyc
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.303128 avocado-framework-99.0/selftests/functional/plugin/spawners/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/spawners/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.303128 avocado-framework-99.0/selftests/functional/plugin/spawners/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2768 2022-11-07 21:20:44.000000 avocado-framework-99.0/selftests/functional/plugin/spawners/__pycache__/test_podman.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1325 2022-11-07 21:20:44.000000 avocado-framework-99.0/selftests/functional/plugin/spawners/__pycache__/test_process.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2594 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/spawners/test_podman.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      951 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/spawners/test_process.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    12450 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/test_assets.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      788 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/test_bystatus.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2458 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/test_diff.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4426 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/test_jobscripts.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1858 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/test_jsonresult.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3474 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/test_logs.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      775 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/test_podman_image.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2935 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/plugin/test_vmimage.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.303128 avocado-framework-99.0/selftests/functional/serial/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.303128 avocado-framework-99.0/selftests/functional/serial/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5014 2022-11-07 21:16:50.000000 avocado-framework-99.0/selftests/functional/serial/__pycache__/test_requirements.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5839 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/serial/test_requirements.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2951 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_argument_parsing.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    48414 2022-11-04 18:41:09.000000 avocado-framework-99.0/selftests/functional/test_basic.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      731 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_coroutine.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1323 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_export_variables.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5442 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_fetch_asset.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1154 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_getdata.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10204 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_interrupt.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1321 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_job_api_features.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7129 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_job_timeout.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2049 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_journal.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2404 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_json_variants.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10228 2022-11-10 18:19:16.000000 avocado-framework-99.0/selftests/functional/test_list.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5927 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_lv_utils.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8680 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_nrunner.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4458 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.305127 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1130 2022-10-27 21:06:44.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/capabilities.schema.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       17 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       84 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_avocado_instrumented.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       20 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_dry_run.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       72 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_exec_test.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       17 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_noop.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       99 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_python_unittest.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       87 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_robot.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       58 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_runnable_tap.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       42 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_task.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      109 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_avocado_instrumented.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       45 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_dry_run.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       97 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_exec_test.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       42 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_noop.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      124 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_python_unittest.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      112 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_robot.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       83 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/recipe_task_tap.json
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    22884 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_output.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    17925 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_output_check.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2870 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_replay.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3731 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_requirements_cache.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4436 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_resolver.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2304 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_runner_asset.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2565 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_runner_package.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10472 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_skiptests.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1379 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_software_manager.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6472 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_statuses.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5273 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_streams.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5422 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_sysinfo.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1267 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_task_statemachine.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1102 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_task_timeout.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3114 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_teststmpdir.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2105 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_thirdparty_bugs.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3714 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/test_unittest_compat.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6398 2022-11-08 20:36:22.000000 avocado-framework-99.0/selftests/functional/test_utils.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.305127 avocado-framework-99.0/selftests/functional/utils/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/utils/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.305127 avocado-framework-99.0/selftests/functional/utils/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6448 2022-11-07 21:20:30.000000 avocado-framework-99.0/selftests/functional/utils/__pycache__/test_asset.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1296 2022-11-07 21:20:36.000000 avocado-framework-99.0/selftests/functional/utils/__pycache__/test_podman.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7895 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/utils/test_asset.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1168 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/functional/utils/test_podman.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      282 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/isort.sh
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.306128 avocado-framework-99.0/selftests/jobs/
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      466 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/jobs/example_passjob
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      358 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/jobs/example_passjob_cit_varianter
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      331 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/jobs/example_passjob_html
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      369 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/jobs/example_sleepjob_dict_varianter
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      369 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/jobs/example_sleepjob_json_varianter
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      785 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/jobs/example_unix_status_server
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      465 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/jobs/pass
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      739 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/jobs/status_server_auto
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      994 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/jobs/status_server_different_uri_listen
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.306128 avocado-framework-99.0/selftests/jobs/tests/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.306128 avocado-framework-99.0/selftests/jobs/tests/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      611 2022-11-07 21:18:59.000000 avocado-framework-99.0/selftests/jobs/tests/__pycache__/passtest.cpython-310.pyc
+-rwxrwxr-x   0 cleber    (1000) cleber    (1000)       17 2021-03-04 22:57:12.000000 avocado-framework-99.0/selftests/jobs/tests/pass
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      226 2022-08-11 17:38:14.000000 avocado-framework-99.0/selftests/jobs/tests/passtest.py
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)     1550 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/lint.sh
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)     1265 2022-10-27 20:58:37.000000 avocado-framework-99.0/selftests/modules-boundaries.sh
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.251127 avocado-framework-99.0/selftests/pre_release/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.307128 avocado-framework-99.0/selftests/pre_release/jobs/
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)     1057 2022-11-10 18:19:16.000000 avocado-framework-99.0/selftests/pre_release/jobs/pre_release.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.307128 avocado-framework-99.0/selftests/pre_release/tests/
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.307128 avocado-framework-99.0/selftests/pre_release/tests/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      795 2022-11-08 22:09:20.000000 avocado-framework-99.0/selftests/pre_release/tests/__pycache__/cirrusci.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1210 2022-11-08 16:45:53.000000 avocado-framework-99.0/selftests/pre_release/tests/__pycache__/readthedocs.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3980 2022-11-08 22:56:40.000000 avocado-framework-99.0/selftests/pre_release/tests/__pycache__/vmimage.cpython-310.pyc
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)     1103 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/pre_release/tests/check-copr-rpm-version.sh
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      462 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/pre_release/tests/cirrusci.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1082 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/pre_release/tests/readthedocs.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2938 2022-11-09 20:21:55.000000 avocado-framework-99.0/selftests/pre_release/tests/vmimage.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.307128 avocado-framework-99.0/selftests/pre_release/tests/vmimage.py.data/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2846 2022-11-08 20:36:22.000000 avocado-framework-99.0/selftests/pre_release/tests/vmimage.py.data/variants.yml
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      424 2022-10-27 21:06:44.000000 avocado-framework-99.0/selftests/run
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      926 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/run_coverage
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)     1068 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/safeloader.sh
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      318 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/signedoff-check.sh
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)      228 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/spell.sh
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)       72 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/style.sh
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.311128 avocado-framework-99.0/selftests/unit/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-06-21 14:31:52.000000 avocado-framework-99.0/selftests/unit/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.314128 avocado-framework-99.0/selftests/unit/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      152 2022-11-07 21:17:19.000000 avocado-framework-99.0/selftests/unit/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7183 2022-11-07 21:16:58.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_datadir.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1152 2022-11-07 21:16:58.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_dependencies_resolver.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1473 2022-11-07 21:16:58.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_dispatcher.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2199 2022-11-07 21:16:58.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_hintfiles.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    12750 2022-11-07 21:16:58.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_job.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8715 2022-11-07 21:17:01.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_loader.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    19673 2022-11-07 21:17:03.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_nrunner.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1411 2022-11-07 21:17:07.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_output.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1547 2022-11-07 21:17:08.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_parameters.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1898 2022-11-07 21:17:08.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_parser.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2490 2022-11-07 21:17:08.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_plugin_interfaces.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1230 2022-11-07 21:17:09.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_references.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2324 2022-11-07 21:17:10.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_result.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3241 2022-11-07 21:17:10.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_runner_asset.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5734 2022-11-07 21:17:11.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_runner_package.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1944 2022-11-07 21:17:11.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_runner_sysinfo.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1060 2022-11-07 21:17:12.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_caveats.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9089 2022-11-07 21:17:12.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_core.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6658 2022-11-07 21:17:13.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_docstring.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9634 2022-11-07 21:17:15.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_imported.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3950 2022-11-07 21:17:19.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_module.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1901 2022-11-07 21:17:20.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_utils.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6294 2022-11-07 21:17:20.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_settings.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6215 2022-11-07 21:17:22.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_status_repo.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1239 2022-11-07 21:17:24.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_status_utils.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3086 2022-11-07 21:17:24.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_suite.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2941 2022-11-07 21:17:24.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_sysinfo.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    11446 2022-11-07 21:17:25.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_tags.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10077 2022-11-07 21:17:28.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_tap.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3716 2022-11-07 21:17:31.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_task_runtime.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7200 2022-11-07 21:16:40.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_test.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3951 2022-11-07 21:17:33.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_test_id.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2988 2022-11-07 21:17:33.000000 avocado-framework-99.0/selftests/unit/__pycache__/test_tree.cpython-310.pyc
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.315127 avocado-framework-99.0/selftests/unit/plugin/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/plugin/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.315127 avocado-framework-99.0/selftests/unit/plugin/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7521 2022-11-07 21:17:34.000000 avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_assets.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4293 2022-11-07 21:17:35.000000 avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_jsonresult.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6783 2022-11-07 21:17:35.000000 avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_resolver.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2365 2022-11-07 21:17:37.000000 avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_spawner.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7473 2022-11-07 21:17:38.000000 avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_vmimage.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7483 2022-11-07 21:17:38.000000 avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_xunit.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10006 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/plugin/test_assets.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4168 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/plugin/test_jsonresult.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6830 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/plugin/test_resolver.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2089 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/plugin/test_spawner.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8483 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/plugin/test_vmimage.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5858 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/plugin/test_xunit.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9281 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_datadir.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1037 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_dependencies_resolver.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1158 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_dispatcher.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1844 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_hintfiles.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    14519 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_job.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10967 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_loader.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    20400 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_nrunner.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      911 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_output.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2285 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_parameters.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1015 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_parser.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2036 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_plugin_interfaces.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      832 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_references.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1908 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_result.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2828 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_runner_asset.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6966 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_runner_package.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2204 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_runner_sysinfo.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      741 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_safeloader_caveats.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10254 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_safeloader_core.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6611 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_safeloader_docstring.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8371 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_safeloader_imported.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3106 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_safeloader_module.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1293 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_safeloader_utils.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6537 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_settings.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7883 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_status_repo.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      617 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_status_utils.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2882 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_suite.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3248 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_sysinfo.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    13253 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_tags.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    12312 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_tap.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3740 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_task_runtime.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6667 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_test.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3605 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_test_id.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2638 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/test_tree.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.318127 avocado-framework-99.0/selftests/unit/utils/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        0 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.321128 avocado-framework-99.0/selftests/unit/utils/__pycache__/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1896 2022-11-07 21:17:38.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_ar.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8834 2022-11-07 21:17:39.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_archive.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5324 2022-11-07 21:17:42.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_astring.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3945 2022-11-07 21:17:42.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_cloudinit.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     9295 2022-11-07 21:17:43.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_cpu.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5633 2022-11-07 21:17:46.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_data_structures.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4109 2022-11-07 21:17:48.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_datadrainer.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4303 2022-11-07 21:17:48.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_diff_validator.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3278 2022-11-07 21:17:49.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_disk.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3538 2022-11-07 21:17:49.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_distro.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2075 2022-11-07 21:17:50.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_filelock.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1574 2022-11-07 21:17:51.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_gdb.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2197 2022-11-07 21:17:51.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_genio.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6257 2022-11-07 21:17:52.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_iso9660.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1348 2022-11-07 21:17:53.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_kernel.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2624 2022-11-07 21:17:53.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_linux_modules.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3905 2022-11-07 21:17:54.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_memory.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2976 2022-11-07 21:17:55.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_network.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1328 2022-11-07 21:17:56.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_output.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7848 2022-11-07 21:17:56.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_partition.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1926 2022-11-07 21:17:57.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_path.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1609 2022-11-07 21:17:58.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_pci.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      814 2022-11-07 21:17:58.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_pmem.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    25651 2022-11-07 21:17:58.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_process.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      942 2022-11-07 21:18:05.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_script.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10086 2022-11-07 21:18:05.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_service.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1872 2022-11-07 21:18:08.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_software_manager.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2924 2022-11-07 21:18:08.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_ssh.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3030 2022-11-07 21:18:10.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_stacktrace.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    31717 2022-11-07 21:18:10.000000 avocado-framework-99.0/selftests/unit/utils/__pycache__/test_vmimage.cpython-310.pyc
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1398 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_ar.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8992 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_archive.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6348 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_astring.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2827 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_cloudinit.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    10232 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.322128 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      335 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/armv7
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      221 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/armv8
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      852 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/i386
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      286 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/power8
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      251 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/power9
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       72 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/risc_v
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1182 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/s390x
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1494 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/s390x_2
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3144 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/s390x_3
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8991 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/x86_64
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5193 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_data_structures.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2448 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_datadrainer.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5752 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_diff_validator.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2870 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_disk.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2261 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_distro.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1185 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_filelock.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1220 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_gdb.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1732 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_genio.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5752 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_iso9660.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      866 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_kernel.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2143 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_linux_modules.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:41.322128 avocado-framework-99.0/selftests/unit/utils/test_linux_modules.py.data/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      752 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_linux_modules.py.data/lsmod
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7153 2022-10-07 18:12:16.000000 avocado-framework-99.0/selftests/unit/utils/test_linux_modules.py.data/proc_modules
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3956 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_memory.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2201 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_network.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1170 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_output.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8133 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_partition.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1338 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_path.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1476 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_pci.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      340 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_pmem.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    31526 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_process.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      541 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_script.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    12716 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_service.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1215 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_software_manager.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2408 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_ssh.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2932 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_stacktrace.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    32272 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/unit/utils/test_vmimage.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5138 2022-11-04 17:27:10.000000 avocado-framework-99.0/selftests/utils.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2022-11-10 19:12:41.323128 avocado-framework-99.0/setup.cfg
+-rwxr-xr-x   0 cleber    (1000) cleber    (1000)    17941 2022-11-04 17:27:10.000000 avocado-framework-99.0/setup.py
```

### Comparing `avocado-framework-98.0/LICENSE` & `avocado-framework-99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/Makefile` & `avocado-framework-99.0/Makefile`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/PKG-INFO` & `avocado-framework-99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avocado-framework
-Version: 98.0
+Version: 99.0
 Summary: Avocado Test Framework
 Home-page: https://avocado-framework.github.io/
 Author: Avocado Developers
 Author-email: avocado-devel@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `avocado-framework-98.0/README` & `avocado-framework-99.0/README`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/README.rst` & `avocado-framework-99.0/README.rst`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/__init__.py` & `avocado-framework-99.0/avocado/__init__.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/__init__.py` & `avocado-framework-99.0/avocado/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -267,15 +267,17 @@
 
     help_msg = (
         "Selects the runner implementation from one of the "
         "installed and active implementations.  You can run "
         '"avocado plugins" and find the list of valid runners '
         'under the "Plugins that run test suites on a job '
         '(runners) section.  Defaults to "nrunner", which is '
-        "the new runner and only runner supported at this moment."
+        "the new runner and only runner supported at this moment. "
+        "This option name is currently DEPRECATED and will be "
+        'renamed to "run.suite_runner" on Avocado 100.0 and later.'
     )
     stgs.register_option(
         section="run", key="test_runner", default="nrunner", help_msg=help_msg
     )
 
 
 def initialize_plugin_infrastructure():
```

### Comparing `avocado-framework-98.0/avocado/core/app.py` & `avocado-framework-99.0/avocado/core/app.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/data_dir.py` & `avocado-framework-99.0/avocado/core/data_dir.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/decorators.py` & `avocado-framework-99.0/avocado/core/decorators.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/dependencies/requirements/cache/backends/sqlite.py` & `avocado-framework-99.0/avocado/core/dependencies/requirements/cache/backends/sqlite.py`

 * *Files 13% similar despite different names*

```diff
@@ -329,7 +329,39 @@
 
         for row in result.fetchall():
             if row[0] in requirements:
                 requirements[row[0]].append((row[1], row[2]))
             else:
                 requirements[row[0]] = [(row[1], row[2])]
     return requirements
+
+
+def get_all_requirements():
+    """Fetches all requirements from database.
+
+    :return: Dict with all environments which has requirements.
+
+    """
+    requirements = {}
+    if not os.path.exists(CACHE_DATABASE_PATH):
+        return requirements
+
+    sql = "SELECT * FROM requirement"
+
+    with sqlite3.connect(
+        CACHE_DATABASE_PATH, detect_types=sqlite3.PARSE_DECLTYPES
+    ) as conn:
+        cursor = conn.cursor()
+        result = cursor.execute(sql)
+
+        for row in result.fetchall():
+            environment_type = row[0]
+            if environment_type not in requirements:
+                requirements[environment_type] = []
+            requirements[environment_type].append(
+                {
+                    "environment": row[1],
+                    "requirement_type": row[2],
+                    "requirement": row[3],
+                }
+            )
+    return requirements
```

### Comparing `avocado-framework-98.0/avocado/core/dispatcher.py` & `avocado-framework-99.0/avocado/core/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,7 +140,12 @@
             "avocado.plugins.spawner", invoke_kwds={"job": job, "config": config}
         )
 
 
 class RunnableRunnerDispatcher(EnabledExtensionManager):
     def __init__(self):
         super().__init__("avocado.plugins.runnable.runner")
+
+
+class CacheDispatcher(EnabledExtensionManager):
+    def __init__(self):
+        super().__init__("avocado.plugins.cache")
```

### Comparing `avocado-framework-98.0/avocado/core/enabled_extension_manager.py` & `avocado-framework-99.0/avocado/core/enabled_extension_manager.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/exceptions.py` & `avocado-framework-99.0/avocado/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/exit_codes.py` & `avocado-framework-99.0/avocado/core/exit_codes.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/extension_manager.py` & `avocado-framework-99.0/avocado/core/extension_manager.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/job.py` & `avocado-framework-99.0/avocado/core/job.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/job_id.py` & `avocado-framework-99.0/avocado/core/job_id.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/jobdata.py` & `avocado-framework-99.0/avocado/core/jobdata.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/loader.py` & `avocado-framework-99.0/avocado/core/loader.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/main.py` & `avocado-framework-99.0/avocado/core/main.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/messages.py` & `avocado-framework-99.0/avocado/core/messages.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/nrunner/app.py` & `avocado-framework-99.0/avocado/core/nrunner/app.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/nrunner/config.py` & `avocado-framework-99.0/avocado/core/nrunner/config.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/nrunner/runnable.py` & `avocado-framework-99.0/avocado/core/nrunner/runnable.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,27 +64,27 @@
     Describes an entity that be executed in the context of a task
 
     A instance of :class:`BaseRunner` is the entity that will actually
     execute a runnable.
     """
 
     def __init__(self, kind, uri, *args, config=None, **kwargs):
-        if config is None:
-            config = self.filter_runnable_config(kind, {})
         self.kind = kind
         #: The main reference to what needs to be run.  This is free
         #: form, but commonly set to the path to a file containing the
         #: test or being the test, or an actual URI with multiple
         #: parts
         self.uri = uri
         #: This attributes holds configuration from Avocado proper
         #: that is passed to runners, as long as a runner declares
         #: its interest in using them with
         #: attr:`avocado.core.nrunner.runner.BaseRunner.CONFIGURATION_USED`
         self._config = {}
+        if config is None:
+            config = self.filter_runnable_config(kind, {})
         self.config = config or {}
         self.args = args
         self.tags = kwargs.pop("tags", None)
         self.dependencies = kwargs.pop("dependencies", None)
         self.variant = kwargs.pop("variant", None)
         self.output_dir = kwargs.pop("output_dir", None)
         self.kwargs = kwargs
@@ -166,26 +166,23 @@
         This is not avocado config, it is a runnable config which is a subset
         of avocado config based on `STANDALONE_EXECUTABLE_CONFIG_USED` which
         describes essential configuration values for each runner kind.
 
         :param config: A config dict with new values for Runnable.
         :type config: dict
         """
-        command = self.pick_runner_command(self.kind)
-        if command is not None:
-            command = " ".join(command)
-            configuration_used = STANDALONE_EXECUTABLE_CONFIG_USED.get(command)
-            if not set(configuration_used).issubset(set(config.keys())):
-                LOG.warning(
-                    "The runnable config should have only values "
-                    "essential for its runner. In the next version of "
-                    "avocado, this will raise a Value Error. Please "
-                    "use avocado.core.nrunner.runnable.Runnable.filter_runnable_config "
-                    "or avocado.core.nrunner.runnable.Runnable.from_avocado_config"
-                )
+        configuration_used = Runnable.get_configuration_used_by_kind(self.kind)
+        if not set(configuration_used).issubset(set(config.keys())):
+            LOG.warning(
+                "The runnable config should have only values "
+                "essential for its runner. In the next version of "
+                "avocado, this will raise a Value Error. Please "
+                "use avocado.core.nrunner.runnable.Runnable.filter_runnable_config "
+                "or avocado.core.nrunner.runnable.Runnable.from_avocado_config"
+            )
         self._config = config
 
     @classmethod
     def from_args(cls, args):
         """Returns a runnable from arguments"""
         decoded_args = [_arg_decode_base64(arg) for arg in args.get("arg", ())]
         return cls.from_avocado_config(
@@ -220,16 +217,36 @@
     def from_avocado_config(cls, kind, uri, *args, config=None, **kwargs):
         """Creates runnable with only essential config for runner of specific kind."""
         if not config:
             config = {}
         config = cls.filter_runnable_config(kind, config)
         return cls(kind, uri, *args, config=config, **kwargs)
 
-    @staticmethod
-    def filter_runnable_config(kind, config):
+    @classmethod
+    def get_configuration_used_by_kind(cls, kind):
+        """Returns the configuration used by a runner of a given kind
+
+        :param kind: Kind of runner which should use the configuration.
+        :type kind: str
+        :returns: the configuration used by a runner of a given kind
+        :rtype: list
+        """
+        configuration_used = []
+        klass = cls.pick_runner_class_from_entry_point_kind(kind)
+        if klass is not None:
+            configuration_used = klass.CONFIGURATION_USED
+        else:
+            command = Runnable.pick_runner_command(kind)
+            if command is not None:
+                command = " ".join(command)
+                configuration_used = STANDALONE_EXECUTABLE_CONFIG_USED.get(command)
+        return configuration_used
+
+    @classmethod
+    def filter_runnable_config(cls, kind, config):
         """
         Returns only essential values for specific runner.
 
         It will use configuration from argument completed by values from
         config file and avocado default configuration.
 
         :param kind: Kind of runner which should use the configuration.
@@ -238,26 +255,21 @@
                        missing the default ones and from config file will be
                        used.
         :type config: dict
         :returns: Config dict, which has only values essential for runner
                   based on STANDALONE_EXECUTABLE_CONFIG_USED
         :rtype: dict
         """
-        command = Runnable.pick_runner_command(kind)
-        if command is not None:
-            whole_config = settings.as_dict()
-            whole_config.update(config)
-            command = " ".join(command)
-            configuration_used = STANDALONE_EXECUTABLE_CONFIG_USED.get(command)
-            filtered_config = {}
-            for config_item in configuration_used:
-                filtered_config[config_item] = whole_config.get(config_item)
-            return filtered_config
-        else:
-            raise ValueError(f"Unsupported kind of runnable: {kind}")
+        whole_config = settings.as_dict()
+        filtered_config = {}
+        for config_item in cls.get_configuration_used_by_kind(kind):
+            filtered_config[config_item] = config.get(
+                config_item, whole_config.get(config_item)
+            )
+        return filtered_config
 
     def get_command_args(self):
         """
         Returns the command arguments that adhere to the runner interface
 
         This is useful for building 'runnable-run' and 'task-run' commands
         that can be executed on a command line interface.
@@ -430,15 +442,15 @@
             return None
         if runner_cmd is not None:
             return runner_cmd
 
         # When running Avocado Python modules, the interpreter on the new
         # process needs to know where Avocado can be found.
         env = os.environ.copy()
-        env["PYTHONPATH"] = ":".join(p for p in sys.path)
+        env["PYTHONPATH"] = ":".join(p for p in set(sys.path))
 
         standalone_executable_cmd = [f"avocado-runner-{kind}"]
         if Runnable.is_kind_supported_by_runner_command(
             kind, standalone_executable_cmd
         ):
             runners_registry[kind] = standalone_executable_cmd
             return standalone_executable_cmd
@@ -483,37 +495,46 @@
                                  found) runners keyed by runnable kind
         :type runners_registry: dict
         :returns: command line arguments to execute the runner
         :rtype: list of str or None
         """
         return Runnable.pick_runner_command(self.kind, runners_registry)
 
-    def pick_runner_class_from_entry_point(self):
+    @staticmethod
+    def pick_runner_class_from_entry_point_kind(kind):
         """Selects a runner class from entry points based on kind.
 
         This is related to the :data:`SpawnMethod.PYTHON_CLASS`.
 
+        :param kind: Kind of runner
+        :type kind: str
         :returns: a class that inherits from :class:`BaseRunner` or None
         """
         namespace = "avocado.plugins.runnable.runner"
-        for ep in pkg_resources.iter_entry_points(namespace, self.kind):
+        for ep in pkg_resources.iter_entry_points(namespace, kind):
             try:
                 obj = ep.load()
                 return obj
             except ImportError:
                 return
 
+    def pick_runner_class_from_entry_point(self):
+        """Selects a runner class from entry points based on kind.
+
+        This is related to the :data:`SpawnMethod.PYTHON_CLASS`.
+
+        :returns: a class that inherits from :class:`BaseRunner` or None
+        """
+        return Runnable.pick_runner_class_from_entry_point_kind(self.kind)
+
     def pick_runner_class(self):
         """Selects a runner class from the registry based on kind.
 
         This is related to the :data:`SpawnMethod.PYTHON_CLASS`
 
-        :param runners_registry: a registry with previously registered
-                                 runner classes, keyed by runnable kind
-        :param runners_registry: dict
         :returns: a class that inherits from :class:`BaseRunner`
         :raises: ValueError if kind there's no runner from kind of runnable
         """
         runner = self.pick_runner_class_from_entry_point()
         if runner is not None:
             return runner
         raise ValueError(f"Unsupported kind of runnable: {self.kind}")
```

### Comparing `avocado-framework-98.0/avocado/core/nrunner/runner.py` & `avocado-framework-99.0/avocado/core/nrunner/runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -61,7 +61,28 @@
         :rtype: dict
         """
         status = {}
         if isinstance(additional_info, dict):
             status = additional_info
         status.update({"status": status_type, "time": time.monotonic()})
         return status
+
+    def running_loop(self, condition):
+        """Produces timely running messages until end condition is found.
+
+        :param condition: a callable that will be evaluated as a
+                          condition for continuing the loop
+        """
+        most_current_execution_state_time = None
+        while not condition():
+            now = time.monotonic()
+            if most_current_execution_state_time is not None:
+                next_execution_state_mark = (
+                    most_current_execution_state_time + RUNNER_RUN_STATUS_INTERVAL
+                )
+            if (
+                most_current_execution_state_time is None
+                or now > next_execution_state_mark
+            ):
+                most_current_execution_state_time = now
+                yield self.prepare_status("running")
+            time.sleep(RUNNER_RUN_CHECK_INTERVAL)
```

### Comparing `avocado-framework-98.0/avocado/core/nrunner/task.py` & `avocado-framework-99.0/avocado/core/nrunner/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,17 +96,17 @@
         :param identifier: any identifier that is guaranteed to be unique
                            within the context of a Job. A recommended value
                            is a :class:`avocado.core.test_id.TestID` instance
                            when a task represents a test, because besides the
                            uniqueness aspect, it's also descriptive.  If an
                            identifier is not given, an automatically generated
                            one will be set.
-        :param status_uri: the URIs for the status servers that this task
-                           should send updates to.
-        :type status_uri: list
+        :param status_uris: the URIs for the status servers that this task
+                            should send updates to.
+        :type status_uris: list
         :param category: category of this task. Defaults to
                          :data:`TASK_DEFAULT_CATEGORY`.
         :type category: str
         :param job_id: the ID of the job, for authenticating messages that get
                        sent to the destination job's status server and will make
                        into the job's results.
         :type job_id: str
```

### Comparing `avocado-framework-98.0/avocado/core/output.py` & `avocado-framework-99.0/avocado/core/output.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/parameters.py` & `avocado-framework-99.0/avocado/core/parameters.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/parser.py` & `avocado-framework-99.0/avocado/core/parser.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/parser_common_args.py` & `avocado-framework-99.0/avocado/core/parser_common_args.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/plugin_interfaces.py` & `avocado-framework-99.0/avocado/core/plugin_interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,7 +447,21 @@
 
         Yields dictionary as output, containing status as well as relevant
         information concerning the results.
 
         :param runnable: a Runnable instance that describes what is to be run
         :type runnable: :class:`avocado.core.nrunner.Runnable`
         """
+
+
+class Cache(Plugin):
+    """Plugin for manipulating with cache interface"""
+
+    @abc.abstractmethod
+    def list(self):
+        """List all cache entries
+
+        Creates list of cache entries which represents current cache state.
+
+        :return: Human-readable list of entries which will be printed to console.
+        :rtype: str
+        """
```

### Comparing `avocado-framework-98.0/avocado/core/references.py` & `avocado-framework-99.0/avocado/core/references.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/resolver.py` & `avocado-framework-99.0/avocado/core/resolver.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/result.py` & `avocado-framework-99.0/avocado/core/result.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/runner.py` & `avocado-framework-99.0/avocado/core/runner.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/safeloader/__init__.py` & `avocado-framework-99.0/avocado/core/safeloader/__init__.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/safeloader/core.py` & `avocado-framework-99.0/avocado/core/safeloader/core.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/safeloader/docstring.py` & `avocado-framework-99.0/avocado/core/safeloader/docstring.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/safeloader/imported.py` & `avocado-framework-99.0/avocado/core/safeloader/imported.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/safeloader/module.py` & `avocado-framework-99.0/avocado/core/safeloader/module.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/safeloader/utils.py` & `avocado-framework-99.0/avocado/core/safeloader/utils.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/settings.py` & `avocado-framework-99.0/avocado/core/settings.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/settings_dispatcher.py` & `avocado-framework-99.0/avocado/core/settings_dispatcher.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/spawners/common.py` & `avocado-framework-99.0/avocado/core/spawners/common.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/spawners/mock.py` & `avocado-framework-99.0/avocado/core/spawners/mock.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/status/repo.py` & `avocado-framework-99.0/avocado/core/status/repo.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/status/server.py` & `avocado-framework-99.0/avocado/core/status/server.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/status/utils.py` & `avocado-framework-99.0/avocado/core/status/utils.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/suite.py` & `avocado-framework-99.0/avocado/core/suite.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/sysinfo.py` & `avocado-framework-99.0/avocado/core/sysinfo.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/tags.py` & `avocado-framework-99.0/avocado/core/tags.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/tapparser.py` & `avocado-framework-99.0/avocado/core/tapparser.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/task/runtime.py` & `avocado-framework-99.0/avocado/core/task/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 class RuntimeTaskStatus(Enum):
     WAIT_DEPENDENCIES = "WAITING DEPENDENCIES"
     WAIT = "WAITING"
     FINISHED = "FINISHED"
     TIMEOUT = "FINISHED TIMEOUT"
     IN_CACHE = "FINISHED IN CACHE"
     FAILFAST = "FINISHED FAILFAST"
-    FAIL_TRIAGE = "FAILED ON TRIAGE"
-    FAIL_START = "FAILED ON START"
+    FAIL_TRIAGE = "FINISHED WITH FAILURE ON TRIAGE"
+    FAIL_START = "FINISHED FAILING TO START"
     STARTED = "STARTED"
 
     @staticmethod
     def finished_statuses():
         return [
             status
             for _, status in RuntimeTaskStatus.__members__.items()
@@ -62,15 +62,15 @@
         self.dependencies = []
 
     def __repr__(self):
         if self.status is None:
             return f'<RuntimeTask Task Identifier: "{self.task.identifier}">'
         else:
             return (
-                f'<RuntimeTask Task Identifier: "{self.task.identifier}"'
+                f'<RuntimeTask Task Identifier: "{self.task.identifier}" '
                 f'Status: "{self.status}">'
             )
 
     def __hash__(self):
         return hash(self.task.identifier)
 
     def __eq__(self, other):
```

### Comparing `avocado-framework-98.0/avocado/core/task/statemachine.py` & `avocado-framework-99.0/avocado/core/task/statemachine.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,18 @@
             # dependencies finished, let's check if they finished
             # successfully, so we can move on with the parent task
             dependencies_ok = runtime_task.can_run()
             if not dependencies_ok:
                 LOG.debug(
                     'Task "%s" has failed dependencies', runtime_task.task.identifier
                 )
+                runtime_task.result = "fail"
+                await self._state_machine.finish_task(
+                    runtime_task, RuntimeTaskStatus.FAIL_TRIAGE
+                )
                 return
         if runtime_task.task.category != "test":
             async with self._state_machine.cache_lock:
                 is_task_in_cache = await self._spawner.is_requirement_in_cache(
                     runtime_task
                 )
                 if is_task_in_cache is None:
```

### Comparing `avocado-framework-98.0/avocado/core/test.py` & `avocado-framework-99.0/avocado/core/test.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/test_id.py` & `avocado-framework-99.0/avocado/core/test_id.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/teststatus.py` & `avocado-framework-99.0/avocado/core/teststatus.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/tree.py` & `avocado-framework-99.0/avocado/core/tree.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/utils/loader.py` & `avocado-framework-99.0/avocado/core/utils/loader.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/utils/messages.py` & `avocado-framework-99.0/avocado/core/utils/messages.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/utils/path.py` & `avocado-framework-99.0/avocado/core/utils/path.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/utils/version.py` & `avocado-framework-99.0/avocado/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/varianter.py` & `avocado-framework-99.0/avocado/core/varianter.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/core/version.py` & `avocado-framework-99.0/avocado/core/version.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/libexec/avocado-bash-utils` & `avocado-framework-99.0/avocado/libexec/avocado-bash-utils`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/__init__.py` & `avocado-framework-99.0/avocado/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/archive.py` & `avocado-framework-99.0/avocado/plugins/archive.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/assets.py` & `avocado-framework-99.0/avocado/plugins/assets.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/beaker_result.py` & `avocado-framework-99.0/avocado/plugins/beaker_result.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/bystatus.py` & `avocado-framework-99.0/avocado/plugins/bystatus.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/config.py` & `avocado-framework-99.0/avocado/plugins/config.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/dependency.py` & `avocado-framework-99.0/avocado/plugins/dependency.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,12 +33,14 @@
             return []
         dependency_runnables = []
         for dependency in test_runnable.dependencies:
             # make a copy to change the dictionary and do not affect the
             # original `dependencies` dictionary from the test
             dependency_copy = dependency.copy()
             kind = dependency_copy.pop("type")
+            uri = dependency_copy.pop("uri", None)
+            args = dependency_copy.pop("args", ())
             dependency_runnable = Runnable(
-                kind, None, config=test_runnable.config, **dependency_copy
+                kind, uri, *args, config=test_runnable.config, **dependency_copy
             )
             dependency_runnables.append(dependency_runnable)
         return dependency_runnables
```

### Comparing `avocado-framework-98.0/avocado/plugins/dict_variants.py` & `avocado-framework-99.0/avocado/plugins/dict_variants.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/diff.py` & `avocado-framework-99.0/avocado/plugins/diff.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/distro.py` & `avocado-framework-99.0/avocado/plugins/distro.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/exec_path.py` & `avocado-framework-99.0/avocado/plugins/exec_path.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/human.py` & `avocado-framework-99.0/avocado/plugins/human.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/jobs.py` & `avocado-framework-99.0/avocado/plugins/jobs.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/jobscripts.py` & `avocado-framework-99.0/avocado/plugins/jobscripts.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/journal.py` & `avocado-framework-99.0/avocado/plugins/journal.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/json_variants.py` & `avocado-framework-99.0/avocado/plugins/json_variants.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/jsonresult.py` & `avocado-framework-99.0/avocado/plugins/jsonresult.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/list.py` & `avocado-framework-99.0/avocado/plugins/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,14 @@
 
         parser_common_args.add_tag_filter_args(parser)
 
     def run(self, config):
         verbose = config.get("core.verbose")
         write_to_json_file = config.get("list.write_to_json_file")
         config["run.ignore_missing_references"] = True
-        config["run.test_runner"] = "nrunner"
         try:
             suite = TestSuite.from_config(config)
             matrix = self._get_resolution_matrix(suite)
             self._display(suite, matrix)
 
             directory = config.get("list.recipes.write_to_directory")
             if directory is not None:
```

### Comparing `avocado-framework-98.0/avocado/plugins/plugins.py` & `avocado-framework-99.0/avocado/plugins/plugins.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,14 +89,18 @@
                 dispatcher.SpawnerDispatcher(),
                 "Plugins that spawn tasks and know about their status (spawner): ",
             ),
             (
                 dispatcher.RunnableRunnerDispatcher(),
                 "Plugins that run runnables (under a task and spawner) (runnable.runner): ",
             ),
+            (
+                dispatcher.CacheDispatcher(),
+                "Plugins that manipulates with avocado cache: ",
+            ),
         ]
         for plugins_active, msg in plugin_types:
             LOG_UI.info(msg)
             plugin_matrix = []
             if config.get("plugins.ordered_list"):
                 sorted_plugins = plugins_active.get_extentions_by_priority()
             else:
```

### Comparing `avocado-framework-98.0/avocado/plugins/replay.py` & `avocado-framework-99.0/avocado/plugins/replay.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/resolvers.py` & `avocado-framework-99.0/avocado/plugins/resolvers.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/run.py` & `avocado-framework-99.0/avocado/plugins/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,19 +96,42 @@
             metavar="NAME_VALUE",
             help_msg=help_msg,
             parser=parser,
             long_arg="--test-parameter",
             short_arg="-p",
         )
 
+        help_msg = (
+            "Selects the runner implementation from one of the "
+            "installed and active implementations.  You can run "
+            '"avocado plugins" and find the list of valid runners '
+            'under the "Plugins that run test suites on a job '
+            '(runners) section.  Defaults to "nrunner", which is '
+            "the new runner and only runner supported at this moment. "
+        )
+        settings.add_argparser_to_option(
+            namespace="run.test_runner",
+            parser=parser,
+            long_arg="--suite-runner",
+            metavar="SUITE_RUNNER",
+            help_msg=help_msg,
+        )
+
+        help_msg = (
+            "This option name is currently DEPRECATED and will be "
+            "removed on Avocado 100.0 and later.  Please use "
+            '"--suite-runner" instead.'
+        )
         settings.add_argparser_to_option(
             namespace="run.test_runner",
             parser=parser,
             long_arg="--test-runner",
             metavar="TEST_RUNNER",
+            help_msg=help_msg,
+            allow_multiple=True,
         )
 
         help_msg = "Instead of running the test only list them and log their params."
         settings.register_option(
             section="run.dry_run",
             key="enabled",
             default=False,
```

### Comparing `avocado-framework-98.0/avocado/plugins/runner_nrunner.py` & `avocado-framework-99.0/avocado/plugins/runner_nrunner.py`

 * *Files 22% similar despite different names*

```diff
@@ -64,27 +64,31 @@
             section=section,
             key="status_server_auto",
             default=True,
             key_type=bool,
             help_msg=help_msg,
         )
 
-        help_msg = 'URI for listing the status server. Usually a "HOST:PORT" string'
+        help_msg = (
+            'URI where status server will listen on. Usually a "HOST:PORT" '
+            'string. This is only effective if "status_server_auto" is disabled'
+        )
         settings.register_option(
             section=section,
             key="status_server_listen",
             default="127.0.0.1:8888",
             metavar="HOST:PORT",
             help_msg=help_msg,
         )
 
         help_msg = (
             "URI for connecting to the status server, usually "
             'a "HOST:PORT" string. Use this if your status server '
-            "is in another host, or different port"
+            "is in another host, or different port. This is only "
+            'effective if "status_server_auto" is disabled'
         )
         settings.register_option(
             section=section,
             key="status_server_uri",
             default="127.0.0.1:8888",
             metavar="HOST:PORT",
             help_msg=help_msg,
@@ -147,86 +151,172 @@
         if parser is None:
             return
 
         parser = parser.add_argument_group("nrunner specific options")
         settings.add_argparser_to_option(
             namespace="nrunner.shuffle",
             parser=parser,
+            long_arg="--shuffle",
+            action="store_true",
+        )
+
+        help_msg = (
+            "This option is currently DEPRECATED and will not be available "
+            'on Avocado 100.0 and later.  Please use "--shuffle" instead.'
+        )
+        settings.add_argparser_to_option(
+            namespace="nrunner.shuffle",
+            parser=parser,
             long_arg="--nrunner-shuffle",
             action="store_true",
+            help_msg=help_msg,
+            allow_multiple=True,
         )
 
         settings.add_argparser_to_option(
             namespace="nrunner.status_server_auto",
             parser=parser,
+            long_arg="--status-server-disable-auto",
+            action="store_false",
+        )
+
+        help_msg = (
+            "This option is currently DEPRECATED and will not be available "
+            'on Avocado 100.0 and later.  Please use "--status-server-disable-auto '
+            "instead."
+        )
+        settings.add_argparser_to_option(
+            namespace="nrunner.status_server_auto",
+            parser=parser,
             long_arg="--nrunner-status-server-disable-auto",
             action="store_false",
+            help_msg=help_msg,
+            allow_multiple=True,
         )
 
         settings.add_argparser_to_option(
             namespace="nrunner.status_server_listen",
             parser=parser,
+            long_arg="--status-server-listen",
+            metavar="HOST_PORT",
+        )
+
+        help_msg = (
+            "This option is currently DEPRECATED and will not be available "
+            'on Avocado 100.0 and later.  Please use "--status-server-listen" instead.'
+        )
+        settings.add_argparser_to_option(
+            namespace="nrunner.status_server_listen",
+            parser=parser,
             long_arg="--nrunner-status-server-listen",
             metavar="HOST_PORT",
+            help_msg=help_msg,
+            allow_multiple=True,
         )
 
         settings.add_argparser_to_option(
             namespace="nrunner.status_server_uri",
             parser=parser,
+            long_arg="--status-server-uri",
+            metavar="HOST_PORT",
+        )
+
+        help_msg = (
+            "This option is currently DEPRECATED and will not be available "
+            'on Avocado 100.0 and later.  Please use "--status-server-uri" instead.'
+        )
+        settings.add_argparser_to_option(
+            namespace="nrunner.status_server_uri",
+            parser=parser,
             long_arg="--nrunner-status-server-uri",
             metavar="HOST_PORT",
+            help_msg=help_msg,
+            allow_multiple=True,
         )
 
         settings.add_argparser_to_option(
             namespace="nrunner.max_parallel_tasks",
             parser=parser,
+            long_arg="--max-parallel-tasks",
+            metavar="NUMBER_OF_TASKS",
+        )
+
+        help_msg = (
+            "This option is currently DEPRECATED and will not be available "
+            'on Avocado 100.0 and later.  Please use "--max-parallel-tasks" instead.'
+        )
+        settings.add_argparser_to_option(
+            namespace="nrunner.max_parallel_tasks",
+            parser=parser,
             long_arg="--nrunner-max-parallel-tasks",
             metavar="NUMBER_OF_TASKS",
+            help_msg=help_msg,
+            allow_multiple=True,
         )
 
         settings.add_argparser_to_option(
             namespace="nrunner.spawner",
             parser=parser,
+            long_arg="--spawner",
+            metavar="SPAWNER",
+        )
+
+        help_msg = (
+            "This option is currently DEPRECATED and will not be available "
+            'on Avocado 100.0 and later.  Please use "--spawner" instead.'
+        )
+        settings.add_argparser_to_option(
+            namespace="nrunner.spawner",
+            parser=parser,
             long_arg="--nrunner-spawner",
             metavar="SPAWNER",
+            help_msg=help_msg,
+            allow_multiple=True,
         )
 
     def run(self, config):
         pass
 
 
 class Runner(RunnerInterface):
 
     name = "nrunner"
     description = "nrunner based implementation of job compliant runner"
 
+    def __init__(self):
+        super().__init__()
+        self.status_server_dir = None
+
     @staticmethod
     def _update_avocado_configuration_used_on_runnables(runnables, config):
         """Updates the config used on runnables with this suite's config values
 
         :param runnables: the tasks whose runner requirements will be checked
         :type runnables: list of :class:`Runnable`
         :param config: A config dict to be used on the desired test suite.
         :type config: dict
         """
         for runnable in runnables:
             runnable.config = Runnable.filter_runnable_config(runnable.kind, config)
 
-    def _determine_status_server_uri(self, test_suite):
-        # pylint: disable=W0201
-        self.status_server_dir = None
+    def _determine_status_server(self, test_suite, config_key):
         if test_suite.config.get("nrunner.status_server_auto"):
             # no UNIX domain sockets on Windows
             if platform.system() != "Windows":
-                self.status_server_dir = tempfile.TemporaryDirectory(prefix="avocado_")
+                if self.status_server_dir is None:
+                    self.status_server_dir = tempfile.TemporaryDirectory(
+                        prefix="avocado_"
+                    )
                 return os.path.join(self.status_server_dir.name, ".status_server.sock")
-        return test_suite.config.get("nrunner.status_server_listen")
+        return test_suite.config.get(config_key)
 
     def _create_status_server(self, test_suite, job):
-        listen = self._determine_status_server_uri(test_suite)
+        listen = self._determine_status_server(
+            test_suite, "nrunner.status_server_listen"
+        )
         # pylint: disable=W0201
         self.status_repo = StatusRepo(job.unique_id)
         # pylint: disable=W0201
         self.status_server = StatusServer(listen, self.status_repo)
 
     async def _update_status(self, job):
         tasks_by_id = {
@@ -278,15 +368,15 @@
         )
 
         self._create_status_server(test_suite, job)
 
         graph = RuntimeTaskGraph(
             test_suite.get_test_variants(),
             test_suite.name,
-            self.status_server.uri,
+            self._determine_status_server(test_suite, "nrunner.status_server_uri"),
             job.unique_id,
         )
         # pylint: disable=W0201
         self.runtime_tasks = graph.get_tasks_in_topological_order()
 
         # Start the status server
         asyncio.ensure_future(self.status_server.serve_forever())
```

### Comparing `avocado-framework-98.0/avocado/plugins/runners/asset.py` & `avocado-framework-99.0/avocado/plugins/runners/asset.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/runners/avocado_instrumented.py` & `avocado-framework-99.0/avocado/plugins/runners/avocado_instrumented.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/runners/dry_run.py` & `avocado-framework-99.0/avocado/plugins/runners/dry_run.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/runners/noop.py` & `avocado-framework-99.0/avocado/plugins/runners/noop.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/runners/package.py` & `avocado-framework-99.0/avocado/plugins/runners/package.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/runners/python_unittest.py` & `avocado-framework-99.0/avocado/plugins/runners/python_unittest.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/runners/sysinfo.py` & `avocado-framework-99.0/avocado/plugins/runners/sysinfo.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/runners/tap.py` & `avocado-framework-99.0/avocado/plugins/runners/tap.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                     result = "skip"
                     break
                 else:
                     result = "pass"
         return result
 
     def _process_final_status(
-        self, process, stdout=None, stderr=None
+        self, process, runnable, stdout=None, stderr=None
     ):  # pylint: disable=W0613
         return FinishedMessage.get(
             self._get_tap_result(stdout), returncode=process.returncode
         )
 
 
 class RunnerApp(BaseRunnerApp):
```

### Comparing `avocado-framework-98.0/avocado/plugins/spawners/podman.py` & `avocado-framework-99.0/avocado/plugins/spawners/podman.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/spawners/process.py` & `avocado-framework-99.0/avocado/plugins/spawners/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         task = runtime_task.task
         runner = task.runnable.runner_command()
         args = runner[1:] + ["task-run"] + task.get_command_args()
         runner = runner[0]
         # When running Avocado Python modules, the interpreter on the new
         # process needs to know where Avocado can be found.
         env = os.environ.copy()
-        env["PYTHONPATH"] = ":".join(p for p in sys.path)
+        env["PYTHONPATH"] = ":".join(p for p in set(sys.path))
 
         # pylint: disable=E1133
         try:
             runtime_task.spawner_handle = await asyncio.create_subprocess_exec(
                 runner,
                 *args,
                 stdout=asyncio.subprocess.DEVNULL,
```

### Comparing `avocado-framework-98.0/avocado/plugins/sysinfo.py` & `avocado-framework-99.0/avocado/plugins/sysinfo.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/tap.py` & `avocado-framework-99.0/avocado/plugins/tap.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/testlogs.py` & `avocado-framework-99.0/avocado/plugins/testlogs.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/teststmpdir.py` & `avocado-framework-99.0/avocado/plugins/teststmpdir.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/variants.py` & `avocado-framework-99.0/avocado/plugins/variants.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/plugins/vmimage.py` & `avocado-framework-99.0/avocado/plugins/vmimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import re
 
 from avocado.core import exit_codes, output
 from avocado.core.output import LOG_UI
-from avocado.core.plugin_interfaces import CLICmd
+from avocado.core.plugin_interfaces import Cache, CLICmd
 from avocado.core.settings import settings
 from avocado.utils import astring, vmimage
 
 
 def list_downloaded_images():
     """
     List the available Image inside avocado cache
@@ -95,16 +95,15 @@
     ]
     header = (
         output.TERM_SUPPORT.header_str("Provider"),
         output.TERM_SUPPORT.header_str("Version"),
         output.TERM_SUPPORT.header_str("Architecture"),
         output.TERM_SUPPORT.header_str("File"),
     )
-    for line in astring.iter_tabular_output(image_matrix, header=header, strip=True):
-        LOG_UI.debug(line)
+    return astring.tabular_output(image_matrix, header=header, strip=True)
 
 
 class VMimage(CLICmd):
     """
     Implements the avocado 'vmimage' subcommand
     """
 
@@ -156,20 +155,30 @@
             long_arg="--arch",
         )
 
     def run(self, config):
         subcommand = config.get("vmimage_subcommand")
         if subcommand == "list":
             images = list_downloaded_images()
-            display_images_list(images)
+            LOG_UI.debug(display_images_list(images))
         elif subcommand == "get":
             name = config.get("vmimage.get.distro")
             version = config.get("vmimage.get.version")
             arch = config.get("vmimage.get.arch")
             try:
                 image = download_image(name, version, arch)
             except AttributeError:
                 LOG_UI.debug("The requested image could not be downloaded")
                 return exit_codes.AVOCADO_FAIL
             LOG_UI.debug("The image was downloaded:")
-            display_images_list([image])
+            LOG_UI.debug(display_images_list([image]))
         return exit_codes.AVOCADO_ALL_OK
+
+
+class VMimageCache(Cache):
+
+    name = "vmimage"
+    description = "Provides VM images acquired from official repositories"
+
+    def list(self):
+        images = list_downloaded_images()
+        return display_images_list(images)
```

### Comparing `avocado-framework-98.0/avocado/plugins/xunit.py` & `avocado-framework-99.0/avocado/plugins/xunit.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/__init__.py` & `avocado-framework-99.0/avocado/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/ar.py` & `avocado-framework-99.0/avocado/utils/ar.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/archive.py` & `avocado-framework-99.0/avocado/utils/archive.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/asset.py` & `avocado-framework-99.0/avocado/utils/asset.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/astring.py` & `avocado-framework-99.0/avocado/utils/astring.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/aurl.py` & `avocado-framework-99.0/avocado/utils/aurl.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/build.py` & `avocado-framework-99.0/avocado/utils/build.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/cloudinit.py` & `avocado-framework-99.0/avocado/utils/cloudinit.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/cpu.py` & `avocado-framework-99.0/avocado/utils/cpu.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/crypto.py` & `avocado-framework-99.0/avocado/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/data_factory.py` & `avocado-framework-99.0/avocado/utils/data_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         path = tempfile.mkdtemp(prefix="avocado_" + __name__, dir=basedir)
         n_files = _RAND_POOL.randint(100, 150)
         for _ in range(n_files):
             fd, _ = tempfile.mkstemp(dir=path, text=True)
             str_length = _RAND_POOL.randint(30, 50)
             n_lines = _RAND_POOL.randint(5, 7)
             for _ in range(n_lines):
-                os.write(fd, generate_random_string(str_length))
+                os.write(fd, generate_random_string(str_length).encode())
             os.close(fd)
     except OSError as details:
         log_msg = "Failed to generate dir in '%s' and populate: %s"
         LOG.error(log_msg, basedir, details)
         return None
 
     return path
```

### Comparing `avocado-framework-98.0/avocado/utils/data_structures.py` & `avocado-framework-99.0/avocado/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/datadrainer.py` & `avocado-framework-99.0/avocado/utils/datadrainer.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/debug.py` & `avocado-framework-99.0/avocado/utils/debug.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/diff_validator.py` & `avocado-framework-99.0/avocado/utils/diff_validator.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/disk.py` & `avocado-framework-99.0/avocado/utils/disk.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/distro.py` & `avocado-framework-99.0/avocado/utils/distro.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/dmesg.py` & `avocado-framework-99.0/avocado/utils/dmesg.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/download.py` & `avocado-framework-99.0/avocado/utils/download.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/exit_codes.py` & `avocado-framework-99.0/avocado/utils/exit_codes.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/external/__init__.py` & `avocado-framework-99.0/avocado/utils/external/__init__.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/external/gdbmi_parser.py` & `avocado-framework-99.0/avocado/utils/external/gdbmi_parser.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/external/spark.py` & `avocado-framework-99.0/avocado/utils/external/spark.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/file_utils.py` & `avocado-framework-99.0/avocado/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/filelock.py` & `avocado-framework-99.0/avocado/utils/filelock.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/gdb.py` & `avocado-framework-99.0/avocado/utils/gdb.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/genio.py` & `avocado-framework-99.0/avocado/utils/genio.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/git.py` & `avocado-framework-99.0/avocado/utils/git.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/iso9660.py` & `avocado-framework-99.0/avocado/utils/iso9660.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/kernel.py` & `avocado-framework-99.0/avocado/utils/kernel.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/linux.py` & `avocado-framework-99.0/avocado/utils/linux.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/linux_modules.py` & `avocado-framework-99.0/avocado/utils/linux_modules.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/lv_utils.py` & `avocado-framework-99.0/avocado/utils/lv_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,22 +334,21 @@
     :param pv_list: list of physical volumes to use
     :type pv_list: str or [str]
     :param bool force: create volume group with a force flag
     :raises: :py:class:`LVException` if volume group already exists
     """
     if vg_check(vg_name):
         raise LVException(f"Volume group '{vg_name}' already exist")
-    cmd = "vgcreate"
     if isinstance(pv_list, list):
         pv_list = " ".join(pv_list)
     else:
         pv_list = str(pv_list)
-    cmd += f" {vg_name} {pv_list}"
+    cmd = f"vgcreate {vg_name} {pv_list}"
     if force:
-        cmd += f"{cmd} -f -y"
+        cmd = f"{cmd} -f -y"
     process.run(cmd, sudo=True)
 
 
 def vg_remove(vg_name):
     """
     Remove a volume group.
```

### Comparing `avocado-framework-98.0/avocado/utils/memory.py` & `avocado-framework-99.0/avocado/utils/memory.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/multipath.py` & `avocado-framework-99.0/avocado/utils/multipath.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/network/hosts.py` & `avocado-framework-99.0/avocado/utils/network/hosts.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/network/interfaces.py` & `avocado-framework-99.0/avocado/utils/network/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -591,7 +591,19 @@
             output = run_command(cmd, self.host, sudo=sudo)
             if "0% packet loss" not in output:
                 return False
             return True
         except Exception as ex:
             msg = f"Failed to ping. {ex}"
             raise NWException(msg)
+
+    def netmask_to_cidr(self, netmask):
+        """Function is used to check the netmask value and convert
+
+        it into short form (mask) of netmask values
+        Example : 255.255.255.0 = 24
+        255.255.252.0 = 22
+
+        :param netmask: Netmask value example 255.255.255.0
+        :return : Returns mask value of given netmask
+        """
+        return sum([bin(int(bits)).count("1") for bits in netmask.split(".")])
```

### Comparing `avocado-framework-98.0/avocado/utils/network/ports.py` & `avocado-framework-99.0/avocado/utils/network/ports.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/output.py` & `avocado-framework-99.0/avocado/utils/output.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/partition.py` & `avocado-framework-99.0/avocado/utils/partition.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/path.py` & `avocado-framework-99.0/avocado/utils/path.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/pci.py` & `avocado-framework-99.0/avocado/utils/pci.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,14 +150,15 @@
     pci_class_dic = {
         "0104": "scsi_host",
         "0c04": "fc_host",
         "0200": "net",
         "0108": "nvme",
         "0280": "net",
         "0207": "net",
+        "0c03": "usb",
     }
     pci_class_id = get_pci_prop(pci_address, "Class")
     if pci_class_id not in pci_class_dic:
         if pci_class_id is None:
             raise ValueError(
                 f"Unable to get 'Class' property of given pci " f"address {pci_address}"
             )
@@ -276,14 +277,36 @@
         if not output:
             return
         pci_id.append(output)
     if pci_id:
         return ":".join(pci_id)
 
 
+def get_pci_info(pci_address):
+    """
+    Gets PCI info of given PCI address.
+
+    :param pci_address: Any segment of a PCI address (1f, 0000:00:1f, ...)
+
+    :return: Dictionary attribute name as key and attribute value as value.
+    :rtype: Dict
+    """
+    cmd = f"lspci -Dnvmm -s {pci_address}"
+    output = process.run(cmd, ignore_status=True, shell=True).stdout_text
+    pci_info = {}
+    if not output:
+        return
+    for line in output.splitlines():
+        if line.strip():
+            pci_info[line.split(":")[0].strip()] = (
+                ":".join(line.split(":")[1:])
+            ).strip()
+    return pci_info
+
+
 def get_driver(pci_address):
     """
     Gets the kernel driver in use of given PCI address. (first match only)
 
     :param pci_address: Any segment of a PCI address (1f, 0000:00:1f, ...)
 
     :return: driver of a PCI address.
@@ -403,8 +426,16 @@
             cfg_dic["Mfg"] = line.split(".")[-1]
         if "Machine Type-Model" in line:
             cfg_dic["Model"] = line.split(".")[-1]
         if "Device Specific" in line:
             cfg_dic["YC"] = line.split(".")[-1]
         if "Location Code" in line:
             cfg_dic["YL"] = line.split("..")[-1].strip(".")
+    if "Description" in cfg_dic:
+        pcid = re.search(
+            r"[0-9a-e]{4}\:[0-9a-e]{2}\:[0-9a-e]{2}\.[0-9a-e]{1}",
+            cfg_dic["Description"],
+        )
+        cfg_dic["pci_id"] = pcid.group()
+        device_subvendor = re.search(r"([0-9a-e]{8})", cfg_dic["Description"])
+        cfg_dic["subvendor_device"] = device_subvendor.group()
     return cfg_dic
```

### Comparing `avocado-framework-98.0/avocado/utils/pmem.py` & `avocado-framework-99.0/avocado/utils/pmem.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/podman.py` & `avocado-framework-99.0/avocado/utils/podman.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,16 @@
             # Since this method is also used by other methods, let's
             # log here as well.
             msg = "Could not execute the command."
             LOG.error("%s: %s", msg, str(ex))
             raise PodmanException(msg) from ex
 
         if proc.returncode != 0:
-            msg = f"Could not execute the command: {proc.returncode}:{stderr}."
+            command_args = " ".join(args)
+            msg = f'Failure from command "{self.podman_bin} {command_args}": returned code "{proc.returncode}" stderr: "{stderr}"'
             LOG.error(msg)
             raise PodmanException(msg)
 
         return proc.returncode, stdout, stderr
 
     async def copy_to_container(self, container_id, src, dst):
         """Copy artifacts from src to container:dst.
```

### Comparing `avocado-framework-98.0/avocado/utils/process.py` & `avocado-framework-99.0/avocado/utils/process.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/script.py` & `avocado-framework-99.0/avocado/utils/script.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/service.py` & `avocado-framework-99.0/avocado/utils/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,14 +444,16 @@
                 try:
                     init = os.readlink(init)
                 except OSError:
                     pass
                 return os.path.basename(init)
     else:
         output = run("readlink /proc/1/exe").stdout.strip()
+        if isinstance(output, bytes):
+            output = output.decode(encoding="utf-8")
         return os.path.basename(output)
 
 
 class _SpecificServiceManager:  # pylint: disable=too-few-public-methods
     def __init__(
         self,
         service_name,
```

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/backends/apt.py` & `avocado-framework-99.0/avocado/utils/software_manager/backends/apt.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/backends/base.py` & `avocado-framework-99.0/avocado/utils/software_manager/backends/base.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/backends/dnf.py` & `avocado-framework-99.0/avocado/utils/software_manager/backends/dnf.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/backends/dpkg.py` & `avocado-framework-99.0/avocado/utils/software_manager/backends/dpkg.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,8 +101,8 @@
         :param package: Package name.
         :return: List of paths installed by package.
         """
         if os.path.isfile(package):
             l_cmd = self.lowlevel_base_cmd + " -c " + package
         else:
             l_cmd = self.lowlevel_base_cmd + " -l " + package
-        return process.system_output(l_cmd).split("\n")
+        return process.system_output(l_cmd).decode().split("\n")
```

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/backends/rpm.py` & `avocado-framework-99.0/avocado/utils/software_manager/backends/rpm.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         """
         Rpmbuild the spec path and return build dir
 
         :param spec_path: spec path to install
         :return path: build directory
         """
 
-        build_option = "-bp"
+        build_option = "-bc"
         if dest_path is not None:
             build_option += f" --define '_builddir {dest_path}'"
         else:
             LOG.error("Please provide a valid path")
             return ""
         try:
             process.system(f"rpmbuild {build_option} {spec_file}")
```

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/backends/yum.py` & `avocado-framework-99.0/avocado/utils/software_manager/backends/yum.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/backends/zypper.py` & `avocado-framework-99.0/avocado/utils/software_manager/backends/zypper.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/distro_packages.py` & `avocado-framework-99.0/avocado/utils/software_manager/distro_packages.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/inspector.py` & `avocado-framework-99.0/avocado/utils/software_manager/inspector.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/main.py` & `avocado-framework-99.0/avocado/utils/software_manager/main.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/software_manager/manager.py` & `avocado-framework-99.0/avocado/utils/software_manager/manager.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/softwareraid.py` & `avocado-framework-99.0/avocado/utils/softwareraid.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/ssh.py` & `avocado-framework-99.0/avocado/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/stacktrace.py` & `avocado-framework-99.0/avocado/utils/stacktrace.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/sysinfo.py` & `avocado-framework-99.0/avocado/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado/utils/vmimage.py` & `avocado-framework-99.0/avocado/utils/vmimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,14 +447,62 @@
     ):
         super().__init__(version=version, build=build, arch=arch)
         self.url_versions = "https://download.cirros-cloud.net/"
         self.url_images = self.url_versions + "{version}/"
         self.image_pattern = "cirros-{version}-{arch}-disk.img$"
 
 
+class FreeBSDImageProvider(ImageProviderBase):
+    """
+    FreeBSD Image Provider
+    """
+
+    name = "FreeBSD"
+
+    def __init__(self, version="[0-9]+.[0-9]", build=None, arch=DEFAULT_ARCH):
+        # FreeBSD uses 'amd64' instead of 'x86_64'
+        if arch == "x86_64":
+            arch = "amd64"
+
+        super().__init__(version + "-RELEASE", build, arch)
+        self.url_versions = (
+            "http://ftp-archive.freebsd.org/pub/FreeBSD-Archive/old-releases/VM-IMAGES/"
+        )
+        self.url_images = self.url_versions + "{version}-RELEASE/{arch}/Latest/"
+
+        arch2 = ""
+        if arch == "aarch64":
+            arch2 = "arm64-"
+        elif arch == "riscv64":
+            arch2 = "riscv-"
+        self.image_pattern = (
+            "FreeBSD-(?P<version>{version})-RELEASE-"
+            + arch2
+            + "(?P<arch>{arch}).qcow2.xz"
+        )
+
+    def get_best_version(self, versions):  # pylint: disable=W0221
+        """Return best (more recent) version"""
+        max_float = max([float(item) for item in versions])
+        return str(f"{max_float:2.1f}")
+
+    def get_versions(self):
+        """Return all available versions for the current parameters."""
+        parser = VMImageHtmlParser(self.version_pattern)
+        self._feed_html_parser(self.url_versions, parser)
+
+        resulting_versions = []
+        if parser.items:
+            for version in parser.items:
+                max_float = float(version.split("-")[0])
+                resulting_versions.append(str(f"{max_float:2.1f}"))
+
+        return resulting_versions
+
+
 class Image:
     def __init__(
         self,
         name,
         url,
         version,
         arch,
```

### Comparing `avocado-framework-98.0/avocado/utils/wait.py` & `avocado-framework-99.0/avocado/utils/wait.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/avocado_framework.egg-info/PKG-INFO` & `avocado-framework-99.0/avocado_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avocado-framework
-Version: 98.0
+Version: 99.0
 Summary: Avocado Test Framework
 Home-page: https://avocado-framework.github.io/
 Author: Avocado Developers
 Author-email: avocado-devel@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `avocado-framework-98.0/avocado_framework.egg-info/SOURCES.txt` & `avocado-framework-99.0/avocado_framework.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 avocado/libexec/avocado_info
 avocado/libexec/avocado_warn
 avocado/plugins/__init__.py
 avocado/plugins/archive.py
 avocado/plugins/assets.py
 avocado/plugins/beaker_result.py
 avocado/plugins/bystatus.py
+avocado/plugins/cache.py
 avocado/plugins/config.py
 avocado/plugins/dependency.py
 avocado/plugins/dict_variants.py
 avocado/plugins/diff.py
 avocado/plugins/distro.py
 avocado/plugins/exec_path.py
 avocado/plugins/human.py
@@ -104,14 +105,15 @@
 avocado/plugins/jobscripts.py
 avocado/plugins/journal.py
 avocado/plugins/json_variants.py
 avocado/plugins/jsonresult.py
 avocado/plugins/list.py
 avocado/plugins/plugins.py
 avocado/plugins/replay.py
+avocado/plugins/requirement_cache.py
 avocado/plugins/resolvers.py
 avocado/plugins/run.py
 avocado/plugins/runner_nrunner.py
 avocado/plugins/sysinfo.py
 avocado/plugins/tap.py
 avocado/plugins/testlogs.py
 avocado/plugins/teststmpdir.py
@@ -121,14 +123,15 @@
 avocado/plugins/runners/__init__.py
 avocado/plugins/runners/asset.py
 avocado/plugins/runners/avocado_instrumented.py
 avocado/plugins/runners/dry_run.py
 avocado/plugins/runners/exec_test.py
 avocado/plugins/runners/noop.py
 avocado/plugins/runners/package.py
+avocado/plugins/runners/podman_image.py
 avocado/plugins/runners/python_unittest.py
 avocado/plugins/runners/sysinfo.py
 avocado/plugins/runners/tap.py
 avocado/plugins/spawners/__init__.py
 avocado/plugins/spawners/podman.py
 avocado/plugins/spawners/process.py
 avocado/utils/__init__.py
@@ -238,15 +241,14 @@
 examples/nrunner/recipes/tasks/exec-status/2-dd-result.json
 examples/nrunner/recipes/tasks/exec-status/3-sleep-result.json
 examples/nrunner/recipes/tasks/exec-status/4-sleep-long-result.json
 examples/nrunner/recipes/tasks/exec-test/1-uname.json
 examples/nrunner/recipes/tasks/exec-test/2-echo.json
 examples/nrunner/recipes/tasks/exec-test/3-sleep.json
 examples/nrunner/recipes/tasks/unittest-result/1-unittest-testcase-localhost.json
-examples/nrunner/runners/avocado-runner-foo
 examples/plugins/README.rst
 examples/plugins/cli-cmd/hello/hello.py
 examples/plugins/cli-cmd/hello/setup.py
 examples/plugins/cli-cmd/hello_option/hello_option.py
 examples/plugins/cli-cmd/hello_option/setup.py
 examples/plugins/cli-cmd/hello_parser/hello_parser.py
 examples/plugins/cli-cmd/hello_parser/setup.py
@@ -270,14 +272,15 @@
 examples/tests/cancel_on_exception.py
 examples/tests/cancel_test.py
 examples/tests/cancelonsetup.py
 examples/tests/canceltest.py
 examples/tests/cit_parameters.py
 examples/tests/custom_env_variable.sh
 examples/tests/datadir.py
+examples/tests/dependency_ansible.py
 examples/tests/doublefail.py
 examples/tests/env_variables.sh
 examples/tests/errortest.py
 examples/tests/errortest_nasty.py
 examples/tests/errortest_nasty2.py
 examples/tests/errortest_nasty3.py
 examples/tests/fail_on_exception.py
@@ -291,15 +294,15 @@
 examples/tests/logging_streams.py
 examples/tests/modify_variable.py
 examples/tests/multiple_tests.py
 examples/tests/multiplextest.py
 examples/tests/params.py
 examples/tests/passtest.py
 examples/tests/passtest.sh
-examples/tests/passtest_with_requirement.py
+examples/tests/passtest_with_dependency.py
 examples/tests/phases.py
 examples/tests/property.py
 examples/tests/raise.py
 examples/tests/simplewarning.sh
 examples/tests/skip_conditional.py
 examples/tests/sleeptenmin.py
 examples/tests/sleeptest.py
@@ -322,14 +325,15 @@
 examples/tests/__pycache__/failtest.cpython-310.pyc
 examples/tests/__pycache__/failtest_with_warning.cpython-310.pyc
 examples/tests/__pycache__/gendata.cpython-310.pyc
 examples/tests/__pycache__/logging_streams.cpython-310.pyc
 examples/tests/__pycache__/params.cpython-310.pyc
 examples/tests/__pycache__/passtest.cpython-310.pyc
 examples/tests/__pycache__/phases.cpython-310.pyc
+examples/tests/__pycache__/sleeptenmin.cpython-310.pyc
 examples/tests/__pycache__/sleeptest.cpython-310.pyc
 examples/tests/__pycache__/sleeptest_async.cpython-310.pyc
 examples/tests/__pycache__/timeouttest.cpython-310.pyc
 examples/tests/__pycache__/uncaught_exception.cpython-310.pyc
 examples/tests/__pycache__/warntest.cpython-310.pyc
 examples/tests/__pycache__/whiteboard.cpython-310.pyc
 examples/tests/assets.py.data/gnu_hello_signer.gpg
@@ -522,22 +526,24 @@
 selftests/functional/plugin/__init__.py
 selftests/functional/plugin/test_assets.py
 selftests/functional/plugin/test_bystatus.py
 selftests/functional/plugin/test_diff.py
 selftests/functional/plugin/test_jobscripts.py
 selftests/functional/plugin/test_jsonresult.py
 selftests/functional/plugin/test_logs.py
+selftests/functional/plugin/test_podman_image.py
 selftests/functional/plugin/test_vmimage.py
 selftests/functional/plugin/__pycache__/__init__.cpython-310.pyc
 selftests/functional/plugin/__pycache__/test_assets.cpython-310.pyc
 selftests/functional/plugin/__pycache__/test_bystatus.cpython-310.pyc
 selftests/functional/plugin/__pycache__/test_diff.cpython-310.pyc
 selftests/functional/plugin/__pycache__/test_jobscripts.cpython-310.pyc
 selftests/functional/plugin/__pycache__/test_jsonresult.cpython-310.pyc
 selftests/functional/plugin/__pycache__/test_logs.cpython-310.pyc
+selftests/functional/plugin/__pycache__/test_podman_image.cpython-310.pyc
 selftests/functional/plugin/__pycache__/test_vmimage.cpython-310.pyc
 selftests/functional/plugin/spawners/__init__.py
 selftests/functional/plugin/spawners/test_podman.py
 selftests/functional/plugin/spawners/test_process.py
 selftests/functional/plugin/spawners/__pycache__/test_podman.cpython-310.pyc
 selftests/functional/plugin/spawners/__pycache__/test_process.cpython-310.pyc
 selftests/functional/serial/test_requirements.py
@@ -558,32 +564,36 @@
 selftests/functional/test_nrunner_interface.py.data/recipe_task_noop.json
 selftests/functional/test_nrunner_interface.py.data/recipe_task_python_unittest.json
 selftests/functional/test_nrunner_interface.py.data/recipe_task_robot.json
 selftests/functional/test_nrunner_interface.py.data/recipe_task_tap.json
 selftests/functional/utils/__init__.py
 selftests/functional/utils/test_asset.py
 selftests/functional/utils/test_podman.py
-selftests/functional/utils/__pycache__/__init__.cpython-310.pyc
 selftests/functional/utils/__pycache__/test_asset.cpython-310.pyc
 selftests/functional/utils/__pycache__/test_podman.cpython-310.pyc
 selftests/jobs/example_passjob
 selftests/jobs/example_passjob_cit_varianter
 selftests/jobs/example_passjob_html
 selftests/jobs/example_sleepjob_dict_varianter
 selftests/jobs/example_sleepjob_json_varianter
 selftests/jobs/example_unix_status_server
 selftests/jobs/pass
+selftests/jobs/status_server_auto
+selftests/jobs/status_server_different_uri_listen
 selftests/jobs/tests/pass
 selftests/jobs/tests/passtest.py
 selftests/jobs/tests/__pycache__/passtest.cpython-310.pyc
 selftests/pre_release/jobs/pre_release.py
 selftests/pre_release/tests/check-copr-rpm-version.sh
 selftests/pre_release/tests/cirrusci.py
 selftests/pre_release/tests/readthedocs.py
 selftests/pre_release/tests/vmimage.py
+selftests/pre_release/tests/__pycache__/cirrusci.cpython-310.pyc
+selftests/pre_release/tests/__pycache__/readthedocs.cpython-310.pyc
+selftests/pre_release/tests/__pycache__/vmimage.cpython-310.pyc
 selftests/pre_release/tests/vmimage.py.data/variants.yml
 selftests/unit/__init__.py
 selftests/unit/test_datadir.py
 selftests/unit/test_dependencies_resolver.py
 selftests/unit/test_dispatcher.py
 selftests/unit/test_hintfiles.py
 selftests/unit/test_job.py
```

### Comparing `avocado-framework-98.0/avocado_framework.egg-info/entry_points.txt` & `avocado-framework-99.0/avocado_framework.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+[avocado.plugins.cache]
+requirement = avocado.plugins.requirement_cache:RequirementCache
+vmimage = avocado.plugins.vmimage:VMimageCache
+
 [avocado.plugins.cli]
 journal = avocado.plugins.journal:Journal
 json = avocado.plugins.jsonresult:JSONCLI
 json_variants = avocado.plugins.json_variants:JsonVariantsCLI
 nrunner = avocado.plugins.runner_nrunner:RunnerCLI
 podman = avocado.plugins.spawners.podman:PodmanCLI
 tap = avocado.plugins.tap:TAP
 xunit = avocado.plugins.xunit:XUnitCLI
 zip_archive = avocado.plugins.archive:ArchiveCLI
 
 [avocado.plugins.cli.cmd]
 assets = avocado.plugins.assets:Assets
+cache = avocado.plugins.cache:Cache
 config = avocado.plugins.config:Config
 diff = avocado.plugins.diff:Diff
 distro = avocado.plugins.distro:Distro
 exec-path = avocado.plugins.exec_path:ExecPath
 jobs = avocado.plugins.jobs:Jobs
 list = avocado.plugins.list:List
 plugins = avocado.plugins.plugins:Plugins
@@ -67,14 +72,15 @@
 [avocado.plugins.runnable.runner]
 asset = avocado.plugins.runners.asset:AssetRunner
 avocado-instrumented = avocado.plugins.runners.avocado_instrumented:AvocadoInstrumentedTestRunner
 dry-run = avocado.plugins.runners.dry_run:DryRunRunner
 exec-test = avocado.plugins.runners.exec_test:ExecTestRunner
 noop = avocado.plugins.runners.noop:NoOpRunner
 package = avocado.plugins.runners.package:PackageRunner
+podman-image = avocado.plugins.runners.podman_image:PodmanImageRunner
 python-unittest = avocado.plugins.runners.python_unittest:PythonUnittestRunner
 sysinfo = avocado.plugins.runners.sysinfo:SysinfoRunner
 tap = avocado.plugins.runners.tap:TAPRunner
 
 [avocado.plugins.runner]
 nrunner = avocado.plugins.runner_nrunner:Runner
 
@@ -95,11 +101,12 @@
 avocado-runner = avocado.core.nrunner.__main__:main
 avocado-runner-asset = avocado.plugins.runners.asset:main
 avocado-runner-avocado-instrumented = avocado.plugins.runners.avocado_instrumented:main
 avocado-runner-dry-run = avocado.plugins.runners.dry_run:main
 avocado-runner-exec-test = avocado.plugins.runners.exec_test:main
 avocado-runner-noop = avocado.plugins.runners.noop:main
 avocado-runner-package = avocado.plugins.runners.package:main
+avocado-runner-podman-image = avocado.plugins.runners.podman_image:main
 avocado-runner-python-unittest = avocado.plugins.runners.python_unittest:main
 avocado-runner-sysinfo = avocado.plugins.runners.sysinfo:main
 avocado-runner-tap = avocado.plugins.runners.tap:main
 avocado-software-manager = avocado.utils.software_manager.main:main
```

### Comparing `avocado-framework-98.0/examples/apis/utils/ssh.py` & `avocado-framework-99.0/examples/apis/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/jobs/custom_exec_test.py` & `avocado-framework-99.0/examples/jobs/custom_exec_test.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/jobs/multiple_suites_from_config.py` & `avocado-framework-99.0/examples/jobs/multiple_suites_from_config.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/jobs/passjob_custom.py` & `avocado-framework-99.0/examples/jobs/passjob_custom.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/jobs/unix_status_server.py` & `avocado-framework-99.0/examples/jobs/unix_status_server.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/plugins/cli-cmd/hello_option/hello_option.py` & `avocado-framework-99.0/examples/plugins/cli-cmd/hello_option/hello_option.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/plugins/cli-cmd/hello_parser/hello_parser.py` & `avocado-framework-99.0/examples/plugins/cli-cmd/hello_parser/hello_parser.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/plugins/job-pre-post/mail/avocado_job_mail.py` & `avocado-framework-99.0/examples/plugins/job-pre-post/mail/avocado_job_mail.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/plugins/job-pre-post/sleep/avocado_job_sleep.py` & `avocado-framework-99.0/examples/plugins/job-pre-post/sleep/avocado_job_sleep.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/plugins/tests/README.rst` & `avocado-framework-99.0/examples/plugins/tests/README.rst`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/plugins/tests/magic/avocado_magic/resolver.py` & `avocado-framework-99.0/examples/plugins/tests/magic/avocado_magic/resolver.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/plugins/tests/magic/avocado_magic/runner.py` & `avocado-framework-99.0/examples/plugins/tests/magic/avocado_magic/runner.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/plugins/tests/magic/setup.py` & `avocado-framework-99.0/examples/plugins/tests/magic/setup.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/testplans/release/pre.json` & `avocado-framework-99.0/examples/testplans/release/pre.json`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/testplans/release/release.json` & `avocado-framework-99.0/examples/testplans/release/release.json`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/assert.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/assert.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 344 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 5801 0000  o.......i&.bX...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 5801 0000  o.......nKecX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 8303 5a03 6404 6405 8400  ..d.e...Z.d.d...
 00000050: 5a04 4700 6406 6407 8400 6407 6501 8303  Z.G.d.d...d.e...
 00000060: 5a05 6408 5300 2909 e900 0000 0029 01da  Z.d.S.)......)..
 00000070: 0454 6573 7463 0000 0000 0000 0000 0000  .Testc..........
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/cancel_on_exception.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/cancel_on_exception.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 583 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4702 0000  o.......i&.bG...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4702 0000  o.......nKecG...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 6401 5300 2904 e900  e.j...Z.d.S.)...
 00000050: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
 00000060: 0000 0000 0003 0000 0040 0000 0073 1c00  .........@...s..
 00000070: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/cancelonsetup.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/cancelonsetup.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 352 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 6001 0000  o.......i&.b`...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 6001 0000  o.......nKec`...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7320 0000 0065 005a 0164  ..@...s ...e.Z.d
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/canceltest.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/canceltest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/cit_parameters.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/cit_parameters.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 363 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 6b01 0000  o.......i&.bk...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 6b01 0000  o.......nKeck...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/doublefail.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/doublefail.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 422 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 a601 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 a601 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7320 0000 0065 005a 0164  ..@...s ...e.Z.d
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/errortest.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/errortest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 274 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 1201 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 1201 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/fail_on_exception.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/fail_on_exception.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 655 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 8f02 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 8f02 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 6401 5300 2904 e900  e.j...Z.d.S.)...
 00000050: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
 00000060: 0000 0000 0004 0000 0040 0000 0073 2200  .........@...s".
 00000070: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/failtest.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/failtest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 277 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 1501 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 1501 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/failtest_with_warning.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/failtest_with_warning.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 22:01:20 2022 UTC, .py size: 321 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b09d cc62 4101 0000  o..........bA...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4101 0000  o.......nKecA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/gendata.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/gendata.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 450 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 c201 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 c201 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000060: da04 5465 7374 6300 0000 0000 0000 0000  ..Testc.........
 00000070: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/logging_streams.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/logging_streams.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1007 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 ef03 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 ef03 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6503 8303 5a04 6401 5300 2905  ..d.e...Z.d.S.).
 00000060: e900 0000 004e 2901 da04 5465 7374 6300  .....N)...Testc.
 00000070: 0000 0000 0000 0000 0000 0000 0000 0002  ................
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/params.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/params.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 275 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 1301 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 1301 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7314 0000 0065 005a 0164  ..@...s....e.Z.d
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/passtest.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/passtest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  9 19:17:14 2022 UTC, .py size: 226 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3a47 a262 e200 0000  o.......:G.b....
+00000000: 6f0d 0d0a 0000 0000 863e f562 e200 0000  o........>.b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/phases.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/phases.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 327 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4701 0000  o.......i&.bG...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4701 0000  o.......nKecG...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7328 0000 0065 005a 0164  ..@...s(...e.Z.d
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/sleeptest.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/sleeptest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 411 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 9b01 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 9b01 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000060: da04 5465 7374 6300 0000 0000 0000 0000  ..Testc.........
 00000070: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/sleeptest_async.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/sleeptest_async.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 434 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 b201 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 b201 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000060: da04 5465 7374 6300 0000 0000 0000 0000  ..Testc.........
 00000070: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/timeouttest.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/timeouttest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 486 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 e601 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 e601 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000060: da04 5465 7374 6300 0000 0000 0000 0000  ..Testc.........
 00000070: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/uncaught_exception.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/uncaught_exception.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Nov  1 18:09:57 2021 UTC, .py size: 301 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 752d 8061 2d01 0000  o.......u-.a-...
+00000000: 6f0d 0d0a 0000 0000 006c 4063 2d01 0000  o........l@c-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0300  ................
 00000070: 0000 4000 0000 731c 0000 0065 005a 0164  ..@...s....e.Z.d
```

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/warntest.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/warntest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/__pycache__/whiteboard.cpython-310.pyc` & `avocado-framework-99.0/examples/tests/__pycache__/whiteboard.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 356 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 6401 0000  o.......i&.bd...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 6401 0000  o.......nKecd...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000060: da04 5465 7374 6300 0000 0000 0000 0000  ..Testc.........
 00000070: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
```

### Comparing `avocado-framework-98.0/examples/tests/assets.py` & `avocado-framework-99.0/examples/tests/assets.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/assets.py.data/gnu_hello_signer.gpg` & `avocado-framework-99.0/examples/tests/assets.py.data/gnu_hello_signer.gpg`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/cabort.py` & `avocado-framework-99.0/examples/tests/cabort.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/cancel_on_exception.py` & `avocado-framework-99.0/examples/tests/cancel_on_exception.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/cancel_test.py` & `avocado-framework-99.0/examples/tests/cancel_test.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/datadir.py` & `avocado-framework-99.0/examples/tests/datadir.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/env_variables.sh` & `avocado-framework-99.0/examples/tests/env_variables.sh`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/errortest_nasty.py` & `avocado-framework-99.0/examples/tests/errortest_nasty.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/errortest_nasty2.py` & `avocado-framework-99.0/examples/tests/errortest_nasty2.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/errortest_nasty3.py` & `avocado-framework-99.0/examples/tests/errortest_nasty3.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/fail_on_exception.py` & `avocado-framework-99.0/examples/tests/fail_on_exception.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/gdbtest.py` & `avocado-framework-99.0/examples/tests/gdbtest.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/gdbtest.py.data/return99.c` & `avocado-framework-99.0/examples/tests/gdbtest.py.data/return99.c`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/linuxbuild.py` & `avocado-framework-99.0/examples/tests/linuxbuild.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/logging_streams.py` & `avocado-framework-99.0/examples/tests/logging_streams.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/modify_variable.py` & `avocado-framework-99.0/examples/tests/modify_variable.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/multiple_tests.py` & `avocado-framework-99.0/examples/tests/multiple_tests.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/multiplextest.py` & `avocado-framework-99.0/examples/tests/multiplextest.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/multiplextest.py.data/multiplextest.yaml` & `avocado-framework-99.0/examples/tests/multiplextest.py.data/multiplextest.yaml`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/raise.py` & `avocado-framework-99.0/examples/tests/raise.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/raise.py.data/raise.c` & `avocado-framework-99.0/examples/tests/raise.py.data/raise.c`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/skip_conditional.py` & `avocado-framework-99.0/examples/tests/skip_conditional.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/sleeptenmin.py` & `avocado-framework-99.0/examples/tests/sleeptenmin.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/synctest.py` & `avocado-framework-99.0/examples/tests/synctest.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/synctest.py.data/synctest.tar.bz2` & `avocado-framework-99.0/examples/tests/synctest.py.data/synctest.tar.bz2`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/tests/test_env.py` & `avocado-framework-99.0/examples/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/examples/yaml_to_mux/types.yaml` & `avocado-framework-99.0/examples/yaml_to_mux/types.yaml`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/__pycache__/get_data.cpython-310.pyc` & `avocado-framework-99.0/selftests/.data/__pycache__/get_data.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 3376 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 300d 0000  o.......i&.b0...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 300d 0000  o.......nKec0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7320 0000 0065 005a 0164  ..@...s ...e.Z.d
```

### Comparing `avocado-framework-98.0/selftests/.data/__pycache__/test_statuses.cpython-310.pyc` & `avocado-framework-99.0/selftests/.data/__pycache__/test_statuses.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 7200 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 201c 0000  o.......i&.b ...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 201c 0000  o.......nKec ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c01 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6502 8303 5a04 4700 6405 6406 8400 6406  e...Z.G.d.d...d.
 00000060: 6502 8303 5a05 4700 6407 6408 8400 6408  e...Z.G.d.d...d.
 00000070: 6502 8303 5a06 4700 6409 640a 8400 640a  e...Z.G.d.d...d.
```

### Comparing `avocado-framework-98.0/selftests/.data/__pycache__/unittests.cpython-310.pyc` & `avocado-framework-99.0/selftests/.data/__pycache__/unittests.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Nov  1 18:09:57 2021 UTC, .py size: 438 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 752d 8061 b601 0000  o.......u-.a....
+00000000: 6f0d 0d0a 0000 0000 006c 4063 b601 0000  o........l@c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 4700 6404 6405 8400  e.j...Z.G.d.d...
 00000050: 6405 6500 6a01 8303 5a03 6504 6406 6b02  d.e.j...Z.e.d.k.
 00000060: 7220 6500 a005 a100 0100 6401 5300 6401  r e.......d.S.d.
 00000070: 5300 2907 e900 0000 004e 6300 0000 0000  S.)......Nc.....
```

### Comparing `avocado-framework-98.0/selftests/.data/get_data.py` & `avocado-framework-99.0/selftests/.data/get_data.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/hello.deb` & `avocado-framework-99.0/selftests/.data/hello.deb`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/hello.rpm` & `avocado-framework-99.0/selftests/.data/hello.rpm`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/jenkins-junit.xsd` & `avocado-framework-99.0/selftests/.data/jenkins-junit.xsd`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/safeloader/data/dont_crash.py` & `avocado-framework-99.0/selftests/.data/safeloader/data/dont_crash.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/safeloader/data/dont_detect_non_avocado.py` & `avocado-framework-99.0/selftests/.data/safeloader/data/dont_detect_non_avocado.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/safeloader/data/imports.py` & `avocado-framework-99.0/selftests/.data/safeloader/data/imports.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/sample.iso` & `avocado-framework-99.0/selftests/.data/sample.iso`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/test_archive__symlinks.zip` & `avocado-framework-99.0/selftests/.data/test_archive__symlinks.zip`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/test_statuses.py` & `avocado-framework-99.0/selftests/.data/test_statuses.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/.data/whiteboard.py` & `avocado-framework-99.0/selftests/.data/whiteboard.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/__pycache__/check.cpython-310.pyc` & `avocado-framework-99.0/selftests/__pycache__/check.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 28628 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 d46f 0000  o.......i&.b.o..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 8e72 0000  o.......nKec.r..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6402 6c08 6d09 5a09 0100 6400 6403 6c0a  d.l.m.Z...d.d.l.
@@ -688,272 +688,284 @@
 00002af0: 0104 fc04 ff08 0902 0202 0102 0102 0104  ................
 00002b00: fc04 ff04 0918 0104 ff06 0806 0102 0302  ................
 00002b10: 0102 0104 fd02 0702 0102 0104 fd02 0602  ................
 00002b20: 0102 0104 fd02 f406 fd06 1804 ff08 0204  ................
 00002b30: fe08 0502 0202 0102 0104 fd04 ff04 0818  ................
 00002b40: 0104 ff06 0806 010a 0202 ff06 fd04 0804  ................
 00002b50: 0112 0102 ff04 ff04 0572 7c00 0000 6301  .........r|...c.
-00002b60: 0000 0000 0000 0000 0000 0010 0000 000d  ................
-00002b70: 0000 0043 0000 0073 cc02 0000 6700 7d01  ...C...s....g.}.
+00002b60: 0000 0000 0000 0000 0000 0010 0000 000e  ................
+00002b70: 0000 0043 0000 0073 0203 0000 6700 7d01  ...C...s....g.}.
 00002b80: 6401 6701 6402 6701 6403 6404 6404 6404  d.g.d.g.d.d.d.d.
 00002b90: 6405 9c04 6406 6407 6407 6407 6405 9c04  d...d.d.d.d.d...
 00002ba0: 6408 6407 6407 6407 6405 9c04 6409 6407  d.d.d.d.d...d.d.
 00002bb0: 6407 6407 6405 9c04 640a 6407 6407 6407  d.d.d...d.d.d.d.
 00002bc0: 6405 9c04 640b 6407 6407 6407 6405 9c04  d...d.d.d.d.d...
-00002bd0: 640c 6407 6407 6407 6405 9c04 6707 640d  d.d.d.d.d...g.d.
-00002be0: 9c03 7d02 7400 640e 8301 7249 640f 7c00  ..}.t.d...rId.|.
-00002bf0: 6a01 7601 7249 7c02 6410 1900 a002 6411  j.v.rI|.d.....d.
-00002c00: 6407 6407 6407 6405 9c04 a101 0100 7400  d.d.d.d.......t.
-00002c10: 6412 8301 725e 6413 7c00 6a01 7601 725e  d...r^d.|.j.v.r^
-00002c20: 7c02 6410 1900 a002 6414 6407 6407 6407  |.d.....d.d.d.d.
-00002c30: 6405 9c04 a101 0100 7c00 6a03 6415 1900  d.......|.j.d...
-00002c40: 726c 7c01 a002 7404 a005 7c02 6415 a102  rl|...t...|.d...
-00002c50: a101 0100 6416 6701 6417 6418 6419 6901  ....d.g.d.d.d.i.
-00002c60: 6418 641a 6901 6702 641b 9c03 7d03 7c00  d.d.i.g.d...}.|.
-00002c70: 6a03 641c 1900 7287 7c01 a002 7404 a005  j.d...r.|...t...
-00002c80: 7c03 641c a102 a101 0100 641d 641e 6901  |.d.......d.d.i.
-00002c90: 7d04 7c00 6a03 641f 1900 72a3 7406 a006  }.|.j.d...r.t...
-00002ca0: 7c04 a101 7d05 6420 6701 7c05 6421 3c00  |...}.d g.|.d!<.
-00002cb0: 7c01 a002 7404 a005 7c05 641f a102 a101  |...t...|.d.....
-00002cc0: 0100 7c00 6a03 6422 1900 72bb 7406 a006  ..|.j.d"..r.t...
-00002cd0: 7c04 a101 7d06 6423 6701 7c06 6421 3c00  |...}.d#g.|.d!<.
-00002ce0: 7c01 a002 7404 a005 7c06 6422 a102 a101  |...t...|.d"....
-00002cf0: 0100 7c00 6a03 6424 1900 9001 720c 7407  ..|.j.d$....r.t.
-00002d00: 6a08 a009 6425 6424 a102 7d07 740a a00a  j...d%d$..}.t...
-00002d10: 7407 6a08 a009 7c07 6426 a102 a101 7d08  t.j...|.d&....}.
-00002d20: 7c08 a00b 7407 6a08 a009 7c07 6427 a102  |...t.j...|.d'..
-00002d30: 7407 6a08 a009 7c07 6428 a102 6702 a101  t.j...|.d(..g...
-00002d40: 0100 7406 a006 7c04 a101 7d09 7c08 7c09  ..t...|...}.|.|.
-00002d50: 6421 3c00 7c01 a002 7404 a005 7c09 6429  d!<.|...t...|.d)
-00002d60: a102 a101 0100 7406 a006 7c04 a101 7d0a  ......t...|...}.
-00002d70: 642a 6701 7c0a 6421 3c00 6417 7c0a 642b  d*g.|.d!<.d.|.d+
-00002d80: 3c00 7c01 a002 7404 a005 7c0a 642c a102  <.|...t...|.d,..
-00002d90: a101 0100 7c00 6a03 642d 1900 9001 7227  ....|.j.d-....r'
-00002da0: 7406 a006 7c04 a101 7d0b 740a a00a 642e  t...|...}.t...d.
-00002db0: a101 7c0b 6421 3c00 7c01 a002 7404 a005  ..|.d!<.|...t...
-00002dc0: 7c0b 642d a102 a101 0100 7c00 6a03 642f  |.d-......|.j.d/
-00002dd0: 1900 9001 7264 7406 a006 7c04 a101 7d0c  ....rdt...|...}.
-00002de0: 6700 7c0c 6421 3c00 740a a00a 6430 a101  g.|.d!<.t...d0..
-00002df0: 4400 5d1f 7d0d 7407 6a08 a00c 7c0d a101  D.].}.t.j...|...
-00002e00: 7d0e 7c0e 7c00 6a01 7601 9001 7259 7c0d  }.|.|.j.v...rY|.
-00002e10: 9b00 6431 9d02 7d0f 7c0c 6421 0500 1900  ..d1..}.|.d!....
-00002e20: 740a a00a 7c0f a101 3700 0300 3c00 9001  t...|...7...<...
-00002e30: 713b 7c01 a002 7404 a005 7c0c 642f a102  q;|...t...|.d/..
-00002e40: a101 0100 7c01 5300 2932 4e7a 2e73 656c  ....|.S.)2Nz.sel
-00002e50: 6674 6573 7473 2f66 756e 6374 696f 6e61  ftests/functiona
-00002e60: 6c2f 7465 7374 5f6e 7275 6e6e 6572 5f69  l/test_nrunner_i
-00002e70: 6e74 6572 6661 6365 2e70 79da 0672 756e  nterface.py..run
-00002e80: 6e65 727a 0e61 766f 6361 646f 2d72 756e  nerz.avocado-run
-00002e90: 6e65 72e9 0200 0000 2904 727d 0000 007a  ner.....).r}...z
-00002ea0: 1e72 756e 6e61 626c 652d 7275 6e2d 6e6f  .runnable-run-no
-00002eb0: 2d61 7267 732d 6578 6974 2d63 6f64 657a  -args-exit-codez
-00002ec0: 1f72 756e 6e61 626c 652d 7275 6e2d 7572  .runnable-run-ur
-00002ed0: 692d 6f6e 6c79 2d65 7869 742d 636f 6465  i-only-exit-code
-00002ee0: 7a1a 7461 736b 2d72 756e 2d69 642d 6f6e  z.task-run-id-on
-00002ef0: 6c79 2d65 7869 742d 636f 6465 7a16 6176  ly-exit-codez.av
-00002f00: 6f63 6164 6f2d 7275 6e6e 6572 2d64 7279  ocado-runner-dry
-00002f10: 2d72 756e 7201 0000 007a 1361 766f 6361  -runr....z.avoca
-00002f20: 646f 2d72 756e 6e65 722d 6e6f 6f70 7a18  do-runner-noopz.
-00002f30: 6176 6f63 6164 6f2d 7275 6e6e 6572 2d65  avocado-runner-e
-00002f40: 7865 632d 7465 7374 7a1e 6176 6f63 6164  xec-testz.avocad
-00002f50: 6f2d 7275 6e6e 6572 2d70 7974 686f 6e2d  o-runner-python-
-00002f60: 756e 6974 7465 7374 7a23 6176 6f63 6164  unittestz#avocad
-00002f70: 6f2d 7275 6e6e 6572 2d61 766f 6361 646f  o-runner-avocado
-00002f80: 2d69 6e73 7472 756d 656e 7465 647a 1261  -instrumentedz.a
-00002f90: 766f 6361 646f 2d72 756e 6e65 722d 7461  vocado-runner-ta
-00002fa0: 7072 6c00 0000 7a1f 6176 6f63 6164 6f2d  prl...z.avocado-
-00002fb0: 6672 616d 6577 6f72 6b2d 706c 7567 696e  framework-plugin
-00002fc0: 2d67 6f6c 616e 675a 0667 6f6c 616e 6772  -golangZ.golangr
-00002fd0: 6d00 0000 7a15 6176 6f63 6164 6f2d 7275  m...z.avocado-ru
-00002fe0: 6e6e 6572 2d67 6f6c 616e 677a 1e61 766f  nner-golangz.avo
-00002ff0: 6361 646f 2d66 7261 6d65 776f 726b 2d70  cado-framework-p
-00003000: 6c75 6769 6e2d 726f 626f 745a 0572 6f62  lugin-robotZ.rob
-00003010: 6f74 7a14 6176 6f63 6164 6f2d 7275 6e6e  otz.avocado-runn
-00003020: 6572 2d72 6f62 6f74 fa11 6e72 756e 6e65  er-robot..nrunne
-00003030: 722d 696e 7465 7266 6163 657a 3073 656c  r-interfacez0sel
-00003040: 6674 6573 7473 2f66 756e 6374 696f 6e61  ftests/functiona
-00003050: 6c2f 7365 7269 616c 2f74 6573 745f 7265  l/serial/test_re
-00003060: 7175 6972 656d 656e 7473 2e70 7972 6e00  quirements.pyrn.
-00003070: 0000 da07 7370 6177 6e65 72da 0770 726f  ....spawner..pro
-00003080: 6365 7373 da06 706f 646d 616e 2903 7227  cess..podman).r'
-00003090: 0000 0072 7300 0000 726d 0000 00fa 136e  ...rs...rm.....n
-000030a0: 7275 6e6e 6572 2d72 6571 7569 7265 6d65  runner-requireme
-000030b0: 6e74 7274 0000 0054 da04 756e 6974 7a0f  ntrt...T..unitz.
-000030c0: 7365 6c66 7465 7374 732f 756e 6974 2f72  selftests/unit/r
-000030d0: 2700 0000 da04 6a6f 6273 7a0f 7365 6c66  '.....jobsz.self
-000030e0: 7465 7374 732f 6a6f 6273 2fda 0a66 756e  tests/jobs/..fun
-000030f0: 6374 696f 6e61 6c5a 0973 656c 6674 6573  ctionalZ.selftes
-00003100: 7473 7a08 7465 7374 2a2e 7079 da05 7574  tsz.test*.py..ut
-00003110: 696c 73da 0670 6c75 6769 6efa 1366 756e  ils..plugin..fun
-00003120: 6374 696f 6e61 6c2d 7061 7261 6c6c 656c  ctional-parallel
-00003130: 7a1c 7365 6c66 7465 7374 732f 6675 6e63  z.selftests/func
-00003140: 7469 6f6e 616c 2f73 6572 6961 6c2f 7273  tional/serial/rs
-00003150: 0000 007a 1166 756e 6374 696f 6e61 6c2d  ...z.functional-
-00003160: 7365 7269 616c fa0d 7374 6174 6963 2d63  serial..static-c
-00003170: 6865 636b 737a 0e73 656c 6674 6573 7473  hecksz.selftests
-00003180: 2f2a 2e73 68fa 106f 7074 696f 6e61 6c2d  /*.sh..optional-
-00003190: 706c 7567 696e 737a 126f 7074 696f 6e61  pluginsz.optiona
-000031a0: 6c5f 706c 7567 696e 732f 2a7a 082f 7465  l_plugins/*z./te
-000031b0: 7374 732f 2a29 0d72 0600 0000 7279 0000  sts/*).r....ry..
-000031c0: 0072 5f00 0000 da0a 6469 6374 5f74 6573  .r_.....dict_tes
-000031d0: 7473 7205 0000 0072 3d00 0000 da04 636f  tsr....r=.....co
-000031e0: 7079 7209 0000 0072 0a00 0000 720b 0000  pyr....r....r...
-000031f0: 00da 0467 6c6f 62da 0665 7874 656e 64da  ...glob..extend.
-00003200: 0862 6173 656e 616d 6529 1072 7a00 0000  .basename).rz...
-00003210: 727b 0000 005a 1863 6f6e 6669 675f 6e72  r{...Z.config_nr
-00003220: 756e 6e65 725f 696e 7465 7266 6163 655a  unner_interfaceZ
-00003230: 1a63 6f6e 6669 675f 6e72 756e 6e65 725f  .config_nrunner_
-00003240: 7265 7175 6972 656d 656e 745a 0c63 6f6e  requirementZ.con
-00003250: 6669 675f 6368 6563 6b5a 1163 6f6e 6669  fig_checkZ.confi
-00003260: 675f 6368 6563 6b5f 756e 6974 5a11 636f  g_check_unitZ.co
-00003270: 6e66 6967 5f63 6865 636b 5f6a 6f62 735a  nfig_check_jobsZ
-00003280: 0f66 756e 6374 696f 6e61 6c5f 7061 7468  .functional_path
-00003290: da0a 7265 6665 7265 6e63 6573 5a20 636f  ..referencesZ co
-000032a0: 6e66 6967 5f63 6865 636b 5f66 756e 6374  nfig_check_funct
-000032b0: 696f 6e61 6c5f 7061 7261 6c6c 656c 5a1e  ional_parallelZ.
-000032c0: 636f 6e66 6967 5f63 6865 636b 5f66 756e  config_check_fun
-000032d0: 6374 696f 6e61 6c5f 7365 7269 616c 5a13  ctional_serialZ.
-000032e0: 636f 6e66 6967 5f63 6865 636b 5f73 7461  config_check_sta
-000032f0: 7469 635a 1563 6f6e 6669 675f 6368 6563  ticZ.config_chec
-00003300: 6b5f 6f70 7469 6f6e 616c 5a0f 6f70 7469  k_optionalZ.opti
-00003310: 6f6e 616c 5f70 6c75 6769 6e5a 0b70 6c75  onal_pluginZ.plu
-00003320: 6769 6e5f 6e61 6d65 da07 7061 7474 6572  gin_name..patter
-00003330: 6e72 1300 0000 7213 0000 0072 1400 0000  nr....r....r....
-00003340: da0d 6372 6561 7465 5f73 7569 7465 7339  ..create_suites9
-00003350: 0200 0073 f600 0000 0401 0405 0401 0203  ...s............
-00003360: 0201 0201 0201 04fc 0207 0201 0201 0201  ................
-00003370: 04fc 0207 0201 0201 0201 04fc 0207 0201  ................
-00003380: 0201 0201 04fc 0207 0201 0201 0201 04fc  ................
-00003390: 0207 0201 0201 0201 04fc 0207 0201 0201  ................
-000033a0: 0201 04fc 02db 06fd 0632 02ff 0802 02fe  .........2......
-000033b0: 0804 0202 0201 0201 0201 04fc 04ff 060a  ................
-000033c0: 02ff 0802 02fe 0804 0202 0201 0201 0201  ................
-000033d0: 04fc 04ff 0a09 0401 0a01 04ff 0408 0201  ................
-000033e0: 0602 0601 02fe 06fd 0a09 0401 0a01 04ff  ................
-000033f0: 0409 04ff 0a04 0a01 0a01 1201 0a02 0a01  ................
-00003400: 0a01 1201 0c02 0e01 1401 0401 0c02 0c01  ................
-00003410: 02fe 04ff 0a06 0801 0401 0401 0401 02ff  ................
-00003420: 04ff 0a06 0202 08ff 0803 0401 0a01 04ff  ................
-00003430: 0c04 0a01 0e01 1201 0c02 0a01 0801 0e01  ................
-00003440: 0c01 0c01 0a01 1601 0480 1202 0402 7293  ..............r.
-00003450: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00003460: 0b00 0000 0900 0000 4300 0000 7378 0200  ........C...sx..
-00003470: 0064 0164 0164 0164 0164 0164 0164 0164  .d.d.d.d.d.d.d.d
-00003480: 0164 029c 087c 005f 0074 017c 006a 0283  .d...|._.t.|.j..
-00003490: 0164 036b 0472 1c7c 006a 0264 0319 00a0  .d.k.r.|.j.d....
-000034a0: 0364 04a1 017c 005f 0274 017c 006a 0483  .d...|._.t.|.j..
-000034b0: 0164 036b 0472 2c7c 006a 0464 0319 00a0  .d.k.r,|.j.d....
-000034c0: 0364 04a1 017c 005f 0474 017c 006a 0583  .d...|._.t.|.j..
-000034d0: 0164 036b 0472 3c7c 006a 0564 0319 00a0  .d.k.r<|.j.d....
-000034e0: 0364 04a1 017c 005f 057c 006a 0672 8074  .d...|._.|.j.r.t
-000034f0: 077c 0083 017d 017c 0174 087c 0083 0137  .|...}.|.t.|...7
-00003500: 007d 0167 007d 027c 0144 005d 167d 037c  .}.g.}.|.D.].}.|
-00003510: 036a 0964 0519 0044 005d 0e7d 047c 04a0  .j.d...D.].}.|..
-00003520: 0a64 06a1 0172 627c 02a0 0b7c 0464 0619  .d...rb|...|.d..
-00003530: 00a1 0101 0071 5471 4d74 0c74 0d7c 0283  .....qTqMt.t.|..
-00003540: 0183 017d 0574 0e64 0774 017c 0583 019b  ...}.t.d.t.|....
-00003550: 0064 089d 0383 0101 0074 0e64 09a0 0f7c  .d.......t.d...|
-00003560: 05a1 0183 0101 0074 1064 0383 0101 006e  .......t.d.....n
-00003570: 657c 006a 0472 a07c 006a 0444 005d 187d  e|.j.r.|.j.D.].}
-00003580: 067c 067c 006a 00a0 11a1 0076 0172 9974  .|.|.j.....v.r.t
-00003590: 0e7c 0664 0a83 0201 0074 1064 0383 0101  .|.d.....t.d....
-000035a0: 0071 8664 0b7c 006a 007c 063c 0071 866e  .q.d.|.j.|.<.q.n
-000035b0: 457c 006a 0572 c964 0c64 0d84 007c 006a  E|.j.r.d.d...|.j
-000035c0: 0044 0083 017c 005f 007c 006a 0544 005d  .D...|._.|.j.D.]
-000035d0: 187d 067c 067c 006a 00a0 11a1 0076 0172  .}.|.|.j.....v.r
-000035e0: c274 0e7c 0664 0a83 0201 0074 1064 0383  .t.|.d.....t.d..
-000035f0: 0101 0071 af64 017c 006a 007c 063c 0071  ...q.d.|.j.|.<.q
-00003600: af6e 1c7c 006a 0573 dd7c 006a 0473 dd74  .n.|.j.s.|.j.s.t
-00003610: 0e64 0e83 0101 0064 0f64 0d84 007c 006a  .d.....d.d...|.j
-00003620: 0044 0083 017c 005f 006e 0874 0e64 1083  .D...|._.n.t.d..
-00003630: 0101 0074 1064 1183 0101 0067 007d 017c  ...t.d.....g.}.|
-00003640: 006a 0064 1219 0072 f27c 0174 077c 0083  .j.d...r.|.t.|..
-00003650: 0137 007d 017c 0174 087c 0083 0137 007d  .7.}.|.t.|...7.}
-00003660: 0164 1367 0064 14a2 0164 159c 027d 0774  .d.g.d...d...}.t
-00003670: 12a0 13a1 0064 166b 0290 0172 1f74 1474  .....d.k...r.t.t
-00003680: 15a0 16a1 0064 171b 0083 017d 087c 0144  .....d.....}.|.D
-00003690: 005d 0e7d 037c 036a 1764 186b 0290 0172  .].}.|.j.d.k...r
-000036a0: 1d7c 087c 036a 0964 193c 0090 0171 1074  .|.|.j.d.<...q.t
-000036b0: 187c 077c 0183 028f 0d7d 097c 09a0 19a1  .|.|.....}.|....
-000036c0: 007d 0a57 0064 0004 0004 0083 0301 007c  .}.W.d.........|
-000036d0: 0a53 0031 0090 0173 3577 0101 0001 0001  .S.1...s5w......
-000036e0: 0059 0001 007c 0a53 0029 1a4e 4629 0872  .Y...|.S.).NF).r
-000036f0: 8a00 0000 fa07 6a6f 622d 6170 6972 7f00  ......job-apir..
-00003700: 0000 7283 0000 0072 8400 0000 7285 0000  ..r....r....r...
-00003710: 0072 8600 0000 728b 0000 0072 0100 0000  .r....r....r....
-00003720: fa01 2c72 6d00 0000 7228 0000 007a 1246  ..,rm...r(...z.F
-00003730: 6561 7475 7265 7320 636f 7665 7265 6420  eatures covered 
-00003740: 287a 0229 3ada 010a 7a22 6973 206e 6f74  (z.):...z"is not
-00003750: 2069 6e20 7468 6520 6c69 7374 206f 6620   in the list of 
-00003760: 7661 6c69 6420 7465 7374 732e 5463 0100  valid tests.Tc..
-00003770: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00003780: 0000 5300 0000 f312 0000 0069 007c 005d  ..S........i.|.]
-00003790: 057d 017c 0164 0093 0271 0253 00a9 0154  .}.|.d...q.S...T
-000037a0: 7213 0000 00a9 02da 022e 30da 0178 7213  r.........0..xr.
-000037b0: 0000 0072 1300 0000 7214 0000 00da 0a3c  ...r....r......<
-000037c0: 6469 6374 636f 6d70 3e0e 0300 00f3 0200  dictcomp>.......
-000037d0: 0000 1200 7a18 6d61 696e 2e3c 6c6f 6361  ....z.main.<loca
-000037e0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7a32  ls>.<dictcomp>z2
-000037f0: 4e6f 2074 6573 7420 7765 7265 2073 656c  No test were sel
-00003800: 6563 7465 6420 746f 2072 756e 2c20 7275  ected to run, ru
-00003810: 6e6e 696e 6720 616c 6c20 6f66 2074 6865  nning all of the
-00003820: 6d2e 6301 0000 0000 0000 0000 0000 0002  m.c.............
-00003830: 0000 0004 0000 0053 0000 0072 9700 0000  .......S...r....
-00003840: 7298 0000 0072 1300 0000 7299 0000 0072  r....r....r....r
-00003850: 1300 0000 7213 0000 0072 1400 0000 729c  ....r....r....r.
-00003860: 0000 001a 0300 0072 9d00 0000 7a2a 536f  .......r....z*So
-00003870: 6d65 7468 696e 6720 7765 6e74 2077 726f  mething went wro
-00003880: 6e67 2c20 706c 6561 7365 2072 6570 6f72  ng, please repor
-00003890: 7420 6120 6275 6721 726e 0000 0072 9400  t a bug!rn...r..
-000038a0: 0000 7a11 6176 6f63 6164 6f2d 7365 6c66  ..z.avocado-self
-000038b0: 7465 7374 7329 03da 0446 4149 4cda 0545  tests)...FAIL..E
-000038c0: 5252 4f52 da09 494e 5445 5252 5550 5429  RROR..INTERRUPT)
-000038d0: 0272 6f00 0000 7a1c 6a6f 622e 6f75 7470  .ro...z.job.outp
-000038e0: 7574 2e74 6573 746c 6f67 732e 7374 6174  ut.testlogs.stat
-000038f0: 7573 6573 da07 6161 7263 6836 3472 7e00  uses..aarch64r~.
-00003900: 0000 7289 0000 0072 7300 0000 291a 728c  ..r....rs...).r.
-00003910: 0000 0072 7800 0000 7279 0000 00da 0573  ...rx...ry.....s
-00003920: 706c 6974 da06 7365 6c65 6374 da04 736b  plit..select..sk
-00003930: 6970 5a0d 6c69 7374 5f66 6561 7475 7265  ipZ.list_feature
-00003940: 7372 7c00 0000 7293 0000 0072 2c00 0000  sr|...r....r,...
-00003950: 720e 0000 0072 5f00 0000 da06 736f 7274  r....r_.....sort
-00003960: 6564 da03 7365 74da 0570 7269 6e74 720b  ed..set..printr.
-00003970: 0000 00da 0465 7869 74da 046b 6579 73da  .....exit..keys.
-00003980: 0870 6c61 7466 6f72 6dda 076d 6163 6869  .platform..machi
-00003990: 6e65 da03 696e 74da 0f6d 756c 7469 7072  ne..int..multipr
-000039a0: 6f63 6573 7369 6e67 da09 6370 755f 636f  ocessing..cpu_co
-000039b0: 756e 74da 046e 616d 6572 0400 0000 723e  unt..namer....r>
-000039c0: 0000 0029 0b72 7a00 0000 727b 0000 00da  ...).rz...r{....
-000039d0: 0866 6561 7475 7265 7372 4000 0000 da08  .featuresr@.....
-000039e0: 7661 7269 616e 7473 5a0f 756e 6971 7565  variantsZ.unique
-000039f0: 5f66 6561 7475 7265 73da 0465 6c65 6d72  _features..elemr
-00003a00: 2c00 0000 5a0c 6d61 785f 7061 7261 6c6c  ,...Z.max_parall
-00003a10: 656c 7241 0000 0072 1600 0000 7213 0000  elrA...r....r...
-00003a20: 0072 1300 0000 7214 0000 00da 046d 6169  .r....r......mai
-00003a30: 6ede 0200 0073 8800 0000 0203 0201 0201  n....s..........
-00003a40: 0201 0201 0201 0201 0201 08f8 0e0c 1201  ................
-00003a50: 0e01 1201 0e01 1201 0603 0801 0c01 0401  ................
-00003a60: 0801 0e01 0a01 0e01 0280 02fe 0c04 1401  ................
-00003a70: 0e01 0a01 0603 0a01 0e01 0a01 0a01 0c02  ................
-00003a80: 02fb 0608 1202 0a02 0e01 0a01 0a01 0c02  ................
-00003a90: 02fb 0c08 0801 1401 0803 0801 0402 0a01  ................
-00003aa0: 0c01 0c01 0206 0601 06fe 0e06 1001 0801  ................
-00003ab0: 0c01 0a01 0480 0c02 0a01 0aff 0402 12fe  ................
-00003ac0: 0402 72b3 0000 00da 085f 5f6d 6169 6e5f  ..r......__main_
-00003ad0: 5f29 1a72 6000 0000 728d 0000 0072 8e00  _).r`...r....r..
-00003ae0: 0000 72ad 0000 0072 0900 0000 72aa 0000  ..r....r....r...
-00003af0: 0072 3300 0000 da03 7379 73da 0761 766f  .r3.....sys..avo
-00003b00: 6361 646f 7202 0000 00da 0c61 766f 6361  cador......avoca
-00003b10: 646f 2e63 6f72 6572 0300 0000 5a10 6176  do.corer....Z.av
-00003b20: 6f63 6164 6f2e 636f 7265 2e6a 6f62 7204  ocado.core.jobr.
-00003b30: 0000 00da 1261 766f 6361 646f 2e63 6f72  .....avocado.cor
-00003b40: 652e 7375 6974 6572 0500 0000 5a0f 7365  e.suiter....Z.se
-00003b50: 6c66 7465 7374 732e 7574 696c 7372 0600  lftests.utilsr..
-00003b60: 0000 7207 0000 0072 6600 0000 727c 0000  ..r....rf...r|..
-00003b70: 0072 9300 0000 72b3 0000 0072 5500 0000  .r....r....rU...
-00003b80: 727a 0000 0072 a800 0000 7213 0000 0072  rz...r....r....r
-00003b90: 1300 0000 7213 0000 0072 1400 0000 da08  ....r....r......
-00003ba0: 3c6d 6f64 756c 653e 0100 0000 7334 0000  <module>....s4..
-00003bb0: 0008 0208 0108 0108 0108 0108 0108 0108  ................
-00003bc0: 010c 020c 010c 010c 010c 0110 0300 7f08  ................
-00003bd0: 3708 3000 7f00 7f08 4200 7f08 2608 5b06  7.0.....B...&.[.
-00003be0: 0112 0104 fe                             .....
+00002bd0: 640c 6407 6407 6407 6405 9c04 640d 6407  d.d.d.d.d...d.d.
+00002be0: 6407 6407 6405 9c04 6708 640e 9c03 7d02  d.d.d...g.d...}.
+00002bf0: 7400 640f 8301 724f 6410 7c00 6a01 7601  t.d...rOd.|.j.v.
+00002c00: 724f 7c02 6411 1900 a002 6412 6407 6407  rO|.d.....d.d.d.
+00002c10: 6407 6405 9c04 a101 0100 7400 6413 8301  d.d.......t.d...
+00002c20: 7264 6414 7c00 6a01 7601 7264 7c02 6411  rdd.|.j.v.rd|.d.
+00002c30: 1900 a002 6415 6407 6407 6407 6405 9c04  ....d.d.d.d.d...
+00002c40: a101 0100 7400 6416 8301 7279 6417 7c00  ....t.d...ryd.|.
+00002c50: 6a01 7601 7279 7c02 6411 1900 a002 6418  j.v.ry|.d.....d.
+00002c60: 6407 6407 6407 6405 9c04 a101 0100 7c00  d.d.d.d.......|.
+00002c70: 6a03 6419 1900 7287 7c01 a002 7404 a005  j.d...r.|...t...
+00002c80: 7c02 6419 a102 a101 0100 641a 6701 641b  |.d.......d.g.d.
+00002c90: 641c 641d 6901 641c 641e 6901 6702 641f  d.d.i.d.d.i.g.d.
+00002ca0: 9c03 7d03 7c00 6a03 6420 1900 72a2 7c01  ..}.|.j.d ..r.|.
+00002cb0: a002 7404 a005 7c03 6420 a102 a101 0100  ..t...|.d ......
+00002cc0: 6421 6422 6901 7d04 7c00 6a03 6423 1900  d!d"i.}.|.j.d#..
+00002cd0: 72be 7406 a006 7c04 a101 7d05 6424 6701  r.t...|...}.d$g.
+00002ce0: 7c05 6425 3c00 7c01 a002 7404 a005 7c05  |.d%<.|...t...|.
+00002cf0: 6423 a102 a101 0100 7c00 6a03 6426 1900  d#......|.j.d&..
+00002d00: 72d6 7406 a006 7c04 a101 7d06 6427 6701  r.t...|...}.d'g.
+00002d10: 7c06 6425 3c00 7c01 a002 7404 a005 7c06  |.d%<.|...t...|.
+00002d20: 6426 a102 a101 0100 7c00 6a03 6428 1900  d&......|.j.d(..
+00002d30: 9001 7227 7407 6a08 a009 6429 6428 a102  ..r't.j...d)d(..
+00002d40: 7d07 740a a00a 7407 6a08 a009 7c07 642a  }.t...t.j...|.d*
+00002d50: a102 a101 7d08 7c08 a00b 7407 6a08 a009  ....}.|...t.j...
+00002d60: 7c07 642b a102 7407 6a08 a009 7c07 642c  |.d+..t.j...|.d,
+00002d70: a102 6702 a101 0100 7406 a006 7c04 a101  ..g.....t...|...
+00002d80: 7d09 7c08 7c09 6425 3c00 7c01 a002 7404  }.|.|.d%<.|...t.
+00002d90: a005 7c09 642d a102 a101 0100 7406 a006  ..|.d-......t...
+00002da0: 7c04 a101 7d0a 642e 6701 7c0a 6425 3c00  |...}.d.g.|.d%<.
+00002db0: 641b 7c0a 642f 3c00 7c01 a002 7404 a005  d.|.d/<.|...t...
+00002dc0: 7c0a 6430 a102 a101 0100 7c00 6a03 6431  |.d0......|.j.d1
+00002dd0: 1900 9001 7242 7406 a006 7c04 a101 7d0b  ....rBt...|...}.
+00002de0: 740a a00a 6432 a101 7c0b 6425 3c00 7c01  t...d2..|.d%<.|.
+00002df0: a002 7404 a005 7c0b 6431 a102 a101 0100  ..t...|.d1......
+00002e00: 7c00 6a03 6433 1900 9001 727f 7406 a006  |.j.d3....r.t...
+00002e10: 7c04 a101 7d0c 6700 7c0c 6425 3c00 740a  |...}.g.|.d%<.t.
+00002e20: a00a 6434 a101 4400 5d1f 7d0d 7407 6a08  ..d4..D.].}.t.j.
+00002e30: a00c 7c0d a101 7d0e 7c0e 7c00 6a01 7601  ..|...}.|.|.j.v.
+00002e40: 9001 7274 7c0d 9b00 6435 9d02 7d0f 7c0c  ..rt|...d5..}.|.
+00002e50: 6425 0500 1900 740a a00a 7c0f a101 3700  d%....t...|...7.
+00002e60: 0300 3c00 9001 7156 7c01 a002 7404 a005  ..<...qV|...t...
+00002e70: 7c0c 6433 a102 a101 0100 7c01 5300 2936  |.d3......|.S.)6
+00002e80: 4e7a 2e73 656c 6674 6573 7473 2f66 756e  Nz.selftests/fun
+00002e90: 6374 696f 6e61 6c2f 7465 7374 5f6e 7275  ctional/test_nru
+00002ea0: 6e6e 6572 5f69 6e74 6572 6661 6365 2e70  nner_interface.p
+00002eb0: 79da 0672 756e 6e65 727a 0e61 766f 6361  y..runnerz.avoca
+00002ec0: 646f 2d72 756e 6e65 72e9 0200 0000 2904  do-runner.....).
+00002ed0: 727d 0000 007a 1e72 756e 6e61 626c 652d  r}...z.runnable-
+00002ee0: 7275 6e2d 6e6f 2d61 7267 732d 6578 6974  run-no-args-exit
+00002ef0: 2d63 6f64 657a 1f72 756e 6e61 626c 652d  -codez.runnable-
+00002f00: 7275 6e2d 7572 692d 6f6e 6c79 2d65 7869  run-uri-only-exi
+00002f10: 742d 636f 6465 7a1a 7461 736b 2d72 756e  t-codez.task-run
+00002f20: 2d69 642d 6f6e 6c79 2d65 7869 742d 636f  -id-only-exit-co
+00002f30: 6465 7a16 6176 6f63 6164 6f2d 7275 6e6e  dez.avocado-runn
+00002f40: 6572 2d64 7279 2d72 756e 7201 0000 007a  er-dry-runr....z
+00002f50: 1361 766f 6361 646f 2d72 756e 6e65 722d  .avocado-runner-
+00002f60: 6e6f 6f70 7a18 6176 6f63 6164 6f2d 7275  noopz.avocado-ru
+00002f70: 6e6e 6572 2d65 7865 632d 7465 7374 7a1e  nner-exec-testz.
+00002f80: 6176 6f63 6164 6f2d 7275 6e6e 6572 2d70  avocado-runner-p
+00002f90: 7974 686f 6e2d 756e 6974 7465 7374 7a23  ython-unittestz#
+00002fa0: 6176 6f63 6164 6f2d 7275 6e6e 6572 2d61  avocado-runner-a
+00002fb0: 766f 6361 646f 2d69 6e73 7472 756d 656e  vocado-instrumen
+00002fc0: 7465 647a 1261 766f 6361 646f 2d72 756e  tedz.avocado-run
+00002fd0: 6e65 722d 7461 707a 1b61 766f 6361 646f  ner-tapz.avocado
+00002fe0: 2d72 756e 6e65 722d 706f 646d 616e 2d69  -runner-podman-i
+00002ff0: 6d61 6765 726c 0000 007a 1f61 766f 6361  magerl...z.avoca
+00003000: 646f 2d66 7261 6d65 776f 726b 2d70 6c75  do-framework-plu
+00003010: 6769 6e2d 676f 6c61 6e67 5a06 676f 6c61  gin-golangZ.gola
+00003020: 6e67 726d 0000 007a 1561 766f 6361 646f  ngrm...z.avocado
+00003030: 2d72 756e 6e65 722d 676f 6c61 6e67 7a1e  -runner-golangz.
+00003040: 6176 6f63 6164 6f2d 6672 616d 6577 6f72  avocado-framewor
+00003050: 6b2d 706c 7567 696e 2d72 6f62 6f74 da05  k-plugin-robot..
+00003060: 726f 626f 747a 1461 766f 6361 646f 2d72  robotz.avocado-r
+00003070: 756e 6e65 722d 726f 626f 747a 2061 766f  unner-robotz avo
+00003080: 6361 646f 2d66 7261 6d65 776f 726b 2d70  cado-framework-p
+00003090: 6c75 6769 6e2d 616e 7369 626c 65da 0761  lugin-ansible..a
+000030a0: 6e73 6962 6c65 7a1d 6176 6f63 6164 6f2d  nsiblez.avocado-
+000030b0: 7275 6e6e 6572 2d61 6e73 6962 6c65 2d6d  runner-ansible-m
+000030c0: 6f64 756c 65fa 116e 7275 6e6e 6572 2d69  odule..nrunner-i
+000030d0: 6e74 6572 6661 6365 7a30 7365 6c66 7465  nterfacez0selfte
+000030e0: 7374 732f 6675 6e63 7469 6f6e 616c 2f73  sts/functional/s
+000030f0: 6572 6961 6c2f 7465 7374 5f72 6571 7569  erial/test_requi
+00003100: 7265 6d65 6e74 732e 7079 726e 0000 00da  rements.pyrn....
+00003110: 0773 7061 776e 6572 da07 7072 6f63 6573  .spawner..proces
+00003120: 73da 0670 6f64 6d61 6e29 0372 2700 0000  s..podman).r'...
+00003130: 7273 0000 0072 6d00 0000 fa13 6e72 756e  rs...rm.....nrun
+00003140: 6e65 722d 7265 7175 6972 656d 656e 7472  ner-requirementr
+00003150: 7400 0000 54da 0475 6e69 747a 0f73 656c  t...T..unitz.sel
+00003160: 6674 6573 7473 2f75 6e69 742f 7227 0000  ftests/unit/r'..
+00003170: 00da 046a 6f62 737a 0f73 656c 6674 6573  ...jobsz.selftes
+00003180: 7473 2f6a 6f62 732f da0a 6675 6e63 7469  ts/jobs/..functi
+00003190: 6f6e 616c 5a09 7365 6c66 7465 7374 737a  onalZ.selftestsz
+000031a0: 0874 6573 742a 2e70 79da 0575 7469 6c73  .test*.py..utils
+000031b0: da06 706c 7567 696e fa13 6675 6e63 7469  ..plugin..functi
+000031c0: 6f6e 616c 2d70 6172 616c 6c65 6c7a 1c73  onal-parallelz.s
+000031d0: 656c 6674 6573 7473 2f66 756e 6374 696f  elftests/functio
+000031e0: 6e61 6c2f 7365 7269 616c 2f72 7300 0000  nal/serial/rs...
+000031f0: 7a11 6675 6e63 7469 6f6e 616c 2d73 6572  z.functional-ser
+00003200: 6961 6cfa 0d73 7461 7469 632d 6368 6563  ial..static-chec
+00003210: 6b73 7a0e 7365 6c66 7465 7374 732f 2a2e  ksz.selftests/*.
+00003220: 7368 fa10 6f70 7469 6f6e 616c 2d70 6c75  sh..optional-plu
+00003230: 6769 6e73 7a12 6f70 7469 6f6e 616c 5f70  ginsz.optional_p
+00003240: 6c75 6769 6e73 2f2a 7a08 2f74 6573 7473  lugins/*z./tests
+00003250: 2f2a 290d 7206 0000 0072 7900 0000 725f  /*).r....ry...r_
+00003260: 0000 00da 0a64 6963 745f 7465 7374 7372  .....dict_testsr
+00003270: 0500 0000 723d 0000 00da 0463 6f70 7972  ....r=.....copyr
+00003280: 0900 0000 720a 0000 0072 0b00 0000 da04  ....r....r......
+00003290: 676c 6f62 da06 6578 7465 6e64 da08 6261  glob..extend..ba
+000032a0: 7365 6e61 6d65 2910 727a 0000 0072 7b00  sename).rz...r{.
+000032b0: 0000 5a18 636f 6e66 6967 5f6e 7275 6e6e  ..Z.config_nrunn
+000032c0: 6572 5f69 6e74 6572 6661 6365 5a1a 636f  er_interfaceZ.co
+000032d0: 6e66 6967 5f6e 7275 6e6e 6572 5f72 6571  nfig_nrunner_req
+000032e0: 7569 7265 6d65 6e74 5a0c 636f 6e66 6967  uirementZ.config
+000032f0: 5f63 6865 636b 5a11 636f 6e66 6967 5f63  _checkZ.config_c
+00003300: 6865 636b 5f75 6e69 745a 1163 6f6e 6669  heck_unitZ.confi
+00003310: 675f 6368 6563 6b5f 6a6f 6273 5a0f 6675  g_check_jobsZ.fu
+00003320: 6e63 7469 6f6e 616c 5f70 6174 68da 0a72  nctional_path..r
+00003330: 6566 6572 656e 6365 735a 2063 6f6e 6669  eferencesZ confi
+00003340: 675f 6368 6563 6b5f 6675 6e63 7469 6f6e  g_check_function
+00003350: 616c 5f70 6172 616c 6c65 6c5a 1e63 6f6e  al_parallelZ.con
+00003360: 6669 675f 6368 6563 6b5f 6675 6e63 7469  fig_check_functi
+00003370: 6f6e 616c 5f73 6572 6961 6c5a 1363 6f6e  onal_serialZ.con
+00003380: 6669 675f 6368 6563 6b5f 7374 6174 6963  fig_check_static
+00003390: 5a15 636f 6e66 6967 5f63 6865 636b 5f6f  Z.config_check_o
+000033a0: 7074 696f 6e61 6c5a 0f6f 7074 696f 6e61  ptionalZ.optiona
+000033b0: 6c5f 706c 7567 696e 5a0b 706c 7567 696e  l_pluginZ.plugin
+000033c0: 5f6e 616d 65da 0770 6174 7465 726e 7213  _name..patternr.
+000033d0: 0000 0072 1300 0000 7214 0000 00da 0d63  ...r....r......c
+000033e0: 7265 6174 655f 7375 6974 6573 3902 0000  reate_suites9...
+000033f0: 7316 0100 0004 0104 0504 0102 0302 0102  s...............
+00003400: 0102 0104 fc02 0702 0102 0102 0104 fc02  ................
+00003410: 0702 0102 0102 0104 fc02 0702 0102 0102  ................
+00003420: 0104 fc02 0702 0102 0102 0104 fc02 0702  ................
+00003430: 0102 0102 0104 fc02 0702 0102 0102 0104  ................
+00003440: fc02 0702 0102 0102 0104 fc02 d506 fd06  ................
+00003450: 3802 ff08 0202 fe08 0402 0202 0102 0102  8...............
+00003460: 0104 fc04 ff06 0a02 ff08 0202 fe08 0402  ................
+00003470: 0202 0102 0102 0104 fc04 ff06 0a02 ff08  ................
+00003480: 0202 fe08 0402 0202 0102 0102 0104 fc04  ................
+00003490: ff0a 0904 010a 0104 ff04 0802 0106 0206  ................
+000034a0: 0102 fe06 fd0a 0904 010a 0104 ff04 0904  ................
+000034b0: ff0a 040a 010a 0112 010a 020a 010a 0112  ................
+000034c0: 010c 020e 0114 0104 010c 020c 0102 fe04  ................
+000034d0: ff0a 0608 0104 0104 0104 0102 ff04 ff0a  ................
+000034e0: 0602 0208 ff08 0304 010a 0104 ff0c 040a  ................
+000034f0: 010e 0112 010c 020a 0108 010e 010c 010c  ................
+00003500: 010a 0116 0104 8012 0204 0272 9500 0000  ...........r....
+00003510: 6301 0000 0000 0000 0000 0000 000b 0000  c...............
+00003520: 0009 0000 0043 0000 0073 7802 0000 6401  .....C...sx...d.
+00003530: 6401 6401 6401 6401 6401 6401 6401 6402  d.d.d.d.d.d.d.d.
+00003540: 9c08 7c00 5f00 7401 7c00 6a02 8301 6403  ..|._.t.|.j...d.
+00003550: 6b04 721c 7c00 6a02 6403 1900 a003 6404  k.r.|.j.d.....d.
+00003560: a101 7c00 5f02 7401 7c00 6a04 8301 6403  ..|._.t.|.j...d.
+00003570: 6b04 722c 7c00 6a04 6403 1900 a003 6404  k.r,|.j.d.....d.
+00003580: a101 7c00 5f04 7401 7c00 6a05 8301 6403  ..|._.t.|.j...d.
+00003590: 6b04 723c 7c00 6a05 6403 1900 a003 6404  k.r<|.j.d.....d.
+000035a0: a101 7c00 5f05 7c00 6a06 7280 7407 7c00  ..|._.|.j.r.t.|.
+000035b0: 8301 7d01 7c01 7408 7c00 8301 3700 7d01  ..}.|.t.|...7.}.
+000035c0: 6700 7d02 7c01 4400 5d16 7d03 7c03 6a09  g.}.|.D.].}.|.j.
+000035d0: 6405 1900 4400 5d0e 7d04 7c04 a00a 6406  d...D.].}.|...d.
+000035e0: a101 7262 7c02 a00b 7c04 6406 1900 a101  ..rb|...|.d.....
+000035f0: 0100 7154 714d 740c 740d 7c02 8301 8301  ..qTqMt.t.|.....
+00003600: 7d05 740e 6407 7401 7c05 8301 9b00 6408  }.t.d.t.|.....d.
+00003610: 9d03 8301 0100 740e 6409 a00f 7c05 a101  ......t.d...|...
+00003620: 8301 0100 7410 6403 8301 0100 6e65 7c00  ....t.d.....ne|.
+00003630: 6a04 72a0 7c00 6a04 4400 5d18 7d06 7c06  j.r.|.j.D.].}.|.
+00003640: 7c00 6a00 a011 a100 7601 7299 740e 7c06  |.j.....v.r.t.|.
+00003650: 640a 8302 0100 7410 6403 8301 0100 7186  d.....t.d.....q.
+00003660: 640b 7c00 6a00 7c06 3c00 7186 6e45 7c00  d.|.j.|.<.q.nE|.
+00003670: 6a05 72c9 640c 640d 8400 7c00 6a00 4400  j.r.d.d...|.j.D.
+00003680: 8301 7c00 5f00 7c00 6a05 4400 5d18 7d06  ..|._.|.j.D.].}.
+00003690: 7c06 7c00 6a00 a011 a100 7601 72c2 740e  |.|.j.....v.r.t.
+000036a0: 7c06 640a 8302 0100 7410 6403 8301 0100  |.d.....t.d.....
+000036b0: 71af 6401 7c00 6a00 7c06 3c00 71af 6e1c  q.d.|.j.|.<.q.n.
+000036c0: 7c00 6a05 73dd 7c00 6a04 73dd 740e 640e  |.j.s.|.j.s.t.d.
+000036d0: 8301 0100 640f 640d 8400 7c00 6a00 4400  ....d.d...|.j.D.
+000036e0: 8301 7c00 5f00 6e08 740e 6410 8301 0100  ..|._.n.t.d.....
+000036f0: 7410 6411 8301 0100 6700 7d01 7c00 6a00  t.d.....g.}.|.j.
+00003700: 6412 1900 72f2 7c01 7407 7c00 8301 3700  d...r.|.t.|...7.
+00003710: 7d01 7c01 7408 7c00 8301 3700 7d01 6413  }.|.t.|...7.}.d.
+00003720: 6700 6414 a201 6415 9c02 7d07 7412 a013  g.d...d...}.t...
+00003730: a100 6416 6b02 9001 721f 7414 7415 a016  ..d.k...r.t.t...
+00003740: a100 6417 1b00 8301 7d08 7c01 4400 5d0e  ..d.....}.|.D.].
+00003750: 7d03 7c03 6a17 6418 6b02 9001 721d 7c08  }.|.j.d.k...r.|.
+00003760: 7c03 6a09 6419 3c00 9001 7110 7418 7c07  |.j.d.<...q.t.|.
+00003770: 7c01 8302 8f0d 7d09 7c09 a019 a100 7d0a  |.....}.|.....}.
+00003780: 5700 6400 0400 0400 8303 0100 7c0a 5300  W.d.........|.S.
+00003790: 3100 9001 7335 7701 0100 0100 0100 5900  1...s5w.......Y.
+000037a0: 0100 7c0a 5300 291a 4e46 2908 728c 0000  ..|.S.).NF).r...
+000037b0: 00fa 076a 6f62 2d61 7069 7281 0000 0072  ...job-apir....r
+000037c0: 8500 0000 7286 0000 0072 8700 0000 7288  ....r....r....r.
+000037d0: 0000 0072 8d00 0000 7201 0000 00fa 012c  ...r....r......,
+000037e0: 726d 0000 0072 2800 0000 7a12 4665 6174  rm...r(...z.Feat
+000037f0: 7572 6573 2063 6f76 6572 6564 2028 7a02  ures covered (z.
+00003800: 293a da01 0a7a 2269 7320 6e6f 7420 696e  ):...z"is not in
+00003810: 2074 6865 206c 6973 7420 6f66 2076 616c   the list of val
+00003820: 6964 2074 6573 7473 2e54 6301 0000 0000  id tests.Tc.....
+00003830: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00003840: 0000 00f3 1200 0000 6900 7c00 5d05 7d01  ........i.|.].}.
+00003850: 7c01 6400 9302 7102 5300 a901 5472 1300  |.d...q.S...Tr..
+00003860: 0000 a902 da02 2e30 da01 7872 1300 0000  .......0..xr....
+00003870: 7213 0000 0072 1400 0000 da0a 3c64 6963  r....r......<dic
+00003880: 7463 6f6d 703e 2103 0000 f302 0000 0012  tcomp>!.........
+00003890: 007a 186d 6169 6e2e 3c6c 6f63 616c 733e  .z.main.<locals>
+000038a0: 2e3c 6469 6374 636f 6d70 3e7a 324e 6f20  .<dictcomp>z2No 
+000038b0: 7465 7374 2077 6572 6520 7365 6c65 6374  test were select
+000038c0: 6564 2074 6f20 7275 6e2c 2072 756e 6e69  ed to run, runni
+000038d0: 6e67 2061 6c6c 206f 6620 7468 656d 2e63  ng all of them.c
+000038e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000038f0: 0400 0000 5300 0000 7299 0000 0072 9a00  ....S...r....r..
+00003900: 0000 7213 0000 0072 9b00 0000 7213 0000  ..r....r....r...
+00003910: 0072 1300 0000 7214 0000 0072 9e00 0000  .r....r....r....
+00003920: 2d03 0000 729f 0000 007a 2a53 6f6d 6574  -...r....z*Somet
+00003930: 6869 6e67 2077 656e 7420 7772 6f6e 672c  hing went wrong,
+00003940: 2070 6c65 6173 6520 7265 706f 7274 2061   please report a
+00003950: 2062 7567 2172 6e00 0000 7296 0000 007a   bug!rn...r....z
+00003960: 1161 766f 6361 646f 2d73 656c 6674 6573  .avocado-selftes
+00003970: 7473 2903 da04 4641 494c da05 4552 524f  ts)...FAIL..ERRO
+00003980: 52da 0949 4e54 4552 5255 5054 2902 726f  R..INTERRUPT).ro
+00003990: 0000 007a 1c6a 6f62 2e6f 7574 7075 742e  ...z.job.output.
+000039a0: 7465 7374 6c6f 6773 2e73 7461 7475 7365  testlogs.statuse
+000039b0: 73da 0761 6172 6368 3634 727e 0000 0072  s..aarch64r~...r
+000039c0: 8b00 0000 7273 0000 0029 1a72 8e00 0000  ....rs...).r....
+000039d0: 7278 0000 0072 7900 0000 da05 7370 6c69  rx...ry.....spli
+000039e0: 74da 0673 656c 6563 74da 0473 6b69 705a  t..select..skipZ
+000039f0: 0d6c 6973 745f 6665 6174 7572 6573 727c  .list_featuresr|
+00003a00: 0000 0072 9500 0000 722c 0000 0072 0e00  ...r....r,...r..
+00003a10: 0000 725f 0000 00da 0673 6f72 7465 64da  ..r_.....sorted.
+00003a20: 0373 6574 da05 7072 696e 7472 0b00 0000  .set..printr....
+00003a30: da04 6578 6974 da04 6b65 7973 da08 706c  ..exit..keys..pl
+00003a40: 6174 666f 726d da07 6d61 6368 696e 65da  atform..machine.
+00003a50: 0369 6e74 da0f 6d75 6c74 6970 726f 6365  .int..multiproce
+00003a60: 7373 696e 67da 0963 7075 5f63 6f75 6e74  ssing..cpu_count
+00003a70: da04 6e61 6d65 7204 0000 0072 3e00 0000  ..namer....r>...
+00003a80: 290b 727a 0000 0072 7b00 0000 da08 6665  ).rz...r{.....fe
+00003a90: 6174 7572 6573 7240 0000 00da 0876 6172  aturesr@.....var
+00003aa0: 6961 6e74 735a 0f75 6e69 7175 655f 6665  iantsZ.unique_fe
+00003ab0: 6174 7572 6573 da04 656c 656d 722c 0000  atures..elemr,..
+00003ac0: 005a 0c6d 6178 5f70 6172 616c 6c65 6c72  .Z.max_parallelr
+00003ad0: 4100 0000 7216 0000 0072 1300 0000 7213  A...r....r....r.
+00003ae0: 0000 0072 1400 0000 da04 6d61 696e f102  ...r......main..
+00003af0: 0000 7388 0000 0002 0302 0102 0102 0102  ..s.............
+00003b00: 0102 0102 0102 0108 f80e 0c12 010e 0112  ................
+00003b10: 010e 0112 0106 0308 010c 0104 0108 010e  ................
+00003b20: 010a 010e 0102 8002 fe0c 0414 010e 010a  ................
+00003b30: 0106 030a 010e 010a 010a 010c 0202 fb06  ................
+00003b40: 0812 020a 020e 010a 010a 010c 0202 fb0c  ................
+00003b50: 0808 0114 0108 0308 0104 020a 010c 010c  ................
+00003b60: 0102 0606 0106 fe0e 0610 0108 010c 010a  ................
+00003b70: 0104 800c 020a 010a ff04 0212 fe04 0272  ...............r
+00003b80: b500 0000 da08 5f5f 6d61 696e 5f5f 291a  ......__main__).
+00003b90: 7260 0000 0072 8f00 0000 7290 0000 0072  r`...r....r....r
+00003ba0: af00 0000 7209 0000 0072 ac00 0000 7233  ....r....r....r3
+00003bb0: 0000 00da 0373 7973 da07 6176 6f63 6164  .....sys..avocad
+00003bc0: 6f72 0200 0000 da0c 6176 6f63 6164 6f2e  or......avocado.
+00003bd0: 636f 7265 7203 0000 005a 1061 766f 6361  corer....Z.avoca
+00003be0: 646f 2e63 6f72 652e 6a6f 6272 0400 0000  do.core.jobr....
+00003bf0: da12 6176 6f63 6164 6f2e 636f 7265 2e73  ..avocado.core.s
+00003c00: 7569 7465 7205 0000 005a 0f73 656c 6674  uiter....Z.selft
+00003c10: 6573 7473 2e75 7469 6c73 7206 0000 0072  ests.utilsr....r
+00003c20: 0700 0000 7266 0000 0072 7c00 0000 7295  ....rf...r|...r.
+00003c30: 0000 0072 b500 0000 7255 0000 0072 7a00  ...r....rU...rz.
+00003c40: 0000 72aa 0000 0072 1300 0000 7213 0000  ..r....r....r...
+00003c50: 0072 1300 0000 7214 0000 00da 083c 6d6f  .r....r......<mo
+00003c60: 6475 6c65 3e01 0000 0073 3400 0000 0802  dule>....s4.....
+00003c70: 0801 0801 0801 0801 0801 0801 0801 0c02  ................
+00003c80: 0c01 0c01 0c01 0c01 1003 007f 0837 0830  .............7.0
+00003c90: 007f 007f 0842 007f 0839 085b 0601 1201  .....B...9.[....
+00003ca0: 04fe                                     ..
```

### Comparing `avocado-framework-98.0/selftests/__pycache__/utils.cpython-310.pyc` & `avocado-framework-99.0/selftests/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 5138 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 1214 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 1214 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6501  d.l.Z.d.d.l.Z.e.
 00000060: 6a06 a007 6501 6a06 a008 6509 a101 a101  j...e.j...e.....
 00000070: 5a0a 6501 6a06 a008 6501 6a06 a00b 650a  Z.e.j...e.j...e.
```

### Comparing `avocado-framework-98.0/selftests/check.py` & `avocado-framework-99.0/selftests/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -613,14 +613,20 @@
             },
             {
                 "runner": "avocado-runner-tap",
                 "runnable-run-no-args-exit-code": 0,
                 "runnable-run-uri-only-exit-code": 0,
                 "task-run-id-only-exit-code": 0,
             },
+            {
+                "runner": "avocado-runner-podman-image",
+                "runnable-run-no-args-exit-code": 0,
+                "runnable-run-uri-only-exit-code": 0,
+                "task-run-id-only-exit-code": 0,
+            },
         ],
     }
 
     if (
         python_module_available("avocado-framework-plugin-golang")
         and "golang" not in args.disable_plugin_checks
     ):
@@ -642,14 +648,27 @@
                 "runner": "avocado-runner-robot",
                 "runnable-run-no-args-exit-code": 0,
                 "runnable-run-uri-only-exit-code": 0,
                 "task-run-id-only-exit-code": 0,
             }
         )
 
+    if (
+        python_module_available("avocado-framework-plugin-ansible")
+        and "ansible" not in args.disable_plugin_checks
+    ):
+        config_nrunner_interface["run.dict_variants"].append(
+            {
+                "runner": "avocado-runner-ansible-module",
+                "runnable-run-no-args-exit-code": 0,
+                "runnable-run-uri-only-exit-code": 0,
+                "task-run-id-only-exit-code": 0,
+            }
+        )
+
     if args.dict_tests["nrunner-interface"]:
         suites.append(
             TestSuite.from_config(config_nrunner_interface, "nrunner-interface")
         )
 
     # ========================================================================
     # Run functional requirement tests
```

### Comparing `avocado-framework-98.0/selftests/check_tmp_dirs` & `avocado-framework-99.0/selftests/check_tmp_dirs`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/deployment/README.rst` & `avocado-framework-99.0/selftests/deployment/README.rst`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/copr/plugins.yml` & `avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/copr/plugins.yml`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/official/plugins.yml` & `avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/official/plugins.yml`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/pip/plugins.yml` & `avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/pip/plugins.yml`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/deployment/roles/avocado/tasks/rpm/plugins.yml` & `avocado-framework-99.0/selftests/deployment/roles/avocado/tasks/rpm/plugins.yml`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/deployment/roles/common/tasks/dependencies.yml` & `avocado-framework-99.0/selftests/deployment/roles/common/tasks/dependencies.yml`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/deployment/roles/common/tasks/repos.yml` & `avocado-framework-99.0/selftests/deployment/roles/common/tasks/repos.yml`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/deployment/roles/tests/tasks/main.yml` & `avocado-framework-99.0/selftests/deployment/roles/tests/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_argument_parsing.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_argument_parsing.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2951 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 870b 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 870b 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 6d0c 5a0c 0100 4700  d.l.m.Z.m.Z...G.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_basic.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_basic.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 22:01:20 2022 UTC, .py size: 48414 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b09d cc62 1ebd 0000  o..........b....
+00000000: 6f0d 0d0a 0000 0000 c55c 6563 1ebd 0000  o........\ec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 1a02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a08 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c09 5a09 6400 6402 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_coroutine.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_coroutine.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 731 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 db02 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 db02 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6506 8303 5a07 6401 5300 2906 e900 0000  e...Z.d.S.).....
 00000070: 004e 2901 da07 7072 6f63 6573 7329 03da  .N)...process)..
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_export_variables.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_export_variables.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1323 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 2b05 0000  o.......i&.b+...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 2b05 0000  o.......nKec+...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6406 6503 9b00  m.Z.m.Z...d.e...
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_fetch_asset.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_fetch_asset.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 5442 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4215 0000  o.......i&.bB...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4215 0000  o.......nKecB...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 0100 6406 5a0c 4700  m.Z.m.Z...d.Z.G.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_getdata.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_getdata.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1154 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 8204 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 8204 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 4700 6405 6406  m.Z.m.Z...G.d.d.
 00000070: 8400 6406 6509 8303 5a0a 650b 6407 6b02  ..d.e...Z.e.d.k.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_interrupt.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_interrupt.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 10204 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 dc27 0000  o.......i&.b.'..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 dc27 0000  o.......nKec.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 ee00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0a 5a0a 0100 6400 6403 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_job_api_features.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_job_api_features.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1321 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 2905 0000  o.......i&.b)...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 2905 0000  o.......nKec)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
 00000070: 6508 8303 5a09 650a 6408 6b02 722e 6502  e...Z.e.d.k.r.e.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_job_timeout.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_job_timeout.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 7129 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 d91b 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 d91b 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6404 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_journal.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_journal.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2049 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 0108 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 0108 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 6d0a 5a0a 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_json_variants.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_json_variants.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2404 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 6409 0000  o.......i&.bd...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 6409 0000  o.......nKecd...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 4700 6404 6405 8400 6405 6507 8303  ..G.d.d...d.e...
 00000070: 5a08 6509 6406 6b02 722c 6502 a00a a100  Z.e.d.k.r,e.....
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_list.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_list.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 10228 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 f427 0000  o.......i&.b.'..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 f427 0000  o.......nKec.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6402 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6400 6403 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_lv_utils.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_lv_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 5927 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 2717 0000  o.......i&.b'...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 2717 0000  o.......nKec'...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6404 6c0b 6d0c 5a0c 0100 4700  ..d.d.l.m.Z...G.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_nrunner.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_nrunner.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 8680 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 e821 0000  o.......i&.b.!..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 e821 0000  o.......nKec.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6501 6a0c 9b00 6405 9d02  m.Z...e.j...d...
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_nrunner_interface.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_nrunner_interface.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 4458 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 6a11 0000  o.......i&.bj...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 6a11 0000  o.......nKecj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6403 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 7a08 6400 6401 6c09 5a09  m.Z...z.d.d.l.Z.
 00000070: 6404 5a0a 5700 6e0b 0400 650b 792f 0100  d.Z.W.n...e.y/..
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_output.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_output.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 22884 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 6459 0000  o.......i&.bdY..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 6459 0000  o.......nKecdY..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d07 5a07 0100 6400 6403 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6400 6404 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_output_check.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_output_check.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 17925 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 0546 0000  o.......i&.b.F..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 0546 0000  o.......nKec.F..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6405 5a0b 6406 5a0c 6407 5a0d 6408  ..d.Z.d.Z.d.Z.d.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_replay.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_replay.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2870 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 360b 0000  o.......i&.b6...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 360b 0000  o.......nKec6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 0100 4700  d.l.m.Z.m.Z...G.
 00000070: 6405 6406 8400 6406 6509 8303 5a0a 650b  d.d...d.e...Z.e.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_requirements_cache.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_requirements_cache.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 3731 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 930e 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 930e 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6700 6404 a201 5a07 4700  m.Z...g.d...Z.G.
 00000060: 6405 6406 8400 6406 6506 8303 5a08 6401  d.d...d.e...Z.d.
 00000070: 5300 2907 e900 0000 004e 2901 da05 6361  S.)......N)...ca
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_resolver.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_resolver.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 4436 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 5411 0000  o.......i&.bT...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 5411 0000  o.......nKecT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c06 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 6d0c 5a0c 0100 4700  d.l.m.Z.m.Z...G.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_runner_asset.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_runner_asset.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2304 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 0009 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 0009 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6501  ..d.d.l.m.Z...e.
 00000060: 6a07 9b00 6404 9d02 5a08 4700 6405 6406  j...d...Z.G.d.d.
 00000070: 8400 6406 6502 6a09 8303 5a0a 4700 6407  ..d.e.j...Z.G.d.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_runner_package.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_runner_package.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2565 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 050a 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 050a 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6501  ..d.d.l.m.Z...e.
 00000060: 6a07 9b00 6404 9d02 5a08 4700 6405 6406  j...d...Z.G.d.d.
 00000070: 8400 6406 6502 6a09 8303 5a0a 4700 6407  ..d.e.j...Z.G.d.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_skiptests.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_skiptests.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 10472 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 e828 0000  o.......i&.b.(..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 e828 0000  o.......nKec.(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 6405 5a0c 6406 5a0d 6407  m.Z...d.Z.d.Z.d.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_software_manager.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_software_manager.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1379 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 6305 0000  o.......i&.bc...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 6305 0000  o.......nKecc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6507  m.Z.m.Z.m.Z...e.
 00000060: 6404 8301 6507 6405 8301 4700 6406 6407  d...e.d...G.d.d.
 00000070: 8400 6407 6506 8303 8301 8301 5a08 6509  ..d.e.......Z.e.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_statuses.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_statuses.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 6472 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4819 0000  o.......i&.bH...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4819 0000  o.......nKecH...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6601 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6700 6404 a201 5a09 6900  m.Z...g.d...Z.i.
 00000070: 6405 6406 6407 6701 6602 9301 6408 6406  d.d.d.g.f...d.d.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_streams.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_streams.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 5273 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 9914 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 9914 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 4700 6405 6406  m.Z.m.Z...G.d.d.
 00000070: 8400 6406 6509 8303 5a0a 650b 6407 6b02  ..d.e...Z.e.d.k.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_sysinfo.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_sysinfo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 5422 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 2e15 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 2e15 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6405  m.Z.m.Z.m.Z...d.
 00000070: 5a0b 4700 6406 6407 8400 6407 6509 8303  Z.G.d.d...d.e...
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_task_statemachine.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_task_statemachine.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1267 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 f304 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 f304 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_task_timeout.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_task_timeout.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1102 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4e04 0000  o.......i&.bN...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4e04 0000  o.......nKecN...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6404 5a07 4700 6405 6406  m.Z...d.Z.G.d.d.
 00000060: 8400 6406 6505 8303 5a08 6407 5300 2908  ..d.e...Z.d.S.).
 00000070: e900 0000 0029 01da 034a 6f62 2901 da06  .....)...Job)...
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_teststmpdir.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_teststmpdir.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 3114 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 2a0c 0000  o.......i&.b*...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 2a0c 0000  o.......nKec*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 6405 5a0c 6406 6505 6a0d  m.Z...d.Z.d.e.j.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_thirdparty_bugs.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_thirdparty_bugs.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2105 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 3908 0000  o.......i&.b9...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 3908 0000  o.......nKec9...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6404 6405 8400 5a08 4700 6406 6407  ..d.d...Z.G.d.d.
 00000070: 8400 6407 6502 6a09 8303 5a0a 650b 6408  ..d.e.j...Z.e.d.
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_unittest_compat.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_unittest_compat.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 3714 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 820e 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 820e 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6404 5a09 6405 5a0a 6406  m.Z...d.Z.d.Z.d.
 00000070: 5a0b 4700 6407 6408 8400 6408 6508 8303  Z.G.d.d...d.e...
```

### Comparing `avocado-framework-98.0/selftests/functional/__pycache__/test_utils.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/__pycache__/test_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 6435 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 2319 0000  o.......i&.b#...
+00000000: 6f0d 0d0a 0000 0000 c6bd 6a63 fe18 0000  o.........jc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 f800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6402 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6400 6403 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
@@ -369,16 +369,16 @@
 00001700: 007d 0364 047d 0474 06a0 077c 04a1 017d  .}.d.}.t...|...}
 00001710: 057c 006a 046a 057c 047c 0366 0367 017c  .|.j.j.|.|.f.g.|
 00001720: 0414 007d 067a 097c 05a0 0874 097c 06a1  ...}.z.|...t.|..
 00001730: 0201 0057 0064 0253 0004 0074 0a79 5e01  ...W.d.S...t.y^.
 00001740: 0001 0001 0064 057d 077c 077c 0474 0b74  .....d.}.|.|.t.t
 00001750: 0ca0 0da1 0083 0166 023b 007d 077c 00a0  .......f.;.}.|..
 00001760: 0e7c 07a1 0101 0059 0064 0253 0077 0029  .|.....Y.d.S.w.)
-00001770: 0672 1f00 0000 7242 0000 004e 677b 14ae  .r....rB...Ng{..
-00001780: 47e1 7a94 3f69 e803 0000 7a2a 4661 696c  G.z.?i....z*Fail
+00001770: 0672 1f00 0000 e932 0000 004e 677b 14ae  .r.....2...Ng{..
+00001780: 47e1 7a94 3f69 f401 0000 7a2a 4661 696c  G.z.?i....z*Fail
 00001790: 6564 2074 6f20 7275 6e20 4669 6c65 4c6f  ed to run FileLo
 000017a0: 636b 2077 6974 6820 2573 2070 6c61 7965  ck with %s playe
 000017b0: 7273 3a0a 2573 290f 7226 0000 00da 096d  rs:.%s).r&.....m
 000017c0: 6f6e 6f74 6f6e 6963 da05 7261 6e67 6572  onotonic..ranger
 000017d0: 0300 0000 720f 0000 0072 1000 0000 da0f  ....r....r......
 000017e0: 6d75 6c74 6970 726f 6365 7373 696e 67da  multiprocessing.
 000017f0: 0450 6f6f 6cda 036d 6170 7246 0000 00da  .Pool..maprF....
@@ -390,20 +390,20 @@
 00001850: 0000 721c 0000 0072 1d00 0000 da0d 7465  ..r....r......te
 00001860: 7374 5f66 696c 656c 6f63 6bc6 0000 0073  st_filelock....s
 00001870: 2200 0000 0806 0c01 0e01 0201 1cff 0280  "...............
 00001880: 1002 0401 0a01 1401 0201 1201 0c01 0401  ................
 00001890: 1401 1001 02fd 7a1a 4669 6c65 4c6f 636b  ......z.FileLock
 000018a0: 5465 7374 2e74 6573 745f 6669 6c65 6c6f  Test.test_filelo
 000018b0: 636b 4e29 0572 3e00 0000 723f 0000 0072  ckN).r>...r?...r
-000018c0: 4000 0000 7206 0000 0072 5400 0000 721c  @...r....rT...r.
+000018c0: 4000 0000 7206 0000 0072 5500 0000 721c  @...r....rU...r.
 000018d0: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
 000018e0: 0000 7247 0000 00c5 0000 0073 0600 0000  ..rG.......s....
 000018f0: 0800 0601 0e01 7247 0000 00da 085f 5f6d  ......rG.....__m
-00001900: 6169 6e5f 5f29 2172 4a00 0000 720c 0000  ain__)!rJ...r...
-00001910: 0072 4300 0000 da04 7374 6174 724e 0000  .rC.....statrN..
+00001900: 6169 6e5f 5f29 2172 4b00 0000 720c 0000  ain__)!rK...r...
+00001910: 0072 4300 0000 da04 7374 6174 724f 0000  .rC.....statrO..
 00001920: 0072 2600 0000 da08 756e 6974 7465 7374  .r&.....unittest
 00001930: da0d 6176 6f63 6164 6f2e 7574 696c 7372  ..avocado.utilsr
 00001940: 0200 0000 da16 6176 6f63 6164 6f2e 7574  ......avocado.ut
 00001950: 696c 732e 6669 6c65 6c6f 636b 7203 0000  ils.filelockr...
 00001960: 005a 1861 766f 6361 646f 2e75 7469 6c73  .Z.avocado.utils
 00001970: 2e73 7461 636b 7472 6163 6572 0400 0000  .stacktracer....
 00001980: 5a0f 7365 6c66 7465 7374 732e 7574 696c  Z.selftests.util
```

### Comparing `avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_assets.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_assets.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 12450 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 a230 0000  o.......i&.b.0..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 a230 0000  o.......nKec.0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6401 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_bystatus.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_bystatus.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 788 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 1403 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 1403 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6506 8303 5a07 6401 5300 2906  ..d.e...Z.d.S.).
 00000070: e900 0000 004e 2901 da07 7072 6f63 6573  .....N)...proces
```

### Comparing `avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_diff.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_diff.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2458 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 9a09 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 9a09 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 0100 4700 6405 6406  m.Z.m.Z...G.d.d.
```

### Comparing `avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_jobscripts.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_jobscripts.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 4426 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4a11 0000  o.......i&.bJ...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4a11 0000  o.......nKecJ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6405 5a0a 6406  m.Z.m.Z...d.Z.d.
 00000070: 5a0b 6407 5a0c 6408 5a0d 6409 5a0e 640a  Z.d.Z.d.Z.d.Z.d.
```

### Comparing `avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_jsonresult.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_jsonresult.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1858 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4207 0000  o.......i&.bB...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4207 0000  o.......nKecB...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 4700  d.l.m.Z.m.Z...G.
 00000060: 6405 6406 8400 6406 6507 8303 5a08 6401  d.d...d.e...Z.d.
 00000070: 5300 2907 e900 0000 004e 2901 da04 7061  S.)......N)...pa
```

### Comparing `avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_logs.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_logs.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 3474 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 920d 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 920d 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6405 5a0a 4700 6406 6407  m.Z...d.Z.G.d.d.
 00000070: 8400 6407 6509 8303 5a0b 4700 6408 6409  ..d.e...Z.G.d.d.
```

### Comparing `avocado-framework-98.0/selftests/functional/plugin/__pycache__/test_vmimage.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/plugin/__pycache__/test_vmimage.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2935 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 770b 0000  o.......i&.bw...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 770b 0000  o.......nKecw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6405 6406 8400 5a0c 6407 6408 8400  ..d.d...Z.d.d...
```

### Comparing `avocado-framework-98.0/selftests/functional/plugin/spawners/__pycache__/test_podman.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/plugin/spawners/__pycache__/test_podman.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2594 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 220a 0000  o.......i&.b"...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 220a 0000  o.......nKec"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6405 5a0b 6406 5a0c 6502 a00d 6501  ..d.Z.d.Z.e...e.
```

### Comparing `avocado-framework-98.0/selftests/functional/plugin/spawners/__pycache__/test_process.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/plugin/spawners/__pycache__/test_process.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 951 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 b703 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 b703 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 6d06 5a06 6d07 5a07 0100 6404  d.l.m.Z.m.Z...d.
 00000060: 5a08 4700 6405 6406 8400 6406 6507 8303  Z.G.d.d...d.e...
 00000070: 5a09 6401 5300 2907 e900 0000 004e 2902  Z.d.S.)......N).
```

### Comparing `avocado-framework-98.0/selftests/functional/plugin/spawners/test_podman.py` & `avocado-framework-99.0/selftests/functional/plugin/spawners/test_podman.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/plugin/spawners/test_process.py` & `avocado-framework-99.0/selftests/functional/plugin/spawners/test_process.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/plugin/test_assets.py` & `avocado-framework-99.0/selftests/functional/plugin/test_assets.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/plugin/test_bystatus.py` & `avocado-framework-99.0/selftests/functional/plugin/test_bystatus.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/plugin/test_diff.py` & `avocado-framework-99.0/selftests/functional/plugin/test_diff.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/plugin/test_jobscripts.py` & `avocado-framework-99.0/selftests/functional/plugin/test_jobscripts.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/plugin/test_jsonresult.py` & `avocado-framework-99.0/selftests/functional/plugin/test_jsonresult.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/plugin/test_logs.py` & `avocado-framework-99.0/selftests/functional/plugin/test_logs.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/plugin/test_vmimage.py` & `avocado-framework-99.0/selftests/functional/plugin/test_vmimage.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/serial/__pycache__/test_requirements.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/serial/__pycache__/test_requirements.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 5839 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 cf16 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 cf16 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 6d06 5a06 0100 6400 6404 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6406 5a0c 6407 5a0d 6408  m.Z...d.Z.d.Z.d.
```

### Comparing `avocado-framework-98.0/selftests/functional/serial/test_requirements.py` & `avocado-framework-99.0/selftests/functional/serial/test_requirements.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_argument_parsing.py` & `avocado-framework-99.0/selftests/functional/test_argument_parsing.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_basic.py` & `avocado-framework-99.0/selftests/functional/test_basic.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_coroutine.py` & `avocado-framework-99.0/selftests/functional/test_coroutine.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_export_variables.py` & `avocado-framework-99.0/selftests/functional/test_export_variables.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_fetch_asset.py` & `avocado-framework-99.0/selftests/functional/test_fetch_asset.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_getdata.py` & `avocado-framework-99.0/selftests/functional/test_getdata.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_interrupt.py` & `avocado-framework-99.0/selftests/functional/test_interrupt.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_job_api_features.py` & `avocado-framework-99.0/selftests/functional/test_job_api_features.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_job_timeout.py` & `avocado-framework-99.0/selftests/functional/test_job_timeout.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_journal.py` & `avocado-framework-99.0/selftests/functional/test_journal.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_json_variants.py` & `avocado-framework-99.0/selftests/functional/test_json_variants.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_list.py` & `avocado-framework-99.0/selftests/functional/test_list.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_lv_utils.py` & `avocado-framework-99.0/selftests/functional/test_lv_utils.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_nrunner.py` & `avocado-framework-99.0/selftests/functional/test_nrunner.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_nrunner_interface.py` & `avocado-framework-99.0/selftests/functional/test_nrunner_interface.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_nrunner_interface.py.data/capabilities.schema.json` & `avocado-framework-99.0/selftests/functional/test_nrunner_interface.py.data/capabilities.schema.json`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_output.py` & `avocado-framework-99.0/selftests/functional/test_output.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_output_check.py` & `avocado-framework-99.0/selftests/functional/test_output_check.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_replay.py` & `avocado-framework-99.0/selftests/functional/test_replay.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_requirements_cache.py` & `avocado-framework-99.0/selftests/functional/test_requirements_cache.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_resolver.py` & `avocado-framework-99.0/selftests/functional/test_resolver.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_runner_asset.py` & `avocado-framework-99.0/selftests/functional/test_runner_asset.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_runner_package.py` & `avocado-framework-99.0/selftests/functional/test_runner_package.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_skiptests.py` & `avocado-framework-99.0/selftests/functional/test_skiptests.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_software_manager.py` & `avocado-framework-99.0/selftests/functional/test_software_manager.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_statuses.py` & `avocado-framework-99.0/selftests/functional/test_statuses.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_streams.py` & `avocado-framework-99.0/selftests/functional/test_streams.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_sysinfo.py` & `avocado-framework-99.0/selftests/functional/test_sysinfo.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_task_statemachine.py` & `avocado-framework-99.0/selftests/functional/test_task_statemachine.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_task_timeout.py` & `avocado-framework-99.0/selftests/functional/test_task_timeout.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_teststmpdir.py` & `avocado-framework-99.0/selftests/functional/test_teststmpdir.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_thirdparty_bugs.py` & `avocado-framework-99.0/selftests/functional/test_thirdparty_bugs.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_unittest_compat.py` & `avocado-framework-99.0/selftests/functional/test_unittest_compat.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/test_utils.py` & `avocado-framework-99.0/selftests/functional/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,21 +196,21 @@
 
 class FileLockTest(TestCaseTmpDir):
     @skipOnLevelsInferiorThan(3)
     def test_filelock(self):
         """
         :avocado: tags=parallel:1
         """
-        # Calculate the timeout based on t_100_iter + 2e-5*players
+        # Calculate the timeout
         start = time.monotonic()
-        for _ in range(100):
+        for _ in range(50):
             with FileLock(self.tmpdir.name):
                 pass
         timeout = 0.02 + (time.monotonic() - start)
-        players = 1000
+        players = 500
         pool = multiprocessing.Pool(players)
         args = [(self.tmpdir.name, players, timeout)] * players
         try:
             pool.map(file_lock_action, args)
         except Exception:
             msg = "Failed to run FileLock with %s players:\n%s"
             msg %= (players, prepare_exc_info(sys.exc_info()))
```

### Comparing `avocado-framework-98.0/selftests/functional/utils/__pycache__/test_asset.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/utils/__pycache__/test_asset.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 7895 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 d71e 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 d71e 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 0100 6509  d.l.m.Z.m.Z...e.
 00000070: 8300 0100 4700 6405 6406 8400 6406 6508  ....G.d.d...d.e.
```

### Comparing `avocado-framework-98.0/selftests/functional/utils/__pycache__/test_podman.cpython-310.pyc` & `avocado-framework-99.0/selftests/functional/utils/__pycache__/test_podman.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1019 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 fb03 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 9004 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6501 8303 5a04 6405 5300 2906 e900 0000  e...Z.d.S.).....
 00000060: 0029 01da 0454 6573 7429 01da 0650 6f64  .)...Test)...Pod
 00000070: 6d61 6e63 0000 0000 0000 0000 0000 0000  manc............
@@ -10,68 +10,72 @@
 00000090: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
 000000a0: 0364 0364 0484 005a 0464 0553 0029 06da  .d.d...Z.d.S.)..
 000000b0: 0a50 6f64 6d61 6e54 6573 7463 0100 0000  .PodmanTestc....
 000000c0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
 000000d0: c300 0000 7328 0000 0081 0174 0083 007d  ....s(.....t...}
 000000e0: 017c 01a0 0164 01a1 0149 0064 0248 007d  .|...d...I.d.H.}
 000000f0: 027c 00a0 027c 0264 03a1 0201 0064 0253  .|...|.d.....d.S
-00000100: 0029 04fa 7b0a 2020 2020 2020 2020 3a61  .)..{.        :a
+00000100: 0029 04fa c50a 2020 2020 2020 2020 3a61  .)....        :a
 00000110: 766f 6361 646f 3a20 6465 7065 6e64 656e  vocado: dependen
 00000120: 6379 3d7b 2274 7970 6522 3a20 2270 6163  cy={"type": "pac
 00000130: 6b61 6765 222c 2022 6e61 6d65 223a 2022  kage", "name": "
 00000140: 706f 646d 616e 222c 2022 6163 7469 6f6e  podman", "action
 00000150: 223a 2022 6368 6563 6b22 7d0a 2020 2020  ": "check"}.    
-00000160: 2020 2020 3a61 766f 6361 646f 3a20 7461      :avocado: ta
-00000170: 6773 3d73 6c6f 770a 2020 2020 2020 2020  gs=slow.        
-00000180: fa09 6665 646f 7261 3a33 344e 2903 e903  ..fedora:34N)...
-00000190: 0000 00e9 0900 0000 7a10 2f75 7372 2f62  ........z./usr/b
-000001a0: 696e 2f70 7974 686f 6e33 2903 7203 0000  in/python3).r...
-000001b0: 00da 1267 6574 5f70 7974 686f 6e5f 7665  ...get_python_ve
-000001c0: 7273 696f 6eda 0b61 7373 6572 7445 7175  rsion..assertEqu
-000001d0: 616c 2903 da04 7365 6c66 da06 706f 646d  al)...self..podm
-000001e0: 616e da06 7265 7375 6c74 a900 720e 0000  an..result..r...
-000001f0: 00fa 4a2f 686f 6d65 2f63 6c65 6265 722f  ..J/home/cleber/
-00000200: 7372 632f 6176 6f63 6164 6f2f 6176 6f63  src/avocado/avoc
-00000210: 6164 6f2f 7365 6c66 7465 7374 732f 6675  ado/selftests/fu
-00000220: 6e63 7469 6f6e 616c 2f75 7469 6c73 2f74  nctional/utils/t
-00000230: 6573 745f 706f 646d 616e 2e70 79da 1374  est_podman.py..t
-00000240: 6573 745f 7079 7468 6f6e 5f76 6572 7369  est_python_versi
-00000250: 6f6e 0600 0000 7308 0000 0002 8006 0510  on....s.........
-00000260: 0110 017a 1e50 6f64 6d61 6e54 6573 742e  ...z.PodmanTest.
-00000270: 7465 7374 5f70 7974 686f 6e5f 7665 7273  test_python_vers
-00000280: 696f 6e63 0100 0000 0000 0000 0000 0000  ionc............
-00000290: 0600 0000 0500 0000 c300 0000 7380 0000  ............s...
-000002a0: 0081 0174 0083 007d 017c 01a0 0164 0164  ...t...}.|...d.d
-000002b0: 0264 03a1 0349 0064 0448 005c 037d 027d  .d...I.d.H.\.}.}
-000002c0: 037d 027c 03a0 02a1 00a0 03a1 007d 047c  .}.|.........}.|
-000002d0: 01a0 047c 04a1 0149 0064 0448 007d 057c  ...|...I.d.H.}.|
-000002e0: 00a0 057c 0564 0519 007c 04a1 0201 007c  ...|.d...|.....|
-000002f0: 01a0 0164 067c 04a1 0249 0064 0448 0001  ...d.|...I.d.H..
-00000300: 007c 01a0 047c 04a1 0149 0064 0448 007d  .|...|...I.d.H.}
-00000310: 057c 00a0 057c 0569 00a1 0201 0064 0453  .|...|.i.....d.S
-00000320: 0029 0772 0500 0000 da06 6372 6561 7465  .).r......create
-00000330: 7206 0000 007a 092f 6269 6e2f 6261 7368  r....z./bin/bash
-00000340: 4eda 0249 645a 0272 6d29 0672 0300 0000  N..IdZ.rm).r....
-00000350: da07 6578 6563 7574 65da 0664 6563 6f64  ..execute..decod
-00000360: 65da 0573 7472 6970 da12 6765 745f 636f  e..strip..get_co
-00000370: 6e74 6169 6e65 725f 696e 666f 720a 0000  ntainer_infor...
-00000380: 0029 0672 0b00 0000 720c 0000 00da 015f  .).r....r......_
-00000390: da06 7374 646f 7574 da0c 636f 6e74 6169  ..stdout..contai
-000003a0: 6e65 725f 6964 720d 0000 0072 0e00 0000  ner_idr....r....
-000003b0: 720e 0000 0072 0f00 0000 da13 7465 7374  r....r......test
-000003c0: 5f63 6f6e 7461 696e 6572 5f69 6e66 6f0f  _container_info.
-000003d0: 0000 0073 1200 0000 0280 0605 1a01 0c01  ...s............
-000003e0: 1001 1001 1202 1002 1001 7a1e 506f 646d  ..........z.Podm
-000003f0: 616e 5465 7374 2e74 6573 745f 636f 6e74  anTest.test_cont
-00000400: 6169 6e65 725f 696e 666f 4e29 05da 085f  ainer_infoN)..._
-00000410: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000420: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000430: 5f72 1000 0000 721a 0000 0072 0e00 0000  _r....r....r....
-00000440: 720e 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-00000450: 0400 0000 0500 0000 7306 0000 0008 0008  ........s.......
-00000460: 010c 0972 0400 0000 4e29 05da 0761 766f  ...r....N)...avo
-00000470: 6361 646f 7202 0000 00da 1461 766f 6361  cador......avoca
-00000480: 646f 2e75 7469 6c73 2e70 6f64 6d61 6e72  do.utils.podmanr
-00000490: 0300 0000 7204 0000 0072 0e00 0000 720e  ....r....r....r.
-000004a0: 0000 0072 0e00 0000 720f 0000 00da 083c  ...r....r......<
-000004b0: 6d6f 6475 6c65 3e01 0000 0073 0600 0000  module>....s....
-000004c0: 0c00 0c01 1403                           ......
+00000160: 2020 2020 3a61 766f 6361 646f 3a20 6465      :avocado: de
+00000170: 7065 6e64 656e 6379 3d7b 2274 7970 6522  pendency={"type"
+00000180: 3a20 2270 6f64 6d61 6e2d 696d 6167 6522  : "podman-image"
+00000190: 2c20 2275 7269 223a 2022 6665 646f 7261  , "uri": "fedora
+000001a0: 3a33 3622 7d0a 2020 2020 2020 2020 3a61  :36"}.        :a
+000001b0: 766f 6361 646f 3a20 7461 6773 3d73 6c6f  vocado: tags=slo
+000001c0: 770a 2020 2020 2020 2020 fa09 6665 646f  w.        ..fedo
+000001d0: 7261 3a33 364e 2903 e903 0000 00e9 0a00  ra:36N).........
+000001e0: 0000 7a10 2f75 7372 2f62 696e 2f70 7974  ..z./usr/bin/pyt
+000001f0: 686f 6e33 2903 7203 0000 00da 1267 6574  hon3).r......get
+00000200: 5f70 7974 686f 6e5f 7665 7273 696f 6eda  _python_version.
+00000210: 0b61 7373 6572 7445 7175 616c 2903 da04  .assertEqual)...
+00000220: 7365 6c66 da06 706f 646d 616e da06 7265  self..podman..re
+00000230: 7375 6c74 a900 720e 0000 00fa 4a2f 686f  sult..r.....J/ho
+00000240: 6d65 2f63 6c65 6265 722f 7372 632f 6176  me/cleber/src/av
+00000250: 6f63 6164 6f2f 6176 6f63 6164 6f2f 7365  ocado/avocado/se
+00000260: 6c66 7465 7374 732f 6675 6e63 7469 6f6e  lftests/function
+00000270: 616c 2f75 7469 6c73 2f74 6573 745f 706f  al/utils/test_po
+00000280: 646d 616e 2e70 79da 1374 6573 745f 7079  dman.py..test_py
+00000290: 7468 6f6e 5f76 6572 7369 6f6e 0600 0000  thon_version....
+000002a0: 7308 0000 0002 8006 0610 0110 017a 1e50  s............z.P
+000002b0: 6f64 6d61 6e54 6573 742e 7465 7374 5f70  odmanTest.test_p
+000002c0: 7974 686f 6e5f 7665 7273 696f 6e63 0100  ython_versionc..
+000002d0: 0000 0000 0000 0000 0000 0600 0000 0500  ................
+000002e0: 0000 c300 0000 7380 0000 0081 0174 0083  ......s......t..
+000002f0: 007d 017c 01a0 0164 0164 0264 03a1 0349  .}.|...d.d.d...I
+00000300: 0064 0448 005c 037d 027d 037d 027c 03a0  .d.H.\.}.}.}.|..
+00000310: 02a1 00a0 03a1 007d 047c 01a0 047c 04a1  .......}.|...|..
+00000320: 0149 0064 0448 007d 057c 00a0 057c 0564  .I.d.H.}.|...|.d
+00000330: 0519 007c 04a1 0201 007c 01a0 0164 067c  ...|.....|...d.|
+00000340: 04a1 0249 0064 0448 0001 007c 01a0 047c  ...I.d.H...|...|
+00000350: 04a1 0149 0064 0448 007d 057c 00a0 057c  ...I.d.H.}.|...|
+00000360: 0569 00a1 0201 0064 0453 0029 0772 0500  .i.....d.S.).r..
+00000370: 0000 da06 6372 6561 7465 7206 0000 007a  ....creater....z
+00000380: 092f 6269 6e2f 6261 7368 4eda 0249 645a  ./bin/bashN..IdZ
+00000390: 0272 6d29 0672 0300 0000 da07 6578 6563  .rm).r......exec
+000003a0: 7574 65da 0664 6563 6f64 65da 0573 7472  ute..decode..str
+000003b0: 6970 da12 6765 745f 636f 6e74 6169 6e65  ip..get_containe
+000003c0: 725f 696e 666f 720a 0000 0029 0672 0b00  r_infor....).r..
+000003d0: 0000 720c 0000 00da 015f da06 7374 646f  ..r......_..stdo
+000003e0: 7574 da0c 636f 6e74 6169 6e65 725f 6964  ut..container_id
+000003f0: 720d 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000400: 0f00 0000 da13 7465 7374 5f63 6f6e 7461  ......test_conta
+00000410: 696e 6572 5f69 6e66 6f10 0000 0073 1200  iner_info....s..
+00000420: 0000 0280 0606 1a01 0c01 1001 1001 1202  ................
+00000430: 1002 1001 7a1e 506f 646d 616e 5465 7374  ....z.PodmanTest
+00000440: 2e74 6573 745f 636f 6e74 6169 6e65 725f  .test_container_
+00000450: 696e 666f 4e29 05da 085f 5f6e 616d 655f  infoN)...__name_
+00000460: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000470: 5f71 7561 6c6e 616d 655f 5f72 1000 0000  _qualname__r....
+00000480: 721a 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000490: 0e00 0000 720f 0000 0072 0400 0000 0500  ....r....r......
+000004a0: 0000 7306 0000 0008 0008 010c 0a72 0400  ..s..........r..
+000004b0: 0000 4e29 05da 0761 766f 6361 646f 7202  ..N)...avocador.
+000004c0: 0000 00da 1461 766f 6361 646f 2e75 7469  .....avocado.uti
+000004d0: 6c73 2e70 6f64 6d61 6e72 0300 0000 7204  ls.podmanr....r.
+000004e0: 0000 0072 0e00 0000 720e 0000 0072 0e00  ...r....r....r..
+000004f0: 0000 720f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000500: 3e01 0000 0073 0600 0000 0c00 0c01 1403  >....s..........
```

### Comparing `avocado-framework-98.0/selftests/functional/utils/test_asset.py` & `avocado-framework-99.0/selftests/functional/utils/test_asset.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/functional/utils/test_podman.py` & `avocado-framework-99.0/selftests/functional/utils/test_podman.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 from avocado.utils.podman import Podman
 
 
 class PodmanTest(Test):
     async def test_python_version(self):
         """
         :avocado: dependency={"type": "package", "name": "podman", "action": "check"}
+        :avocado: dependency={"type": "podman-image", "uri": "fedora:36"}
         :avocado: tags=slow
         """
         podman = Podman()
-        result = await podman.get_python_version("fedora:34")
-        self.assertEqual(result, (3, 9, "/usr/bin/python3"))
+        result = await podman.get_python_version("fedora:36")
+        self.assertEqual(result, (3, 10, "/usr/bin/python3"))
 
     async def test_container_info(self):
         """
         :avocado: dependency={"type": "package", "name": "podman", "action": "check"}
+        :avocado: dependency={"type": "podman-image", "uri": "fedora:36"}
         :avocado: tags=slow
         """
         podman = Podman()
-        _, stdout, _ = await podman.execute("create", "fedora:34", "/bin/bash")
+        _, stdout, _ = await podman.execute("create", "fedora:36", "/bin/bash")
         container_id = stdout.decode().strip()
         result = await podman.get_container_info(container_id)
         self.assertEqual(result["Id"], container_id)
 
         await podman.execute("rm", container_id)
 
         result = await podman.get_container_info(container_id)
```

### Comparing `avocado-framework-98.0/selftests/jobs/example_unix_status_server` & `avocado-framework-99.0/selftests/jobs/example_unix_status_server`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/jobs/tests/__pycache__/passtest.cpython-310.pyc` & `avocado-framework-99.0/selftests/jobs/tests/__pycache__/passtest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  9 19:17:14 2022 UTC, .py size: 226 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3a47 a262 e200 0000  o.......:G.b....
+00000000: 6f0d 0d0a 0000 0000 863e f562 e200 0000  o........>.b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0454 6573 7463 0000  .....)...Testc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0200  ................
 00000070: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
```

### Comparing `avocado-framework-98.0/selftests/lint.sh` & `avocado-framework-99.0/selftests/lint.sh`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/modules-boundaries.sh` & `avocado-framework-99.0/selftests/modules-boundaries.sh`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/pre_release/jobs/pre_release.py` & `avocado-framework-99.0/selftests/pre_release/jobs/pre_release.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/pre_release/tests/check-copr-rpm-version.sh` & `avocado-framework-99.0/selftests/pre_release/tests/check-copr-rpm-version.sh`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/pre_release/tests/readthedocs.py` & `avocado-framework-99.0/selftests/pre_release/tests/readthedocs.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/pre_release/tests/vmimage.py` & `avocado-framework-99.0/selftests/pre_release/tests/vmimage.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/pre_release/tests/vmimage.py.data/variants.yml` & `avocado-framework-99.0/selftests/pre_release/tests/vmimage.py.data/variants.yml`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,26 @@
     !filter-out : /run/architectures/ppc64le
     !filter-out : /run/architectures/s390x
     version: !mux
       15.2:
         version: 15.2
       15.3:
         version: 15.3
+  freebsd:
+    name: freebsd
+    version: !mux
+      13.0:
+        version: '13.0'
+      12.2:
+        version: '12.2'
+    !filter-out : /run/architectures/arm
+    !filter-out : /run/architectures/ppc
+    !filter-out : /run/architectures/ppc64
+    !filter-out : /run/architectures/ppc64le
+    !filter-out : /run/architectures/s390x
 
 architectures: !mux
   arm:
     arch: arm
   aarch64:
     arch: aarch64
   i386:
```

### Comparing `avocado-framework-98.0/selftests/run_coverage` & `avocado-framework-99.0/selftests/run_coverage`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/safeloader.sh` & `avocado-framework-99.0/selftests/safeloader.sh`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_datadir.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_datadir.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 9281 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4124 0000  o.......i&.bA$..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4124 0000  o.......nKecA$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6404 6405 8400 6405 6503 6a08 8303 5a09  d.d...d.e.j...Z.
 00000070: 4700 6406 6407 8400 6407 6509 8303 5a0a  G.d.d...d.e...Z.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_dependencies_resolver.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_dependencies_resolver.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1037 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 0d04 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 0d04 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 6500 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6507 6406 6b02 7223 6500 a008 a100 0100  e.d.k.r#e.......
 00000070: 6401 5300 6401 5300 2907 e900 0000 004e  d.S.d.S.)......N
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_dispatcher.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_dispatcher.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1158 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 8604 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 8604 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 6500 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6507 6406 6b02 7223 6500 a008 a100 0100  e.d.k.r#e.......
 00000070: 6401 5300 6401 5300 2907 e900 0000 004e  d.S.d.S.)......N
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_hintfiles.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_hintfiles.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1844 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 3407 0000  o.......i&.b4...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 3407 0000  o.......nKec4...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6407  d.l.m.Z.m.Z...d.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_job.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_job.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 14519 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 b738 0000  o.......i&.b.8..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 b738 0000  o.......nKec.8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 6d07 5a07 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6403 6c08 6d09 5a09 6d0a 5a0a 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6404 6c0b 6d0c 5a0c 0100 6400 6405 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_loader.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_loader.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 10967 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 d72a 0000  o.......i&.b.*..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 d72a 0000  o.......nKec.*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 650a 8300 0100 6501 6a0c  m.Z...e.....e.j.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_nrunner.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_nrunner.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 17616 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 d044 0000  o.......i&.b.D..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 b04f 0000  o.......nKec.O..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
@@ -518,580 +518,713 @@
 00002050: 0072 4e00 0000 724f 0000 0072 6e00 0000  .rN...rO...rn...
 00002060: 727a 0000 0072 7b00 0000 727d 0000 0072  rz...r{...r}...r
 00002070: 8100 0000 7211 0000 0072 1100 0000 7211  ....r....r....r.
 00002080: 0000 0072 1200 0000 7265 0000 00ac 0000  ...r....re......
 00002090: 0073 0c00 0000 0800 0801 0804 0808 0809  .s..............
 000020a0: 0c0a 7265 0000 0063 0000 0000 0000 0000  ..re...c........
 000020b0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-000020c0: 7344 0000 0065 005a 0164 005a 0264 0164  sD...e.Z.d.Z.d.d
+000020c0: 735c 0000 0065 005a 0164 005a 0264 0164  s\...e.Z.d.Z.d.d
 000020d0: 0284 005a 0364 0364 0484 005a 0464 0564  ...Z.d.d...Z.d.d
 000020e0: 0684 005a 0565 0664 0783 0164 0864 0984  ...Z.e.d...d.d..
 000020f0: 0083 015a 0764 0a64 0b84 005a 0864 0c64  ...Z.d.d...Z.d.d
-00002100: 0d84 005a 0964 0e53 0029 0fda 0652 756e  ...Z.d.S.)...Run
-00002110: 6e65 7263 0100 0000 0000 0000 0000 0000  nerc............
-00002120: 0600 0000 0400 0000 4300 0000 7354 0000  ........C...sT..
-00002130: 0074 0064 0164 0083 027d 017c 01a0 01a1  .t.d.d...}.|....
-00002140: 007d 027c 0283 007d 0364 0264 0384 007c  .}.|...}.d.d...|
-00002150: 03a0 027c 01a1 0144 0083 017d 047c 0464  ...|...D...}.|.d
-00002160: 0419 007d 057c 00a0 037c 0564 0519 0064  ...}.|...|.d...d
-00002170: 06a1 0201 007c 00a0 0464 077c 05a1 0201  .....|...d.|....
-00002180: 0064 0053 0029 084e 7208 0000 0063 0100  .d.S.).Nr....c..
-00002190: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000021a0: 0000 5300 0000 f310 0000 0067 007c 005d  ..S........g.|.]
-000021b0: 047d 017c 0191 0271 0253 0072 1100 0000  .}.|...q.S.r....
-000021c0: 7211 0000 00a9 02da 022e 30da 0673 7461  r.........0..sta
-000021d0: 7475 7372 1100 0000 7211 0000 0072 1200  tusr....r....r..
-000021e0: 0000 da0a 3c6c 6973 7463 6f6d 703e d500  ....<listcomp>..
-000021f0: 0000 f302 0000 0010 007a 2b52 756e 6e65  .........z+Runne
-00002200: 722e 7465 7374 5f72 756e 6e65 725f 6e6f  r.test_runner_no
-00002210: 6f70 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  op.<locals>.<lis
-00002220: 7463 6f6d 703e e9ff ffff ff72 8700 0000  tcomp>.....r....
-00002230: da08 6669 6e69 7368 6564 da04 7469 6d65  ..finished..time
-00002240: a905 7202 0000 0072 4800 0000 da03 7275  ..r....rH.....ru
-00002250: 6e72 1900 0000 720c 0000 0029 0672 0f00  nr....r....).r..
-00002260: 0000 7210 0000 00da 0c72 756e 6e65 725f  ..r......runner_
-00002270: 6b6c 6173 73da 0672 756e 6e65 72da 0772  klass..runner..r
-00002280: 6573 756c 7473 da0b 6c61 7374 5f72 6573  esults..last_res
-00002290: 756c 7472 1100 0000 7211 0000 0072 1200  ultr....r....r..
-000022a0: 0000 da10 7465 7374 5f72 756e 6e65 725f  ....test_runner_
-000022b0: 6e6f 6f70 d100 0000 730e 0000 000a 0108  noop....s.......
-000022c0: 0106 0114 0108 0110 0110 017a 1752 756e  ...........z.Run
-000022d0: 6e65 722e 7465 7374 5f72 756e 6e65 725f  ner.test_runner_
-000022e0: 6e6f 6f70 6301 0000 0000 0000 0000 0000  noopc...........
-000022f0: 0008 0000 0005 0000 0043 0000 0073 ba00  .........C...s..
-00002300: 0000 7400 6401 7401 6a02 6402 6403 8304  ..t.d.t.j.d.d...
-00002310: 7d01 7c01 a003 a100 7d02 7c02 8300 7d03  }.|.....}.|...}.
-00002320: 6404 6405 8400 7c03 a004 7c01 a101 4400  d.d...|...|...D.
-00002330: 8301 7d04 7c04 6406 1900 7d05 7c04 6407  ..}.|.d...}.|.d.
-00002340: 1900 7d06 7c04 6408 1900 7d07 7c00 a005  ..}.|.d...}.|...
-00002350: 7c05 6409 1900 640a a102 0100 7c00 a005  |.d...d.....|...
-00002360: 7c05 640b 1900 640c a102 0100 7c00 a005  |.d...d.....|...
-00002370: 7c06 6409 1900 640d a102 0100 7c00 a005  |.d...d.....|...
-00002380: 7c06 640b 1900 640c a102 0100 7c00 a005  |.d...d.....|...
-00002390: 7c07 640e 1900 640f a102 0100 7c00 a005  |.d...d.....|...
-000023a0: 7c07 6410 1900 6411 a102 0100 7c00 a006  |.d...d.....|...
-000023b0: 6412 7c07 a102 0100 6400 5300 2913 4e72  d.|.....d.S.).Nr
-000023c0: 3700 0000 7258 0000 00fa 1d69 6d70 6f72  7...rX.....impor
-000023d0: 7420 7469 6d65 3b20 7469 6d65 2e73 6c65  t time; time.sle
-000023e0: 6570 2830 2e30 3129 6301 0000 0000 0000  ep(0.01)c.......
-000023f0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-00002400: 0072 8400 0000 7211 0000 0072 1100 0000  .r....r....r....
-00002410: 7285 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00002420: 1200 0000 7288 0000 00e0 0000 0072 8900  ....r........r..
-00002430: 0000 7a2b 5275 6e6e 6572 2e74 6573 745f  ..z+Runner.test_
-00002440: 7275 6e6e 6572 5f65 7865 632e 3c6c 6f63  runner_exec.<loc
-00002450: 616c 733e 2e3c 6c69 7374 636f 6d70 3ee9  als>.<listcomp>.
-00002460: fdff ffff e9fe ffff ff72 8a00 0000 da04  .........r......
-00002470: 7479 7065 da06 7374 646f 7574 da03 6c6f  type..stdout..lo
-00002480: 67f3 0000 0000 da06 7374 6465 7272 7287  g.......stderrr.
-00002490: 0000 0072 8b00 0000 da0a 7265 7475 726e  ...r......return
-000024a0: 636f 6465 7201 0000 0072 8c00 0000 a907  coder....r......
-000024b0: 7202 0000 00da 0373 7973 da0a 6578 6563  r......sys..exec
-000024c0: 7574 6162 6c65 7248 0000 0072 8e00 0000  utablerH...r....
-000024d0: 7219 0000 0072 0c00 0000 a908 720f 0000  r....r......r...
-000024e0: 0072 1000 0000 728f 0000 0072 9000 0000  .r....r....r....
-000024f0: 7291 0000 005a 0d73 7464 6f75 745f 7265  r....Z.stdout_re
-00002500: 7375 6c74 5a0d 7374 6465 7272 5f72 6573  sultZ.stderr_res
-00002510: 756c 7472 9200 0000 7211 0000 0072 1100  ultr....r....r..
-00002520: 0000 7212 0000 00da 1074 6573 745f 7275  ..r......test_ru
-00002530: 6e6e 6572 5f65 7865 63da 0000 0073 2000  nner_exec....s .
-00002540: 0000 0201 0a01 04ff 0803 0601 1401 0801  ................
-00002550: 0801 0801 1001 1001 1001 1001 1001 1001  ................
-00002560: 1001 7a17 5275 6e6e 6572 2e74 6573 745f  ..z.Runner.test_
-00002570: 7275 6e6e 6572 5f65 7865 6363 0100 0000  runner_execc....
-00002580: 0000 0000 0000 0000 0800 0000 0500 0000  ................
-00002590: 4300 0000 73ca 0000 0074 0064 0174 016a  C...s....t.d.t.j
-000025a0: 0264 0264 0383 047d 017c 01a0 03a1 007d  .d.d...}.|.....}
-000025b0: 027c 0283 007d 0364 0464 0584 007c 03a0  .|...}.d.d...|..
-000025c0: 047c 01a1 0144 0083 017d 047c 0464 0619  .|...D...}.|.d..
-000025d0: 007d 057c 0464 0719 007d 067c 0464 0819  .}.|.d...}.|.d..
-000025e0: 007d 077c 00a0 057c 0564 0919 0064 0aa1  .}.|...|.d...d..
-000025f0: 0201 007c 00a0 057c 0564 0b19 0064 0ca1  ...|...|.d...d..
-00002600: 0201 007c 00a0 057c 0664 0919 0064 0da1  ...|...|.d...d..
-00002610: 0201 007c 00a0 057c 0664 0b19 0064 0ca1  ...|...|.d...d..
-00002620: 0201 007c 00a0 057c 0764 0e19 0064 0fa1  ...|...|.d...d..
-00002630: 0201 007c 00a0 057c 0764 1019 0064 11a1  ...|...|.d...d..
-00002640: 0201 007c 00a0 057c 0764 1219 0064 13a1  ...|...|.d...d..
-00002650: 0201 007c 00a0 0664 147c 07a1 0201 0064  ...|...d.|.....d
-00002660: 0053 0029 154e 7237 0000 0072 5800 0000  .S.).Nr7...rX...
-00002670: 7294 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00002680: 0000 0200 0000 0300 0000 5300 0000 7284  ..........S...r.
-00002690: 0000 0072 1100 0000 7211 0000 0072 8500  ...r....r....r..
-000026a0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-000026b0: 0072 8800 0000 f200 0000 7289 0000 007a  .r........r....z
-000026c0: 3352 756e 6e65 722e 7465 7374 5f72 756e  3Runner.test_run
-000026d0: 6e65 725f 6578 6563 5f74 6573 745f 6f6b  ner_exec_test_ok
-000026e0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000026f0: 6f6d 703e 7295 0000 0072 9600 0000 728a  omp>r....r....r.
-00002700: 0000 0072 9700 0000 7298 0000 0072 9900  ...r....r....r..
-00002710: 0000 729a 0000 0072 9b00 0000 7287 0000  ..r....r....r...
-00002720: 0072 8b00 0000 da06 7265 7375 6c74 da04  .r......result..
-00002730: 7061 7373 729c 0000 0072 0100 0000 728c  passr....r....r.
-00002740: 0000 0072 9d00 0000 72a0 0000 0072 1100  ...r....r....r..
-00002750: 0000 7211 0000 0072 1200 0000 da18 7465  ..r....r......te
-00002760: 7374 5f72 756e 6e65 725f 6578 6563 5f74  st_runner_exec_t
-00002770: 6573 745f 6f6b ec00 0000 7322 0000 0002  est_ok....s"....
-00002780: 010a 0104 ff08 0306 0114 0108 0108 0108  ................
-00002790: 0110 0110 0110 0110 0110 0110 0110 0110  ................
-000027a0: 017a 1f52 756e 6e65 722e 7465 7374 5f72  .z.Runner.test_r
-000027b0: 756e 6e65 725f 6578 6563 5f74 6573 745f  unner_exec_test_
-000027c0: 6f6b fa0a 2f62 696e 2f66 616c 7365 6301  ok../bin/falsec.
-000027d0: 0000 0000 0000 0000 0000 0008 0000 0004  ................
-000027e0: 0000 0043 0000 0073 c400 0000 7400 6401  ...C...s....t.d.
-000027f0: 6402 8302 7d01 7c01 a001 a100 7d02 7c02  d...}.|.....}.|.
-00002800: 8300 7d03 6403 6404 8400 7c03 a002 7c01  ..}.d.d...|...|.
-00002810: a101 4400 8301 7d04 7c04 6405 1900 7d05  ..D...}.|.d...}.
-00002820: 7c04 6406 1900 7d06 7c04 6407 1900 7d07  |.d...}.|.d...}.
-00002830: 7c00 a003 7c05 6408 1900 6409 a102 0100  |...|.d...d.....
-00002840: 7c00 a003 7c05 640a 1900 640b a102 0100  |...|.d...d.....
-00002850: 7c00 a003 7c06 6408 1900 640c a102 0100  |...|.d...d.....
-00002860: 7c00 a003 7c06 640a 1900 640b a102 0100  |...|.d...d.....
-00002870: 7c00 a003 7c07 640d 1900 640e a102 0100  |...|.d...d.....
-00002880: 7c00 a003 7c07 640f 1900 6410 a102 0100  |...|.d...d.....
-00002890: 7c00 a003 7c07 6411 1900 6412 a102 0100  |...|.d...d.....
-000028a0: 7c00 a004 6413 7c07 a102 0100 6400 5300  |...d.|.....d.S.
-000028b0: 2914 4e72 3700 0000 72a5 0000 0063 0100  ).Nr7...r....c..
-000028c0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000028d0: 0000 5300 0000 7284 0000 0072 1100 0000  ..S...r....r....
-000028e0: 7211 0000 0072 8500 0000 7211 0000 0072  r....r....r....r
-000028f0: 1100 0000 7212 0000 0072 8800 0000 0401  ....r....r......
-00002900: 0000 7289 0000 007a 3552 756e 6e65 722e  ..r....z5Runner.
-00002910: 7465 7374 5f72 756e 6e65 725f 6578 6563  test_runner_exec
-00002920: 5f74 6573 745f 6661 696c 2e3c 6c6f 6361  _test_fail.<loca
-00002930: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7295  ls>.<listcomp>r.
-00002940: 0000 0072 9600 0000 728a 0000 0072 9700  ...r....r....r..
-00002950: 0000 7298 0000 0072 9900 0000 729a 0000  ..r....r....r...
-00002960: 0072 9b00 0000 7287 0000 0072 8b00 0000  .r....r....r....
-00002970: 72a2 0000 00da 0466 6169 6c72 9c00 0000  r......failr....
-00002980: e901 0000 0072 8c00 0000 728d 0000 0072  .....r....r....r
-00002990: a000 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-000029a0: 0000 00da 1a74 6573 745f 7275 6e6e 6572  .....test_runner
-000029b0: 5f65 7865 635f 7465 7374 5f66 6169 6cff  _exec_test_fail.
-000029c0: 0000 0073 1e00 0000 0a02 0801 0601 1401  ...s............
-000029d0: 0801 0801 0801 1001 1001 1001 1001 1001  ................
-000029e0: 1001 1001 1001 7a21 5275 6e6e 6572 2e74  ......z!Runner.t
-000029f0: 6573 745f 7275 6e6e 6572 5f65 7865 635f  est_runner_exec_
-00002a00: 7465 7374 5f66 6169 6c63 0100 0000 0000  test_failc......
-00002a10: 0000 0000 0000 0700 0000 0400 0000 4300  ..............C.
-00002a20: 0000 736c 0000 0074 0064 0164 0283 027d  ..sl...t.d.d...}
-00002a30: 017c 01a0 01a1 007d 027c 0283 007d 0364  .|.....}.|...}.d
-00002a40: 0364 0484 007c 03a0 027c 01a1 0144 0083  .d...|...|...D..
-00002a50: 017d 0464 057d 057c 0464 0619 007d 067c  .}.d.}.|.d...}.|
-00002a60: 00a0 037c 0664 0719 0064 08a1 0201 007c  ...|.d...d.....|
-00002a70: 00a0 037c 0664 0919 0064 02a1 0201 007c  ...|.d...d.....|
-00002a80: 00a0 037c 0664 0a19 007c 05a1 0201 0064  ...|.d...|.....d
-00002a90: 0053 0029 0b4e fa0f 7079 7468 6f6e 2d75  .S.).N..python-u
-00002aa0: 6e69 7474 6573 74da 0565 7272 6f72 6301  nittest..errorc.
-00002ab0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00002ac0: 0000 0053 0000 0072 8400 0000 7211 0000  ...S...r....r...
-00002ad0: 0072 1100 0000 7285 0000 0072 1100 0000  .r....r....r....
-00002ae0: 7211 0000 0072 1200 0000 7288 0000 0015  r....r....r.....
-00002af0: 0100 0072 8900 0000 7a3c 5275 6e6e 6572  ...r....z<Runner
-00002b00: 2e74 6573 745f 7275 6e6e 6572 5f70 7974  .test_runner_pyt
-00002b10: 686f 6e5f 756e 6974 7465 7374 5f65 7272  hon_unittest_err
-00002b20: 6f72 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  or.<locals>.<lis
-00002b30: 7463 6f6d 703e fa3f 496e 7661 6c69 6420  tcomp>.?Invalid 
-00002b40: 5552 493a 2063 6f75 6c64 206e 6f74 2062  URI: could not b
-00002b50: 6520 636f 6e76 6572 7465 6420 746f 2061  e converted to a
-00002b60: 6e20 756e 6974 7465 7374 2064 6f74 7465  n unittest dotte
-00002b70: 6420 6e61 6d65 2e72 8a00 0000 7287 0000  d name.r....r...
-00002b80: 0072 8b00 0000 72a2 0000 00da 066f 7574  .r....r......out
-00002b90: 7075 74a9 0472 0200 0000 7248 0000 0072  put..r....rH...r
-00002ba0: 8e00 0000 7219 0000 00a9 0772 0f00 0000  ....r......r....
-00002bb0: 7210 0000 0072 8f00 0000 7290 0000 0072  r....r....r....r
-00002bc0: 9100 0000 72ac 0000 0072 a200 0000 7211  ....r....r....r.
-00002bd0: 0000 0072 1100 0000 7212 0000 00da 2174  ...r....r.....!t
-00002be0: 6573 745f 7275 6e6e 6572 5f70 7974 686f  est_runner_pytho
-00002bf0: 6e5f 756e 6974 7465 7374 5f65 7272 6f72  n_unittest_error
-00002c00: 1101 0000 f312 0000 000a 0108 0106 0114  ................
-00002c10: 0104 0108 0110 0110 0114 017a 2852 756e  ...........z(Run
-00002c20: 6e65 722e 7465 7374 5f72 756e 6e65 725f  ner.test_runner_
-00002c30: 7079 7468 6f6e 5f75 6e69 7474 6573 745f  python_unittest_
-00002c40: 6572 726f 7263 0100 0000 0000 0000 0000  errorc..........
-00002c50: 0000 0700 0000 0400 0000 4300 0000 736c  ..........C...sl
-00002c60: 0000 0074 0064 0164 0283 027d 017c 01a0  ...t.d.d...}.|..
-00002c70: 01a1 007d 027c 0283 007d 0364 0364 0484  ...}.|...}.d.d..
-00002c80: 007c 03a0 027c 01a1 0144 0083 017d 0464  .|...|...D...}.d
-00002c90: 057d 057c 0464 0619 007d 067c 00a0 037c  .}.|.d...}.|...|
-00002ca0: 0664 0719 0064 08a1 0201 007c 00a0 037c  .d...d.....|...|
-00002cb0: 0664 0919 0064 0aa1 0201 007c 00a0 037c  .d...d.....|...|
-00002cc0: 0664 0b19 007c 05a1 0201 0064 0053 0029  .d...|.....d.S.)
-00002cd0: 0c4e 72a9 0000 0072 4700 0000 6301 0000  .Nr....rG...c...
-00002ce0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00002cf0: 0053 0000 0072 8400 0000 7211 0000 0072  .S...r....r....r
-00002d00: 1100 0000 7285 0000 0072 1100 0000 7211  ....r....r....r.
-00002d10: 0000 0072 1200 0000 7288 0000 0020 0100  ...r....r.... ..
-00002d20: 0072 8900 0000 7a46 5275 6e6e 6572 2e74  .r....zFRunner.t
-00002d30: 6573 745f 7275 6e6e 6572 5f70 7974 686f  est_runner_pytho
-00002d40: 6e5f 756e 6974 7465 7374 5f65 6d70 7479  n_unittest_empty
-00002d50: 5f75 7269 5f65 7272 6f72 2e3c 6c6f 6361  _uri_error.<loca
-00002d60: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 72ab  ls>.<listcomp>r.
-00002d70: 0000 0072 8a00 0000 7287 0000 0072 8b00  ...r....r....r..
-00002d80: 0000 72a2 0000 0072 aa00 0000 72ac 0000  ..r....r....r...
-00002d90: 0072 ad00 0000 72ae 0000 0072 1100 0000  .r....r....r....
-00002da0: 7211 0000 0072 1200 0000 da2b 7465 7374  r....r.....+test
-00002db0: 5f72 756e 6e65 725f 7079 7468 6f6e 5f75  _runner_python_u
-00002dc0: 6e69 7474 6573 745f 656d 7074 795f 7572  nittest_empty_ur
-00002dd0: 695f 6572 726f 721c 0100 0072 b000 0000  i_error....r....
-00002de0: 7a32 5275 6e6e 6572 2e74 6573 745f 7275  z2Runner.test_ru
-00002df0: 6e6e 6572 5f70 7974 686f 6e5f 756e 6974  nner_python_unit
-00002e00: 7465 7374 5f65 6d70 7479 5f75 7269 5f65  test_empty_uri_e
-00002e10: 7272 6f72 4e29 0a72 4d00 0000 724e 0000  rrorN).rM...rN..
-00002e20: 0072 4f00 0000 7293 0000 0072 a100 0000  .rO...r....r....
-00002e30: 72a4 0000 0072 0500 0000 72a8 0000 0072  r....r....r....r
-00002e40: af00 0000 72b1 0000 0072 1100 0000 7211  ....r....r....r.
-00002e50: 0000 0072 1100 0000 7212 0000 0072 8300  ...r....r....r..
-00002e60: 0000 d000 0000 7310 0000 0008 0008 0108  ......s.........
-00002e70: 0908 1206 130a 0108 110c 0b72 8300 0000  ...........r....
-00002e80: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002e90: 0003 0000 0040 0000 0073 6c00 0000 6500  .....@...sl...e.
-00002ea0: 5a01 6400 5a02 6401 6402 8400 5a03 6504  Z.d.Z.d.d...Z.e.
-00002eb0: 6403 8301 6404 6405 8400 8301 5a05 6504  d...d.d.....Z.e.
-00002ec0: 6403 8301 6406 6407 8400 8301 5a06 6504  d...d.d.....Z.e.
-00002ed0: 6403 8301 6408 6409 8400 8301 5a07 6504  d...d.d.....Z.e.
-00002ee0: 6403 8301 640a 640b 8400 8301 5a08 6504  d...d.d.....Z.e.
-00002ef0: 6403 8301 640c 640d 8400 8301 5a09 640e  d...d.d.....Z.d.
-00002f00: 640f 8400 5a0a 6410 5300 2911 da09 5275  d...Z.d.S.)...Ru
-00002f10: 6e6e 6572 546d 7063 0100 0000 0000 0000  nnerTmpc........
-00002f20: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00002f30: 7266 0000 0072 6700 0000 7269 0000 0072  rf...rg...ri...r
-00002f40: 6d00 0000 7211 0000 0072 1100 0000 7212  m...r....r....r.
-00002f50: 0000 0072 6e00 0000 2901 0000 726f 0000  ...rn...)...ro..
-00002f60: 007a 0f52 756e 6e65 7254 6d70 2e73 6574  .z.RunnerTmp.set
-00002f70: 5570 7238 0000 0063 0100 0000 0000 0000  Upr8...c........
-00002f80: 0000 0000 0800 0000 0800 0000 4300 0000  ............C...
-00002f90: f3b2 0000 0064 017d 0174 006a 01a0 027c  .....d.}.t.j...|
-00002fa0: 006a 036a 0464 02a1 027d 0274 057c 0264  .j.j.d...}.t.|.d
-00002fb0: 0364 0464 058d 038f 0d7d 037c 03a0 067c  .d.d.....}.|...|
-00002fc0: 01a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-00002fd0: 006e 0831 0073 2277 0101 0001 0001 0059  .n.1.s"w.......Y
-00002fe0: 0001 0074 0764 0664 077c 0283 037d 0474  ...t.d.d.|...}.t
-00002ff0: 08a0 09a1 007d 0564 0864 0984 007c 05a0  .....}.d.d...|..
-00003000: 0a7c 04a1 0144 0083 017d 067c 0664 0a19  .|...D...}.|.d..
-00003010: 007d 077c 00a0 0b7c 0764 0b19 0064 0ca1  .}.|...|.d...d..
-00003020: 0201 007c 00a0 0b7c 0764 0d19 0064 0ea1  ...|...|.d...d..
-00003030: 0201 007c 00a0 0b7c 0764 0f19 0064 10a1  ...|...|.d...d..
-00003040: 0201 0064 0053 0029 114e 7a71 2321 2f62  ...d.S.).Nzq#!/b
-00003050: 696e 2f73 680a 6563 686f 2027 312e 2e32  in/sh.echo '1..2
-00003060: 270a 6563 686f 2027 2320 4465 6669 6e69  '.echo '# Defini
-00003070: 6e67 2061 6e20 6261 7369 6320 7465 7374  ng an basic test
-00003080: 270a 6563 686f 2027 6f6b 2031 202d 2064  '.echo 'ok 1 - d
-00003090: 6573 6372 6970 7469 6f6e 2031 270a 6563  escription 1'.ec
-000030a0: 686f 2027 6e6f 7420 6f6b 2032 202d 2064  ho 'not ok 2 - d
-000030b0: 6573 6372 6970 7469 6f6e 2032 27fa 0674  escription 2'..t
-000030c0: 6170 2e73 68da 0177 fa05 7574 662d 38a9  ap.sh..w..utf-8.
-000030d0: 01da 0865 6e63 6f64 696e 6772 0400 0000  ...encodingr....
-000030e0: 7238 0000 0063 0100 0000 0000 0000 0000  r8...c..........
-000030f0: 0000 0200 0000 0300 0000 5300 0000 7284  ..........S...r.
-00003100: 0000 0072 1100 0000 7211 0000 0072 8500  ...r....r....r..
-00003110: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00003120: 0072 8800 0000 3b01 0000 7289 0000 007a  .r....;...r....z
-00003130: 3252 756e 6e65 7254 6d70 2e74 6573 745f  2RunnerTmp.test_
-00003140: 7275 6e6e 6572 5f74 6170 5f66 6169 6c2e  runner_tap_fail.
-00003150: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00003160: 6d70 3e72 8a00 0000 7287 0000 0072 8b00  mp>r....r....r..
-00003170: 0000 72a2 0000 0072 a600 0000 729c 0000  ..r....r....r...
-00003180: 0072 0100 0000 a90c 7271 0000 0072 7200  .r......rq...rr.
-00003190: 0000 7273 0000 0072 6c00 0000 7274 0000  ..rs...rl...rt..
-000031a0: 00da 046f 7065 6eda 0577 7269 7465 7202  ...open..writer.
-000031b0: 0000 00da 0a72 756e 6e65 725f 7461 705a  .....runner_tapZ
-000031c0: 0954 4150 5275 6e6e 6572 728e 0000 0072  .TAPRunnerr....r
-000031d0: 1900 0000 a908 720f 0000 005a 0a74 6170  ......r....Z.tap
-000031e0: 5f73 6372 6970 745a 0874 6170 5f70 6174  _scriptZ.tap_pat
-000031f0: 68da 0266 7072 1000 0000 7290 0000 0072  h..fpr....r....r
-00003200: 9100 0000 7292 0000 0072 1100 0000 7211  ....r....r....r.
-00003210: 0000 0072 1200 0000 da14 7465 7374 5f72  ...r......test_r
-00003220: 756e 6e65 725f 7461 705f 6661 696c 2d01  unner_tap_fail-.
-00003230: 0000 f318 0000 0004 0212 0510 020c 011c  ................
-00003240: ff0c 0308 0114 0108 0110 0110 0114 017a  ...............z
-00003250: 1e52 756e 6e65 7254 6d70 2e74 6573 745f  .RunnerTmp.test_
-00003260: 7275 6e6e 6572 5f74 6170 5f66 6169 6c63  runner_tap_failc
-00003270: 0100 0000 0000 0000 0000 0000 0800 0000  ................
-00003280: 0800 0000 4300 0000 72b3 0000 0029 114e  ....C...r....).N
-00003290: 7a6d 2321 2f62 696e 2f73 680a 6563 686f  zm#!/bin/sh.echo
-000032a0: 2027 312e 2e32 270a 6563 686f 2027 2320   '1..2'.echo '# 
-000032b0: 4465 6669 6e69 6e67 2061 6e20 6261 7369  Defining an basi
-000032c0: 6320 7465 7374 270a 6563 686f 2027 6f6b  c test'.echo 'ok
-000032d0: 2031 202d 2064 6573 6372 6970 7469 6f6e   1 - description
-000032e0: 2031 270a 6563 686f 2027 6f6b 2032 202d   1'.echo 'ok 2 -
-000032f0: 2064 6573 6372 6970 7469 6f6e 2032 2772   description 2'r
-00003300: b400 0000 72b5 0000 0072 b600 0000 72b7  ....r....r....r.
-00003310: 0000 0072 0400 0000 7238 0000 0063 0100  ...r....r8...c..
-00003320: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00003330: 0000 5300 0000 7284 0000 0072 1100 0000  ..S...r....r....
-00003340: 7211 0000 0072 8500 0000 7211 0000 0072  r....r....r....r
-00003350: 1100 0000 7212 0000 0072 8800 0000 4f01  ....r....r....O.
-00003360: 0000 7289 0000 007a 3052 756e 6e65 7254  ..r....z0RunnerT
-00003370: 6d70 2e74 6573 745f 7275 6e6e 6572 5f74  mp.test_runner_t
-00003380: 6170 5f6f 6b2e 3c6c 6f63 616c 733e 2e3c  ap_ok.<locals>.<
-00003390: 6c69 7374 636f 6d70 3e72 8a00 0000 7287  listcomp>r....r.
-000033a0: 0000 0072 8b00 0000 72a2 0000 0072 a300  ...r....r....r..
-000033b0: 0000 729c 0000 0072 0100 0000 72b9 0000  ..r....r....r...
-000033c0: 0072 bd00 0000 7211 0000 0072 1100 0000  .r....r....r....
-000033d0: 7212 0000 00da 1274 6573 745f 7275 6e6e  r......test_runn
-000033e0: 6572 5f74 6170 5f6f 6b41 0100 0072 c000  er_tap_okA...r..
-000033f0: 0000 7a1c 5275 6e6e 6572 546d 702e 7465  ..z.RunnerTmp.te
-00003400: 7374 5f72 756e 6e65 725f 7461 705f 6f6b  st_runner_tap_ok
-00003410: 6301 0000 0000 0000 0000 0000 0008 0000  c...............
-00003420: 0008 0000 0043 0000 0072 b300 0000 2911  .....C...r....).
-00003430: 4e7a 7423 212f 6269 6e2f 7368 0a65 6368  Nzt#!/bin/sh.ech
-00003440: 6f20 2731 2e2e 3227 0a65 6368 6f20 2723  o '1..2'.echo '#
-00003450: 2044 6566 696e 696e 6720 616e 2062 6173   Defining an bas
-00003460: 6963 2074 6573 7427 0a65 6368 6f20 276f  ic test'.echo 'o
-00003470: 6b20 3120 2d20 2320 534b 4950 2064 6573  k 1 - # SKIP des
-00003480: 6372 6970 7469 6f6e 2031 270a 6563 686f  cription 1'.echo
-00003490: 2027 6f6b 2032 202d 2064 6573 6372 6970   'ok 2 - descrip
-000034a0: 7469 6f6e 2032 2772 b400 0000 72b5 0000  tion 2'r....r...
-000034b0: 0072 b600 0000 72b7 0000 0072 0400 0000  .r....r....r....
-000034c0: 7238 0000 0063 0100 0000 0000 0000 0000  r8...c..........
-000034d0: 0000 0200 0000 0300 0000 5300 0000 7284  ..........S...r.
-000034e0: 0000 0072 1100 0000 7211 0000 0072 8500  ...r....r....r..
-000034f0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00003500: 0072 8800 0000 6301 0000 7289 0000 007a  .r....c...r....z
-00003510: 3252 756e 6e65 7254 6d70 2e74 6573 745f  2RunnerTmp.test_
-00003520: 7275 6e6e 6572 5f74 6170 5f73 6b69 702e  runner_tap_skip.
-00003530: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00003540: 6d70 3e72 8a00 0000 7287 0000 0072 8b00  mp>r....r....r..
-00003550: 0000 72a2 0000 00da 0473 6b69 7072 9c00  ..r......skipr..
-00003560: 0000 7201 0000 0072 b900 0000 72bd 0000  ..r....r....r...
-00003570: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
-00003580: da14 7465 7374 5f72 756e 6e65 725f 7461  ..test_runner_ta
-00003590: 705f 736b 6970 5501 0000 72c0 0000 007a  p_skipU...r....z
-000035a0: 1e52 756e 6e65 7254 6d70 2e74 6573 745f  .RunnerTmp.test_
-000035b0: 7275 6e6e 6572 5f74 6170 5f73 6b69 7063  runner_tap_skipc
-000035c0: 0100 0000 0000 0000 0000 0000 0800 0000  ................
-000035d0: 0800 0000 4300 0000 72b3 0000 0029 114e  ....C...r....).N
-000035e0: 7a72 2321 2f62 696e 2f73 680a 6563 686f  zr#!/bin/sh.echo
-000035f0: 2027 312e 2e32 270a 6563 686f 2027 2320   '1..2'.echo '# 
-00003600: 4465 6669 6e69 6e67 2061 6e20 6261 7369  Defining an basi
-00003610: 6320 7465 7374 270a 6563 686f 2027 4261  c test'.echo 'Ba
-00003620: 696c 206f 7574 2120 2d20 6465 7363 7269  il out! - descri
-00003630: 7074 696f 6e20 3127 0a65 6368 6f20 276f  ption 1'.echo 'o
-00003640: 6b20 3220 2d20 6465 7363 7269 7074 696f  k 2 - descriptio
-00003650: 6e20 3227 72b4 0000 0072 b500 0000 72b6  n 2'r....r....r.
-00003660: 0000 0072 b700 0000 7204 0000 0072 3800  ...r....r....r8.
-00003670: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00003680: 0000 0003 0000 0053 0000 0072 8400 0000  .......S...r....
-00003690: 7211 0000 0072 1100 0000 7285 0000 0072  r....r....r....r
-000036a0: 1100 0000 7211 0000 0072 1200 0000 7288  ....r....r....r.
-000036b0: 0000 0077 0100 0072 8900 0000 7a35 5275  ...w...r....z5Ru
-000036c0: 6e6e 6572 546d 702e 7465 7374 5f72 756e  nnerTmp.test_run
-000036d0: 6e65 725f 7461 705f 6261 696c 6f75 742e  ner_tap_bailout.
-000036e0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000036f0: 6d70 3e72 8a00 0000 7287 0000 0072 8b00  mp>r....r....r..
-00003700: 0000 72a2 0000 0072 aa00 0000 729c 0000  ..r....r....r...
-00003710: 0072 0100 0000 72b9 0000 0072 bd00 0000  .r....r....r....
-00003720: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00003730: 1774 6573 745f 7275 6e6e 6572 5f74 6170  .test_runner_tap
-00003740: 5f62 6169 6c6f 7574 6901 0000 72c0 0000  _bailouti...r...
-00003750: 007a 2152 756e 6e65 7254 6d70 2e74 6573  .z!RunnerTmp.tes
-00003760: 745f 7275 6e6e 6572 5f74 6170 5f62 6169  t_runner_tap_bai
-00003770: 6c6f 7574 6301 0000 0000 0000 0000 0000  loutc...........
-00003780: 0008 0000 0008 0000 0043 0000 0072 b300  .........C...r..
-00003790: 0000 2911 4e7a 6e23 212f 6269 6e2f 7368  ..).Nzn#!/bin/sh
-000037a0: 0a65 6368 6f20 2731 2e2e 3227 0a65 6368  .echo '1..2'.ech
-000037b0: 6f20 2723 2044 6566 696e 696e 6720 616e  o '# Defining an
-000037c0: 2062 6173 6963 2074 6573 7427 0a65 6368   basic test'.ech
-000037d0: 6f20 2765 7272 6f72 202d 2064 6573 6372  o 'error - descr
-000037e0: 6970 7469 6f6e 2031 270a 6563 686f 2027  iption 1'.echo '
-000037f0: 6f6b 2032 202d 2064 6573 6372 6970 7469  ok 2 - descripti
-00003800: 6f6e 2032 2772 b400 0000 72b5 0000 0072  on 2'r....r....r
-00003810: b600 0000 72b7 0000 0072 0400 0000 7238  ....r....r....r8
-00003820: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00003830: 0200 0000 0300 0000 5300 0000 7284 0000  ........S...r...
-00003840: 0072 1100 0000 7211 0000 0072 8500 0000  .r....r....r....
-00003850: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00003860: 8800 0000 8b01 0000 7289 0000 007a 3352  ........r....z3R
-00003870: 756e 6e65 7254 6d70 2e74 6573 745f 7275  unnerTmp.test_ru
-00003880: 6e6e 6572 5f74 6170 5f65 7272 6f72 2e3c  nner_tap_error.<
-00003890: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-000038a0: 703e 728a 0000 0072 8700 0000 728b 0000  p>r....r....r...
-000038b0: 0072 a200 0000 72aa 0000 0072 9c00 0000  .r....r....r....
-000038c0: 7201 0000 0072 b900 0000 72bd 0000 0072  r....r....r....r
-000038d0: 1100 0000 7211 0000 0072 1200 0000 da15  ....r....r......
-000038e0: 7465 7374 5f72 756e 6e65 725f 7461 705f  test_runner_tap_
-000038f0: 6572 726f 727d 0100 0072 c000 0000 7a1f  error}...r....z.
-00003900: 5275 6e6e 6572 546d 702e 7465 7374 5f72  RunnerTmp.test_r
-00003910: 756e 6e65 725f 7461 705f 6572 726f 7263  unner_tap_errorc
-00003920: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00003930: 0200 0000 4300 0000 727e 0000 0072 2600  ....C...r~...r&.
-00003940: 0000 727f 0000 0072 2900 0000 7211 0000  ..r....r)...r...
-00003950: 0072 1100 0000 7212 0000 0072 8100 0000  .r....r....r....
-00003960: 9101 0000 7282 0000 007a 1252 756e 6e65  ....r....z.Runne
-00003970: 7254 6d70 2e74 6561 7244 6f77 6e4e 290b  rTmp.tearDownN).
-00003980: 724d 0000 0072 4e00 0000 724f 0000 0072  rM...rN...rO...r
-00003990: 6e00 0000 7205 0000 0072 bf00 0000 72c1  n...r....r....r.
-000039a0: 0000 0072 c300 0000 72c4 0000 0072 c500  ...r....r....r..
-000039b0: 0000 7281 0000 0072 1100 0000 7211 0000  ..r....r....r...
-000039c0: 0072 1100 0000 7212 0000 0072 b200 0000  .r....r....r....
-000039d0: 2801 0000 731a 0000 0008 0008 0106 040a  (...s...........
-000039e0: 0106 130a 0106 130a 0106 130a 0106 130a  ................
-000039f0: 010c 1372 b200 0000 7238 0000 0063 0000  ...r....r8...c..
-00003a00: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00003a10: 0000 4000 0000 732c 0000 0065 005a 0164  ..@...s,...e.Z.d
-00003a20: 005a 0264 0164 0284 005a 0364 0364 0484  .Z.d.d...Z.d.d..
-00003a30: 005a 0464 0564 0684 005a 0564 0764 0884  .Z.d.d...Z.d.d..
-00003a40: 005a 0664 0953 0029 0ada 1652 756e 6e65  .Z.d.S.)...Runne
-00003a50: 7243 6f6d 6d61 6e64 5365 6c65 6374 696f  rCommandSelectio
-00003a60: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
-00003a70: 0000 0200 0000 4300 0000 f30a 0000 0064  ......C........d
-00003a80: 017c 005f 0064 0053 0029 024e 5a06 6d79  .|._.d.S.).NZ.my
-00003a90: 6b69 6e64 a901 722b 0000 0072 2900 0000  kind..r+...r)...
-00003aa0: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00003ab0: 6e00 0000 9701 0000 f302 0000 000a 017a  n..............z
-00003ac0: 1c52 756e 6e65 7243 6f6d 6d61 6e64 5365  .RunnerCommandSe
-00003ad0: 6c65 6374 696f 6e2e 7365 7455 7063 0100  lection.setUpc..
-00003ae0: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-00003af0: 0000 4300 0000 f320 0000 0067 0064 01a2  ..C.... ...g.d..
-00003b00: 017d 017c 00a0 0074 01a0 027c 006a 037c  .}.|...t...|.j.|
-00003b10: 01a1 02a1 0101 0064 0053 0029 024e 2903  .......d.S.).N).
-00003b20: da02 7368 7258 0000 007a 3f74 6573 7420  ..shrX...z?test 
-00003b30: 2430 203d 2063 6170 6162 696c 6974 6965  $0 = capabilitie
-00003b40: 7320 2626 2065 6368 6f20 2d6e 207b 5c22  s && echo -n {\"
-00003b50: 7275 6e6e 6162 6c65 735c 223a 205b 5c22  runnables\": [\"
-00003b60: 6d79 6b69 6e64 5c22 5d7d 2904 7276 0000  mykind\"]}).rv..
-00003b70: 0072 0200 0000 da23 6973 5f6b 696e 645f  .r.....#is_kind_
-00003b80: 7375 7070 6f72 7465 645f 6279 5f72 756e  supported_by_run
-00003b90: 6e65 725f 636f 6d6d 616e 6472 2b00 0000  ner_commandr+...
-00003ba0: a902 720f 0000 00da 0363 6d64 7211 0000  ..r......cmdr...
-00003bb0: 0072 1100 0000 7212 0000 00da 1b74 6573  .r....r......tes
-00003bc0: 745f 6973 5f74 6173 6b5f 6b69 6e64 5f73  t_is_task_kind_s
-00003bd0: 7570 706f 7274 6564 9a01 0000 f304 0000  upported........
-00003be0: 0008 0118 057a 3252 756e 6e65 7243 6f6d  .....z2RunnerCom
-00003bf0: 6d61 6e64 5365 6c65 6374 696f 6e2e 7465  mandSelection.te
-00003c00: 7374 5f69 735f 7461 736b 5f6b 696e 645f  st_is_task_kind_
-00003c10: 7375 7070 6f72 7465 6463 0100 0000 0000  supportedc......
-00003c20: 0000 0000 0000 0200 0000 0600 0000 4300  ..............C.
-00003c30: 0000 72ca 0000 0029 024e 2903 72cb 0000  ..r....).N).r...
-00003c40: 0072 5800 0000 7a42 7465 7374 2024 3020  .rX...zBtest $0 
-00003c50: 3d20 6361 7061 6269 6c69 7469 6573 2026  = capabilities &
-00003c60: 2620 6563 686f 202d 6e20 7b5c 2272 756e  & echo -n {\"run
-00003c70: 6e61 626c 6573 5c22 3a20 5b5c 226f 7468  nables\": [\"oth
-00003c80: 6572 6b69 6e64 5c22 5d7d a904 da0b 6173  erkind\"]}....as
-00003c90: 7365 7274 4661 6c73 6572 0200 0000 72cc  sertFalser....r.
-00003ca0: 0000 0072 2b00 0000 72cd 0000 0072 1100  ...r+...r....r..
-00003cb0: 0000 7211 0000 0072 1200 0000 da26 7465  ..r....r.....&te
-00003cc0: 7374 5f69 735f 7461 736b 5f6b 696e 645f  st_is_task_kind_
-00003cd0: 7375 7070 6f72 7465 645f 6f74 6865 725f  supported_other_
-00003ce0: 6b69 6e64 a201 0000 72d0 0000 007a 3d52  kind....r....z=R
-00003cf0: 756e 6e65 7243 6f6d 6d61 6e64 5365 6c65  unnerCommandSele
-00003d00: 6374 696f 6e2e 7465 7374 5f69 735f 7461  ction.test_is_ta
-00003d10: 736b 5f6b 696e 645f 7375 7070 6f72 7465  sk_kind_supporte
-00003d20: 645f 6f74 6865 725f 6b69 6e64 6301 0000  d_other_kindc...
-00003d30: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00003d40: 0043 0000 0072 ca00 0000 2902 4e29 0372  .C...r....).N).r
-00003d50: cb00 0000 7258 0000 007a 0a65 6368 6f20  ....rX...z.echo 
-00003d60: 2d6e 2022 2272 d100 0000 72cd 0000 0072  -n ""r....r....r
-00003d70: 1100 0000 7211 0000 0072 1200 0000 da25  ....r....r.....%
-00003d80: 7465 7374 5f69 735f 7461 736b 5f6b 696e  test_is_task_kin
-00003d90: 645f 7375 7070 6f72 7465 645f 6e6f 5f6f  d_supported_no_o
-00003da0: 7574 7075 74aa 0100 0073 0400 0000 0801  utput....s......
-00003db0: 1801 7a3c 5275 6e6e 6572 436f 6d6d 616e  ..z<RunnerComman
-00003dc0: 6453 656c 6563 7469 6f6e 2e74 6573 745f  dSelection.test_
-00003dd0: 6973 5f74 6173 6b5f 6b69 6e64 5f73 7570  is_task_kind_sup
-00003de0: 706f 7274 6564 5f6e 6f5f 6f75 7470 7574  ported_no_output
-00003df0: 4e29 0772 4d00 0000 724e 0000 0072 4f00  N).rM...rN...rO.
-00003e00: 0000 726e 0000 0072 cf00 0000 72d3 0000  ..rn...r....r...
-00003e10: 0072 d400 0000 7211 0000 0072 1100 0000  .r....r....r....
-00003e20: 7211 0000 0072 1200 0000 72c6 0000 0095  r....r....r.....
-00003e30: 0100 0073 0a00 0000 0800 0802 0803 0808  ...s............
-00003e40: 0c08 72c6 0000 0063 0000 0000 0000 0000  ..r....c........
-00003e50: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-00003e60: 7324 0000 0065 005a 0164 005a 0264 0164  s$...e.Z.d.Z.d.d
-00003e70: 0284 005a 0364 0364 0484 005a 0464 0564  ...Z.d.d...Z.d.d
-00003e80: 0684 005a 0564 0753 0029 08da 0a50 6963  ...Z.d.S.)...Pic
-00003e90: 6b52 756e 6e65 7263 0100 0000 0000 0000  kRunnerc........
-00003ea0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00003eb0: 72c7 0000 0029 024e fa11 6c65 7473 2d69  r....).N..lets-i
-00003ec0: 6d61 6765 2d61 2d6b 696e 6472 c800 0000  mage-a-kindr....
-00003ed0: 7229 0000 0072 1100 0000 7211 0000 0072  r)...r....r....r
-00003ee0: 1200 0000 726e 0000 00b0 0100 0072 c900  ....rn.......r..
-00003ef0: 0000 7a10 5069 636b 5275 6e6e 6572 2e73  ..z.PickRunner.s
-00003f00: 6574 5570 6301 0000 0000 0000 0000 0000  etUpc...........
-00003f10: 0003 0000 0006 0000 0043 0000 0073 2800  .........C...s(.
-00003f20: 0000 6401 6701 7d01 6402 7c01 6901 7d02  ..d.g.}.d.|.i.}.
-00003f30: 7c00 a000 7401 a002 7c00 6a03 7c02 a102  |...t...|.j.|...
-00003f40: 7c01 a102 0100 6400 5300 2903 4e7a 2061  |.....d.S.).Nz a
-00003f50: 766f 6361 646f 2d72 756e 6e65 722d 6c65  vocado-runner-le
-00003f60: 7473 2d69 6d61 6765 2d61 2d6b 696e 6472  ts-image-a-kindr
-00003f70: d600 0000 2904 7219 0000 0072 0200 0000  ....).r....r....
-00003f80: da13 7069 636b 5f72 756e 6e65 725f 636f  ..pick_runner_co
-00003f90: 6d6d 616e 6472 2b00 0000 2903 720f 0000  mmandr+...).r...
-00003fa0: 0072 9000 0000 5a05 6b6e 6f77 6e72 1100  .r....Z.knownr..
-00003fb0: 0000 7211 0000 0072 1200 0000 da18 7465  ..r....r......te
-00003fc0: 7374 5f70 6963 6b5f 7275 6e6e 6572 5f63  st_pick_runner_c
-00003fd0: 6f6d 6d61 6e64 b301 0000 7306 0000 0006  ommand....s.....
-00003fe0: 0108 011a 017a 2350 6963 6b52 756e 6e65  .....z#PickRunne
-00003ff0: 722e 7465 7374 5f70 6963 6b5f 7275 6e6e  r.test_pick_runn
-00004000: 6572 5f63 6f6d 6d61 6e64 6301 0000 0000  er_commandc.....
-00004010: 0000 0000 0000 0001 0000 0006 0000 0043  ...............C
-00004020: 0000 0073 1800 0000 7c00 a000 7401 a002  ...s....|...t...
-00004030: 7c00 6a03 6900 a102 a101 0100 6400 5300  |.j.i.......d.S.
-00004040: 7226 0000 0029 0472 d200 0000 7202 0000  r&...).r....r...
-00004050: 0072 d700 0000 722b 0000 0072 2900 0000  .r....r+...r)...
-00004060: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00004070: 1e74 6573 745f 7069 636b 5f72 756e 6e65  .test_pick_runne
-00004080: 725f 636f 6d6d 616e 645f 656d 7074 79b8  r_command_empty.
-00004090: 0100 0073 0200 0000 1801 7a29 5069 636b  ...s......z)Pick
-000040a0: 5275 6e6e 6572 2e74 6573 745f 7069 636b  Runner.test_pick
-000040b0: 5f72 756e 6e65 725f 636f 6d6d 616e 645f  _runner_command_
-000040c0: 656d 7074 794e 2906 724d 0000 0072 4e00  emptyN).rM...rN.
-000040d0: 0000 724f 0000 0072 6e00 0000 72d8 0000  ..rO...rn...r...
-000040e0: 0072 d900 0000 7211 0000 0072 1100 0000  .r....r....r....
-000040f0: 7211 0000 0072 1200 0000 72d5 0000 00af  r....r....r.....
-00004100: 0100 0073 0800 0000 0800 0801 0803 0c05  ...s............
-00004110: 72d5 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00004120: 0000 0000 0000 0200 0000 4000 0000 731c  ..........@...s.
-00004130: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
-00004140: 005a 0364 0364 0484 005a 0464 0553 0029  .Z.d.d...Z.d.S.)
-00004150: 06da 0854 6173 6b54 6573 7463 0100 0000  ...TaskTestc....
-00004160: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00004170: 4300 0000 7326 0000 0074 0064 0164 0283  C...s&...t.d.d..
-00004180: 027d 0174 017c 0164 0383 027d 027c 00a0  .}.t.|.d...}.|..
-00004190: 027c 026a 0364 04a1 0201 0064 0053 0029  .|.j.d.....d.S.)
-000041a0: 054e 7208 0000 00da 086e 6f6f 705f 7572  .Nr......noop_ur
-000041b0: 69da 0774 6173 6b5f 6964 da04 7465 7374  i..task_id..test
-000041c0: a904 7202 0000 0072 0300 0000 7219 0000  ..r....r....r...
-000041d0: 00da 0863 6174 6567 6f72 79a9 0372 0f00  ...category..r..
-000041e0: 0000 7210 0000 00da 0474 6173 6b72 1100  ..r......taskr..
-000041f0: 0000 7211 0000 0072 1200 0000 da15 7465  ..r....r......te
-00004200: 7374 5f64 6566 6175 6c74 5f63 6174 6567  st_default_categ
-00004210: 6f72 79bd 0100 0073 0600 0000 0a01 0a01  ory....s........
-00004220: 1201 7a1e 5461 736b 5465 7374 2e74 6573  ..z.TaskTest.tes
-00004230: 745f 6465 6661 756c 745f 6361 7465 676f  t_default_catego
-00004240: 7279 6301 0000 0000 0000 0000 0000 0003  ryc.............
-00004250: 0000 0005 0000 0043 0000 0073 2a00 0000  .......C...s*...
-00004260: 7400 6401 6402 8302 7d01 7401 7c01 6403  t.d.d...}.t.|.d.
-00004270: 6404 6405 8d03 7d02 7c00 a002 7c02 6a03  d.d...}.|...|.j.
-00004280: 6404 a102 0100 6400 5300 2906 4e72 0800  d.....d.S.).Nr..
-00004290: 0000 72db 0000 0072 dc00 0000 5a0c 6e65  ..r....r....Z.ne
-000042a0: 775f 6361 7465 676f 7279 2901 72df 0000  w_category).r...
-000042b0: 0072 de00 0000 72e0 0000 0072 1100 0000  .r....r....r....
-000042c0: 7211 0000 0072 1200 0000 da11 7465 7374  r....r......test
-000042d0: 5f73 6574 5f63 6174 6567 6f72 79c2 0100  _set_category...
-000042e0: 0073 0600 0000 0a01 0e01 1201 7a1a 5461  .s..........z.Ta
-000042f0: 736b 5465 7374 2e74 6573 745f 7365 745f  skTest.test_set_
-00004300: 6361 7465 676f 7279 4e29 0572 4d00 0000  categoryN).rM...
-00004310: 724e 0000 0072 4f00 0000 72e2 0000 0072  rN...rO...r....r
-00004320: e300 0000 7211 0000 0072 1100 0000 7211  ....r....r....r.
-00004330: 0000 0072 1200 0000 72da 0000 00bc 0100  ...r....r.......
-00004340: 0073 0600 0000 0800 0801 0c05 72da 0000  .s..........r...
-00004350: 00da 085f 5f6d 6169 6e5f 5f29 1a72 7100  ...__main__).rq.
-00004360: 0000 729e 0000 0072 6a00 0000 5a0d 756e  ..r....rj...Z.un
-00004370: 6974 7465 7374 2e6d 6f63 6b72 3000 0000  ittest.mockr0...
-00004380: da1d 6176 6f63 6164 6f2e 636f 7265 2e6e  ..avocado.core.n
-00004390: 7275 6e6e 6572 2e72 756e 6e61 626c 6572  runner.runnabler
-000043a0: 0200 0000 da19 6176 6f63 6164 6f2e 636f  ......avocado.co
-000043b0: 7265 2e6e 7275 6e6e 6572 2e74 6173 6b72  re.nrunner.taskr
-000043c0: 0300 0000 5a17 6176 6f63 6164 6f2e 706c  ....Z.avocado.pl
-000043d0: 7567 696e 732e 7275 6e6e 6572 7372 0400  ugins.runnersr..
-000043e0: 0000 72bc 0000 005a 0f73 656c 6674 6573  ..r....Z.selftes
-000043f0: 7473 2e75 7469 6c73 7205 0000 0072 0600  ts.utilsr....r..
-00004400: 0000 da08 5465 7374 4361 7365 7207 0000  ....TestCaser...
-00004410: 0072 5100 0000 7265 0000 0072 8300 0000  .rQ...re...r....
-00004420: 72b2 0000 0072 c600 0000 72d5 0000 0072  r....r....r....r
-00004430: da00 0000 724d 0000 00da 046d 6169 6e72  ....rM.....mainr
-00004440: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00004450: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00004460: 0073 2800 0000 0800 0801 0801 0801 0c02  .s(.............
-00004470: 0c01 0c01 1001 1203 1268 1238 1224 1258  .........h.8.$.X
-00004480: 066d 1401 1219 120d 080c 0c01 04ff       .m............
+00002100: 0d84 005a 0964 0e64 0f84 005a 0a64 1064  ...Z.d.d...Z.d.d
+00002110: 1184 005a 0b64 1264 1384 005a 0c64 1453  ...Z.d.d...Z.d.S
+00002120: 0029 15da 0652 756e 6e65 7263 0100 0000  .)...Runnerc....
+00002130: 0000 0000 0000 0000 0600 0000 0400 0000  ................
+00002140: 4300 0000 7354 0000 0074 0064 0164 0083  C...sT...t.d.d..
+00002150: 027d 017c 01a0 01a1 007d 027c 0283 007d  .}.|.....}.|...}
+00002160: 0364 0264 0384 007c 03a0 027c 01a1 0144  .d.d...|...|...D
+00002170: 0083 017d 047c 0464 0419 007d 057c 00a0  ...}.|.d...}.|..
+00002180: 037c 0564 0519 0064 06a1 0201 007c 00a0  .|.d...d.....|..
+00002190: 0464 077c 05a1 0201 0064 0053 0029 084e  .d.|.....d.S.).N
+000021a0: 7208 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000021b0: 0000 0200 0000 0300 0000 5300 0000 f310  ..........S.....
+000021c0: 0000 0067 007c 005d 047d 017c 0191 0271  ...g.|.].}.|...q
+000021d0: 0253 0072 1100 0000 7211 0000 00a9 02da  .S.r....r.......
+000021e0: 022e 30da 0673 7461 7475 7372 1100 0000  ..0..statusr....
+000021f0: 7211 0000 0072 1200 0000 da0a 3c6c 6973  r....r......<lis
+00002200: 7463 6f6d 703e d500 0000 f302 0000 0010  tcomp>..........
+00002210: 007a 2b52 756e 6e65 722e 7465 7374 5f72  .z+Runner.test_r
+00002220: 756e 6e65 725f 6e6f 6f70 2e3c 6c6f 6361  unner_noop.<loca
+00002230: 6c73 3e2e 3c6c 6973 7463 6f6d 703e e9ff  ls>.<listcomp>..
+00002240: ffff ff72 8700 0000 da08 6669 6e69 7368  ...r......finish
+00002250: 6564 da04 7469 6d65 a905 7202 0000 0072  ed..time..r....r
+00002260: 4800 0000 da03 7275 6e72 1900 0000 720c  H.....runr....r.
+00002270: 0000 0029 0672 0f00 0000 7210 0000 00da  ...).r....r.....
+00002280: 0c72 756e 6e65 725f 6b6c 6173 73da 0672  .runner_klass..r
+00002290: 756e 6e65 72da 0772 6573 756c 7473 da0b  unner..results..
+000022a0: 6c61 7374 5f72 6573 756c 7472 1100 0000  last_resultr....
+000022b0: 7211 0000 0072 1200 0000 da10 7465 7374  r....r......test
+000022c0: 5f72 756e 6e65 725f 6e6f 6f70 d100 0000  _runner_noop....
+000022d0: 730e 0000 000a 0108 0106 0114 0108 0110  s...............
+000022e0: 0110 017a 1752 756e 6e65 722e 7465 7374  ...z.Runner.test
+000022f0: 5f72 756e 6e65 725f 6e6f 6f70 6301 0000  _runner_noopc...
+00002300: 0000 0000 0000 0000 0008 0000 0005 0000  ................
+00002310: 0043 0000 0073 ba00 0000 7400 6401 7401  .C...s....t.d.t.
+00002320: 6a02 6402 6403 8304 7d01 7c01 a003 a100  j.d.d...}.|.....
+00002330: 7d02 7c02 8300 7d03 6404 6405 8400 7c03  }.|...}.d.d...|.
+00002340: a004 7c01 a101 4400 8301 7d04 7c04 6406  ..|...D...}.|.d.
+00002350: 1900 7d05 7c04 6407 1900 7d06 7c04 6408  ..}.|.d...}.|.d.
+00002360: 1900 7d07 7c00 a005 7c05 6409 1900 640a  ..}.|...|.d...d.
+00002370: a102 0100 7c00 a005 7c05 640b 1900 640c  ....|...|.d...d.
+00002380: a102 0100 7c00 a005 7c06 6409 1900 640d  ....|...|.d...d.
+00002390: a102 0100 7c00 a005 7c06 640b 1900 640c  ....|...|.d...d.
+000023a0: a102 0100 7c00 a005 7c07 640e 1900 640f  ....|...|.d...d.
+000023b0: a102 0100 7c00 a005 7c07 6410 1900 6411  ....|...|.d...d.
+000023c0: a102 0100 7c00 a006 6412 7c07 a102 0100  ....|...d.|.....
+000023d0: 6400 5300 2913 4e72 3700 0000 7258 0000  d.S.).Nr7...rX..
+000023e0: 00fa 1d69 6d70 6f72 7420 7469 6d65 3b20  ...import time; 
+000023f0: 7469 6d65 2e73 6c65 6570 2830 2e30 3129  time.sleep(0.01)
+00002400: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00002410: 0003 0000 0053 0000 0072 8400 0000 7211  .....S...r....r.
+00002420: 0000 0072 1100 0000 7285 0000 0072 1100  ...r....r....r..
+00002430: 0000 7211 0000 0072 1200 0000 7288 0000  ..r....r....r...
+00002440: 00e0 0000 0072 8900 0000 7a2b 5275 6e6e  .....r....z+Runn
+00002450: 6572 2e74 6573 745f 7275 6e6e 6572 5f65  er.test_runner_e
+00002460: 7865 632e 3c6c 6f63 616c 733e 2e3c 6c69  xec.<locals>.<li
+00002470: 7374 636f 6d70 3ee9 fdff ffff e9fe ffff  stcomp>.........
+00002480: ff72 8a00 0000 da04 7479 7065 da06 7374  .r......type..st
+00002490: 646f 7574 da03 6c6f 67f3 0000 0000 da06  dout..log.......
+000024a0: 7374 6465 7272 7287 0000 0072 8b00 0000  stderrr....r....
+000024b0: da0a 7265 7475 726e 636f 6465 7201 0000  ..returncoder...
+000024c0: 0072 8c00 0000 a907 7202 0000 00da 0373  .r......r......s
+000024d0: 7973 da0a 6578 6563 7574 6162 6c65 7248  ys..executablerH
+000024e0: 0000 0072 8e00 0000 7219 0000 0072 0c00  ...r....r....r..
+000024f0: 0000 a908 720f 0000 0072 1000 0000 728f  ....r....r....r.
+00002500: 0000 0072 9000 0000 7291 0000 005a 0d73  ...r....r....Z.s
+00002510: 7464 6f75 745f 7265 7375 6c74 5a0d 7374  tdout_resultZ.st
+00002520: 6465 7272 5f72 6573 756c 7472 9200 0000  derr_resultr....
+00002530: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00002540: 1074 6573 745f 7275 6e6e 6572 5f65 7865  .test_runner_exe
+00002550: 63da 0000 0073 2000 0000 0201 0a01 04ff  c....s .........
+00002560: 0803 0601 1401 0801 0801 0801 1001 1001  ................
+00002570: 1001 1001 1001 1001 1001 7a17 5275 6e6e  ..........z.Runn
+00002580: 6572 2e74 6573 745f 7275 6e6e 6572 5f65  er.test_runner_e
+00002590: 7865 6363 0100 0000 0000 0000 0000 0000  xecc............
+000025a0: 0800 0000 0500 0000 4300 0000 73ca 0000  ........C...s...
+000025b0: 0074 0064 0174 016a 0264 0264 0383 047d  .t.d.t.j.d.d...}
+000025c0: 017c 01a0 03a1 007d 027c 0283 007d 0364  .|.....}.|...}.d
+000025d0: 0464 0584 007c 03a0 047c 01a1 0144 0083  .d...|...|...D..
+000025e0: 017d 047c 0464 0619 007d 057c 0464 0719  .}.|.d...}.|.d..
+000025f0: 007d 067c 0464 0819 007d 077c 00a0 057c  .}.|.d...}.|...|
+00002600: 0564 0919 0064 0aa1 0201 007c 00a0 057c  .d...d.....|...|
+00002610: 0564 0b19 0064 0ca1 0201 007c 00a0 057c  .d...d.....|...|
+00002620: 0664 0919 0064 0da1 0201 007c 00a0 057c  .d...d.....|...|
+00002630: 0664 0b19 0064 0ca1 0201 007c 00a0 057c  .d...d.....|...|
+00002640: 0764 0e19 0064 0fa1 0201 007c 00a0 057c  .d...d.....|...|
+00002650: 0764 1019 0064 11a1 0201 007c 00a0 057c  .d...d.....|...|
+00002660: 0764 1219 0064 13a1 0201 007c 00a0 0664  .d...d.....|...d
+00002670: 147c 07a1 0201 0064 0053 0029 154e 7237  .|.....d.S.).Nr7
+00002680: 0000 0072 5800 0000 7294 0000 0063 0100  ...rX...r....c..
+00002690: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000026a0: 0000 5300 0000 7284 0000 0072 1100 0000  ..S...r....r....
+000026b0: 7211 0000 0072 8500 0000 7211 0000 0072  r....r....r....r
+000026c0: 1100 0000 7212 0000 0072 8800 0000 f200  ....r....r......
+000026d0: 0000 7289 0000 007a 3352 756e 6e65 722e  ..r....z3Runner.
+000026e0: 7465 7374 5f72 756e 6e65 725f 6578 6563  test_runner_exec
+000026f0: 5f74 6573 745f 6f6b 2e3c 6c6f 6361 6c73  _test_ok.<locals
+00002700: 3e2e 3c6c 6973 7463 6f6d 703e 7295 0000  >.<listcomp>r...
+00002710: 0072 9600 0000 728a 0000 0072 9700 0000  .r....r....r....
+00002720: 7298 0000 0072 9900 0000 729a 0000 0072  r....r....r....r
+00002730: 9b00 0000 7287 0000 0072 8b00 0000 da06  ....r....r......
+00002740: 7265 7375 6c74 da04 7061 7373 729c 0000  result..passr...
+00002750: 0072 0100 0000 728c 0000 0072 9d00 0000  .r....r....r....
+00002760: 72a0 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00002770: 1200 0000 da18 7465 7374 5f72 756e 6e65  ......test_runne
+00002780: 725f 6578 6563 5f74 6573 745f 6f6b ec00  r_exec_test_ok..
+00002790: 0000 7322 0000 0002 010a 0104 ff08 0306  ..s"............
+000027a0: 0114 0108 0108 0108 0110 0110 0110 0110  ................
+000027b0: 0110 0110 0110 0110 017a 1f52 756e 6e65  .........z.Runne
+000027c0: 722e 7465 7374 5f72 756e 6e65 725f 6578  r.test_runner_ex
+000027d0: 6563 5f74 6573 745f 6f6b fa0a 2f62 696e  ec_test_ok../bin
+000027e0: 2f66 616c 7365 6301 0000 0000 0000 0000  /falsec.........
+000027f0: 0000 0008 0000 0004 0000 0043 0000 0073  ...........C...s
+00002800: c400 0000 7400 6401 6402 8302 7d01 7c01  ....t.d.d...}.|.
+00002810: a001 a100 7d02 7c02 8300 7d03 6403 6404  ....}.|...}.d.d.
+00002820: 8400 7c03 a002 7c01 a101 4400 8301 7d04  ..|...|...D...}.
+00002830: 7c04 6405 1900 7d05 7c04 6406 1900 7d06  |.d...}.|.d...}.
+00002840: 7c04 6407 1900 7d07 7c00 a003 7c05 6408  |.d...}.|...|.d.
+00002850: 1900 6409 a102 0100 7c00 a003 7c05 640a  ..d.....|...|.d.
+00002860: 1900 640b a102 0100 7c00 a003 7c06 6408  ..d.....|...|.d.
+00002870: 1900 640c a102 0100 7c00 a003 7c06 640a  ..d.....|...|.d.
+00002880: 1900 640b a102 0100 7c00 a003 7c07 640d  ..d.....|...|.d.
+00002890: 1900 640e a102 0100 7c00 a003 7c07 640f  ..d.....|...|.d.
+000028a0: 1900 6410 a102 0100 7c00 a003 7c07 6411  ..d.....|...|.d.
+000028b0: 1900 6412 a102 0100 7c00 a004 6413 7c07  ..d.....|...d.|.
+000028c0: a102 0100 6400 5300 2914 4e72 3700 0000  ....d.S.).Nr7...
+000028d0: 72a5 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000028e0: 0000 0200 0000 0300 0000 5300 0000 7284  ..........S...r.
+000028f0: 0000 0072 1100 0000 7211 0000 0072 8500  ...r....r....r..
+00002900: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00002910: 0072 8800 0000 0401 0000 7289 0000 007a  .r........r....z
+00002920: 3552 756e 6e65 722e 7465 7374 5f72 756e  5Runner.test_run
+00002930: 6e65 725f 6578 6563 5f74 6573 745f 6661  ner_exec_test_fa
+00002940: 696c 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  il.<locals>.<lis
+00002950: 7463 6f6d 703e 7295 0000 0072 9600 0000  tcomp>r....r....
+00002960: 728a 0000 0072 9700 0000 7298 0000 0072  r....r....r....r
+00002970: 9900 0000 729a 0000 0072 9b00 0000 7287  ....r....r....r.
+00002980: 0000 0072 8b00 0000 72a2 0000 00da 0466  ...r....r......f
+00002990: 6169 6c72 9c00 0000 e901 0000 0072 8c00  ailr.........r..
+000029a0: 0000 728d 0000 0072 a000 0000 7211 0000  ..r....r....r...
+000029b0: 0072 1100 0000 7212 0000 00da 1a74 6573  .r....r......tes
+000029c0: 745f 7275 6e6e 6572 5f65 7865 635f 7465  t_runner_exec_te
+000029d0: 7374 5f66 6169 6cff 0000 0073 1e00 0000  st_fail....s....
+000029e0: 0a02 0801 0601 1401 0801 0801 0801 1001  ................
+000029f0: 1001 1001 1001 1001 1001 1001 1001 7a21  ..............z!
+00002a00: 5275 6e6e 6572 2e74 6573 745f 7275 6e6e  Runner.test_runn
+00002a10: 6572 5f65 7865 635f 7465 7374 5f66 6169  er_exec_test_fai
+00002a20: 6c63 0100 0000 0000 0000 0000 0000 0900  lc..............
+00002a30: 0000 0500 0000 4300 0000 f394 0000 0074  ......C........t
+00002a40: 0064 0164 0283 027d 017c 01a0 01a1 007d  .d.d...}.|.....}
+00002a50: 027c 0283 007d 0364 0364 0484 007c 03a0  .|...}.d.d...|..
+00002a60: 027c 01a1 0144 0083 017d 0464 057d 0564  .|...D...}.d.}.d
+00002a70: 067d 067c 0464 0719 007d 077c 0464 0819  .}.|.d...}.|.d..
+00002a80: 007d 087c 00a0 037c 0864 0919 0064 0aa1  .}.|...|.d...d..
+00002a90: 0201 007c 00a0 037c 0864 0b19 0064 0ca1  ...|...|.d...d..
+00002aa0: 0201 007c 00a0 047c 0764 0d19 00a0 057c  ...|...|.d.....|
+00002ab0: 05a1 0164 0ea1 0201 007c 00a0 047c 0764  ...d.....|...|.d
+00002ac0: 0d19 00a0 067c 06a1 0164 0fa1 0201 0064  .....|...d.....d
+00002ad0: 0053 0029 104e fa0f 7079 7468 6f6e 2d75  .S.).N..python-u
+00002ae0: 6e69 7474 6573 747a 2c73 656c 6674 6573  nittestz,selftes
+00002af0: 7473 2f2e 6461 7461 2f75 6e69 7474 6573  ts/.data/unittes
+00002b00: 7473 2e70 793a 4669 7273 742e 7465 7374  ts.py:First.test
+00002b10: 5f70 6173 7363 0100 0000 0000 0000 0000  _passc..........
+00002b20: 0000 0200 0000 0300 0000 5300 0000 7284  ..........S...r.
+00002b30: 0000 0072 1100 0000 7211 0000 0072 8500  ...r....r....r..
+00002b40: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00002b50: 0072 8800 0000 1701 0000 7289 0000 007a  .r........r....z
+00002b60: 3952 756e 6e65 722e 7465 7374 5f72 756e  9Runner.test_run
+00002b70: 6e65 725f 7079 7468 6f6e 5f75 6e69 7474  ner_python_unitt
+00002b80: 6573 745f 6f6b 2e3c 6c6f 6361 6c73 3e2e  est_ok.<locals>.
+00002b90: 3c6c 6973 7463 6f6d 703e f355 0000 002d  <listcomp>.U...-
+00002ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002be0: 2d2d 2d2d 2d0a 5261 6e20 3120 7465 7374  -----.Ran 1 test
+00002bf0: 2069 6e20 7306 0000 0073 0a0a 4f4b 0a72   in s....s..OK.r
+00002c00: 9600 0000 728a 0000 0072 8700 0000 728b  ....r....r....r.
+00002c10: 0000 0072 a200 0000 72a3 0000 0072 9900  ...r....r....r..
+00002c20: 0000 fa17 5374 6172 7420 6f66 206f 7574  ....Start of out
+00002c30: 7075 7420 6469 6666 6572 73fa 1545 6e64  put differs..End
+00002c40: 206f 6620 6f75 7470 7574 2064 6966 6665   of output diffe
+00002c50: 7273 a907 7202 0000 0072 4800 0000 728e  rs..r....rH...r.
+00002c60: 0000 0072 1900 0000 7276 0000 00da 0a73  ...r....rv.....s
+00002c70: 7461 7274 7377 6974 68da 0865 6e64 7377  tartswith..endsw
+00002c80: 6974 68a9 0972 0f00 0000 7210 0000 0072  ith..r....r....r
+00002c90: 8f00 0000 7290 0000 0072 9100 0000 5a07  ....r....r....Z.
+00002ca0: 6f75 7470 7574 315a 076f 7574 7075 7432  output1Z.output2
+00002cb0: da06 6f75 7470 7574 72a2 0000 0072 1100  ..outputr....r..
+00002cc0: 0000 7211 0000 0072 1200 0000 da1e 7465  ..r....r......te
+00002cd0: 7374 5f72 756e 6e65 725f 7079 7468 6f6e  st_runner_python
+00002ce0: 5f75 6e69 7474 6573 745f 6f6b 1101 0000  _unittest_ok....
+00002cf0: f31e 0000 0002 0104 0104 ff08 0306 0114  ................
+00002d00: 0102 0202 ff04 0408 0108 0110 0110 0116  ................
+00002d10: 011a 017a 2552 756e 6e65 722e 7465 7374  ...z%Runner.test
+00002d20: 5f72 756e 6e65 725f 7079 7468 6f6e 5f75  _runner_python_u
+00002d30: 6e69 7474 6573 745f 6f6b 6301 0000 0000  nittest_okc.....
+00002d40: 0000 0000 0000 0009 0000 0005 0000 0043  ...............C
+00002d50: 0000 0073 a400 0000 7400 6401 6402 8302  ...s....t.d.d...
+00002d60: 7d01 7c01 a001 a100 7d02 7c02 8300 7d03  }.|.....}.|...}.
+00002d70: 6403 6404 8400 7c03 a002 7c01 a101 4400  d.d...|...|...D.
+00002d80: 8301 7d04 7403 6a04 6405 6b00 721e 6406  ..}.t.j.d.k.r.d.
+00002d90: 7d05 6e02 6407 7d05 6408 7d06 7c04 6409  }.n.d.}.d.}.|.d.
+00002da0: 1900 7d07 7c04 640a 1900 7d08 7c00 a005  ..}.|.d...}.|...
+00002db0: 7c08 640b 1900 640c a102 0100 7c00 a005  |.d...d.....|...
+00002dc0: 7c08 640d 1900 640e a102 0100 7c00 a006  |.d...d.....|...
+00002dd0: 7c07 640f 1900 a007 7c05 a101 6410 a102  |.d.....|...d...
+00002de0: 0100 7c00 a006 7c07 640f 1900 a008 7c06  ..|...|.d.....|.
+00002df0: a101 6411 a102 0100 6400 5300 2912 4e72  ..d.....d.S.).Nr
+00002e00: aa00 0000 7a2d 7365 6c66 7465 7374 732f  ....z-selftests/
+00002e10: 2e64 6174 612f 756e 6974 7465 7374 732e  .data/unittests.
+00002e20: 7079 3a53 6563 6f6e 642e 7465 7374 5f66  py:Second.test_f
+00002e30: 6169 6c63 0100 0000 0000 0000 0000 0000  ailc............
+00002e40: 0200 0000 0300 0000 5300 0000 7284 0000  ........S...r...
+00002e50: 0072 1100 0000 7211 0000 0072 8500 0000  .r....r....r....
+00002e60: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00002e70: 8800 0000 2a01 0000 7289 0000 007a 3b52  ....*...r....z;R
+00002e80: 756e 6e65 722e 7465 7374 5f72 756e 6e65  unner.test_runne
+00002e90: 725f 7079 7468 6f6e 5f75 6e69 7474 6573  r_python_unittes
+00002ea0: 745f 6661 696c 2e3c 6c6f 6361 6c73 3e2e  t_fail.<locals>.
+00002eb0: 3c6c 6973 7463 6f6d 703e 2902 e903 0000  <listcomp>).....
+00002ec0: 00e9 0b00 0000 736a 0000 003d 3d3d 3d3d  ......sj...=====
+00002ed0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002ee0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002ef0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002f00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002f10: 3d0a 4641 494c 3a20 7465 7374 5f66 6169  =.FAIL: test_fai
+00002f20: 6c20 2875 6e69 7474 6573 7473 2e53 6563  l (unittests.Sec
+00002f30: 6f6e 6429 0a73 7400 0000 3d3d 3d3d 3d3d  ond).st...======
+00002f40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002f50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002f60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002f70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002f80: 0a46 4149 4c3a 2074 6573 745f 6661 696c  .FAIL: test_fail
+00002f90: 2028 756e 6974 7465 7374 732e 5365 636f   (unittests.Seco
+00002fa0: 6e64 2e74 6573 745f 6661 696c 290a 7316  nd.test_fail).s.
+00002fb0: 0000 000a 0a46 4149 4c45 4420 2866 6169  .....FAILED (fai
+00002fc0: 6c75 7265 733d 3129 0a72 9600 0000 728a  lures=1).r....r.
+00002fd0: 0000 0072 8700 0000 728b 0000 0072 a200  ...r....r....r..
+00002fe0: 0000 72a6 0000 0072 9900 0000 72ac 0000  ..r....r....r...
+00002ff0: 0072 ad00 0000 2909 7202 0000 0072 4800  .r....).r....rH.
+00003000: 0000 728e 0000 0072 9e00 0000 da0c 7665  ..r....r......ve
+00003010: 7273 696f 6e5f 696e 666f 7219 0000 0072  rsion_infor....r
+00003020: 7600 0000 72af 0000 0072 b000 0000 72b1  v...r....r....r.
+00003030: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00003040: 0000 da20 7465 7374 5f72 756e 6e65 725f  ... test_runner_
+00003050: 7079 7468 6f6e 5f75 6e69 7474 6573 745f  python_unittest_
+00003060: 6661 696c 2401 0000 7324 0000 0002 0104  fail$...s$......
+00003070: 0104 ff08 0306 0114 010a 0102 0204 ff02  ................
+00003080: 0602 ff04 0408 0108 0110 0110 0116 011a  ................
+00003090: 017a 2752 756e 6e65 722e 7465 7374 5f72  .z'Runner.test_r
+000030a0: 756e 6e65 725f 7079 7468 6f6e 5f75 6e69  unner_python_uni
+000030b0: 7474 6573 745f 6661 696c 6301 0000 0000  ttest_failc.....
+000030c0: 0000 0000 0000 0009 0000 0005 0000 0043  ...............C
+000030d0: 0000 0072 a900 0000 2910 4e72 aa00 0000  ...r....).Nr....
+000030e0: 7a2d 7365 6c66 7465 7374 732f 2e64 6174  z-selftests/.dat
+000030f0: 612f 756e 6974 7465 7374 732e 7079 3a53  a/unittests.py:S
+00003100: 6563 6f6e 642e 7465 7374 5f73 6b69 7063  econd.test_skipc
+00003110: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003120: 0300 0000 5300 0000 7284 0000 0072 1100  ....S...r....r..
+00003130: 0000 7211 0000 0072 8500 0000 7211 0000  ..r....r....r...
+00003140: 0072 1100 0000 7212 0000 0072 8800 0000  .r....r....r....
+00003150: 4301 0000 7289 0000 007a 3b52 756e 6e65  C...r....z;Runne
+00003160: 722e 7465 7374 5f72 756e 6e65 725f 7079  r.test_runner_py
+00003170: 7468 6f6e 5f75 6e69 7474 6573 745f 736b  thon_unittest_sk
+00003180: 6970 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ip.<locals>.<lis
+00003190: 7463 6f6d 703e 72ab 0000 0073 1200 0000  tcomp>r....s....
+000031a0: 730a 0a4f 4b20 2873 6b69 7070 6564 3d31  s..OK (skipped=1
+000031b0: 290a 7296 0000 0072 8a00 0000 7287 0000  ).r....r....r...
+000031c0: 0072 8b00 0000 72a2 0000 00da 0473 6b69  .r....r......ski
+000031d0: 7072 9900 0000 72ac 0000 0072 ad00 0000  pr....r....r....
+000031e0: 72ae 0000 0072 b100 0000 7211 0000 0072  r....r....r....r
+000031f0: 1100 0000 7212 0000 00da 2074 6573 745f  ....r..... test_
+00003200: 7275 6e6e 6572 5f70 7974 686f 6e5f 756e  runner_python_un
+00003210: 6974 7465 7374 5f73 6b69 703d 0100 0072  ittest_skip=...r
+00003220: b400 0000 7a27 5275 6e6e 6572 2e74 6573  ....z'Runner.tes
+00003230: 745f 7275 6e6e 6572 5f70 7974 686f 6e5f  t_runner_python_
+00003240: 756e 6974 7465 7374 5f73 6b69 7063 0100  unittest_skipc..
+00003250: 0000 0000 0000 0000 0000 0700 0000 0400  ................
+00003260: 0000 4300 0000 736c 0000 0074 0064 0164  ..C...sl...t.d.d
+00003270: 0283 027d 017c 01a0 01a1 007d 027c 0283  ...}.|.....}.|..
+00003280: 007d 0364 0364 0484 007c 03a0 027c 01a1  .}.d.d...|...|..
+00003290: 0144 0083 017d 0464 057d 057c 0464 0619  .D...}.d.}.|.d..
+000032a0: 007d 067c 00a0 037c 0664 0719 0064 08a1  .}.|...|.d...d..
+000032b0: 0201 007c 00a0 037c 0664 0919 0064 02a1  ...|...|.d...d..
+000032c0: 0201 007c 00a0 037c 0664 0a19 007c 05a1  ...|...|.d...|..
+000032d0: 0201 0064 0053 0029 0b4e 72aa 0000 00da  ...d.S.).Nr.....
+000032e0: 0565 7272 6f72 6301 0000 0000 0000 0000  .errorc.........
+000032f0: 0000 0002 0000 0003 0000 0053 0000 0072  ...........S...r
+00003300: 8400 0000 7211 0000 0072 1100 0000 7285  ....r....r....r.
+00003310: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00003320: 0000 7288 0000 0054 0100 0072 8900 0000  ..r....T...r....
+00003330: 7a3c 5275 6e6e 6572 2e74 6573 745f 7275  z<Runner.test_ru
+00003340: 6e6e 6572 5f70 7974 686f 6e5f 756e 6974  nner_python_unit
+00003350: 7465 7374 5f65 7272 6f72 2e3c 6c6f 6361  test_error.<loca
+00003360: 6c73 3e2e 3c6c 6973 7463 6f6d 703e fa3f  ls>.<listcomp>.?
+00003370: 496e 7661 6c69 6420 5552 493a 2063 6f75  Invalid URI: cou
+00003380: 6c64 206e 6f74 2062 6520 636f 6e76 6572  ld not be conver
+00003390: 7465 6420 746f 2061 6e20 756e 6974 7465  ted to an unitte
+000033a0: 7374 2064 6f74 7465 6420 6e61 6d65 2e72  st dotted name.r
+000033b0: 8a00 0000 7287 0000 0072 8b00 0000 72a2  ....r....r....r.
+000033c0: 0000 0072 b200 0000 a904 7202 0000 0072  ...r......r....r
+000033d0: 4800 0000 728e 0000 0072 1900 0000 a907  H...r....r......
+000033e0: 720f 0000 0072 1000 0000 728f 0000 0072  r....r....r....r
+000033f0: 9000 0000 7291 0000 0072 b200 0000 72a2  ....r....r....r.
+00003400: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00003410: 0000 da21 7465 7374 5f72 756e 6e65 725f  ...!test_runner_
+00003420: 7079 7468 6f6e 5f75 6e69 7474 6573 745f  python_unittest_
+00003430: 6572 726f 7250 0100 00f3 1200 0000 0a01  errorP..........
+00003440: 0801 0601 1401 0401 0801 1001 1001 1401  ................
+00003450: 7a28 5275 6e6e 6572 2e74 6573 745f 7275  z(Runner.test_ru
+00003460: 6e6e 6572 5f70 7974 686f 6e5f 756e 6974  nner_python_unit
+00003470: 7465 7374 5f65 7272 6f72 6301 0000 0000  test_errorc.....
+00003480: 0000 0000 0000 0007 0000 0004 0000 0043  ...............C
+00003490: 0000 0073 6c00 0000 7400 6401 6402 8302  ...sl...t.d.d...
+000034a0: 7d01 7c01 a001 a100 7d02 7c02 8300 7d03  }.|.....}.|...}.
+000034b0: 6403 6404 8400 7c03 a002 7c01 a101 4400  d.d...|...|...D.
+000034c0: 8301 7d04 6405 7d05 7c04 6406 1900 7d06  ..}.d.}.|.d...}.
+000034d0: 7c00 a003 7c06 6407 1900 6408 a102 0100  |...|.d...d.....
+000034e0: 7c00 a003 7c06 6409 1900 640a a102 0100  |...|.d...d.....
+000034f0: 7c00 a003 7c06 640b 1900 7c05 a102 0100  |...|.d...|.....
+00003500: 6400 5300 290c 4e72 aa00 0000 7247 0000  d.S.).Nr....rG..
+00003510: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00003520: 0000 0300 0000 5300 0000 7284 0000 0072  ......S...r....r
+00003530: 1100 0000 7211 0000 0072 8500 0000 7211  ....r....r....r.
+00003540: 0000 0072 1100 0000 7212 0000 0072 8800  ...r....r....r..
+00003550: 0000 5f01 0000 7289 0000 007a 4652 756e  .._...r....zFRun
+00003560: 6e65 722e 7465 7374 5f72 756e 6e65 725f  ner.test_runner_
+00003570: 7079 7468 6f6e 5f75 6e69 7474 6573 745f  python_unittest_
+00003580: 656d 7074 795f 7572 695f 6572 726f 722e  empty_uri_error.
+00003590: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+000035a0: 6d70 3e72 bc00 0000 728a 0000 0072 8700  mp>r....r....r..
+000035b0: 0000 728b 0000 0072 a200 0000 72bb 0000  ..r....r....r...
+000035c0: 0072 b200 0000 72bd 0000 0072 be00 0000  .r....r....r....
+000035d0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+000035e0: 2b74 6573 745f 7275 6e6e 6572 5f70 7974  +test_runner_pyt
+000035f0: 686f 6e5f 756e 6974 7465 7374 5f65 6d70  hon_unittest_emp
+00003600: 7479 5f75 7269 5f65 7272 6f72 5b01 0000  ty_uri_error[...
+00003610: 72c0 0000 007a 3252 756e 6e65 722e 7465  r....z2Runner.te
+00003620: 7374 5f72 756e 6e65 725f 7079 7468 6f6e  st_runner_python
+00003630: 5f75 6e69 7474 6573 745f 656d 7074 795f  _unittest_empty_
+00003640: 7572 695f 6572 726f 724e 290d 724d 0000  uri_errorN).rM..
+00003650: 0072 4e00 0000 724f 0000 0072 9300 0000  .rN...rO...r....
+00003660: 72a1 0000 0072 a400 0000 7205 0000 0072  r....r....r....r
+00003670: a800 0000 72b3 0000 0072 b800 0000 72ba  ....r....r....r.
+00003680: 0000 0072 bf00 0000 72c1 0000 0072 1100  ...r....r....r..
+00003690: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+000036a0: 0072 8300 0000 d000 0000 7316 0000 0008  .r........s.....
+000036b0: 0008 0108 0908 1206 130a 0108 1108 1308  ................
+000036c0: 1908 130c 0b72 8300 0000 6300 0000 0000  .....r....c.....
+000036d0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+000036e0: 0000 0073 6c00 0000 6500 5a01 6400 5a02  ...sl...e.Z.d.Z.
+000036f0: 6401 6402 8400 5a03 6504 6403 8301 6404  d.d...Z.e.d...d.
+00003700: 6405 8400 8301 5a05 6504 6403 8301 6406  d.....Z.e.d...d.
+00003710: 6407 8400 8301 5a06 6504 6403 8301 6408  d.....Z.e.d...d.
+00003720: 6409 8400 8301 5a07 6504 6403 8301 640a  d.....Z.e.d...d.
+00003730: 640b 8400 8301 5a08 6504 6403 8301 640c  d.....Z.e.d...d.
+00003740: 640d 8400 8301 5a09 640e 640f 8400 5a0a  d.....Z.d.d...Z.
+00003750: 6410 5300 2911 da09 5275 6e6e 6572 546d  d.S.)...RunnerTm
+00003760: 7063 0100 0000 0000 0000 0000 0000 0200  pc..............
+00003770: 0000 0300 0000 4300 0000 7266 0000 0072  ......C...rf...r
+00003780: 6700 0000 7269 0000 0072 6d00 0000 7211  g...ri...rm...r.
+00003790: 0000 0072 1100 0000 7212 0000 0072 6e00  ...r....r....rn.
+000037a0: 0000 6801 0000 726f 0000 007a 0f52 756e  ..h...ro...z.Run
+000037b0: 6e65 7254 6d70 2e73 6574 5570 7238 0000  nerTmp.setUpr8..
+000037c0: 0063 0100 0000 0000 0000 0000 0000 0800  .c..............
+000037d0: 0000 0800 0000 4300 0000 f3b2 0000 0064  ......C........d
+000037e0: 017d 0174 006a 01a0 027c 006a 036a 0464  .}.t.j...|.j.j.d
+000037f0: 02a1 027d 0274 057c 0264 0364 0464 058d  ...}.t.|.d.d.d..
+00003800: 038f 0d7d 037c 03a0 067c 01a1 0101 0057  ...}.|...|.....W
+00003810: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+00003820: 2277 0101 0001 0001 0059 0001 0074 0764  "w.......Y...t.d
+00003830: 0664 077c 0283 037d 0474 08a0 09a1 007d  .d.|...}.t.....}
+00003840: 0564 0864 0984 007c 05a0 0a7c 04a1 0144  .d.d...|...|...D
+00003850: 0083 017d 067c 0664 0a19 007d 077c 00a0  ...}.|.d...}.|..
+00003860: 0b7c 0764 0b19 0064 0ca1 0201 007c 00a0  .|.d...d.....|..
+00003870: 0b7c 0764 0d19 0064 0ea1 0201 007c 00a0  .|.d...d.....|..
+00003880: 0b7c 0764 0f19 0064 10a1 0201 0064 0053  .|.d...d.....d.S
+00003890: 0029 114e 7a71 2321 2f62 696e 2f73 680a  .).Nzq#!/bin/sh.
+000038a0: 6563 686f 2027 312e 2e32 270a 6563 686f  echo '1..2'.echo
+000038b0: 2027 2320 4465 6669 6e69 6e67 2061 6e20   '# Defining an 
+000038c0: 6261 7369 6320 7465 7374 270a 6563 686f  basic test'.echo
+000038d0: 2027 6f6b 2031 202d 2064 6573 6372 6970   'ok 1 - descrip
+000038e0: 7469 6f6e 2031 270a 6563 686f 2027 6e6f  tion 1'.echo 'no
+000038f0: 7420 6f6b 2032 202d 2064 6573 6372 6970  t ok 2 - descrip
+00003900: 7469 6f6e 2032 27fa 0674 6170 2e73 68da  tion 2'..tap.sh.
+00003910: 0177 fa05 7574 662d 38a9 01da 0865 6e63  .w..utf-8....enc
+00003920: 6f64 696e 6772 0400 0000 7238 0000 0063  odingr....r8...c
+00003930: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003940: 0300 0000 5300 0000 7284 0000 0072 1100  ....S...r....r..
+00003950: 0000 7211 0000 0072 8500 0000 7211 0000  ..r....r....r...
+00003960: 0072 1100 0000 7212 0000 0072 8800 0000  .r....r....r....
+00003970: 7a01 0000 7289 0000 007a 3252 756e 6e65  z...r....z2Runne
+00003980: 7254 6d70 2e74 6573 745f 7275 6e6e 6572  rTmp.test_runner
+00003990: 5f74 6170 5f66 6169 6c2e 3c6c 6f63 616c  _tap_fail.<local
+000039a0: 733e 2e3c 6c69 7374 636f 6d70 3e72 8a00  s>.<listcomp>r..
+000039b0: 0000 7287 0000 0072 8b00 0000 72a2 0000  ..r....r....r...
+000039c0: 0072 a600 0000 729c 0000 0072 0100 0000  .r....r....r....
+000039d0: a90c 7271 0000 0072 7200 0000 7273 0000  ..rq...rr...rs..
+000039e0: 0072 6c00 0000 7274 0000 00da 046f 7065  .rl...rt.....ope
+000039f0: 6eda 0577 7269 7465 7202 0000 00da 0a72  n..writer......r
+00003a00: 756e 6e65 725f 7461 705a 0954 4150 5275  unner_tapZ.TAPRu
+00003a10: 6e6e 6572 728e 0000 0072 1900 0000 a908  nnerr....r......
+00003a20: 720f 0000 005a 0a74 6170 5f73 6372 6970  r....Z.tap_scrip
+00003a30: 745a 0874 6170 5f70 6174 68da 0266 7072  tZ.tap_path..fpr
+00003a40: 1000 0000 7290 0000 0072 9100 0000 7292  ....r....r....r.
+00003a50: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00003a60: 0000 da14 7465 7374 5f72 756e 6e65 725f  ....test_runner_
+00003a70: 7461 705f 6661 696c 6c01 0000 f318 0000  tap_faill.......
+00003a80: 0004 0212 0510 020c 011c ff0c 0308 0114  ................
+00003a90: 0108 0110 0110 0114 017a 1e52 756e 6e65  .........z.Runne
+00003aa0: 7254 6d70 2e74 6573 745f 7275 6e6e 6572  rTmp.test_runner
+00003ab0: 5f74 6170 5f66 6169 6c63 0100 0000 0000  _tap_failc......
+00003ac0: 0000 0000 0000 0800 0000 0800 0000 4300  ..............C.
+00003ad0: 0000 72c3 0000 0029 114e 7a6d 2321 2f62  ..r....).Nzm#!/b
+00003ae0: 696e 2f73 680a 6563 686f 2027 312e 2e32  in/sh.echo '1..2
+00003af0: 270a 6563 686f 2027 2320 4465 6669 6e69  '.echo '# Defini
+00003b00: 6e67 2061 6e20 6261 7369 6320 7465 7374  ng an basic test
+00003b10: 270a 6563 686f 2027 6f6b 2031 202d 2064  '.echo 'ok 1 - d
+00003b20: 6573 6372 6970 7469 6f6e 2031 270a 6563  escription 1'.ec
+00003b30: 686f 2027 6f6b 2032 202d 2064 6573 6372  ho 'ok 2 - descr
+00003b40: 6970 7469 6f6e 2032 2772 c400 0000 72c5  iption 2'r....r.
+00003b50: 0000 0072 c600 0000 72c7 0000 0072 0400  ...r....r....r..
+00003b60: 0000 7238 0000 0063 0100 0000 0000 0000  ..r8...c........
+00003b70: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+00003b80: 7284 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00003b90: 8500 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00003ba0: 0000 0072 8800 0000 8e01 0000 7289 0000  ...r........r...
+00003bb0: 007a 3052 756e 6e65 7254 6d70 2e74 6573  .z0RunnerTmp.tes
+00003bc0: 745f 7275 6e6e 6572 5f74 6170 5f6f 6b2e  t_runner_tap_ok.
+00003bd0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00003be0: 6d70 3e72 8a00 0000 7287 0000 0072 8b00  mp>r....r....r..
+00003bf0: 0000 72a2 0000 0072 a300 0000 729c 0000  ..r....r....r...
+00003c00: 0072 0100 0000 72c9 0000 0072 cd00 0000  .r....r....r....
+00003c10: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00003c20: 1274 6573 745f 7275 6e6e 6572 5f74 6170  .test_runner_tap
+00003c30: 5f6f 6b80 0100 0072 d000 0000 7a1c 5275  _ok....r....z.Ru
+00003c40: 6e6e 6572 546d 702e 7465 7374 5f72 756e  nnerTmp.test_run
+00003c50: 6e65 725f 7461 705f 6f6b 6301 0000 0000  ner_tap_okc.....
+00003c60: 0000 0000 0000 0008 0000 0008 0000 0043  ...............C
+00003c70: 0000 0072 c300 0000 2911 4e7a 7423 212f  ...r....).Nzt#!/
+00003c80: 6269 6e2f 7368 0a65 6368 6f20 2731 2e2e  bin/sh.echo '1..
+00003c90: 3227 0a65 6368 6f20 2723 2044 6566 696e  2'.echo '# Defin
+00003ca0: 696e 6720 616e 2062 6173 6963 2074 6573  ing an basic tes
+00003cb0: 7427 0a65 6368 6f20 276f 6b20 3120 2d20  t'.echo 'ok 1 - 
+00003cc0: 2320 534b 4950 2064 6573 6372 6970 7469  # SKIP descripti
+00003cd0: 6f6e 2031 270a 6563 686f 2027 6f6b 2032  on 1'.echo 'ok 2
+00003ce0: 202d 2064 6573 6372 6970 7469 6f6e 2032   - description 2
+00003cf0: 2772 c400 0000 72c5 0000 0072 c600 0000  'r....r....r....
+00003d00: 72c7 0000 0072 0400 0000 7238 0000 0063  r....r....r8...c
+00003d10: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003d20: 0300 0000 5300 0000 7284 0000 0072 1100  ....S...r....r..
+00003d30: 0000 7211 0000 0072 8500 0000 7211 0000  ..r....r....r...
+00003d40: 0072 1100 0000 7212 0000 0072 8800 0000  .r....r....r....
+00003d50: a201 0000 7289 0000 007a 3252 756e 6e65  ....r....z2Runne
+00003d60: 7254 6d70 2e74 6573 745f 7275 6e6e 6572  rTmp.test_runner
+00003d70: 5f74 6170 5f73 6b69 702e 3c6c 6f63 616c  _tap_skip.<local
+00003d80: 733e 2e3c 6c69 7374 636f 6d70 3e72 8a00  s>.<listcomp>r..
+00003d90: 0000 7287 0000 0072 8b00 0000 72a2 0000  ..r....r....r...
+00003da0: 0072 b900 0000 729c 0000 0072 0100 0000  .r....r....r....
+00003db0: 72c9 0000 0072 cd00 0000 7211 0000 0072  r....r....r....r
+00003dc0: 1100 0000 7212 0000 00da 1474 6573 745f  ....r......test_
+00003dd0: 7275 6e6e 6572 5f74 6170 5f73 6b69 7094  runner_tap_skip.
+00003de0: 0100 0072 d000 0000 7a1e 5275 6e6e 6572  ...r....z.Runner
+00003df0: 546d 702e 7465 7374 5f72 756e 6e65 725f  Tmp.test_runner_
+00003e00: 7461 705f 736b 6970 6301 0000 0000 0000  tap_skipc.......
+00003e10: 0000 0000 0008 0000 0008 0000 0043 0000  .............C..
+00003e20: 0072 c300 0000 2911 4e7a 7223 212f 6269  .r....).Nzr#!/bi
+00003e30: 6e2f 7368 0a65 6368 6f20 2731 2e2e 3227  n/sh.echo '1..2'
+00003e40: 0a65 6368 6f20 2723 2044 6566 696e 696e  .echo '# Definin
+00003e50: 6720 616e 2062 6173 6963 2074 6573 7427  g an basic test'
+00003e60: 0a65 6368 6f20 2742 6169 6c20 6f75 7421  .echo 'Bail out!
+00003e70: 202d 2064 6573 6372 6970 7469 6f6e 2031   - description 1
+00003e80: 270a 6563 686f 2027 6f6b 2032 202d 2064  '.echo 'ok 2 - d
+00003e90: 6573 6372 6970 7469 6f6e 2032 2772 c400  escription 2'r..
+00003ea0: 0000 72c5 0000 0072 c600 0000 72c7 0000  ..r....r....r...
+00003eb0: 0072 0400 0000 7238 0000 0063 0100 0000  .r....r8...c....
+00003ec0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00003ed0: 5300 0000 7284 0000 0072 1100 0000 7211  S...r....r....r.
+00003ee0: 0000 0072 8500 0000 7211 0000 0072 1100  ...r....r....r..
+00003ef0: 0000 7212 0000 0072 8800 0000 b601 0000  ..r....r........
+00003f00: 7289 0000 007a 3552 756e 6e65 7254 6d70  r....z5RunnerTmp
+00003f10: 2e74 6573 745f 7275 6e6e 6572 5f74 6170  .test_runner_tap
+00003f20: 5f62 6169 6c6f 7574 2e3c 6c6f 6361 6c73  _bailout.<locals
+00003f30: 3e2e 3c6c 6973 7463 6f6d 703e 728a 0000  >.<listcomp>r...
+00003f40: 0072 8700 0000 728b 0000 0072 a200 0000  .r....r....r....
+00003f50: 72bb 0000 0072 9c00 0000 7201 0000 0072  r....r....r....r
+00003f60: c900 0000 72cd 0000 0072 1100 0000 7211  ....r....r....r.
+00003f70: 0000 0072 1200 0000 da17 7465 7374 5f72  ...r......test_r
+00003f80: 756e 6e65 725f 7461 705f 6261 696c 6f75  unner_tap_bailou
+00003f90: 74a8 0100 0072 d000 0000 7a21 5275 6e6e  t....r....z!Runn
+00003fa0: 6572 546d 702e 7465 7374 5f72 756e 6e65  erTmp.test_runne
+00003fb0: 725f 7461 705f 6261 696c 6f75 7463 0100  r_tap_bailoutc..
+00003fc0: 0000 0000 0000 0000 0000 0800 0000 0800  ................
+00003fd0: 0000 4300 0000 72c3 0000 0029 114e 7a6e  ..C...r....).Nzn
+00003fe0: 2321 2f62 696e 2f73 680a 6563 686f 2027  #!/bin/sh.echo '
+00003ff0: 312e 2e32 270a 6563 686f 2027 2320 4465  1..2'.echo '# De
+00004000: 6669 6e69 6e67 2061 6e20 6261 7369 6320  fining an basic 
+00004010: 7465 7374 270a 6563 686f 2027 6572 726f  test'.echo 'erro
+00004020: 7220 2d20 6465 7363 7269 7074 696f 6e20  r - description 
+00004030: 3127 0a65 6368 6f20 276f 6b20 3220 2d20  1'.echo 'ok 2 - 
+00004040: 6465 7363 7269 7074 696f 6e20 3227 72c4  description 2'r.
+00004050: 0000 0072 c500 0000 72c6 0000 0072 c700  ...r....r....r..
+00004060: 0000 7204 0000 0072 3800 0000 6301 0000  ..r....r8...c...
+00004070: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00004080: 0053 0000 0072 8400 0000 7211 0000 0072  .S...r....r....r
+00004090: 1100 0000 7285 0000 0072 1100 0000 7211  ....r....r....r.
+000040a0: 0000 0072 1200 0000 7288 0000 00ca 0100  ...r....r.......
+000040b0: 0072 8900 0000 7a33 5275 6e6e 6572 546d  .r....z3RunnerTm
+000040c0: 702e 7465 7374 5f72 756e 6e65 725f 7461  p.test_runner_ta
+000040d0: 705f 6572 726f 722e 3c6c 6f63 616c 733e  p_error.<locals>
+000040e0: 2e3c 6c69 7374 636f 6d70 3e72 8a00 0000  .<listcomp>r....
+000040f0: 7287 0000 0072 8b00 0000 72a2 0000 0072  r....r....r....r
+00004100: bb00 0000 729c 0000 0072 0100 0000 72c9  ....r....r....r.
+00004110: 0000 0072 cd00 0000 7211 0000 0072 1100  ...r....r....r..
+00004120: 0000 7212 0000 00da 1574 6573 745f 7275  ..r......test_ru
+00004130: 6e6e 6572 5f74 6170 5f65 7272 6f72 bc01  nner_tap_error..
+00004140: 0000 72d0 0000 007a 1f52 756e 6e65 7254  ..r....z.RunnerT
+00004150: 6d70 2e74 6573 745f 7275 6e6e 6572 5f74  mp.test_runner_t
+00004160: 6170 5f65 7272 6f72 6301 0000 0000 0000  ap_errorc.......
+00004170: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00004180: 0072 7e00 0000 7226 0000 0072 7f00 0000  .r~...r&...r....
+00004190: 7229 0000 0072 1100 0000 7211 0000 0072  r)...r....r....r
+000041a0: 1200 0000 7281 0000 00d0 0100 0072 8200  ....r........r..
+000041b0: 0000 7a12 5275 6e6e 6572 546d 702e 7465  ..z.RunnerTmp.te
+000041c0: 6172 446f 776e 4e29 0b72 4d00 0000 724e  arDownN).rM...rN
+000041d0: 0000 0072 4f00 0000 726e 0000 0072 0500  ...rO...rn...r..
+000041e0: 0000 72cf 0000 0072 d100 0000 72d2 0000  ..r....r....r...
+000041f0: 0072 d300 0000 72d4 0000 0072 8100 0000  .r....r....r....
+00004200: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00004210: 1200 0000 72c2 0000 0067 0100 0073 1a00  ....r....g...s..
+00004220: 0000 0800 0801 0604 0a01 0613 0a01 0613  ................
+00004230: 0a01 0613 0a01 0613 0a01 0c13 72c2 0000  ............r...
+00004240: 0072 3800 0000 6300 0000 0000 0000 0000  .r8...c.........
+00004250: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+00004260: 2c00 0000 6500 5a01 6400 5a02 6401 6402  ,...e.Z.d.Z.d.d.
+00004270: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
+00004280: 8400 5a05 6407 6408 8400 5a06 6409 5300  ..Z.d.d...Z.d.S.
+00004290: 290a da16 5275 6e6e 6572 436f 6d6d 616e  )...RunnerComman
+000042a0: 6453 656c 6563 7469 6f6e 6301 0000 0000  dSelectionc.....
+000042b0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+000042c0: 0000 00f3 0a00 0000 6401 7c00 5f00 6400  ........d.|._.d.
+000042d0: 5300 2902 4e5a 066d 796b 696e 64a9 0172  S.).NZ.mykind..r
+000042e0: 2b00 0000 7229 0000 0072 1100 0000 7211  +...r)...r....r.
+000042f0: 0000 0072 1200 0000 726e 0000 00d6 0100  ...r....rn......
+00004300: 00f3 0200 0000 0a01 7a1c 5275 6e6e 6572  ........z.Runner
+00004310: 436f 6d6d 616e 6453 656c 6563 7469 6f6e  CommandSelection
+00004320: 2e73 6574 5570 6301 0000 0000 0000 0000  .setUpc.........
+00004330: 0000 0002 0000 0006 0000 0043 0000 00f3  ...........C....
+00004340: 2000 0000 6700 6401 a201 7d01 7c00 a000   ...g.d...}.|...
+00004350: 7401 a002 7c00 6a03 7c01 a102 a101 0100  t...|.j.|.......
+00004360: 6400 5300 2902 4e29 03da 0273 6872 5800  d.S.).N)...shrX.
+00004370: 0000 7a3f 7465 7374 2024 3020 3d20 6361  ..z?test $0 = ca
+00004380: 7061 6269 6c69 7469 6573 2026 2620 6563  pabilities && ec
+00004390: 686f 202d 6e20 7b5c 2272 756e 6e61 626c  ho -n {\"runnabl
+000043a0: 6573 5c22 3a20 5b5c 226d 796b 696e 645c  es\": [\"mykind\
+000043b0: 225d 7d29 0472 7600 0000 7202 0000 00da  "]}).rv...r.....
+000043c0: 2369 735f 6b69 6e64 5f73 7570 706f 7274  #is_kind_support
+000043d0: 6564 5f62 795f 7275 6e6e 6572 5f63 6f6d  ed_by_runner_com
+000043e0: 6d61 6e64 722b 0000 00a9 0272 0f00 0000  mandr+.....r....
+000043f0: da03 636d 6472 1100 0000 7211 0000 0072  ..cmdr....r....r
+00004400: 1200 0000 da1b 7465 7374 5f69 735f 7461  ......test_is_ta
+00004410: 736b 5f6b 696e 645f 7375 7070 6f72 7465  sk_kind_supporte
+00004420: 64d9 0100 00f3 0400 0000 0801 1805 7a32  d.............z2
+00004430: 5275 6e6e 6572 436f 6d6d 616e 6453 656c  RunnerCommandSel
+00004440: 6563 7469 6f6e 2e74 6573 745f 6973 5f74  ection.test_is_t
+00004450: 6173 6b5f 6b69 6e64 5f73 7570 706f 7274  ask_kind_support
+00004460: 6564 6301 0000 0000 0000 0000 0000 0002  edc.............
+00004470: 0000 0006 0000 0043 0000 0072 d900 0000  .......C...r....
+00004480: 2902 4e29 0372 da00 0000 7258 0000 007a  ).N).r....rX...z
+00004490: 4274 6573 7420 2430 203d 2063 6170 6162  Btest $0 = capab
+000044a0: 696c 6974 6965 7320 2626 2065 6368 6f20  ilities && echo 
+000044b0: 2d6e 207b 5c22 7275 6e6e 6162 6c65 735c  -n {\"runnables\
+000044c0: 223a 205b 5c22 6f74 6865 726b 696e 645c  ": [\"otherkind\
+000044d0: 225d 7da9 04da 0b61 7373 6572 7446 616c  "]}....assertFal
+000044e0: 7365 7202 0000 0072 db00 0000 722b 0000  ser....r....r+..
+000044f0: 0072 dc00 0000 7211 0000 0072 1100 0000  .r....r....r....
+00004500: 7212 0000 00da 2674 6573 745f 6973 5f74  r.....&test_is_t
+00004510: 6173 6b5f 6b69 6e64 5f73 7570 706f 7274  ask_kind_support
+00004520: 6564 5f6f 7468 6572 5f6b 696e 64e1 0100  ed_other_kind...
+00004530: 0072 df00 0000 7a3d 5275 6e6e 6572 436f  .r....z=RunnerCo
+00004540: 6d6d 616e 6453 656c 6563 7469 6f6e 2e74  mmandSelection.t
+00004550: 6573 745f 6973 5f74 6173 6b5f 6b69 6e64  est_is_task_kind
+00004560: 5f73 7570 706f 7274 6564 5f6f 7468 6572  _supported_other
+00004570: 5f6b 696e 6463 0100 0000 0000 0000 0000  _kindc..........
+00004580: 0000 0200 0000 0600 0000 4300 0000 72d9  ..........C...r.
+00004590: 0000 0029 024e 2903 72da 0000 0072 5800  ...).N).r....rX.
+000045a0: 0000 7a0a 6563 686f 202d 6e20 2222 72e0  ..z.echo -n ""r.
+000045b0: 0000 0072 dc00 0000 7211 0000 0072 1100  ...r....r....r..
+000045c0: 0000 7212 0000 00da 2574 6573 745f 6973  ..r.....%test_is
+000045d0: 5f74 6173 6b5f 6b69 6e64 5f73 7570 706f  _task_kind_suppo
+000045e0: 7274 6564 5f6e 6f5f 6f75 7470 7574 e901  rted_no_output..
+000045f0: 0000 7304 0000 0008 0118 017a 3c52 756e  ..s........z<Run
+00004600: 6e65 7243 6f6d 6d61 6e64 5365 6c65 6374  nerCommandSelect
+00004610: 696f 6e2e 7465 7374 5f69 735f 7461 736b  ion.test_is_task
+00004620: 5f6b 696e 645f 7375 7070 6f72 7465 645f  _kind_supported_
+00004630: 6e6f 5f6f 7574 7075 744e 2907 724d 0000  no_outputN).rM..
+00004640: 0072 4e00 0000 724f 0000 0072 6e00 0000  .rN...rO...rn...
+00004650: 72de 0000 0072 e200 0000 72e3 0000 0072  r....r....r....r
+00004660: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00004670: 0000 0072 d500 0000 d401 0000 730a 0000  ...r........s...
+00004680: 0008 0008 0208 0308 080c 0872 d500 0000  ...........r....
+00004690: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000046a0: 0002 0000 0040 0000 0073 2400 0000 6500  .....@...s$...e.
+000046b0: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
+000046c0: 6404 8400 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
+000046d0: 5300 2908 da0a 5069 636b 5275 6e6e 6572  S.)...PickRunner
+000046e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000046f0: 0002 0000 0043 0000 0072 d600 0000 2902  .....C...r....).
+00004700: 4efa 116c 6574 732d 696d 6167 652d 612d  N..lets-image-a-
+00004710: 6b69 6e64 72d7 0000 0072 2900 0000 7211  kindr....r)...r.
+00004720: 0000 0072 1100 0000 7212 0000 0072 6e00  ...r....r....rn.
+00004730: 0000 ef01 0000 72d8 0000 007a 1050 6963  ......r....z.Pic
+00004740: 6b52 756e 6e65 722e 7365 7455 7063 0100  kRunner.setUpc..
+00004750: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00004760: 0000 4300 0000 7328 0000 0064 0167 017d  ..C...s(...d.g.}
+00004770: 0164 027c 0169 017d 027c 00a0 0074 01a0  .d.|.i.}.|...t..
+00004780: 027c 006a 037c 02a1 027c 01a1 0201 0064  .|.j.|...|.....d
+00004790: 0053 0029 034e 7a20 6176 6f63 6164 6f2d  .S.).Nz avocado-
+000047a0: 7275 6e6e 6572 2d6c 6574 732d 696d 6167  runner-lets-imag
+000047b0: 652d 612d 6b69 6e64 72e5 0000 0029 0472  e-a-kindr....).r
+000047c0: 1900 0000 7202 0000 00da 1370 6963 6b5f  ....r......pick_
+000047d0: 7275 6e6e 6572 5f63 6f6d 6d61 6e64 722b  runner_commandr+
+000047e0: 0000 0029 0372 0f00 0000 7290 0000 005a  ...).r....r....Z
+000047f0: 056b 6e6f 776e 7211 0000 0072 1100 0000  .knownr....r....
+00004800: 7212 0000 00da 1874 6573 745f 7069 636b  r......test_pick
+00004810: 5f72 756e 6e65 725f 636f 6d6d 616e 64f2  _runner_command.
+00004820: 0100 0073 0600 0000 0601 0801 1a01 7a23  ...s..........z#
+00004830: 5069 636b 5275 6e6e 6572 2e74 6573 745f  PickRunner.test_
+00004840: 7069 636b 5f72 756e 6e65 725f 636f 6d6d  pick_runner_comm
+00004850: 616e 6463 0100 0000 0000 0000 0000 0000  andc............
+00004860: 0100 0000 0600 0000 4300 0000 7318 0000  ........C...s...
+00004870: 007c 00a0 0074 01a0 027c 006a 0369 00a1  .|...t...|.j.i..
+00004880: 02a1 0101 0064 0053 0072 2600 0000 2904  .....d.S.r&...).
+00004890: 72e1 0000 0072 0200 0000 72e6 0000 0072  r....r....r....r
+000048a0: 2b00 0000 7229 0000 0072 1100 0000 7211  +...r)...r....r.
+000048b0: 0000 0072 1200 0000 da1e 7465 7374 5f70  ...r......test_p
+000048c0: 6963 6b5f 7275 6e6e 6572 5f63 6f6d 6d61  ick_runner_comma
+000048d0: 6e64 5f65 6d70 7479 f701 0000 7302 0000  nd_empty....s...
+000048e0: 0018 017a 2950 6963 6b52 756e 6e65 722e  ...z)PickRunner.
+000048f0: 7465 7374 5f70 6963 6b5f 7275 6e6e 6572  test_pick_runner
+00004900: 5f63 6f6d 6d61 6e64 5f65 6d70 7479 4e29  _command_emptyN)
+00004910: 0672 4d00 0000 724e 0000 0072 4f00 0000  .rM...rN...rO...
+00004920: 726e 0000 0072 e700 0000 72e8 0000 0072  rn...r....r....r
+00004930: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00004940: 0000 0072 e400 0000 ee01 0000 7308 0000  ...r........s...
+00004950: 0008 0008 0108 030c 0572 e400 0000 6300  .........r....c.
+00004960: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00004970: 0000 0040 0000 0073 1c00 0000 6500 5a01  ...@...s....e.Z.
+00004980: 6400 5a02 6401 6402 8400 5a03 6403 6404  d.Z.d.d...Z.d.d.
+00004990: 8400 5a04 6405 5300 2906 da08 5461 736b  ..Z.d.S.)...Task
+000049a0: 5465 7374 6301 0000 0000 0000 0000 0000  Testc...........
+000049b0: 0003 0000 0004 0000 0043 0000 0073 2600  .........C...s&.
+000049c0: 0000 7400 6401 6402 8302 7d01 7401 7c01  ..t.d.d...}.t.|.
+000049d0: 6403 8302 7d02 7c00 a002 7c02 6a03 6404  d...}.|...|.j.d.
+000049e0: a102 0100 6400 5300 2905 4e72 0800 0000  ....d.S.).Nr....
+000049f0: da08 6e6f 6f70 5f75 7269 da07 7461 736b  ..noop_uri..task
+00004a00: 5f69 64da 0474 6573 74a9 0472 0200 0000  _id..test..r....
+00004a10: 7203 0000 0072 1900 0000 da08 6361 7465  r....r......cate
+00004a20: 676f 7279 a903 720f 0000 0072 1000 0000  gory..r....r....
+00004a30: da04 7461 736b 7211 0000 0072 1100 0000  ..taskr....r....
+00004a40: 7212 0000 00da 1574 6573 745f 6465 6661  r......test_defa
+00004a50: 756c 745f 6361 7465 676f 7279 fc01 0000  ult_category....
+00004a60: 7306 0000 000a 010a 0112 017a 1e54 6173  s..........z.Tas
+00004a70: 6b54 6573 742e 7465 7374 5f64 6566 6175  kTest.test_defau
+00004a80: 6c74 5f63 6174 6567 6f72 7963 0100 0000  lt_categoryc....
+00004a90: 0000 0000 0000 0000 0300 0000 0500 0000  ................
+00004aa0: 4300 0000 732a 0000 0074 0064 0164 0283  C...s*...t.d.d..
+00004ab0: 027d 0174 017c 0164 0364 0464 058d 037d  .}.t.|.d.d.d...}
+00004ac0: 027c 00a0 027c 026a 0364 04a1 0201 0064  .|...|.j.d.....d
+00004ad0: 0053 0029 064e 7208 0000 0072 ea00 0000  .S.).Nr....r....
+00004ae0: 72eb 0000 005a 0c6e 6577 5f63 6174 6567  r....Z.new_categ
+00004af0: 6f72 7929 0172 ee00 0000 72ed 0000 0072  ory).r....r....r
+00004b00: ef00 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00004b10: 0000 00da 1174 6573 745f 7365 745f 6361  .....test_set_ca
+00004b20: 7465 676f 7279 0102 0000 7306 0000 000a  tegory....s.....
+00004b30: 010e 0112 017a 1a54 6173 6b54 6573 742e  .....z.TaskTest.
+00004b40: 7465 7374 5f73 6574 5f63 6174 6567 6f72  test_set_categor
+00004b50: 794e 2905 724d 0000 0072 4e00 0000 724f  yN).rM...rN...rO
+00004b60: 0000 0072 f100 0000 72f2 0000 0072 1100  ...r....r....r..
+00004b70: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00004b80: 0072 e900 0000 fb01 0000 7306 0000 0008  .r........s.....
+00004b90: 0008 010c 0572 e900 0000 da08 5f5f 6d61  .....r......__ma
+00004ba0: 696e 5f5f 291a 7271 0000 0072 9e00 0000  in__).rq...r....
+00004bb0: 726a 0000 005a 0d75 6e69 7474 6573 742e  rj...Z.unittest.
+00004bc0: 6d6f 636b 7230 0000 00da 1d61 766f 6361  mockr0.....avoca
+00004bd0: 646f 2e63 6f72 652e 6e72 756e 6e65 722e  do.core.nrunner.
+00004be0: 7275 6e6e 6162 6c65 7202 0000 00da 1961  runnabler......a
+00004bf0: 766f 6361 646f 2e63 6f72 652e 6e72 756e  vocado.core.nrun
+00004c00: 6e65 722e 7461 736b 7203 0000 005a 1761  ner.taskr....Z.a
+00004c10: 766f 6361 646f 2e70 6c75 6769 6e73 2e72  vocado.plugins.r
+00004c20: 756e 6e65 7273 7204 0000 0072 cc00 0000  unnersr....r....
+00004c30: 5a0f 7365 6c66 7465 7374 732e 7574 696c  Z.selftests.util
+00004c40: 7372 0500 0000 7206 0000 00da 0854 6573  sr....r......Tes
+00004c50: 7443 6173 6572 0700 0000 7251 0000 0072  tCaser....rQ...r
+00004c60: 6500 0000 7283 0000 0072 c200 0000 72d5  e...r....r....r.
+00004c70: 0000 0072 e400 0000 72e9 0000 0072 4d00  ...r....r....rM.
+00004c80: 0000 da04 6d61 696e 7211 0000 0072 1100  ....mainr....r..
+00004c90: 0000 7211 0000 0072 1200 0000 da08 3c6d  ..r....r......<m
+00004ca0: 6f64 756c 653e 0100 0000 732a 0000 0008  odule>....s*....
+00004cb0: 0008 0108 0108 010c 020c 010c 0110 0112  ................
+00004cc0: 0312 6812 3812 2400 7f12 1806 6d14 0112  ..h.8.$.....m...
+00004cd0: 1912 0d08 0c0c 0104 ff                   .........
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_output.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_output.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 911 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 8f03 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 8f03 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6502 6a08 8303 5a09 650a 6406 6b02 7227  e.j...Z.e.d.k.r'
 00000070: 6502 a00b a100 0100 6401 5300 6401 5300  e.......d.S.d.S.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_parameters.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_parameters.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2285 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 ed08 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 ed08 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6500 6a04 8303 5a05 6506 6405 6b02 721f  e.j...Z.e.d.k.r.
 00000060: 6500 a007 a100 0100 6401 5300 6401 5300  e.......d.S.d.S.
 00000070: 2906 e900 0000 004e 2902 da0a 7061 7261  )......N)...para
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_parser.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1015 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 f703 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 f703 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6500 6a04 8303 5a05 4700 6405  ..d.e.j...Z.G.d.
 00000060: 6406 8400 6406 6501 6a06 8303 5a07 6508  d...d.e.j...Z.e.
 00000070: 6407 6b02 722a 6501 a009 a100 0100 6401  d.k.r*e.......d.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_plugin_interfaces.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_plugin_interfaces.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2036 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 f407 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 f407 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6500 6a03  ..G.d.d...d.e.j.
 00000050: 8303 5a04 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000060: 2901 da11 706c 7567 696e 5f69 6e74 6572  )...plugin_inter
 00000070: 6661 6365 7363 0000 0000 0000 0000 0000  facesc..........
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_references.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_references.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 832 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4003 0000  o.......i&.b@...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4003 0000  o.......nKec@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6501 6a04  ..G.d.d...d.e.j.
 00000050: 8303 5a05 6506 6405 6b02 721d 6501 a007  ..Z.e.d.k.r.e...
 00000060: a100 0100 6401 5300 6401 5300 2906 e900  ....d.S.d.S.)...
 00000070: 0000 004e 2901 da0a 7265 6665 7265 6e63  ...N)...referenc
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_result.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_result.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1908 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 7407 0000  o.......i&.bt...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 7407 0000  o.......nKect...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 5a03 6401 5a04 4700 6404 6405  ..d.Z.d.Z.G.d.d.
 00000050: 8400 6405 6500 6a05 8303 5a06 6507 6406  ..d.e.j...Z.e.d.
 00000060: 6b02 7221 6500 a008 a100 0100 6401 5300  k.r!e.......d.S.
 00000070: 6401 5300 2907 e900 0000 004e 2901 da06  d.S.)......N)...
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_runner_asset.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_runner_asset.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2828 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 0c0b 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 0c0b 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6500 6a07 8303 5a08 4700 6407  ..d.e.j...Z.G.d.
 00000070: 6408 8400 6408 6500 6a07 8303 5a09 650a  d...d.e.j...Z.e.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_runner_package.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_runner_package.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 6966 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 361b 0000  o.......i&.b6...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 361b 0000  o.......nKec6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6500 6a07 8303 5a08 4700 6407  ..d.e.j...Z.G.d.
 00000070: 6408 8400 6408 6500 6a07 8303 5a09 650a  d...d.e.j...Z.e.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_runner_sysinfo.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_runner_sysinfo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2204 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 9c08 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 9c08 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6501 6a08  ..G.d.d...d.e.j.
 00000070: 8303 5a09 6401 5300 2907 e900 0000 004e  ..Z.d.S.)......N
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_caveats.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_caveats.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 741 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 e502 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 e502 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6404 6405 8400 6405 6503 6a08 8303 5a09  d.d...d.e.j...Z.
 00000070: 6401 5300 2906 e900 0000 004e 2901 da12  d.S.)......N)...
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_core.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_core.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 10254 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 0e28 0000  o.......i&.b.(..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 0e28 0000  o.......nKec.(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 6d08 5a08 0100 6400 6404 6c09  m.Z.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_docstring.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_docstring.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 6611 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 d319 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 d319 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 4700 6403 6404 8400 6404 6500 6a07  ..G.d.d...d.e.j.
 00000060: 8303 5a08 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2905 da16 444f 4353 5452 494e 475f 4449  )...DOCSTRING_DI
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_imported.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_imported.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 8371 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 b320 0000  o.......i&.b. ..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 b320 0000  o.......nKec. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6501 6a04 8303 5a05 4700 6405  ..d.e.j...Z.G.d.
 00000060: 6406 8400 6406 6501 6a04 8303 5a06 4700  d...d.e.j...Z.G.
 00000070: 6407 6408 8400 6408 6501 6a04 8303 5a07  d.d...d.e.j...Z.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_module.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_module.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 3106 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 220c 0000  o.......i&.b"...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 220c 0000  o.......nKec"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000070: 8400 6406 6502 6a09 8303 5a0a 4700 6407  ..d.e.j...Z.G.d.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_safeloader_utils.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_safeloader_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1293 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 0d05 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 0d05 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 4700 6403 6404 8400 6404 6502 6a05  ..G.d.d...d.e.j.
 00000060: 8303 5a06 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da17 6765 745f 7374 6174 656d 656e  )...get_statemen
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_settings.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_settings.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 6537 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 8919 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 8919 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6404 5a08 4700 6405 6406  m.Z...d.Z.G.d.d.
 00000070: 8400 6406 6507 8303 5a09 4700 6407 6408  ..d.e...Z.G.d.d.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_status_repo.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_status_repo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 7883 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 cb1e 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 cb1e 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 4700 6403 6404  m.Z.m.Z...G.d.d.
 00000050: 8400 6404 6501 8303 5a05 6405 5300 2906  ..d.e...Z.d.S.).
 00000060: e900 0000 0029 01da 0854 6573 7443 6173  .....)...TestCas
 00000070: 6529 02da 0472 6570 6fda 0575 7469 6c73  e)...repo..utils
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_status_utils.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_status_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 617 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 6902 0000  o.......i&.bi...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 6902 0000  o.......nKeci...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6501 8303 5a04 6405 5300 2906 e900 0000  e...Z.d.S.).....
 00000060: 0029 01da 0854 6573 7443 6173 6529 01da  .)...TestCase)..
 00000070: 0575 7469 6c73 6300 0000 0000 0000 0000  .utilsc.........
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_suite.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_suite.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2882 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 420b 0000  o.......i&.bB...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 420b 0000  o.......nKecB...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 6509 8300 0100 4700 6405  m.Z...e.....G.d.
 00000070: 6406 8400 6406 6502 6a0b 8303 5a0c 650d  d...d.e.j...Z.e.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_sysinfo.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_sysinfo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 3248 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 b00c 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 b00c 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6402 6c05 6d04 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6403 6c07 6d08 5a08 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000070: 8400 6405 6502 6a09 8303 5a0a 650b 6406  ..d.e.j...Z.e.d.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_tags.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_tags.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 13253 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 c533 0000  o.......i&.b.3..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 c533 0000  o.......nKec.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 aa00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 6d06 5a06 0100 6400 6404 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6500 6a09 6500 6a0a 4200  m.Z...e.j.e.j.B.
 00000070: 6500 6a0b 4200 6500 6a0c 4200 6500 6a0d  e.j.B.e.j.B.e.j.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_tap.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_tap.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 12312 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 1830 0000  o.......i&.b.0..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 1830 0000  o.......nKec.0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 4700  d.l.m.Z.m.Z...G.
 00000050: 6403 6404 8400 6404 6501 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6507 6405 6b02 7223 6501 a008 a100 0100  e.d.k.r#e.......
 00000070: 6401 5300 6401 5300 2906 e900 0000 004e  d.S.d.S.)......N
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_task_runtime.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_task_runtime.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 3740 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 9c0e 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 9c0e 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_test.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_test.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 6667 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 0b1a 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 0b1a 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 0100 6400 6405 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 650b 8300 0100  m.Z.m.Z...e.....
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_test_id.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_test_id.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 3605 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 150e 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 150e 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6500 6a06  ..G.d.d...d.e.j.
 00000060: 8303 5a07 6508 6406 6b02 7225 6500 a009  ..Z.e.d.k.r%e...
 00000070: a100 0100 6401 5300 6401 5300 2907 e900  ....d.S.d.S.)...
```

### Comparing `avocado-framework-98.0/selftests/unit/__pycache__/test_tree.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/__pycache__/test_tree.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2638 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4e0a 0000  o.......i&.bN...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4e0a 0000  o.......nKecN...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6500 6a03  ..G.d.d...d.e.j.
 00000050: 8303 5a04 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000060: 2901 da04 7472 6565 6300 0000 0000 0000  )...treec.......
 00000070: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
```

### Comparing `avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_assets.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_assets.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 10006 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 1627 0000  o.......i&.b.'..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 1627 0000  o.......nKec.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6502 6a08 8303 5a09  d.d...d.e.j...Z.
 00000070: 6407 5a0a 6408 5a0b 4700 6409 640a 8400  d.Z.d.Z.G.d.d...
```

### Comparing `avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_jsonresult.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_jsonresult.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 4168 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4810 0000  o.......i&.bH...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4810 0000  o.......nKecH...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_resolver.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_resolver.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 6830 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 ae1a 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 ae1a 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6501  ..d.d.l.m.Z...e.
```

### Comparing `avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_spawner.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_spawner.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2089 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 2908 0000  o.......i&.b)...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 2908 0000  o.......nKec)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
```

### Comparing `avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_vmimage.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_vmimage.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 8483 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 2321 0000  o.......i&.b#!..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 2321 0000  o.......nKec#!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c08 6d09 5a0a 0100 6400 6404 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d09 5a0c 0100 6400 6405 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/unit/plugin/__pycache__/test_xunit.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/plugin/__pycache__/test_xunit.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 5858 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 e216 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 e216 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/unit/plugin/test_assets.py` & `avocado-framework-99.0/selftests/unit/plugin/test_assets.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/plugin/test_jsonresult.py` & `avocado-framework-99.0/selftests/unit/plugin/test_jsonresult.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/plugin/test_resolver.py` & `avocado-framework-99.0/selftests/unit/plugin/test_resolver.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/plugin/test_spawner.py` & `avocado-framework-99.0/selftests/unit/plugin/test_spawner.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/plugin/test_vmimage.py` & `avocado-framework-99.0/selftests/unit/plugin/test_vmimage.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/plugin/test_xunit.py` & `avocado-framework-99.0/selftests/unit/plugin/test_xunit.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_datadir.py` & `avocado-framework-99.0/selftests/unit/test_datadir.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_dependencies_resolver.py` & `avocado-framework-99.0/selftests/unit/test_dependencies_resolver.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_dispatcher.py` & `avocado-framework-99.0/selftests/unit/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_hintfiles.py` & `avocado-framework-99.0/selftests/unit/test_hintfiles.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_job.py` & `avocado-framework-99.0/selftests/unit/test_job.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_loader.py` & `avocado-framework-99.0/selftests/unit/test_loader.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_nrunner.py` & `avocado-framework-99.0/selftests/unit/test_nrunner.py`

 * *Files 4% similar despite different names*

```diff
@@ -266,14 +266,77 @@
         self.assertEqual(stderr_result["type"], "stderr")
         self.assertEqual(stderr_result["log"], b"")
         self.assertEqual(last_result["status"], "finished")
         self.assertEqual(last_result["result"], "fail")
         self.assertEqual(last_result["returncode"], 1)
         self.assertIn("time", last_result)
 
+    def test_runner_python_unittest_ok(self):
+        runnable = Runnable(
+            "python-unittest", "selftests/.data/unittests.py:First.test_pass"
+        )
+        runner_klass = runnable.pick_runner_class()
+        runner = runner_klass()
+        results = [status for status in runner.run(runnable)]
+        output1 = (
+            b"----------------------------------------------------------------------\n"
+            b"Ran 1 test in "
+        )
+        output2 = b"s\n\nOK\n"
+        output = results[-2]
+        result = results[-1]
+        self.assertEqual(result["status"], "finished")
+        self.assertEqual(result["result"], "pass")
+        self.assertTrue(output["log"].startswith(output1), "Start of output differs")
+        self.assertTrue(output["log"].endswith(output2), "End of output differs")
+
+    def test_runner_python_unittest_fail(self):
+        runnable = Runnable(
+            "python-unittest", "selftests/.data/unittests.py:Second.test_fail"
+        )
+        runner_klass = runnable.pick_runner_class()
+        runner = runner_klass()
+        results = [status for status in runner.run(runnable)]
+        if sys.version_info < (3, 11):
+            output1 = (
+                b"======================================================================\n"
+                b"FAIL: test_fail (unittests.Second)\n"
+            )
+        else:
+            output1 = (
+                b"======================================================================\n"
+                b"FAIL: test_fail (unittests.Second.test_fail)\n"
+            )
+        output2 = b"\n\nFAILED (failures=1)\n"
+        output = results[-2]
+        result = results[-1]
+        self.assertEqual(result["status"], "finished")
+        self.assertEqual(result["result"], "fail")
+        self.assertTrue(output["log"].startswith(output1), "Start of output differs")
+        self.assertTrue(output["log"].endswith(output2), "End of output differs")
+
+    def test_runner_python_unittest_skip(self):
+        runnable = Runnable(
+            "python-unittest", "selftests/.data/unittests.py:Second.test_skip"
+        )
+        runner_klass = runnable.pick_runner_class()
+        runner = runner_klass()
+        results = [status for status in runner.run(runnable)]
+        output1 = (
+            b"----------------------------------------------------------------------\n"
+            b"Ran 1 test in "
+        )
+        output2 = b"s\n\nOK (skipped=1)\n"
+        output = results[-2]
+        result = results[-1]
+        self.assertEqual(result["status"], "finished")
+        self.assertEqual(result["result"], "skip")
+        self.assertTrue(output["log"].startswith(output1), "Start of output differs")
+        self.assertTrue(output["log"].endswith(output2), "End of output differs")
+
     def test_runner_python_unittest_error(self):
         runnable = Runnable("python-unittest", "error")
         runner_klass = runnable.pick_runner_class()
         runner = runner_klass()
         results = [status for status in runner.run(runnable)]
         output = "Invalid URI: could not be converted to an unittest dotted name."
         result = results[-1]
```

### Comparing `avocado-framework-98.0/selftests/unit/test_output.py` & `avocado-framework-99.0/selftests/unit/test_output.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_parameters.py` & `avocado-framework-99.0/selftests/unit/test_parameters.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_parser.py` & `avocado-framework-99.0/selftests/unit/test_parser.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_plugin_interfaces.py` & `avocado-framework-99.0/selftests/unit/test_plugin_interfaces.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_references.py` & `avocado-framework-99.0/selftests/unit/test_references.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_result.py` & `avocado-framework-99.0/selftests/unit/test_result.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_runner_asset.py` & `avocado-framework-99.0/selftests/unit/test_runner_asset.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_runner_package.py` & `avocado-framework-99.0/selftests/unit/test_runner_package.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_runner_sysinfo.py` & `avocado-framework-99.0/selftests/unit/test_runner_sysinfo.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_safeloader_caveats.py` & `avocado-framework-99.0/selftests/unit/test_safeloader_caveats.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_safeloader_core.py` & `avocado-framework-99.0/selftests/unit/test_safeloader_core.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_safeloader_docstring.py` & `avocado-framework-99.0/selftests/unit/test_safeloader_docstring.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_safeloader_imported.py` & `avocado-framework-99.0/selftests/unit/test_safeloader_imported.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_safeloader_module.py` & `avocado-framework-99.0/selftests/unit/test_safeloader_module.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_safeloader_utils.py` & `avocado-framework-99.0/selftests/unit/test_safeloader_utils.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_settings.py` & `avocado-framework-99.0/selftests/unit/test_settings.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_status_repo.py` & `avocado-framework-99.0/selftests/unit/test_status_repo.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_status_utils.py` & `avocado-framework-99.0/selftests/unit/test_status_utils.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_suite.py` & `avocado-framework-99.0/selftests/unit/test_suite.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_sysinfo.py` & `avocado-framework-99.0/selftests/unit/test_sysinfo.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_tags.py` & `avocado-framework-99.0/selftests/unit/test_tags.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_tap.py` & `avocado-framework-99.0/selftests/unit/test_tap.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_task_runtime.py` & `avocado-framework-99.0/selftests/unit/test_task_runtime.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_test.py` & `avocado-framework-99.0/selftests/unit/test_test.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_test_id.py` & `avocado-framework-99.0/selftests/unit/test_test_id.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/test_tree.py` & `avocado-framework-99.0/selftests/unit/test_tree.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_ar.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_ar.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1398 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 7605 0000  o.......i&.bv...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 7605 0000  o.......nKecv...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6501 6a06 8303 5a07 6401 5300 2906 e900  e.j...Z.d.S.)...
 00000070: 0000 004e 2901 da02 6172 2901 da07 4241  ...N)...ar)...BA
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_archive.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_archive.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 8992 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 2023 0000  o.......i&.b #..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 2023 0000  o.......nKec #..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_astring.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_astring.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 6348 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 cc18 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 cc18 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 4700  d.l.m.Z.m.Z...G.
 00000050: 6403 6404 8400 6404 6501 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6507 6405 6b02 7223 6501 a008 a100 0100  e.d.k.r#e.......
 00000070: 6401 5300 6401 5300 2906 e900 0000 004e  d.S.d.S.)......N
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_cloudinit.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_cloudinit.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2827 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 0b0b 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 0b0b 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a06 6400 6402 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6403 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 650c 8300 0100  m.Z.m.Z...e.....
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_cpu.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_cpu.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 10232 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 f827 0000  o.......i&.b.'..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 f827 0000  o.......nKec.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6504 8303 5a07 6508 6406 6b02 7226 6502  e...Z.e.d.k.r&e.
 00000070: a009 a100 0100 6401 5300 6401 5300 2907  ......d.S.d.S.).
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_data_structures.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_data_structures.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 5193 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 4914 0000  o.......i&.bI...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 4914 0000  o.......nKecI...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6500 6a03  ..G.d.d...d.e.j.
 00000050: 8303 5a04 4700 6405 6406 8400 6406 6500  ..Z.G.d.d...d.e.
 00000060: 6a03 8303 5a05 6506 6407 6b02 7226 6500  j...Z.e.d.k.r&e.
 00000070: a007 a100 0100 6401 5300 6401 5300 2908  ......d.S.d.S.).
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_datadrainer.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_datadrainer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2448 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 9009 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 9009 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 4700 6403 6404 8400 6404 6502 6a05  ..G.d.d...d.e.j.
 00000060: 8303 5a06 4700 6405 6406 8400 6406 6504  ..Z.G.d.d...d.e.
 00000070: 6a07 8303 5a08 4700 6407 6408 8400 6408  j...Z.G.d.d...d.
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_diff_validator.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_diff_validator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 5752 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 7816 0000  o.......i&.bx...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 7816 0000  o.......nKecx...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6404 6405 8400 6405 6502 6a07 8303 5a08  d.d...d.e.j...Z.
 00000070: 6509 6406 6b02 722b 6502 a00a a100 0100  e.d.k.r+e.......
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_disk.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_disk.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2870 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 360b 0000  o.......i&.b6...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 360b 0000  o.......nKec6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6403 5a05 6404 5a06 6405  m.Z...d.Z.d.Z.d.
 00000050: 5a07 4700 6406 6407 8400 6407 6501 6a08  Z.G.d.d...d.e.j.
 00000060: 8303 5a09 650a 6408 6b02 7225 6501 a00b  ..Z.e.d.k.r%e...
 00000070: a100 0100 6401 5300 6401 5300 2909 e900  ....d.S.d.S.)...
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_distro.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_distro.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2261 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 d508 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 d508 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6502 6a05 8303 5a06 6507 6405  ..d.e.j...Z.e.d.
 00000060: 6b02 7221 6502 a008 a100 0100 6401 5300  k.r!e.......d.S.
 00000070: 6401 5300 2906 e900 0000 004e 2901 da06  d.S.)......N)...
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_filelock.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_filelock.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1185 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 a104 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 a104 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6404 6405 8400 6405 6502 6a08  ..G.d.d...d.e.j.
 00000070: 8303 5a09 650a 6406 6b02 722d 6502 a00b  ..Z.e.d.k.r-e...
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_gdb.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_gdb.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1220 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 c404 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 c404 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6500 6a04 8303 5a05 6506 6405 6b02 721f  e.j...Z.e.d.k.r.
 00000060: 6500 a007 a100 0100 6401 5300 6401 5300  e.......d.S.d.S.
 00000070: 2906 e900 0000 004e 2902 da09 4744 4252  )......N)...GDBR
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_genio.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_genio.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1732 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 c406 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 c406 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6508 8300 0100 4700 6404 6405 8400  ..e.....G.d.d...
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_iso9660.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_iso9660.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 6328 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 b818 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 7816 0000  o.......nKecx...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a04 6401 6403 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 0100 650a  d.l.m.Z.m.Z...e.
 00000070: 8300 0100 4700 6405 6406 8400 6406 6504  ....G.d.d...d.e.
@@ -119,296 +119,274 @@
 00000760: 6c6e 616d 655f 5f72 1500 0000 da08 756e  lname__r......un
 00000770: 6974 7465 7374 5a04 6d6f 636b da05 7061  ittestZ.mock..pa
 00000780: 7463 6872 2000 0000 7222 0000 0072 2400  tchr ...r"...r$.
 00000790: 0000 7213 0000 0072 1300 0000 7213 0000  ..r....r....r...
 000007a0: 0072 1400 0000 7207 0000 000e 0000 0073  .r....r........s
 000007b0: 1400 0000 0800 0801 0e0a 0a01 0e05 0e01  ................
 000007c0: 0e01 0e01 1001 0c0d 7207 0000 0063 0000  ........r....c..
-000007d0: 0000 0000 0000 0000 0000 0000 0000 0700  ................
-000007e0: 0000 4000 0000 738e 0000 0065 005a 0164  ..@...s....e.Z.d
-000007f0: 005a 0264 015a 0364 0264 0384 005a 0465  .Z.d.Z.d.d...Z.e
-00000800: 05a0 0665 07a0 08a1 0064 0419 0064 056b  ...e.....d...d.k
-00000810: 0264 06a1 0264 0764 0884 0083 015a 0965  .d...d.d.....Z.e
-00000820: 05a0 0665 0aa0 0b64 09a1 010c 0064 0aa1  ...e...d.....d..
-00000830: 0265 05a0 0c65 0aa0 0d64 0ba1 0164 0ca1  .e...e...d...d..
-00000840: 0265 05a0 0665 07a0 0e64 0da1 016f 3865  .e...e...d...o8e
-00000850: 07a0 0e64 0ea1 0164 0f76 0064 10a1 0264  ...d...d.v.d...d
-00000860: 1164 1284 0083 0183 0183 015a 0f64 1364  .d.........Z.d.d
-00000870: 1484 005a 1064 1553 0029 16da 0b42 6173  ...Z.d.S.)...Bas
-00000880: 6549 736f 3936 3630 7a4e 0a20 2020 2042  eIso9660zN.    B
-00000890: 6173 6520 636c 6173 7320 6465 6669 6e69  ase class defini
-000008a0: 6e67 2073 6574 7570 2061 6e64 2074 6573  ng setup and tes
-000008b0: 7473 2066 6f72 2073 6861 7265 6420 4973  ts for shared Is
-000008c0: 6f39 3636 3020 6675 6e63 7469 6f6e 616c  o9660 functional
-000008d0: 6974 790a 2020 2020 6301 0000 0000 0000  ity.    c.......
-000008e0: 0000 0000 0002 0000 0009 0000 0043 0000  .............C..
-000008f0: 0073 5000 0000 7400 6a01 a002 7400 6a01  .sP...t.j...t.j.
-00000900: a003 7400 6a01 a004 7400 6a01 a004 7405  ..t.j...t.j...t.
-00000910: a101 a101 7400 6a01 6a06 6401 6402 a104  ....t.j.j.d.d...
-00000920: a101 7c00 5f07 6400 7c00 5f08 7409 7c00  ..|._.d.|._.t.|.
-00000930: 8301 7d01 740a 6a0b 7c01 6403 8d01 7c00  ..}.t.j.|.d...|.
-00000940: 5f0c 6400 5300 2904 4e72 0800 0000 7209  _.d.S.).Nr....r.
-00000950: 0000 0029 01da 0670 7265 6669 7829 0d72  ...)...prefix).r
-00000960: 0a00 0000 7203 0000 0072 0b00 0000 720c  ....r....r....r.
-00000970: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
-00000980: 0000 7210 0000 00da 0369 736f 7206 0000  ..r......isor...
-00000990: 00da 0874 656d 7066 696c 65da 1254 656d  ...tempfile..Tem
-000009a0: 706f 7261 7279 4469 7265 6374 6f72 79da  poraryDirectory.
-000009b0: 0674 6d70 6469 7229 0272 1200 0000 722b  .tmpdir).r....r+
-000009c0: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-000009d0: 0000 7215 0000 003c 0000 0073 1600 0000  ..r....<...s....
-000009e0: 0601 0601 1201 0601 0201 0201 02fc 06ff  ................
-000009f0: 0608 0801 1201 7a11 4261 7365 4973 6f39  ......z.BaseIso9
-00000a00: 3636 302e 7365 7455 70e9 0400 0000 da05  660.setUp.......
-00000a10: 7333 3930 787a 5145 6e64 6961 6e65 7373  s390xzQEndianess
-00000a20: 2069 7373 7565 7320 6f6e 2070 7963 646c   issues on pycdl
-00000a30: 6962 2c20 7365 6520 6874 7470 733a 2f2f  ib, see https://
-00000a40: 6769 7468 7562 2e63 6f6d 2f63 6c61 6c61  github.com/clala
-00000a50: 6e63 6574 7465 2f70 7963 646c 6962 2f69  ncette/pycdlib/i
-00000a60: 7373 7565 732f 3339 6301 0000 0000 0000  ssues/39c.......
-00000a70: 0000 0000 0002 0000 0006 0000 0043 0000  .............C..
-00000a80: 0073 6e00 0000 7c00 a000 7c00 6a01 a002  .sn...|...|.j...
-00000a90: 6401 a101 6402 a102 0100 7403 6a04 a005  d...d.....t.j...
-00000aa0: 7c00 6a06 6a07 6401 a102 7d01 7c00 6a01  |.j.j.d...}.|.j.
-00000ab0: a008 7403 6a04 a005 6403 6404 a102 7c01  ..t.j...d.d...|.
-00000ac0: a102 0100 7c00 a000 7409 7c01 6405 6406  ....|...t.|.d.d.
-00000ad0: 8d02 a002 a100 6407 a102 0100 7c00 6a01  ......d.....|.j.
-00000ae0: a00a a100 0100 7c00 6a01 a00a a100 0100  ......|.j.......
-00000af0: 6408 5300 2909 7a32 0a20 2020 2020 2020  d.S.).z2.       
-00000b00: 2043 6865 636b 2074 6865 2062 6173 6963   Check the basic
-00000b10: 2049 736f 3936 3630 2077 6f72 6b66 6c6f   Iso9660 workflo
-00000b20: 770a 2020 2020 2020 2020 da04 6669 6c65  w.        ..file
-00000b30: f30d 0000 0066 696c 6520 636f 6e74 656e  .....file conten
-00000b40: 740a da03 4469 72da 0b69 6e5f 6469 725f  t...Dir..in_dir_
-00000b50: 6669 6c65 7a05 7574 662d 3829 01da 0865  filez.utf-8)...e
-00000b60: 6e63 6f64 696e 677a 1763 6f6e 7465 6e74  ncodingz.content
-00000b70: 206f 6620 696e 2d64 6972 2d66 696c 650a   of in-dir-file.
-00000b80: 4e29 0bda 0b61 7373 6572 7445 7175 616c  N)...assertEqual
-00000b90: 722c 0000 0072 1700 0000 720a 0000 0072  r,...r....r....r
-00000ba0: 0300 0000 720c 0000 0072 2f00 0000 da04  ....r....r/.....
-00000bb0: 6e61 6d65 da04 636f 7079 da04 6f70 656e  name..copy..open
-00000bc0: da05 636c 6f73 6529 0272 1200 0000 da03  ..close).r......
-00000bd0: 6473 7472 1300 0000 7213 0000 0072 1400  dstr....r....r..
-00000be0: 0000 da13 7465 7374 5f62 6173 6963 5f77  ....test_basic_w
-00000bf0: 6f72 6b66 6c6f 7749 0000 0073 0c00 0000  orkflowI...s....
-00000c00: 140b 1201 1801 1801 0a01 0e01 7a1f 4261  ............z.Ba
-00000c10: 7365 4973 6f39 3636 302e 7465 7374 5f62  seIso9660.test_b
-00000c20: 6173 6963 5f77 6f72 6b66 6c6f 77da 056d  asic_workflow..m
-00000c30: 6f75 6e74 7a32 5468 6973 2074 6573 7420  ountz2This test 
-00000c40: 7265 7175 6972 6573 206d 6f75 6e74 2074  requires mount t
-00000c50: 6f20 7275 6e20 756e 6465 7220 7375 646f  o run under sudo
-00000c60: 206f 7220 726f 6f74 da0d 6361 705f 7379   or root..cap_sy
-00000c70: 735f 6164 6d69 6efa 2f43 6170 6162 696c  s_admin./Capabil
-00000c80: 6974 7920 746f 206d 6f75 6e74 2069 7320  ity to mount is 
-00000c90: 7265 7175 6972 6564 2028 6361 705f 7379  required (cap_sy
-00000ca0: 735f 6164 6d69 6e29 da06 5452 4156 4953  s_admin)..TRAVIS
-00000cb0: da0f 5452 4156 4953 5f43 5055 5f41 5243  ..TRAVIS_CPU_ARC
-00000cc0: 48a9 03da 0561 726d 3634 da07 7070 6336  H....arm64..ppc6
-00000cd0: 346c 6572 3100 0000 fa30 5452 4156 4953  4ler1....0TRAVIS
-00000ce0: 2045 6e76 6972 6f6e 6d65 6e74 2069 7320   Environment is 
-00000cf0: 756e 7375 6974 6162 6c65 2066 6f72 2074  unsuitable for t
-00000d00: 6865 7365 2074 6573 7473 6301 0000 0000  hese testsc.....
-00000d10: 0000 0000 0000 0004 0000 0008 0000 0043  ...............C
-00000d20: 0000 0073 9800 0000 7c00 6a00 6a01 7d01  ...s....|.j.j.}.
-00000d30: 7402 6a03 a004 7c01 6401 a102 7d02 7c00  t.j...|.d...}.|.
-00000d40: a005 7402 6a03 a006 7c02 a101 a101 0100  ..t.j...|.......
-00000d50: 7c00 a007 7408 7409 7402 6a03 a004 7c01  |...t.t.t.j...|.
-00000d60: 6402 a102 6403 8302 a00a a100 8301 6404  d...d.........d.
-00000d70: a102 0100 7402 6a03 a004 7c01 6401 6405  ....t.j...|.d.d.
-00000d80: a103 7d03 7c00 a007 7408 7409 7c03 6403  ..}.|...t.t.|.d.
-00000d90: 8302 a00a a100 8301 6406 a102 0100 7c00  ........d.....|.
-00000da0: 6a00 a00b a100 0100 7c00 a00c 7402 6a03  j.......|...t.j.
-00000db0: a00d 7c01 a101 6407 a102 0100 6408 5300  ..|...d.....d.S.
-00000dc0: 2909 7a31 0a20 2020 2020 2020 2043 6865  ).z1.        Che
-00000dd0: 636b 2074 6865 206d 6e74 5f64 6972 2066  ck the mnt_dir f
-00000de0: 756e 6374 696f 6e61 6c69 7479 0a20 2020  unctionality.   
-00000df0: 2020 2020 2072 3400 0000 7232 0000 00da       r4...r2....
-00000e00: 0272 6272 3300 0000 7235 0000 0073 1700  .rbr3...r5...s..
-00000e10: 0000 636f 6e74 656e 7420 6f66 2069 6e2d  ..content of in-
-00000e20: 6469 722d 6669 6c65 0a7a 3874 6865 206d  dir-file.z8the m
-00000e30: 6e74 5f64 6972 2069 7320 7375 7070 6f73  nt_dir is suppos
-00000e40: 6520 746f 2062 6520 6465 7374 726f 7965  e to be destroye
-00000e50: 6420 6166 7465 7220 6973 6f2e 636c 6f73  d after iso.clos
-00000e60: 6528 294e 290e 722c 0000 005a 076d 6e74  e()N).r,...Z.mnt
-00000e70: 5f64 6972 720a 0000 0072 0300 0000 720c  _dirr....r....r.
-00000e80: 0000 0072 1c00 0000 da05 6973 6469 7272  ...r......isdirr
-00000e90: 3700 0000 da05 6279 7465 7372 3a00 0000  7.....bytesr:...
-00000ea0: 7217 0000 0072 3b00 0000 da0b 6173 7365  r....r;.....asse
-00000eb0: 7274 4661 6c73 65da 0665 7869 7374 7329  rtFalse..exists)
-00000ec0: 0472 1200 0000 da04 6261 7365 da08 6469  .r......base..di
-00000ed0: 725f 7061 7468 5a10 696e 5f64 6972 5f66  r_pathZ.in_dir_f
-00000ee0: 696c 655f 7061 7468 7213 0000 0072 1300  ile_pathr....r..
-00000ef0: 0000 7214 0000 00da 1574 6573 745f 6d6e  ..r......test_mn
-00000f00: 745f 6469 725f 776f 726b 666c 6f77 5b00  t_dir_workflow[.
-00000f10: 0000 731e 0000 0008 110e 0112 0104 011c  ..s.............
-00000f20: 0104 ff10 0304 0112 0104 ff0a 0304 010a  ................
-00000f30: 0102 0108 fe7a 2142 6173 6549 736f 3936  .....z!BaseIso96
-00000f40: 3630 2e74 6573 745f 6d6e 745f 6469 725f  60.test_mnt_dir_
-00000f50: 776f 726b 666c 6f77 6301 0000 0000 0000  workflowc.......
-00000f60: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00000f70: 0073 2200 0000 7c00 6a00 6400 7501 720a  .s"...|.j.d.u.r.
-00000f80: 7c00 6a00 a001 a100 0100 7c00 6a02 a003  |.j.......|.j...
-00000f90: a100 0100 6400 5300 a901 4e29 0472 2c00  ....d.S...N).r,.
-00000fa0: 0000 723b 0000 0072 2f00 0000 da07 636c  ..r;...r/.....cl
-00000fb0: 6561 6e75 7072 1100 0000 7213 0000 0072  eanupr....r....r
-00000fc0: 1300 0000 7214 0000 00da 0874 6561 7244  ....r......tearD
-00000fd0: 6f77 6e7c 0000 0073 0600 0000 0a01 0a01  own|...s........
-00000fe0: 0e01 7a14 4261 7365 4973 6f39 3636 302e  ..z.BaseIso9660.
-00000ff0: 7465 6172 446f 776e 4e29 1172 2500 0000  tearDownN).r%...
-00001000: 7226 0000 0072 2700 0000 da07 5f5f 646f  r&...r'.....__do
-00001010: 635f 5f72 1500 0000 7228 0000 00da 0673  c__r....r(.....s
-00001020: 6b69 7049 6672 0a00 0000 da05 756e 616d  kipIfr......unam
-00001030: 6572 3d00 0000 7204 0000 00da 0863 616e  er=...r......can
-00001040: 5f73 7564 6fda 0a73 6b69 7055 6e6c 6573  _sudo..skipUnles
-00001050: 73da 0e68 6173 5f63 6170 6162 696c 6974  s..has_capabilit
-00001060: 79da 0667 6574 656e 7672 4e00 0000 7251  y..getenvrN...rQ
-00001070: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
-00001080: 0000 7214 0000 0072 2a00 0000 3600 0000  ..r....r*...6...
-00001090: 732e 0000 0008 0004 0208 0404 0d0e 0102  s...............
-000010a0: 0202 fd0a 0704 0b0a 0102 0102 fe04 0408  ................
-000010b0: 0102 0102 fe04 040a 010c 0102 0102 fd0e  ................
-000010c0: 050c 1472 2a00 0000 6300 0000 0000 0000  ...r*...c.......
-000010d0: 0000 0000 0000 0000 0006 0000 0000 0000  ................
-000010e0: 00f3 3600 0000 6500 5a01 6400 5a02 6401  ..6...e.Z.d.Z.d.
-000010f0: 5a03 6504 a005 6506 6a07 6402 6403 6404  Z.e...e.j.d.d.d.
-00001100: 8d02 6405 a102 8700 6601 6406 6407 8408  ..d.....f.d.d...
-00001110: 8301 5a08 8700 0400 5a09 5300 2908 da07  ..Z.....Z.S.)...
-00001120: 4973 6f49 6e66 6f7a 1d0a 2020 2020 4973  IsoInfoz..    Is
-00001130: 6f49 6e66 6f2d 6261 7365 6420 6368 6563  oInfo-based chec
-00001140: 6b0a 2020 2020 5a07 6973 6f69 6e66 6f46  k.    Z.isoinfoF
-00001150: a901 da07 6465 6661 756c 747a 1669 736f  ....defaultz.iso
-00001160: 696e 666f 206e 6f74 2069 6e73 7461 6c6c  info not install
-00001170: 6564 2e63 0100 0000 0000 0000 0000 0000  ed.c............
-00001180: 0100 0000 0300 0000 0300 0000 f31c 0000  ................
-00001190: 0074 0083 00a0 01a1 0001 0074 02a0 037c  .t.........t...|
-000011a0: 006a 04a1 017c 005f 0564 0053 0072 4f00  .j...|._.d.S.rO.
-000011b0: 0000 2906 da05 7375 7065 7272 1500 0000  ..)...superr....
-000011c0: 7202 0000 005a 0e49 736f 3936 3630 4973  r....Z.Iso9660Is
-000011d0: 6f49 6e66 6f72 1000 0000 722c 0000 0072  oInfor....r,...r
-000011e0: 1100 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
-000011f0: 5f72 1300 0000 7214 0000 0072 1500 0000  _r....r....r....
-00001200: 8800 0000 f304 0000 000a 0412 017a 0d49  .............z.I
-00001210: 736f 496e 666f 2e73 6574 5570 a90a 7225  soInfo.setUp..r%
-00001220: 0000 0072 2600 0000 7227 0000 0072 5200  ...r&...r'...rR.
-00001230: 0000 7228 0000 0072 5600 0000 7203 0000  ..r(...rV...r...
-00001240: 00da 0c66 696e 645f 636f 6d6d 616e 6472  ...find_commandr
-00001250: 1500 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
-00001260: 6c5f 5f72 1300 0000 7213 0000 0072 5f00  l__r....r....r_.
-00001270: 0000 7214 0000 0072 5a00 0000 8200 0000  ..r....rZ.......
-00001280: f30c 0000 0008 0004 0204 040e 0102 ff16  ................
-00001290: 0372 5a00 0000 6300 0000 0000 0000 0000  .rZ...c.........
-000012a0: 0000 0000 0000 0006 0000 0000 0000 0072  ...............r
-000012b0: 5900 0000 2908 da07 4973 6f52 6561 647a  Y...)...IsoReadz
-000012c0: 1d0a 2020 2020 4973 6f52 6561 642d 6261  ..    IsoRead-ba
-000012d0: 7365 6420 6368 6563 6b0a 2020 2020 7a08  sed check.    z.
-000012e0: 6973 6f2d 7265 6164 4672 5b00 0000 7a17  iso-readFr[...z.
-000012f0: 6973 6f2d 7265 6164 206e 6f74 2069 6e73  iso-read not ins
-00001300: 7461 6c6c 6564 2e63 0100 0000 0000 0000  talled.c........
-00001310: 0000 0000 0100 0000 0300 0000 0300 0000  ................
-00001320: 725d 0000 0072 4f00 0000 2906 725e 0000  r]...rO...).r^..
-00001330: 0072 1500 0000 7202 0000 005a 0e49 736f  .r....r....Z.Iso
-00001340: 3936 3630 4973 6f52 6561 6472 1000 0000  9660IsoReadr....
-00001350: 722c 0000 0072 1100 0000 725f 0000 0072  r,...r....r_...r
-00001360: 1300 0000 7214 0000 0072 1500 0000 9600  ....r....r......
-00001370: 0000 7261 0000 007a 0d49 736f 5265 6164  ..ra...z.IsoRead
-00001380: 2e73 6574 5570 7262 0000 0072 1300 0000  .setUprb...r....
-00001390: 7213 0000 0072 5f00 0000 7214 0000 0072  r....r_...r....r
-000013a0: 6600 0000 9000 0000 7265 0000 0072 6600  f.......re...rf.
-000013b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000013c0: 0000 0007 0000 0000 0000 0073 6600 0000  ...........sf...
-000013d0: 6500 5a01 6400 5a02 6401 5a03 6504 a005  e.Z.d.Z.d.Z.e...
-000013e0: 6506 a007 6402 a101 0c00 6403 a102 6504  e...d.....d...e.
-000013f0: a008 6506 a009 6404 a101 6405 a102 6504  ..e...d...d...e.
-00001400: a005 650a a00b 6406 a101 6f24 650a a00b  ..e...d...o$e...
-00001410: 6407 a101 6408 7600 6409 a102 8700 6601  d...d.v.d.....f.
-00001420: 640a 640b 8408 8301 8301 8301 5a0c 8700  d.d.........Z...
-00001430: 0400 5a0d 5300 290c da08 4973 6f4d 6f75  ..Z.S.)...IsoMou
-00001440: 6e74 7a1b 0a20 2020 204d 6f75 6e74 2d62  ntz..    Mount-b
-00001450: 6173 6564 2063 6865 636b 0a20 2020 2072  ased check.    r
-00001460: 3e00 0000 7a1f 5468 6973 2074 6573 7420  >...z.This test 
-00001470: 7265 7175 6972 6573 2073 7564 6f20 6f72  requires sudo or
-00001480: 2072 6f6f 7472 3f00 0000 7240 0000 0072   rootr?...r@...r
-00001490: 4100 0000 7242 0000 0072 4300 0000 7246  A...rB...rC...rF
-000014a0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000014b0: 0100 0000 0300 0000 0300 0000 725d 0000  ............r]..
-000014c0: 0072 4f00 0000 2906 725e 0000 0072 1500  .rO...).r^...r..
-000014d0: 0000 7202 0000 005a 0c49 736f 3936 3630  ..r....Z.Iso9660
-000014e0: 4d6f 756e 7472 1000 0000 722c 0000 0072  Mountr....r,...r
-000014f0: 1100 0000 725f 0000 0072 1300 0000 7214  ....r_...r....r.
-00001500: 0000 0072 1500 0000 a400 0000 7304 0000  ...r........s...
-00001510: 000a 0b12 017a 0e49 736f 4d6f 756e 742e  .....z.IsoMount.
-00001520: 7365 7455 7029 0e72 2500 0000 7226 0000  setUp).r%...r&..
-00001530: 0072 2700 0000 7252 0000 0072 2800 0000  .r'...rR...r(...
-00001540: 7253 0000 0072 0400 0000 7255 0000 0072  rS...r....rU...r
-00001550: 5600 0000 7257 0000 0072 0a00 0000 7258  V...rW...r....rX
-00001560: 0000 0072 1500 0000 7264 0000 0072 1300  ...r....rd...r..
-00001570: 0000 7213 0000 0072 5f00 0000 7214 0000  ..r....r_...r...
-00001580: 0072 6700 0000 9e00 0000 731a 0000 0008  .rg.......s.....
-00001590: 0004 0212 0404 0108 0102 0102 fe04 040a  ................
-000015a0: 010c 0102 0102 fd1a 0572 6700 0000 6300  .........rg...c.
-000015b0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-000015c0: 0000 0000 0000 0073 3800 0000 6500 5a01  .......s8...e.Z.
-000015d0: 6400 5a02 6401 5a03 6504 a005 6506 a007  d.Z.d.Z.e...e...
-000015e0: a100 6402 a102 8700 6601 6403 6404 8408  ..d.....f.d.d...
-000015f0: 8301 5a08 6405 6406 8400 5a09 8700 0400  ..Z.d.d...Z.....
-00001600: 5a0a 5300 2907 da07 5079 4344 4c69 627a  Z.S.)...PyCDLibz
-00001610: 1d0a 2020 2020 5079 4344 4c69 622d 6261  ..    PyCDLib-ba
-00001620: 7365 6420 6368 6563 6b0a 2020 2020 7a15  sed check.    z.
-00001630: 7079 6364 6c69 6220 6e6f 7420 696e 7374  pycdlib not inst
-00001640: 616c 6c65 6463 0100 0000 0000 0000 0000  alledc..........
-00001650: 0000 0100 0000 0300 0000 0300 0000 725d  ..............r]
-00001660: 0000 0072 4f00 0000 2906 725e 0000 0072  ...rO...).r^...r
-00001670: 1500 0000 7202 0000 0072 1b00 0000 7210  ....r....r....r.
-00001680: 0000 0072 2c00 0000 7211 0000 0072 5f00  ...r,...r....r_.
-00001690: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-000016a0: 00b9 0000 0073 0400 0000 0a02 1201 7a0d  .....s........z.
-000016b0: 5079 4344 4c69 622e 7365 7455 7063 0100  PyCDLib.setUpc..
-000016c0: 0000 0000 0000 0000 0000 0600 0000 0600  ................
-000016d0: 0000 4300 0000 7378 0000 0074 006a 01a0  ..C...sx...t.j..
-000016e0: 027c 006a 036a 0464 01a1 027d 0174 05a0  .|.j.j.d...}.t..
-000016f0: 067c 01a1 017d 027c 02a0 07a1 0001 0064  .|...}.|.......d
-00001700: 027d 0364 0344 005d 237d 047c 02a0 087c  .}.d.D.]#}.|...|
-00001710: 047c 03a1 0201 007c 02a0 09a1 0001 0074  .|.....|.......t
-00001720: 05a0 067c 01a1 017d 057c 00a0 0a7c 05a0  ...|...}.|...|..
-00001730: 0b7c 04a1 017c 03a1 0201 007c 00a0 0c74  .|...|.....|...t
-00001740: 006a 01a0 0d7c 01a1 01a1 0101 0071 1664  .j...|.......q.d
-00001750: 0053 0029 044e 7a07 6e65 772e 6973 6f73  .S.).Nz.new.isos
-00001760: 0700 0000 4156 4f43 4144 4f29 045a 0652  ....AVOCADO).Z.R
-00001770: 4541 444d 457a 072f 7265 6164 6d65 7a0a  EADMEz./readmez.
-00001780: 7265 6164 6d65 2e74 7874 7a15 7175 6974  readme.txtz.quit
-00001790: 652d 6c6f 6e67 2d72 6561 646d 652e 7478  e-long-readme.tx
-000017a0: 7429 0e72 0a00 0000 7203 0000 0072 0c00  t).r....r....r..
-000017b0: 0000 722f 0000 0072 3800 0000 7202 0000  ..r/...r8...r...
-000017c0: 0072 1b00 0000 7218 0000 0072 1900 0000  .r....r....r....
-000017d0: 723b 0000 0072 3700 0000 7217 0000 0072  r;...r7...r....r
-000017e0: 1c00 0000 da06 6973 6669 6c65 2906 7212  ......isfile).r.
-000017f0: 0000 005a 0c6e 6577 5f69 736f 5f70 6174  ...Z.new_iso_pat
-00001800: 685a 076e 6577 5f69 736f da07 636f 6e74  hZ.new_iso..cont
-00001810: 656e 74da 0966 696c 655f 7061 7468 5a08  ent..file_pathZ.
-00001820: 7265 6164 5f69 736f 7213 0000 0072 1300  read_isor....r..
-00001830: 0000 7214 0000 00da 1174 6573 745f 6372  ..r......test_cr
-00001840: 6561 7465 5f77 7269 7465 be00 0000 7316  eate_write....s.
-00001850: 0000 0012 010a 0108 0104 0108 010c 0108  ................
-00001860: 010a 0112 0114 0104 fb7a 1950 7943 444c  .........z.PyCDL
-00001870: 6962 2e74 6573 745f 6372 6561 7465 5f77  ib.test_create_w
-00001880: 7269 7465 290b 7225 0000 0072 2600 0000  rite).r%...r&...
-00001890: 7227 0000 0072 5200 0000 7228 0000 0072  r'...rR...r(...r
-000018a0: 5600 0000 7202 0000 005a 0b68 6173 5f70  V...r....Z.has_p
-000018b0: 7963 646c 6962 7215 0000 0072 6c00 0000  ycdlibr....rl...
-000018c0: 7264 0000 0072 1300 0000 7213 0000 0072  rd...r....r....r
-000018d0: 5f00 0000 7214 0000 0072 6800 0000 b300  _...r....rh.....
-000018e0: 0000 730a 0000 0008 0004 020e 040e 0110  ..s.............
-000018f0: 0472 6800 0000 da08 5f5f 6d61 696e 5f5f  .rh.....__main__
-00001900: 2915 7252 0000 0072 0a00 0000 722d 0000  ).rR...r....r-..
-00001910: 005a 0d75 6e69 7474 6573 742e 6d6f 636b  .Z.unittest.mock
-00001920: 7228 0000 00da 0d61 766f 6361 646f 2e75  r(.....avocado.u
-00001930: 7469 6c73 7202 0000 0072 0300 0000 7204  tilsr....r....r.
-00001940: 0000 005a 0f73 656c 6674 6573 7473 2e75  ...Z.selftests.u
-00001950: 7469 6c73 7205 0000 0072 0600 0000 da08  tilsr....r......
-00001960: 5465 7374 4361 7365 7207 0000 0072 2a00  TestCaser....r*.
-00001970: 0000 725a 0000 0072 6600 0000 7267 0000  ..rZ...rf...rg..
-00001980: 0072 6800 0000 7225 0000 00da 046d 6169  .rh...r%.....mai
-00001990: 6e72 1300 0000 7213 0000 0072 1300 0000  nr....r....r....
-000019a0: 7214 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000019b0: 0000 0073 2000 0000 0400 0803 0801 0801  ...s ...........
-000019c0: 1402 1001 0602 1203 0e28 144c 140e 140e  .........(.L....
-000019d0: 1415 0818 0c01 04ff                      ........
+000007d0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
+000007e0: 0000 4000 0000 7356 0000 0065 005a 0164  ..@...sV...e.Z.d
+000007f0: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
+00000800: 0464 0584 005a 0565 06a0 0765 08a0 0964  .d...Z.e...e...d
+00000810: 06a1 010c 0064 07a1 0265 06a0 0a65 08a0  .....d...e...e..
+00000820: 0b64 08a1 0164 09a1 0264 0a64 0b84 0083  .d...d...d.d....
+00000830: 0183 015a 0c64 0c64 0d84 005a 0d64 0e53  ...Z.d.d...Z.d.S
+00000840: 0029 0fda 0b42 6173 6549 736f 3936 3630  .)...BaseIso9660
+00000850: 7a4e 0a20 2020 2042 6173 6520 636c 6173  zN.    Base clas
+00000860: 7320 6465 6669 6e69 6e67 2073 6574 7570  s defining setup
+00000870: 2061 6e64 2074 6573 7473 2066 6f72 2073   and tests for s
+00000880: 6861 7265 6420 4973 6f39 3636 3020 6675  hared Iso9660 fu
+00000890: 6e63 7469 6f6e 616c 6974 790a 2020 2020  nctionality.    
+000008a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000008b0: 0009 0000 0043 0000 0073 5000 0000 7400  .....C...sP...t.
+000008c0: 6a01 a002 7400 6a01 a003 7400 6a01 a004  j...t.j...t.j...
+000008d0: 7400 6a01 a004 7405 a101 a101 7400 6a01  t.j...t.....t.j.
+000008e0: 6a06 6401 6402 a104 a101 7c00 5f07 6400  j.d.d.....|._.d.
+000008f0: 7c00 5f08 7409 7c00 8301 7d01 740a 6a0b  |._.t.|...}.t.j.
+00000900: 7c01 6403 8d01 7c00 5f0c 6400 5300 2904  |.d...|._.d.S.).
+00000910: 4e72 0800 0000 7209 0000 0029 01da 0670  Nr....r....)...p
+00000920: 7265 6669 7829 0d72 0a00 0000 7203 0000  refix).r....r...
+00000930: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000940: 720e 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
+00000950: 0369 736f 7206 0000 00da 0874 656d 7066  .isor......tempf
+00000960: 696c 65da 1254 656d 706f 7261 7279 4469  ile..TemporaryDi
+00000970: 7265 6374 6f72 79da 0674 6d70 6469 7229  rectory..tmpdir)
+00000980: 0272 1200 0000 722b 0000 0072 1300 0000  .r....r+...r....
+00000990: 7213 0000 0072 1400 0000 7215 0000 003c  r....r....r....<
+000009a0: 0000 0073 1600 0000 0601 0601 1201 0601  ...s............
+000009b0: 0201 0201 02fc 06ff 0608 0801 1201 7a11  ..............z.
+000009c0: 4261 7365 4973 6f39 3636 302e 7365 7455  BaseIso9660.setU
+000009d0: 7063 0100 0000 0000 0000 0000 0000 0200  pc..............
+000009e0: 0000 0600 0000 4300 0000 736e 0000 007c  ......C...sn...|
+000009f0: 00a0 007c 006a 01a0 0264 01a1 0164 02a1  ...|.j...d...d..
+00000a00: 0201 0074 036a 04a0 057c 006a 066a 0764  ...t.j...|.j.j.d
+00000a10: 01a1 027d 017c 006a 01a0 0874 036a 04a0  ...}.|.j...t.j..
+00000a20: 0564 0364 04a1 027c 01a1 0201 007c 00a0  .d.d...|.....|..
+00000a30: 0074 097c 0164 0564 068d 02a0 02a1 0064  .t.|.d.d.......d
+00000a40: 07a1 0201 007c 006a 01a0 0aa1 0001 007c  .....|.j.......|
+00000a50: 006a 01a0 0aa1 0001 0064 0853 0029 097a  .j.......d.S.).z
+00000a60: 320a 2020 2020 2020 2020 4368 6563 6b20  2.        Check 
+00000a70: 7468 6520 6261 7369 6320 4973 6f39 3636  the basic Iso966
+00000a80: 3020 776f 726b 666c 6f77 0a20 2020 2020  0 workflow.     
+00000a90: 2020 20da 0466 696c 65f3 0d00 0000 6669     ..file.....fi
+00000aa0: 6c65 2063 6f6e 7465 6e74 0ada 0344 6972  le content...Dir
+00000ab0: da0b 696e 5f64 6972 5f66 696c 657a 0575  ..in_dir_filez.u
+00000ac0: 7466 2d38 2901 da08 656e 636f 6469 6e67  tf-8)...encoding
+00000ad0: 7a17 636f 6e74 656e 7420 6f66 2069 6e2d  z.content of in-
+00000ae0: 6469 722d 6669 6c65 0a4e 290b da0b 6173  dir-file.N)...as
+00000af0: 7365 7274 4571 7561 6c72 2c00 0000 7217  sertEqualr,...r.
+00000b00: 0000 0072 0a00 0000 7203 0000 0072 0c00  ...r....r....r..
+00000b10: 0000 722f 0000 00da 046e 616d 65da 0463  ..r/.....name..c
+00000b20: 6f70 79da 046f 7065 6eda 0563 6c6f 7365  opy..open..close
+00000b30: 2902 7212 0000 00da 0364 7374 7213 0000  ).r......dstr...
+00000b40: 0072 1300 0000 7214 0000 00da 1374 6573  .r....r......tes
+00000b50: 745f 6261 7369 635f 776f 726b 666c 6f77  t_basic_workflow
+00000b60: 4900 0000 730c 0000 0014 0412 0118 0118  I...s...........
+00000b70: 010a 010e 017a 1f42 6173 6549 736f 3936  .....z.BaseIso96
+00000b80: 3630 2e74 6573 745f 6261 7369 635f 776f  60.test_basic_wo
+00000b90: 726b 666c 6f77 da05 6d6f 756e 747a 3254  rkflow..mountz2T
+00000ba0: 6869 7320 7465 7374 2072 6571 7569 7265  his test require
+00000bb0: 7320 6d6f 756e 7420 746f 2072 756e 2075  s mount to run u
+00000bc0: 6e64 6572 2073 7564 6f20 6f72 2072 6f6f  nder sudo or roo
+00000bd0: 74da 0d63 6170 5f73 7973 5f61 646d 696e  t..cap_sys_admin
+00000be0: fa2f 4361 7061 6269 6c69 7479 2074 6f20  ./Capability to 
+00000bf0: 6d6f 756e 7420 6973 2072 6571 7569 7265  mount is require
+00000c00: 6420 2863 6170 5f73 7973 5f61 646d 696e  d (cap_sys_admin
+00000c10: 2963 0100 0000 0000 0000 0000 0000 0400  )c..............
+00000c20: 0000 0800 0000 4300 0000 7398 0000 007c  ......C...s....|
+00000c30: 006a 006a 017d 0174 026a 03a0 047c 0164  .j.j.}.t.j...|.d
+00000c40: 01a1 027d 027c 00a0 0574 026a 03a0 067c  ...}.|...t.j...|
+00000c50: 02a1 01a1 0101 007c 00a0 0774 0874 0974  .......|...t.t.t
+00000c60: 026a 03a0 047c 0164 02a1 0264 0383 02a0  .j...|.d...d....
+00000c70: 0aa1 0083 0164 04a1 0201 0074 026a 03a0  .....d.....t.j..
+00000c80: 047c 0164 0164 05a1 037d 037c 00a0 0774  .|.d.d...}.|...t
+00000c90: 0874 097c 0364 0383 02a0 0aa1 0083 0164  .t.|.d.........d
+00000ca0: 06a1 0201 007c 006a 00a0 0ba1 0001 007c  .....|.j.......|
+00000cb0: 00a0 0c74 026a 03a0 0d7c 01a1 0164 07a1  ...t.j...|...d..
+00000cc0: 0201 0064 0853 0029 097a 310a 2020 2020  ...d.S.).z1.    
+00000cd0: 2020 2020 4368 6563 6b20 7468 6520 6d6e      Check the mn
+00000ce0: 745f 6469 7220 6675 6e63 7469 6f6e 616c  t_dir functional
+00000cf0: 6974 790a 2020 2020 2020 2020 7232 0000  ity.        r2..
+00000d00: 0072 3000 0000 da02 7262 7231 0000 0072  .r0.....rbr1...r
+00000d10: 3300 0000 7317 0000 0063 6f6e 7465 6e74  3...s....content
+00000d20: 206f 6620 696e 2d64 6972 2d66 696c 650a   of in-dir-file.
+00000d30: 7a38 7468 6520 6d6e 745f 6469 7220 6973  z8the mnt_dir is
+00000d40: 2073 7570 706f 7365 2074 6f20 6265 2064   suppose to be d
+00000d50: 6573 7472 6f79 6564 2061 6674 6572 2069  estroyed after i
+00000d60: 736f 2e63 6c6f 7365 2829 4e29 0e72 2c00  so.close()N).r,.
+00000d70: 0000 5a07 6d6e 745f 6469 7272 0a00 0000  ..Z.mnt_dirr....
+00000d80: 7203 0000 0072 0c00 0000 721c 0000 00da  r....r....r.....
+00000d90: 0569 7364 6972 7235 0000 00da 0562 7974  .isdirr5.....byt
+00000da0: 6573 7238 0000 0072 1700 0000 7239 0000  esr8...r....r9..
+00000db0: 00da 0b61 7373 6572 7446 616c 7365 da06  ...assertFalse..
+00000dc0: 6578 6973 7473 2904 7212 0000 00da 0462  exists).r......b
+00000dd0: 6173 65da 0864 6972 5f70 6174 685a 1069  ase..dir_pathZ.i
+00000de0: 6e5f 6469 725f 6669 6c65 5f70 6174 6872  n_dir_file_pathr
+00000df0: 1300 0000 7213 0000 0072 1400 0000 da15  ....r....r......
+00000e00: 7465 7374 5f6d 6e74 5f64 6972 5f77 6f72  test_mnt_dir_wor
+00000e10: 6b66 6c6f 7754 0000 0073 1e00 0000 080c  kflowT...s......
+00000e20: 0e01 1201 0401 1c01 04ff 1003 0401 1201  ................
+00000e30: 04ff 0a03 0401 0a01 0201 08fe 7a21 4261  ............z!Ba
+00000e40: 7365 4973 6f39 3636 302e 7465 7374 5f6d  seIso9660.test_m
+00000e50: 6e74 5f64 6972 5f77 6f72 6b66 6c6f 7763  nt_dir_workflowc
+00000e60: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000e70: 0200 0000 4300 0000 7322 0000 007c 006a  ....C...s"...|.j
+00000e80: 0064 0075 0172 0a7c 006a 00a0 01a1 0001  .d.u.r.|.j......
+00000e90: 007c 006a 02a0 03a1 0001 0064 0053 00a9  .|.j.......d.S..
+00000ea0: 014e 2904 722c 0000 0072 3900 0000 722f  .N).r,...r9...r/
+00000eb0: 0000 00da 0763 6c65 616e 7570 7211 0000  .....cleanupr...
+00000ec0: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000ed0: da08 7465 6172 446f 776e 7000 0000 7306  ..tearDownp...s.
+00000ee0: 0000 000a 010a 010e 017a 1442 6173 6549  .........z.BaseI
+00000ef0: 736f 3936 3630 2e74 6561 7244 6f77 6e4e  so9660.tearDownN
+00000f00: 290e 7225 0000 0072 2600 0000 7227 0000  ).r%...r&...r'..
+00000f10: 00da 075f 5f64 6f63 5f5f 7215 0000 0072  ...__doc__r....r
+00000f20: 3b00 0000 7228 0000 00da 0673 6b69 7049  ;...r(.....skipI
+00000f30: 6672 0400 0000 da08 6361 6e5f 7375 646f  fr......can_sudo
+00000f40: da0a 736b 6970 556e 6c65 7373 da0e 6861  ..skipUnless..ha
+00000f50: 735f 6361 7061 6269 6c69 7479 7246 0000  s_capabilityrF..
+00000f60: 0072 4900 0000 7213 0000 0072 1300 0000  .rI...r....r....
+00000f70: 7213 0000 0072 1400 0000 722a 0000 0036  r....r....r*...6
+00000f80: 0000 0073 1c00 0000 0800 0402 0804 080d  ...s............
+00000f90: 040b 0a01 0201 02fe 0404 0801 0201 02fe  ................
+00000fa0: 0c04 0c14 722a 0000 0063 0000 0000 0000  ....r*...c......
+00000fb0: 0000 0000 0000 0000 0000 0600 0000 0000  ................
+00000fc0: 0000 f336 0000 0065 005a 0164 005a 0264  ...6...e.Z.d.Z.d
+00000fd0: 015a 0365 04a0 0565 066a 0764 0264 0364  .Z.e...e.j.d.d.d
+00000fe0: 048d 0264 05a1 0287 0066 0164 0664 0784  ...d.....f.d.d..
+00000ff0: 0883 015a 0887 0004 005a 0953 0029 08da  ...Z.....Z.S.)..
+00001000: 0749 736f 496e 666f 7a1d 0a20 2020 2049  .IsoInfoz..    I
+00001010: 736f 496e 666f 2d62 6173 6564 2063 6865  soInfo-based che
+00001020: 636b 0a20 2020 205a 0769 736f 696e 666f  ck.    Z.isoinfo
+00001030: 46a9 01da 0764 6566 6175 6c74 7a16 6973  F....defaultz.is
+00001040: 6f69 6e66 6f20 6e6f 7420 696e 7374 616c  oinfo not instal
+00001050: 6c65 642e 6301 0000 0000 0000 0000 0000  led.c...........
+00001060: 0001 0000 0003 0000 0003 0000 00f3 1c00  ................
+00001070: 0000 7400 8300 a001 a100 0100 7402 a003  ..t.........t...
+00001080: 7c00 6a04 a101 7c00 5f05 6400 5300 7247  |.j...|._.d.S.rG
+00001090: 0000 0029 06da 0573 7570 6572 7215 0000  ...)...superr...
+000010a0: 0072 0200 0000 5a0e 4973 6f39 3636 3049  .r....Z.Iso9660I
+000010b0: 736f 496e 666f 7210 0000 0072 2c00 0000  soInfor....r,...
+000010c0: 7211 0000 00a9 01da 095f 5f63 6c61 7373  r........__class
+000010d0: 5f5f 7213 0000 0072 1400 0000 7215 0000  __r....r....r...
+000010e0: 007c 0000 00f3 0400 0000 0a04 1201 7a0d  .|............z.
+000010f0: 4973 6f49 6e66 6f2e 7365 7455 70a9 0a72  IsoInfo.setUp..r
+00001100: 2500 0000 7226 0000 0072 2700 0000 724a  %...r&...r'...rJ
+00001110: 0000 0072 2800 0000 724d 0000 0072 0300  ...r(...rM...r..
+00001120: 0000 da0c 6669 6e64 5f63 6f6d 6d61 6e64  ....find_command
+00001130: 7215 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
+00001140: 6c6c 5f5f 7213 0000 0072 1300 0000 7255  ll__r....r....rU
+00001150: 0000 0072 1400 0000 7250 0000 0076 0000  ...r....rP...v..
+00001160: 00f3 0c00 0000 0800 0402 0404 0e01 02ff  ................
+00001170: 1603 7250 0000 0063 0000 0000 0000 0000  ..rP...c........
+00001180: 0000 0000 0000 0000 0600 0000 0000 0000  ................
+00001190: 724f 0000 0029 08da 0749 736f 5265 6164  rO...)...IsoRead
+000011a0: 7a1d 0a20 2020 2049 736f 5265 6164 2d62  z..    IsoRead-b
+000011b0: 6173 6564 2063 6865 636b 0a20 2020 207a  ased check.    z
+000011c0: 0869 736f 2d72 6561 6446 7251 0000 007a  .iso-readFrQ...z
+000011d0: 1769 736f 2d72 6561 6420 6e6f 7420 696e  .iso-read not in
+000011e0: 7374 616c 6c65 642e 6301 0000 0000 0000  stalled.c.......
+000011f0: 0000 0000 0001 0000 0003 0000 0003 0000  ................
+00001200: 0072 5300 0000 7247 0000 0029 0672 5400  .rS...rG...).rT.
+00001210: 0000 7215 0000 0072 0200 0000 5a0e 4973  ..r....r....Z.Is
+00001220: 6f39 3636 3049 736f 5265 6164 7210 0000  o9660IsoReadr...
+00001230: 0072 2c00 0000 7211 0000 0072 5500 0000  .r,...r....rU...
+00001240: 7213 0000 0072 1400 0000 7215 0000 008a  r....r....r.....
+00001250: 0000 0072 5700 0000 7a0d 4973 6f52 6561  ...rW...z.IsoRea
+00001260: 642e 7365 7455 7072 5800 0000 7213 0000  d.setUprX...r...
+00001270: 0072 1300 0000 7255 0000 0072 1400 0000  .r....rU...r....
+00001280: 725c 0000 0084 0000 0072 5b00 0000 725c  r\.......r[...r\
+00001290: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000012a0: 0000 0000 0600 0000 0000 0000 7346 0000  ............sF..
+000012b0: 0065 005a 0164 005a 0264 015a 0365 04a0  .e.Z.d.Z.d.Z.e..
+000012c0: 0565 06a0 0764 02a1 010c 0064 03a1 0265  .e...d.....d...e
+000012d0: 04a0 0865 06a0 0964 04a1 0164 05a1 0287  ...e...d...d....
+000012e0: 0066 0164 0664 0784 0883 0183 015a 0a87  .f.d.d.......Z..
+000012f0: 0004 005a 0b53 0029 08da 0849 736f 4d6f  ...Z.S.)...IsoMo
+00001300: 756e 747a 1b0a 2020 2020 4d6f 756e 742d  untz..    Mount-
+00001310: 6261 7365 6420 6368 6563 6b0a 2020 2020  based check.    
+00001320: 723c 0000 007a 1f54 6869 7320 7465 7374  r<...z.This test
+00001330: 2072 6571 7569 7265 7320 7375 646f 206f   requires sudo o
+00001340: 7220 726f 6f74 723d 0000 0072 3e00 0000  r rootr=...r>...
+00001350: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001360: 0003 0000 0003 0000 0072 5300 0000 7247  .........rS...rG
+00001370: 0000 0029 0672 5400 0000 7215 0000 0072  ...).rT...r....r
+00001380: 0200 0000 5a0c 4973 6f39 3636 304d 6f75  ....Z.Iso9660Mou
+00001390: 6e74 7210 0000 0072 2c00 0000 7211 0000  ntr....r,...r...
+000013a0: 0072 5500 0000 7213 0000 0072 1400 0000  .rU...r....r....
+000013b0: 7215 0000 0098 0000 0073 0400 0000 0a06  r........s......
+000013c0: 1201 7a0e 4973 6f4d 6f75 6e74 2e73 6574  ..z.IsoMount.set
+000013d0: 5570 290c 7225 0000 0072 2600 0000 7227  Up).r%...r&...r'
+000013e0: 0000 0072 4a00 0000 7228 0000 0072 4b00  ...rJ...r(...rK.
+000013f0: 0000 7204 0000 0072 4c00 0000 724d 0000  ..r....rL...rM..
+00001400: 0072 4e00 0000 7215 0000 0072 5a00 0000  .rN...r....rZ...
+00001410: 7213 0000 0072 1300 0000 7255 0000 0072  r....r....rU...r
+00001420: 1400 0000 725d 0000 0092 0000 0073 1000  ....r].......s..
+00001430: 0000 0800 0402 1204 0401 0801 0201 02fe  ................
+00001440: 1804 725d 0000 0063 0000 0000 0000 0000  ..r]...c........
+00001450: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+00001460: 7338 0000 0065 005a 0164 005a 0264 015a  s8...e.Z.d.Z.d.Z
+00001470: 0365 04a0 0565 06a0 07a1 0064 02a1 0287  .e...e.....d....
+00001480: 0066 0164 0364 0484 0883 015a 0864 0564  .f.d.d.....Z.d.d
+00001490: 0684 005a 0987 0004 005a 0a53 0029 07da  ...Z.....Z.S.)..
+000014a0: 0750 7943 444c 6962 7a1d 0a20 2020 2050  .PyCDLibz..    P
+000014b0: 7943 444c 6962 2d62 6173 6564 2063 6865  yCDLib-based che
+000014c0: 636b 0a20 2020 207a 1570 7963 646c 6962  ck.    z.pycdlib
+000014d0: 206e 6f74 2069 6e73 7461 6c6c 6564 6301   not installedc.
+000014e0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+000014f0: 0000 0003 0000 0072 5300 0000 7247 0000  .......rS...rG..
+00001500: 0029 0672 5400 0000 7215 0000 0072 0200  .).rT...r....r..
+00001510: 0000 721b 0000 0072 1000 0000 722c 0000  ..r....r....r,..
+00001520: 0072 1100 0000 7255 0000 0072 1300 0000  .r....rU...r....
+00001530: 7214 0000 0072 1500 0000 a800 0000 7304  r....r........s.
+00001540: 0000 000a 0212 017a 0d50 7943 444c 6962  .......z.PyCDLib
+00001550: 2e73 6574 5570 6301 0000 0000 0000 0000  .setUpc.........
+00001560: 0000 0006 0000 0006 0000 0043 0000 0073  ...........C...s
+00001570: 7800 0000 7400 6a01 a002 7c00 6a03 6a04  x...t.j...|.j.j.
+00001580: 6401 a102 7d01 7405 a006 7c01 a101 7d02  d...}.t...|...}.
+00001590: 7c02 a007 a100 0100 6402 7d03 6403 4400  |.......d.}.d.D.
+000015a0: 5d23 7d04 7c02 a008 7c04 7c03 a102 0100  ]#}.|...|.|.....
+000015b0: 7c02 a009 a100 0100 7405 a006 7c01 a101  |.......t...|...
+000015c0: 7d05 7c00 a00a 7c05 a00b 7c04 a101 7c03  }.|...|...|...|.
+000015d0: a102 0100 7c00 a00c 7400 6a01 a00d 7c01  ....|...t.j...|.
+000015e0: a101 a101 0100 7116 6400 5300 2904 4e7a  ......q.d.S.).Nz
+000015f0: 076e 6577 2e69 736f 7307 0000 0041 564f  .new.isos....AVO
+00001600: 4341 444f 2904 5a06 5245 4144 4d45 7a07  CADO).Z.READMEz.
+00001610: 2f72 6561 646d 657a 0a72 6561 646d 652e  /readmez.readme.
+00001620: 7478 747a 1571 7569 7465 2d6c 6f6e 672d  txtz.quite-long-
+00001630: 7265 6164 6d65 2e74 7874 290e 720a 0000  readme.txt).r...
+00001640: 0072 0300 0000 720c 0000 0072 2f00 0000  .r....r....r/...
+00001650: 7236 0000 0072 0200 0000 721b 0000 0072  r6...r....r....r
+00001660: 1800 0000 7219 0000 0072 3900 0000 7235  ....r....r9...r5
+00001670: 0000 0072 1700 0000 721c 0000 00da 0669  ...r....r......i
+00001680: 7366 696c 6529 0672 1200 0000 5a0c 6e65  sfile).r....Z.ne
+00001690: 775f 6973 6f5f 7061 7468 5a07 6e65 775f  w_iso_pathZ.new_
+000016a0: 6973 6fda 0763 6f6e 7465 6e74 da09 6669  iso..content..fi
+000016b0: 6c65 5f70 6174 685a 0872 6561 645f 6973  le_pathZ.read_is
+000016c0: 6f72 1300 0000 7213 0000 0072 1400 0000  or....r....r....
+000016d0: da11 7465 7374 5f63 7265 6174 655f 7772  ..test_create_wr
+000016e0: 6974 65ad 0000 0073 1600 0000 1201 0a01  ite....s........
+000016f0: 0801 0401 0801 0c01 0801 0a01 1201 1401  ................
+00001700: 04fb 7a19 5079 4344 4c69 622e 7465 7374  ..z.PyCDLib.test
+00001710: 5f63 7265 6174 655f 7772 6974 6529 0b72  _create_write).r
+00001720: 2500 0000 7226 0000 0072 2700 0000 724a  %...r&...r'...rJ
+00001730: 0000 0072 2800 0000 724d 0000 0072 0200  ...r(...rM...r..
+00001740: 0000 5a0b 6861 735f 7079 6364 6c69 6272  ..Z.has_pycdlibr
+00001750: 1500 0000 7262 0000 0072 5a00 0000 7213  ....rb...rZ...r.
+00001760: 0000 0072 1300 0000 7255 0000 0072 1400  ...r....rU...r..
+00001770: 0000 725e 0000 00a2 0000 0073 0a00 0000  ..r^.......s....
+00001780: 0800 0402 0e04 0e01 1004 725e 0000 00da  ..........r^....
+00001790: 085f 5f6d 6169 6e5f 5f29 1572 4a00 0000  .__main__).rJ...
+000017a0: 720a 0000 0072 2d00 0000 5a0d 756e 6974  r....r-...Z.unit
+000017b0: 7465 7374 2e6d 6f63 6b72 2800 0000 da0d  test.mockr(.....
+000017c0: 6176 6f63 6164 6f2e 7574 696c 7372 0200  avocado.utilsr..
+000017d0: 0000 7203 0000 0072 0400 0000 5a0f 7365  ..r....r....Z.se
+000017e0: 6c66 7465 7374 732e 7574 696c 7372 0500  lftests.utilsr..
+000017f0: 0000 7206 0000 00da 0854 6573 7443 6173  ..r......TestCas
+00001800: 6572 0700 0000 722a 0000 0072 5000 0000  er....r*...rP...
+00001810: 725c 0000 0072 5d00 0000 725e 0000 0072  r\...r]...r^...r
+00001820: 2500 0000 da04 6d61 696e 7213 0000 0072  %.....mainr....r
+00001830: 1300 0000 7213 0000 0072 1400 0000 da08  ....r....r......
+00001840: 3c6d 6f64 756c 653e 0100 0000 7320 0000  <module>....s ..
+00001850: 0004 0008 0308 0108 0114 0210 0106 0212  ................
+00001860: 030e 2814 4014 0e14 0e14 1008 180c 0104  ..(.@...........
+00001870: ff                                       .
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_kernel.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_kernel.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 866 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 6203 0000  o.......i&.bb...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 6203 0000  o.......nKecb...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6504  ..d.d.l.m.Z...e.
 00000050: 8300 0100 4700 6404 6405 8400 6405 6500  ....G.d.d...d.e.
 00000060: 6a05 8303 5a06 6401 5300 2906 e900 0000  j...Z.d.S.).....
 00000070: 004e 2901 da0b 4b65 726e 656c 4275 696c  .N)...KernelBuil
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_linux_modules.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_linux_modules.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2143 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 5f08 0000  o.......i&.b_...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 5f08 0000  o.......nKec_...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6504 8303 5a07 4700 6406 6407 8400 6407  e...Z.G.d.d...d.
 00000070: 6504 8303 5a08 6509 6408 6b02 722e 6502  e...Z.e.d.k.r.e.
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_memory.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_memory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 3956 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 740f 0000  o.......i&.bt...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 740f 0000  o.......nKect...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6501 6a04  ..G.d.d...d.e.j.
 00000050: 8303 5a05 6405 5a06 6501 6a07 6a08 6406  ..Z.d.Z.e.j.j.d.
 00000060: 6506 6407 8d02 4700 6408 6409 8400 6409  e.d...G.d.d...d.
 00000070: 6501 6a04 8303 8301 5a09 650a 640a 6b02  e.j.....Z.e.d.k.
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_network.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_network.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2201 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 9908 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 9908 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 7a08 6400 6401 6c04 5a04 6403 5a05  ..z.d.d.l.Z.d.Z.
 00000050: 5700 6e0b 0400 6506 791d 0100 0100 0100  W.n...e.y.......
 00000060: 6404 5a05 5900 6e01 7700 4700 6405 6406  d.Z.Y.n.w.G.d.d.
 00000070: 8400 6406 6501 6a07 8303 5a08 6407 6408  ..d.e.j...Z.d.d.
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_output.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_output.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1170 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 9204 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 9204 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6500 6a03  ..G.d.d...d.e.j.
 00000050: 8303 5a04 6505 6405 6b02 721d 6500 a006  ..Z.e.d.k.r.e...
 00000060: a100 0100 6401 5300 6401 5300 2906 e900  ....d.S.d.S.)...
 00000070: 0000 004e 2901 da06 6f75 7470 7574 6300  ...N)...outputc.
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_partition.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_partition.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 8324 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 8420 0000  o.......i&.b. ..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 c51f 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 d200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a05 6401 6403 6c06 6d07 5a07 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c06 6d08 5a09 0100 6401 6405 6c06  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 0100 6401 6406 6c0c  m.Z.m.Z...d.d.l.
@@ -37,464 +37,455 @@
 00000240: 2f63 6c65 6265 722f 7372 632f 6176 6f63  /cleber/src/avoc
 00000250: 6164 6f2f 6176 6f63 6164 6f2f 7365 6c66  ado/avocado/self
 00000260: 7465 7374 732f 756e 6974 2f75 7469 6c73  tests/unit/utils
 00000270: 2f74 6573 745f 7061 7274 6974 696f 6e2e  /test_partition.
 00000280: 7079 da0e 6d69 7373 696e 675f 6269 6e61  py..missing_bina
 00000290: 7279 1200 0000 730c 0000 0002 010a 0106  ry....s.........
 000002a0: 010e 0106 0102 ff72 0d00 0000 6300 0000  .......r....c...
-000002b0: 0000 0000 0000 0000 0000 0000 000a 0000  ................
-000002c0: 0040 0000 0073 a400 0000 6500 5a01 6400  .@...s....e.Z.d.
+000002b0: 0000 0000 0000 0000 0000 0000 0009 0000  ................
+000002c0: 0040 0000 0073 8400 0000 6500 5a01 6400  .@...s....e.Z.d.
 000002d0: 5a02 6401 5a03 6504 a005 6506 6a07 a008  Z.d.Z.e...e.j...
 000002e0: 6402 a101 0c00 6403 a102 6504 a005 6509  d.....d...e...e.
 000002f0: a00a 6404 a101 0c00 6405 a102 6504 a005  ..d.....d...e...
 00000300: 6509 a00a 6406 a101 0c00 6407 a102 6504  e...d.....d...e.
 00000310: a00b 650c a00d 6408 6409 a102 640a a102  ..e...d.d...d...
 00000320: 6504 a00b 6509 a00e 640b a101 640c a102  e...e...d...d...
-00000330: 6504 a005 6506 a00f 640d a101 6f40 6506  e...e...d...o@e.
-00000340: a00f 640e a101 640f 7600 6410 a102 6411  ..d...d.v.d...d.
-00000350: 6412 8400 8301 8301 8301 8301 8301 8301  d...............
-00000360: 5a10 6413 6414 8400 5a11 6415 5300 2916  Z.d.d...Z.d.S.).
-00000370: da04 4261 7365 7a33 0a20 2020 2043 6f6d  ..Basez3.    Com
-00000380: 6d6f 6e20 7365 7455 702f 7465 6172 446f  mon setUp/tearDo
-00000390: 776e 2066 6f72 2070 6172 7469 7469 6f6e  wn for partition
-000003a0: 2074 6573 7473 0a20 2020 20fa 0c2f 7072   tests.    ../pr
-000003b0: 6f63 2f6d 6f75 6e74 737a 2173 7973 7465  oc/mountsz!syste
-000003c0: 6d20 646f 6573 206e 6f74 2068 6176 6520  m does not have 
-000003d0: 2f70 726f 632f 6d6f 756e 7473 da05 6d6f  /proc/mounts..mo
-000003e0: 756e 747a 3663 7572 7265 6e74 2075 7365  untz6current use
-000003f0: 7220 6d75 7374 2062 6520 616c 6c6f 7765  r must be allowe
-00000400: 6420 746f 2072 756e 2022 6d6f 756e 7422  d to run "mount"
-00000410: 2075 6e64 6572 2073 7564 6f7a 0c6d 6b66   under sudoz.mkf
-00000420: 732e 6578 7432 202d 567a 3a63 7572 7265  s.ext2 -Vz:curre
-00000430: 6e74 2075 7365 7220 6d75 7374 2062 6520  nt user must be 
-00000440: 616c 6c6f 7765 6420 746f 2072 756e 2022  allowed to run "
-00000450: 6d6b 6673 2e65 7874 3222 2075 6e64 6572  mkfs.ext2" under
-00000460: 2073 7564 6f7a 096d 6b66 732e 6578 7432   sudoz.mkfs.ext2
-00000470: 467a 236d 6b66 732e 6578 7432 2075 7469  Fz#mkfs.ext2 uti
-00000480: 6c69 7479 206d 7573 7420 6265 2061 7661  lity must be ava
-00000490: 696c 6162 6c65 5a0d 6361 705f 7379 735f  ilableZ.cap_sys_
-000004a0: 6164 6d69 6e7a 2f43 6170 6162 696c 6974  adminz/Capabilit
-000004b0: 7920 746f 206d 6f75 6e74 2069 7320 7265  y to mount is re
-000004c0: 7175 6972 6564 2028 6361 705f 7379 735f  quired (cap_sys_
-000004d0: 6164 6d69 6e29 5a06 5452 4156 4953 5a0f  admin)Z.TRAVISZ.
-000004e0: 5452 4156 4953 5f43 5055 5f41 5243 4829  TRAVIS_CPU_ARCH)
-000004f0: 03da 0561 726d 3634 da07 7070 6336 346c  ...arm64..ppc64l
-00000500: 65da 0573 3339 3078 7a30 5452 4156 4953  e..s390xz0TRAVIS
-00000510: 2045 6e76 6972 6f6e 6d65 6e74 2069 7320   Environment is 
-00000520: 756e 7375 6974 6162 6c65 2066 6f72 2074  unsuitable for t
-00000530: 6865 7365 2074 6573 7473 6301 0000 0000  hese testsc.....
-00000540: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
-00000550: 0000 0073 5a00 0000 7400 7c00 8301 7d01  ...sZ...t.|...}.
-00000560: 7401 6a02 7c01 6401 8d01 7c00 5f03 7404  t.j.|.d...|._.t.
-00000570: 6a05 a006 7c00 6a03 6a07 6402 a102 7c00  j...|.j.j.d...|.
-00000580: 5f08 7404 a009 7c00 6a08 a101 0100 740a  _.t...|.j.....t.
-00000590: a00b 7404 6a05 a006 7c00 6a03 6a07 6403  ..t.j...|.j.j.d.
-000005a0: a102 6404 7c00 6a08 a103 7c00 5f0c 6400  ..d.|.j...|._.d.
-000005b0: 5300 2905 4e29 01da 0670 7265 6669 78da  S.).N)...prefix.
-000005c0: 0464 6973 6bda 0562 6c6f 636b e901 0000  .disk..block....
-000005d0: 0029 0d72 0600 0000 da08 7465 6d70 6669  .).r......tempfi
-000005e0: 6c65 da12 5465 6d70 6f72 6172 7944 6972  le..TemporaryDir
-000005f0: 6563 746f 7279 da06 746d 7064 6972 da02  ectory..tmpdir..
-00000600: 6f73 7203 0000 00da 046a 6f69 6eda 046e  osr......join..n
-00000610: 616d 65da 0a6d 6f75 6e74 706f 696e 74da  ame..mountpoint.
-00000620: 056d 6b64 6972 7202 0000 005a 0950 6172  .mkdirr....Z.Par
-00000630: 7469 7469 6f6e 7215 0000 0029 02da 0473  titionr....)...s
-00000640: 656c 6672 1400 0000 720b 0000 0072 0b00  elfr....r....r..
-00000650: 0000 720c 0000 00da 0573 6574 5570 2000  ..r......setUp .
-00000660: 0000 730e 0000 0008 190e 0114 010c 0104  ..s.............
-00000670: 0116 010a ff7a 0a42 6173 652e 7365 7455  .....z.Base.setU
-00000680: 7063 0100 0000 0000 0000 0000 0000 0100  pc..............
-00000690: 0000 0200 0000 4300 0000 7318 0000 007c  ......C...s....|
-000006a0: 006a 00a0 01a1 0001 007c 006a 02a0 03a1  .j.......|.j....
-000006b0: 0001 0064 0053 00a9 014e 2904 7215 0000  ...d.S...N).r...
-000006c0: 00da 0775 6e6d 6f75 6e74 721a 0000 00da  ...unmountr.....
-000006d0: 0763 6c65 616e 7570 a901 7220 0000 0072  .cleanup..r ...r
-000006e0: 0b00 0000 720b 0000 0072 0c00 0000 da08  ....r....r......
-000006f0: 7465 6172 446f 776e 4100 0000 7304 0000  tearDownA...s...
-00000700: 000a 010e 017a 0d42 6173 652e 7465 6172  .....z.Base.tear
-00000710: 446f 776e 4e29 12da 085f 5f6e 616d 655f  DownN)...__name_
-00000720: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000730: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-00000740: 6f63 5f5f da08 756e 6974 7465 7374 da06  oc__..unittest..
-00000750: 736b 6970 4966 721b 0000 0072 0300 0000  skipIfr....r....
-00000760: da06 6973 6669 6c65 7204 0000 00da 0863  ..isfiler......c
-00000770: 616e 5f73 7564 6fda 0a73 6b69 7055 6e6c  an_sudo..skipUnl
-00000780: 6573 7372 0700 0000 7208 0000 00da 0e68  essr....r......h
-00000790: 6173 5f63 6170 6162 696c 6974 79da 0667  as_capability..g
-000007a0: 6574 656e 7672 2100 0000 7226 0000 0072  etenvr!...r&...r
-000007b0: 0b00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
-000007c0: 0000 0072 0e00 0000 1a00 0000 7338 0000  ...r........s8..
-000007d0: 0008 0004 0204 040e 0102 ff04 030a 0102  ................
-000007e0: 0102 fe04 040a 0102 0102 fe04 040a 0102  ................
-000007f0: 0102 fe04 0408 0102 0102 fe04 040a 010c  ................
-00000800: 0102 0102 fd14 050c 0972 0e00 0000 6300  .........r....c.
-00000810: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-00000820: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
-00000830: 6400 5a02 6401 6402 8400 5a03 6403 5300  d.Z.d.d...Z.d.S.
-00000840: 2904 da0d 5465 7374 5061 7274 6974 696f  )...TestPartitio
-00000850: 6e63 0100 0000 0000 0000 0000 0000 0300  nc..............
-00000860: 0000 0800 0000 4300 0000 73c2 0000 007c  ......C...s....|
-00000870: 00a0 007c 006a 01a0 02a1 00a1 0101 007c  ...|.j.........|
-00000880: 006a 01a0 03a1 0001 007c 006a 01a0 04a1  .j.......|.j....
-00000890: 0001 0074 0564 0183 018f 0c7d 017c 01a0  ...t.d.....}.|..
-000008a0: 06a1 007d 0257 0064 0204 0004 0083 0301  ...}.W.d........
-000008b0: 006e 0831 0073 2577 0101 0001 0001 0059  .n.1.s%w.......Y
-000008c0: 0001 007c 00a0 077c 006a 087c 02a1 0201  ...|...|.j.|....
-000008d0: 007c 00a0 097c 006a 087c 006a 01a0 02a1  .|...|.j.|.j....
-000008e0: 00a1 0201 007c 006a 01a0 0aa1 0001 0074  .....|.j.......t
-000008f0: 0564 0183 018f 0c7d 017c 01a0 06a1 007d  .d.....}.|.....}
-00000900: 0257 0064 0204 0004 0083 0301 006e 0831  .W.d.........n.1
-00000910: 0073 5377 0101 0001 0001 0059 0001 007c  .sSw.......Y...|
-00000920: 00a0 0b7c 006a 087c 02a1 0201 0064 0253  ...|.j.|.....d.S
-00000930: 0029 037a 1754 6573 7420 7468 6520 6261  .).z.Test the ba
-00000940: 7369 6320 776f 726b 666c 6f77 720f 0000  sic workflowr...
-00000950: 004e 290c da0c 6173 7365 7274 4973 4e6f  .N)...assertIsNo
-00000960: 6e65 7215 0000 005a 0e67 6574 5f6d 6f75  ner....Z.get_mou
-00000970: 6e74 706f 696e 74da 046d 6b66 7372 1000  ntpoint..mkfsr..
-00000980: 0000 da04 6f70 656e da04 7265 6164 da08  ....open..read..
-00000990: 6173 7365 7274 496e 721e 0000 00da 0b61  assertInr......a
-000009a0: 7373 6572 7445 7175 616c 7223 0000 00da  ssertEqualr#....
-000009b0: 0b61 7373 6572 744e 6f74 496e a903 7220  .assertNotIn..r 
-000009c0: 0000 00da 1070 726f 635f 6d6f 756e 7473  .....proc_mounts
-000009d0: 5f66 696c 65da 0b70 726f 635f 6d6f 756e  _file..proc_moun
-000009e0: 7473 720b 0000 0072 0b00 0000 720c 0000  tsr....r....r...
-000009f0: 00da 0a74 6573 745f 6261 7369 6347 0000  ...test_basicG..
-00000a00: 0073 1a00 0000 1002 0a01 0a01 0a01 0a01  .s..............
-00000a10: 1cff 0e02 1401 0a01 0a01 0a01 1cff 1202  ................
-00000a20: 7a18 5465 7374 5061 7274 6974 696f 6e2e  z.TestPartition.
-00000a30: 7465 7374 5f62 6173 6963 4e29 0472 2700  test_basicN).r'.
-00000a40: 0000 7228 0000 0072 2900 0000 723d 0000  ..r(...r)...r=..
-00000a50: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000a60: 720c 0000 0072 3200 0000 4600 0000 7304  r....r2...F...s.
-00000a70: 0000 0008 000c 0172 3200 0000 6300 0000  .......r2...c...
-00000a80: 0000 0000 0000 0000 0000 0000 0007 0000  ................
-00000a90: 0000 0000 0073 da00 0000 6500 5a01 6400  .....s....e.Z.d.
-00000aa0: 5a02 6401 5a03 8700 6601 6402 6403 8408  Z.d.Z...f.d.d...
-00000ab0: 5a04 6404 6405 8400 5a05 6506 a007 6508  Z.d.d...Z.e...e.
-00000ac0: 6406 8301 6407 a102 6506 a007 6509 a00a  d...d...e...e...
-00000ad0: 650b 6a0c 6408 1700 a101 0c00 6409 a102  e.j.d.......d...
-00000ae0: 6506 a007 6509 a00a 640a a101 0c00 640b  e...e...d.....d.
-00000af0: a102 640c 640d 8400 8301 8301 8301 5a0d  ..d.d.........Z.
-00000b00: 6506 a007 6509 a00a 650b 6a0c 6408 1700  e...e...e.j.d...
-00000b10: a101 0c00 6409 a102 6506 a00e 6508 6406  ....d...e...e.d.
-00000b20: 8301 640e a102 640f 6410 8400 8301 8301  ..d...d.d.......
-00000b30: 5a0f 6506 a007 6509 a00a 650b 6a0c 6408  Z.e...e...e.j.d.
-00000b40: 1700 a101 0c00 6409 a102 6411 6412 8400  ......d...d.d...
-00000b50: 8301 5a10 6413 6414 8400 5a11 6415 6416  ..Z.d.d...Z.d.d.
-00000b60: 8400 5a12 6417 6418 8400 5a13 8700 0400  ..Z.d.d...Z.....
-00000b70: 5a14 5300 2919 da16 5465 7374 5061 7274  Z.S.)...TestPart
-00000b80: 6974 696f 6e4d 6b66 734d 6f75 6e74 7a3e  itionMkfsMountz>
-00000b90: 0a20 2020 2054 6573 7473 2074 6861 7420  .    Tests that 
-00000ba0: 6173 7375 6d65 2061 2066 696c 6573 7973  assume a filesys
-00000bb0: 7465 6d20 616e 6420 6d6f 756e 7465 6420  tem and mounted 
-00000bc0: 7061 7274 6974 696f 6e0a 2020 2020 6301  partition.    c.
-00000bd0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00000be0: 0000 0003 0000 0073 4a00 0000 7400 8300  .......sJ...t...
-00000bf0: a001 a100 0100 7c00 6a02 a003 a100 0100  ......|.j.......
-00000c00: 7c00 6a02 a004 a100 0100 7405 6a06 a007  |.j.......t.j...
-00000c10: 7c00 6a08 6401 a102 7c00 5f09 740a 6a0b  |.j.d...|._.t.j.
-00000c20: 9b00 6402 7c00 6a09 9b00 6403 9d04 7c00  ..d.|.j...d...|.
-00000c30: 5f0c 6400 5300 2904 4eda 0466 696c 657a  _.d.S.).N..filez
-00000c40: 1c20 2d63 2027 696d 706f 7274 2074 696d  . -c 'import tim
-00000c50: 653b 2066 203d 206f 7065 6e28 227a 1822  e; f = open("z."
-00000c60: 2c20 2277 2229 3b20 7469 6d65 2e73 6c65  , "w"); time.sle
-00000c70: 6570 2836 3029 2729 0dda 0573 7570 6572  ep(60)')...super
-00000c80: 7221 0000 0072 1500 0000 7234 0000 0072  r!...r....r4...r
-00000c90: 1000 0000 721b 0000 0072 0300 0000 721c  ....r....r....r.
-00000ca0: 0000 0072 1e00 0000 da0c 7573 655f 6d6e  ...r......use_mn
-00000cb0: 745f 6669 6c65 da03 7379 73da 0a65 7865  t_file..sys..exe
-00000cc0: 6375 7461 626c 65da 0b75 7365 5f6d 6e74  cutable..use_mnt
-00000cd0: 5f63 6d64 7225 0000 00a9 01da 095f 5f63  _cmdr%.......__c
-00000ce0: 6c61 7373 5f5f 720b 0000 0072 0c00 0000  lass__r....r....
-00000cf0: 7221 0000 005c 0000 0073 1000 0000 0a01  r!...\...s......
-00000d00: 0a01 0a01 1201 0802 0401 06ff 08ff 7a1c  ..............z.
-00000d10: 5465 7374 5061 7274 6974 696f 6e4d 6b66  TestPartitionMkf
-00000d20: 734d 6f75 6e74 2e73 6574 5570 6301 0000  sMount.setUpc...
-00000d30: 0000 0000 0000 0000 0002 0000 0008 0000  ................
-00000d40: 0003 0000 0073 3e00 0000 7400 6a01 8800  .....s>...t.j...
-00000d50: 6a02 6401 6402 8d02 7d01 7c01 a003 a100  j.d.d...}.|.....
-00000d60: 0100 8800 a004 7405 6a06 8700 6601 6403  ......t.j...f.d.
-00000d70: 6404 8408 6405 6406 6406 6407 8d04 6408  d...d.d.d.d...d.
-00000d80: a102 0100 7c01 5300 2909 4e54 a901 da04  ....|.S.).NT....
-00000d90: 7375 646f 6300 0000 0000 0000 0000 0000  sudoc...........
-00000da0: 0000 0000 0003 0000 0013 0000 0073 0e00  .............s..
-00000db0: 0000 7400 6a01 a002 8800 6a03 a101 5300  ..t.j.....j...S.
-00000dc0: 7222 0000 0029 0472 1b00 0000 7203 0000  r"...).r....r...
-00000dd0: 00da 0665 7869 7374 7372 4100 0000 720b  ...existsrA...r.
-00000de0: 0000 0072 2500 0000 720b 0000 0072 0c00  ...r%...r....r..
-00000df0: 0000 da08 3c6c 616d 6264 613e 6c00 0000  ....<lambda>l...
-00000e00: 7302 0000 000e 007a 3f54 6573 7450 6172  s......z?TestPar
-00000e10: 7469 7469 6f6e 4d6b 6673 4d6f 756e 742e  titionMkfsMount.
-00000e20: 7275 6e5f 7072 6f63 6573 735f 746f 5f75  run_process_to_u
-00000e30: 7365 5f6d 6e74 2e3c 6c6f 6361 6c73 3e2e  se_mnt.<locals>.
-00000e40: 3c6c 616d 6264 613e 7217 0000 0067 9a99  <lambda>r....g..
-00000e50: 9999 9999 b93f 2903 da07 7469 6d65 6f75  .....?)...timeou
-00000e60: 74da 0566 6972 7374 da04 7374 6570 7a26  t..first..stepz&
-00000e70: 4669 6c65 2077 6173 206e 6f74 2063 7265  File was not cre
-00000e80: 6174 6564 2077 6974 6869 6e20 6d6f 756e  ated within moun
-00000e90: 7470 6f69 6e74 2907 7204 0000 00da 0a53  tpoint).r......S
-00000ea0: 7562 5072 6f63 6573 7372 4400 0000 da05  ubProcessrD.....
-00000eb0: 7374 6172 74da 0a61 7373 6572 7454 7275  start..assertTru
-00000ec0: 6572 0500 0000 da08 7761 6974 5f66 6f72  er......wait_for
-00000ed0: 2902 7220 0000 00da 0470 726f 6372 0b00  ).r .....procr..
-00000ee0: 0000 7225 0000 0072 0c00 0000 da16 7275  ..r%...r......ru
-00000ef0: 6e5f 7072 6f63 6573 735f 746f 5f75 7365  n_process_to_use
-00000f00: 5f6d 6e74 6700 0000 7318 0000 0010 0108  _mntg...s.......
-00000f10: 0104 0104 010a 0102 0102 0102 0104 fc02  ................
-00000f20: 0604 f904 097a 2d54 6573 7450 6172 7469  .....z-TestParti
-00000f30: 7469 6f6e 4d6b 6673 4d6f 756e 742e 7275  tionMkfsMount.ru
-00000f40: 6e5f 7072 6f63 6573 735f 746f 5f75 7365  n_process_to_use
-00000f50: 5f6d 6e74 5a04 6c73 6f66 7a15 7265 7175  _mntZ.lsofz.requ
-00000f60: 6972 6573 2072 756e 6e69 6e67 206c 736f  ires running lso
-00000f70: 667a 0620 2d63 2027 277a 2c72 6571 7569  fz. -c ''z,requi
-00000f80: 7265 7320 7275 6e6e 696e 6720 5079 7468  res running Pyth
-00000f90: 6f6e 2061 7320 6120 7072 6976 696c 6567  on as a privileg
-00000fa0: 6564 2075 7365 727a 076b 696c 6c20 2d6c  ed userz.kill -l
-00000fb0: 7a2a 7265 7175 6972 6573 2072 756e 6e69  z*requires runni
-00000fc0: 6e67 206b 696c 6c20 6173 2061 2070 7269  ng kill as a pri
-00000fd0: 7669 6c65 6765 6420 7573 6572 6301 0000  vileged userc...
-00000fe0: 0000 0000 0000 0000 0004 0000 0008 0000  ................
-00000ff0: 0043 0000 0073 ae00 0000 7400 6401 8301  .C...s....t.d...
-00001000: 8f0c 7d01 7c01 a001 a100 7d02 5700 6402  ..}.|.....}.W.d.
-00001010: 0400 0400 8303 0100 6e08 3100 7313 7701  ........n.1.s.w.
-00001020: 0100 0100 0100 5900 0100 7c00 a002 7c00  ......Y...|...|.
-00001030: 6a03 7c02 a102 0100 7c00 a004 a100 7d03  j.|.....|.....}.
-00001040: 7c00 a005 7c00 6a06 a007 a100 a101 0100  |...|.j.........
-00001050: 7c00 a002 7c03 a008 a100 6403 6404 6702  |...|.....d.d.g.
-00001060: 6405 a103 0100 7400 6401 8301 8f0c 7d01  d.....t.d.....}.
-00001070: 7c01 a001 a100 7d02 5700 6402 0400 0400  |.....}.W.d.....
-00001080: 8303 0100 6e08 3100 7349 7701 0100 0100  ....n.1.sIw.....
-00001090: 0100 5900 0100 7c00 a009 7c00 6a03 7c02  ..Y...|...|.j.|.
-000010a0: a102 0100 6402 5300 2906 7a1a 5465 7374  ....d.S.).z.Test
-000010b0: 2066 6f72 6365 2d75 6e6d 6f75 6e74 2066   force-unmount f
-000010c0: 6561 7475 7265 720f 0000 004e 69f7 ffff  eaturer....Ni...
-000010d0: ffe9 8900 0000 7a47 556e 6578 7065 6374  ......zGUnexpect
-000010e0: 6564 2072 6574 7572 6e20 636f 6465 2077  ed return code w
-000010f0: 6865 6e20 7472 7969 6e67 2074 6f20 6b69  hen trying to ki
-00001100: 6c6c 2070 726f 6365 7373 2075 7369 6e67  ll process using
-00001110: 2074 6865 206d 6f75 6e74 706f 696e 7429   the mountpoint)
-00001120: 0a72 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
-00001130: 721e 0000 0072 5300 0000 7250 0000 0072  r....rS...rP...r
-00001140: 1500 0000 7223 0000 00da 0470 6f6c 6c72  ....r#.....pollr
-00001150: 3900 0000 a904 7220 0000 0072 3b00 0000  9.....r ...r;...
-00001160: 723c 0000 0072 5200 0000 720b 0000 0072  r<...rR...r....r
-00001170: 0b00 0000 720c 0000 00da 1274 6573 745f  ....r......test_
-00001180: 666f 7263 655f 756e 6d6f 756e 7475 0000  force_unmountu..
-00001190: 0073 1e00 0000 0a0a 0a01 1cff 0e02 0801  .s..............
-000011a0: 1001 0403 0601 0601 0201 04fd 0a06 0a01  ................
-000011b0: 1cff 1202 7a29 5465 7374 5061 7274 6974  ....z)TestPartit
-000011c0: 696f 6e4d 6b66 734d 6f75 6e74 2e74 6573  ionMkfsMount.tes
-000011d0: 745f 666f 7263 655f 756e 6d6f 756e 747a  t_force_unmountz
-000011e0: 1872 6571 7569 7265 7320 6e6f 7420 6861  .requires not ha
-000011f0: 7669 6e67 206c 736f 6663 0100 0000 0000  ving lsofc......
-00001200: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
-00001210: 0000 7368 0000 0074 0064 0183 018f 0c7d  ..sh...t.d.....}
-00001220: 017c 01a0 01a1 007d 0257 0064 0204 0004  .|.....}.W.d....
-00001230: 0083 0301 006e 0831 0073 1377 0101 0001  .....n.1.s.w....
-00001240: 0001 0059 0001 007c 00a0 027c 006a 037c  ...Y...|...|.j.|
-00001250: 02a1 0201 007c 00a0 04a1 007d 037c 00a0  .....|.....}.|..
-00001260: 0574 066a 077c 006a 086a 09a1 0201 007c  .t.j.|.j.j.....|
-00001270: 036a 0a64 0364 048d 0101 0064 0253 0029  .j.d.d.....d.S.)
-00001280: 057a 3d43 6865 636b 7320 7468 6174 2061  .z=Checks that a
-00001290: 2066 6f72 6365 2d75 6e6d 6f75 6e74 2077   force-unmount w
-000012a0: 696c 6c20 6661 696c 206f 6e20 7379 7374  ill fail on syst
-000012b0: 656d 7320 7769 7468 6f75 7420 6c73 6f66  ems without lsof
-000012c0: 720f 0000 004e 7217 0000 00a9 0172 4b00  r....Nr......rK.
-000012d0: 0000 290b 7235 0000 0072 3600 0000 7237  ..).r5...r6...r7
-000012e0: 0000 0072 1e00 0000 7253 0000 00da 0c61  ...r....rS.....a
-000012f0: 7373 6572 7452 6169 7365 7372 0200 0000  ssertRaisesr....
-00001300: da0e 5061 7274 6974 696f 6e45 7272 6f72  ..PartitionError
-00001310: 7215 0000 0072 2300 0000 7205 0000 0072  r....r#...r....r
-00001320: 5600 0000 720b 0000 0072 0b00 0000 720c  V...r....r....r.
-00001330: 0000 00da 1a74 6573 745f 666f 7263 655f  .....test_force_
-00001340: 756e 6d6f 756e 745f 6e6f 5f6c 736f 6690  unmount_no_lsof.
-00001350: 0000 0073 0e00 0000 0a07 0a01 1cff 0e02  ...s............
-00001360: 0801 1201 1001 7a31 5465 7374 5061 7274  ......z1TestPart
-00001370: 6974 696f 6e4d 6b66 734d 6f75 6e74 2e74  itionMkfsMount.t
-00001380: 6573 745f 666f 7263 655f 756e 6d6f 756e  est_force_unmoun
-00001390: 745f 6e6f 5f6c 736f 6663 0100 0000 0000  t_no_lsofc......
-000013a0: 0000 0000 0000 0500 0000 0900 0000 4300  ..............C.
-000013b0: 0000 73e8 0000 0074 0064 0183 018f 0c7d  ..s....t.d.....}
-000013c0: 017c 01a0 01a1 007d 0257 0064 0204 0004  .|.....}.W.d....
-000013d0: 0083 0301 006e 0831 0073 1377 0101 0001  .....n.1.s.w....
-000013e0: 0001 0059 0001 007c 00a0 027c 006a 037c  ...Y...|...|.j.|
-000013f0: 02a1 0201 007c 00a0 04a1 007d 0374 056a  .....|.....}.t.j
-00001400: 066a 0764 0374 086a 0964 048d 028f 3301  .j.d.t.j.d....3.
-00001410: 0074 056a 066a 0764 0574 0a64 048d 028f  .t.j.j.d.t.d....
-00001420: 1b7d 047c 00a0 0b74 0c6a 0d7c 006a 0e6a  .}.|...t.j.|.j.j
-00001430: 0fa1 0201 007c 046a 1064 067c 006a 0317  .....|.j.d.|.j..
-00001440: 0064 0764 088d 0201 0057 0064 0204 0004  .d.d.....W.d....
-00001450: 0083 0301 006e 0831 0073 5377 0101 0001  .....n.1.sSw....
-00001460: 0001 0059 0001 0057 0064 0204 0004 0083  ...Y...W.d......
-00001470: 0301 006e 0831 0073 6277 0101 0001 0001  ...n.1.sbw......
-00001480: 0059 0001 007c 006a 0ea0 0fa1 0001 007c  .Y...|.j.......|
-00001490: 036a 1164 0964 0a8d 0101 0064 0253 0029  .j.d.d.....d.S.)
-000014a0: 0b7a 3e43 6865 636b 7320 5061 7274 6974  .z>Checks Partit
-000014b0: 696f 6e45 7272 6f72 2069 7320 7261 6973  ionError is rais
-000014c0: 6564 2069 6620 7468 6572 6527 7320 6e6f  ed if there's no
-000014d0: 206c 736f 6620 746f 2067 6574 2070 6964   lsof to get pid
-000014e0: 7372 0f00 0000 4e7a 2361 766f 6361 646f  sr....Nz#avocado
-000014f0: 2e75 7469 6c73 2e70 6172 7469 7469 6f6e  .utils.partition
-00001500: 2e70 726f 6365 7373 2e72 756e a901 5a0b  .process.run..Z.
-00001510: 7369 6465 5f65 6666 6563 747a 2d61 766f  side_effectz-avo
-00001520: 6361 646f 2e75 7469 6c73 2e70 6172 7469  cado.utils.parti
-00001530: 7469 6f6e 2e70 726f 6365 7373 2e73 7973  tion.process.sys
-00001540: 7465 6d5f 6f75 7470 7574 7a05 6c73 6f66  tem_outputz.lsof
-00001550: 2054 7247 0000 0072 1700 0000 7258 0000   TrG...r....rX..
-00001560: 0029 1272 3500 0000 7236 0000 0072 3700  .).r5...r6...r7.
-00001570: 0000 721e 0000 0072 5300 0000 722b 0000  ..r....rS...r+..
-00001580: 00da 046d 6f63 6bda 0570 6174 6368 7204  ...mock..patchr.
-00001590: 0000 00da 0843 6d64 4572 726f 72da 074f  .....CmdError..O
-000015a0: 5345 7272 6f72 7259 0000 0072 0200 0000  SErrorrY...r....
-000015b0: 725a 0000 0072 1500 0000 7223 0000 005a  rZ...r....r#...Z
-000015c0: 1261 7373 6572 745f 6361 6c6c 6564 5f77  .assert_called_w
-000015d0: 6974 6872 0500 0000 2905 7220 0000 0072  ithr....).r ...r
-000015e0: 3b00 0000 723c 0000 0072 5200 0000 5a14  ;...r<...rR...Z.
-000015f0: 6d6f 636b 6564 5f73 7973 7465 6d5f 6f75  mocked_system_ou
-00001600: 7470 7574 720b 0000 0072 0b00 0000 720c  tputr....r....r.
-00001610: 0000 00da 2074 6573 745f 666f 7263 655f  .... test_force_
-00001620: 756e 6d6f 756e 745f 6765 745f 7069 6473  unmount_get_pids
-00001630: 5f66 6169 6c9e 0000 0073 2a00 0000 0a06  _fail....s*.....
-00001640: 0a01 1cff 0e02 0801 0601 0601 08ff 0603  ................
-00001650: 0401 06ff 0202 1201 0401 0a01 08ff 1cfc  ................
-00001660: 0280 1cfd 0a0a 1001 7a37 5465 7374 5061  ........z7TestPa
-00001670: 7274 6974 696f 6e4d 6b66 734d 6f75 6e74  rtitionMkfsMount
-00001680: 2e74 6573 745f 666f 7263 655f 756e 6d6f  .test_force_unmo
-00001690: 756e 745f 6765 745f 7069 6473 5f66 6169  unt_get_pids_fai
-000016a0: 6c63 0100 0000 0000 0000 0000 0000 0300  lc..............
-000016b0: 0000 0800 0000 4300 0000 7362 0000 0074  ......C...sb...t
-000016c0: 0064 0183 018f 0c7d 017c 01a0 01a1 007d  .d.....}.|.....}
-000016d0: 0257 0064 0204 0004 0083 0301 006e 0831  .W.d.........n.1
-000016e0: 0073 1377 0101 0001 0001 0059 0001 007c  .s.w.......Y...|
-000016f0: 00a0 027c 006a 037c 02a1 0201 007c 00a0  ...|.j.|.....|..
-00001700: 0474 056a 067c 006a 076a 08a1 0201 007c  .t.j.|.j.j.....|
-00001710: 00a0 027c 006a 037c 02a1 0201 0064 0253  ...|.j.|.....d.S
-00001720: 0029 037a 2843 6865 636b 2074 6865 2061  .).z(Check the a
-00001730: 7474 656d 7074 2066 6f72 2073 6563 6f6e  ttempt for secon
-00001740: 6420 6d6f 756e 7420 6661 696c 7372 0f00  d mount failsr..
-00001750: 0000 4e29 0972 3500 0000 7236 0000 0072  ..N).r5...r6...r
-00001760: 3700 0000 721e 0000 0072 5900 0000 7202  7...r....rY...r.
-00001770: 0000 0072 5a00 0000 7215 0000 0072 1000  ...rZ...r....r..
-00001780: 0000 723a 0000 0072 0b00 0000 720b 0000  ..r:...r....r...
-00001790: 0072 0c00 0000 da11 7465 7374 5f64 6f75  .r......test_dou
-000017a0: 626c 655f 6d6f 756e 74b5 0000 0073 0c00  ble_mount....s..
-000017b0: 0000 0a02 0a01 1cff 0e02 1201 1201 7a28  ..............z(
-000017c0: 5465 7374 5061 7274 6974 696f 6e4d 6b66  TestPartitionMkf
-000017d0: 734d 6f75 6e74 2e74 6573 745f 646f 7562  sMount.test_doub
-000017e0: 6c65 5f6d 6f75 6e74 6301 0000 0000 0000  le_mountc.......
-000017f0: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
-00001800: 0073 d200 0000 7400 6401 8301 8f0c 7d01  .s....t.d.....}.
-00001810: 7c01 a001 a100 7d02 5700 6402 0400 0400  |.....}.W.d.....
-00001820: 8303 0100 6e08 3100 7313 7701 0100 0100  ....n.1.s.w.....
-00001830: 0100 5900 0100 7c00 a002 7c00 6a03 7c02  ..Y...|...|.j.|.
-00001840: a102 0100 7c00 6a04 a005 a100 0100 7400  ....|.j.......t.
-00001850: 6401 8301 8f0c 7d01 7c01 a001 a100 7d02  d.....}.|.....}.
-00001860: 5700 6402 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
-00001870: 7337 7701 0100 0100 0100 5900 0100 7c00  s7w.......Y...|.
-00001880: a006 7c00 6a03 7c02 a102 0100 7c00 6a04  ..|.j.|.....|.j.
-00001890: a005 a100 0100 7400 6401 8301 8f0c 7d01  ......t.d.....}.
-000018a0: 7c01 a001 a100 7d02 5700 6402 0400 0400  |.....}.W.d.....
-000018b0: 8303 0100 6e08 3100 735b 7701 0100 0100  ....n.1.s[w.....
-000018c0: 0100 5900 0100 7c00 a006 7c00 6a03 7c02  ..Y...|...|.j.|.
-000018d0: a102 0100 6402 5300 2903 7a1f 4368 6563  ....d.S.).z.Chec
-000018e0: 6b20 646f 7562 6c65 2075 6e6d 6f75 6e74  k double unmount
-000018f0: 2077 6f72 6b73 2077 656c 6c72 0f00 0000   works wellr....
-00001900: 4e29 0772 3500 0000 7236 0000 0072 3700  N).r5...r6...r7.
-00001910: 0000 721e 0000 0072 1500 0000 7223 0000  ..r....r....r#..
-00001920: 0072 3900 0000 723a 0000 0072 0b00 0000  .r9...r:...r....
-00001930: 720b 0000 0072 0c00 0000 da12 7465 7374  r....r......test
-00001940: 5f64 6f75 626c 655f 756d 6f75 6e74 bd00  _double_umount..
-00001950: 0000 731c 0000 000a 020a 011c ff0e 020a  ..s.............
-00001960: 010a 010a 011c ff0e 020a 010a 010a 011c  ................
-00001970: ff12 027a 2954 6573 7450 6172 7469 7469  ...z)TestPartiti
-00001980: 6f6e 4d6b 6673 4d6f 756e 742e 7465 7374  onMkfsMount.test
-00001990: 5f64 6f75 626c 655f 756d 6f75 6e74 6301  _double_umountc.
-000019a0: 0000 0000 0000 0000 0000 0003 0000 0008  ................
-000019b0: 0000 0043 0000 0073 5400 0000 7400 6401  ...C...sT...t.d.
-000019c0: 8301 8f0c 7d01 7c01 a001 a100 7d02 5700  ....}.|.....}.W.
-000019d0: 6402 0400 0400 8303 0100 6e08 3100 7313  d.........n.1.s.
-000019e0: 7701 0100 0100 0100 5900 0100 7c00 a002  w.......Y...|...
-000019f0: 7c00 6a03 7c02 a102 0100 7c00 a004 7405  |.j.|.....|...t.
-00001a00: 6a06 7c00 6a07 6a08 a102 0100 6402 5300  j.|.j.j.....d.S.
-00001a10: 2903 7a24 4368 6563 6b20 666f 726d 6174  ).z$Check format
-00001a20: 206f 6e20 6d6f 756e 7465 6420 6465 7669   on mounted devi
-00001a30: 6365 2066 6169 6c73 720f 0000 004e 2909  ce failsr....N).
-00001a40: 7235 0000 0072 3600 0000 7237 0000 0072  r5...r6...r7...r
-00001a50: 1e00 0000 7259 0000 0072 0200 0000 725a  ....rY...r....rZ
-00001a60: 0000 0072 1500 0000 7234 0000 0072 3a00  ...r....r4...r:.
-00001a70: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00001a80: 00da 1374 6573 745f 666f 726d 6174 5f6d  ...test_format_m
-00001a90: 6f75 6e74 6564 cb00 0000 730a 0000 000a  ounted....s.....
-00001aa0: 020a 011c ff0e 0216 017a 2a54 6573 7450  .........z*TestP
-00001ab0: 6172 7469 7469 6f6e 4d6b 6673 4d6f 756e  artitionMkfsMoun
-00001ac0: 742e 7465 7374 5f66 6f72 6d61 745f 6d6f  t.test_format_mo
-00001ad0: 756e 7465 6429 1572 2700 0000 7228 0000  unted).r'...r(..
-00001ae0: 0072 2900 0000 722a 0000 0072 2100 0000  .r)...r*...r!...
-00001af0: 7253 0000 0072 2b00 0000 722c 0000 0072  rS...r+...r,...r
-00001b00: 0d00 0000 7204 0000 0072 2e00 0000 7242  ....r....r....rB
-00001b10: 0000 0072 4300 0000 7257 0000 0072 2f00  ...rC...rW...r/.
-00001b20: 0000 725b 0000 0072 6100 0000 7262 0000  ..r[...ra...rb..
-00001b30: 0072 6300 0000 7264 0000 00da 0d5f 5f63  .rc...rd.....__c
-00001b40: 6c61 7373 6365 6c6c 5f5f 720b 0000 0072  lasscell__r....r
-00001b50: 0b00 0000 7245 0000 0072 0c00 0000 723e  ....rE...r....r>
-00001b60: 0000 0056 0000 0073 3600 0000 0800 0402  ...V...s6.......
-00001b70: 0c04 080b 0e0e 0401 1001 0201 02fe 0404  ................
-00001b80: 0c01 02ff 0e03 0413 1001 0201 02fe 0e04  ................
-00001b90: 0c01 0409 1001 0201 02fe 0a04 0813 0808  ................
-00001ba0: 100e 723e 0000 007a 092f 6574 632f 6d74  ..r>...z./etc/mt
-00001bb0: 6162 7a1d 6d61 634f 5320 646f 6573 206e  abz.macOS does n
-00001bc0: 6f74 2068 6176 6520 2f65 7463 2f6d 7461  ot have /etc/mta
-00001bd0: 6263 0000 0000 0000 0000 0000 0000 0000  bc..............
-00001be0: 0000 0200 0000 4000 0000 7318 0000 0065  ......@...s....e
-00001bf0: 005a 0164 005a 0264 015a 0364 0264 0384  .Z.d.Z.d.Z.d.d..
-00001c00: 005a 0464 0453 0029 05da 0c54 6573 744d  .Z.d.S.)...TestM
-00001c10: 7461 624c 6f63 6b7a 300a 2020 2020 556e  tabLockz0.    Un
-00001c20: 6974 2074 6573 7473 2066 6f72 2061 766f  it tests for avo
-00001c30: 6361 646f 2e75 7469 6c73 2e70 6172 7469  cado.utils.parti
-00001c40: 7469 6f6e 0a20 2020 2063 0100 0000 0000  tion.    c......
-00001c50: 0000 0000 0000 0100 0000 0900 0000 4300  ..............C.
-00001c60: 0000 738e 0000 0074 00a0 01a1 008f 3901  ..s....t......9.
-00001c70: 0074 026a 03a0 0464 0174 026a 036a 0567  .t.j...d.t.j.j.g
-00001c80: 0064 02a2 0164 038d 01a1 028f 1201 007c  .d...d.........|
-00001c90: 00a0 0674 006a 0774 00a0 01a1 006a 08a1  ...t.j.t.....j..
-00001ca0: 0201 0057 0064 0404 0004 0083 0301 006e  ...W.d.........n
-00001cb0: 1031 0073 2877 0101 0001 0001 0059 0001  .1.s(w.......Y..
-00001cc0: 0057 0064 0404 0004 0083 0301 0064 0453  .W.d.........d.S
-00001cd0: 0057 0064 0404 0004 0083 0301 0064 0453  .W.d.........d.S
-00001ce0: 0031 0073 4077 0101 0001 0001 0059 0001  .1.s@w.......Y..
-00001cf0: 0064 0453 0029 057a 3643 6865 636b 2064  .d.S.).z6Check d
-00001d00: 6f75 626c 652d 6c6f 636b 2072 6169 7365  ouble-lock raise
-00001d10: 7320 6578 6365 7074 696f 6e20 6166 7465  s exception afte
-00001d20: 7220 3630 7320 2869 6e20 302e 3173 297a  r 60s (in 0.1s)z
-00001d30: 2061 766f 6361 646f 2e75 7469 6c73 2e66   avocado.utils.f
-00001d40: 696c 656c 6f63 6b2e 7469 6d65 2e74 696d  ilelock.time.tim
-00001d50: 6529 0372 1700 0000 e902 0000 00e9 3e00  e).r..........>.
-00001d60: 0000 725c 0000 004e 2909 7202 0000 005a  ..r\...N).r....Z
-00001d70: 084d 7461 624c 6f63 6b72 2b00 0000 725d  .MtabLockr+...r]
-00001d80: 0000 0072 5e00 0000 5a09 4d61 6769 634d  ...r^...Z.MagicM
-00001d90: 6f63 6b72 5900 0000 725a 0000 00da 095f  ockrY...rZ....._
-00001da0: 5f65 6e74 6572 5f5f 7225 0000 0072 0b00  _enter__r%...r..
-00001db0: 0000 720b 0000 0072 0c00 0000 da09 7465  ..r....r......te
-00001dc0: 7374 5f6c 6f63 6bda 0000 0073 1800 0000  st_lock....s....
-00001dd0: 0a02 0601 0201 1001 06fe 0404 0c01 06ff  ................
-00001de0: 1efc 0eff 0201 22ff 7a16 5465 7374 4d74  ......".z.TestMt
-00001df0: 6162 4c6f 636b 2e74 6573 745f 6c6f 636b  abLock.test_lock
-00001e00: 4e29 0572 2700 0000 7228 0000 0072 2900  N).r'...r(...r).
-00001e10: 0000 722a 0000 0072 6a00 0000 720b 0000  ..r*...rj...r...
-00001e20: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00001e30: 7266 0000 00d3 0000 0073 0600 0000 0800  rf.......s......
-00001e40: 0403 0c04 7266 0000 00da 085f 5f6d 6169  ....rf.....__mai
-00001e50: 6e5f 5f29 1872 2a00 0000 721b 0000 0072  n__).r*...r....r
-00001e60: 4200 0000 7218 0000 005a 0d75 6e69 7474  B...r....Z.unitt
-00001e70: 6573 742e 6d6f 636b 722b 0000 00da 0d61  est.mockr+.....a
-00001e80: 766f 6361 646f 2e75 7469 6c73 7202 0000  vocado.utilsr...
-00001e90: 0072 0300 0000 7207 0000 0072 0400 0000  .r....r....r....
-00001ea0: 7205 0000 005a 0f73 656c 6674 6573 7473  r....Z.selftests
-00001eb0: 2e75 7469 6c73 7206 0000 0072 0d00 0000  .utilsr....r....
-00001ec0: da08 5465 7374 4361 7365 720e 0000 0072  ..TestCaser....r
-00001ed0: 3200 0000 723e 0000 0072 2c00 0000 722d  2...r>...r,...r-
-00001ee0: 0000 0072 6600 0000 7227 0000 00da 046d  ...rf...r'.....m
-00001ef0: 6169 6e72 0b00 0000 720b 0000 0072 0b00  ainr....r....r..
-00001f00: 0000 720c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00001f10: 3e01 0000 0073 2400 0000 0400 0806 0801  >....s$.........
-00001f20: 0801 0801 0c02 0c01 1001 0c01 0803 1208  ................
-00001f30: 102c 1010 147d 1401 0812 0c01 04ff       .,...}........
+00000330: 640d 640e 8400 8301 8301 8301 8301 8301  d.d.............
+00000340: 5a0f 640f 6410 8400 5a10 6411 5300 2912  Z.d.d...Z.d.S.).
+00000350: da04 4261 7365 7a33 0a20 2020 2043 6f6d  ..Basez3.    Com
+00000360: 6d6f 6e20 7365 7455 702f 7465 6172 446f  mon setUp/tearDo
+00000370: 776e 2066 6f72 2070 6172 7469 7469 6f6e  wn for partition
+00000380: 2074 6573 7473 0a20 2020 20fa 0c2f 7072   tests.    ../pr
+00000390: 6f63 2f6d 6f75 6e74 737a 2173 7973 7465  oc/mountsz!syste
+000003a0: 6d20 646f 6573 206e 6f74 2068 6176 6520  m does not have 
+000003b0: 2f70 726f 632f 6d6f 756e 7473 da05 6d6f  /proc/mounts..mo
+000003c0: 756e 747a 3663 7572 7265 6e74 2075 7365  untz6current use
+000003d0: 7220 6d75 7374 2062 6520 616c 6c6f 7765  r must be allowe
+000003e0: 6420 746f 2072 756e 2022 6d6f 756e 7422  d to run "mount"
+000003f0: 2075 6e64 6572 2073 7564 6f7a 0c6d 6b66   under sudoz.mkf
+00000400: 732e 6578 7432 202d 567a 3a63 7572 7265  s.ext2 -Vz:curre
+00000410: 6e74 2075 7365 7220 6d75 7374 2062 6520  nt user must be 
+00000420: 616c 6c6f 7765 6420 746f 2072 756e 2022  allowed to run "
+00000430: 6d6b 6673 2e65 7874 3222 2075 6e64 6572  mkfs.ext2" under
+00000440: 2073 7564 6f7a 096d 6b66 732e 6578 7432   sudoz.mkfs.ext2
+00000450: 467a 236d 6b66 732e 6578 7432 2075 7469  Fz#mkfs.ext2 uti
+00000460: 6c69 7479 206d 7573 7420 6265 2061 7661  lity must be ava
+00000470: 696c 6162 6c65 5a0d 6361 705f 7379 735f  ilableZ.cap_sys_
+00000480: 6164 6d69 6e7a 2f43 6170 6162 696c 6974  adminz/Capabilit
+00000490: 7920 746f 206d 6f75 6e74 2069 7320 7265  y to mount is re
+000004a0: 7175 6972 6564 2028 6361 705f 7379 735f  quired (cap_sys_
+000004b0: 6164 6d69 6e29 6301 0000 0000 0000 0000  admin)c.........
+000004c0: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
+000004d0: 5a00 0000 7400 7c00 8301 7d01 7401 6a02  Z...t.|...}.t.j.
+000004e0: 7c01 6401 8d01 7c00 5f03 7404 6a05 a006  |.d...|._.t.j...
+000004f0: 7c00 6a03 6a07 6402 a102 7c00 5f08 7404  |.j.j.d...|._.t.
+00000500: a009 7c00 6a08 a101 0100 740a a00b 7404  ..|.j.....t...t.
+00000510: 6a05 a006 7c00 6a03 6a07 6403 a102 6404  j...|.j.j.d...d.
+00000520: 7c00 6a08 a103 7c00 5f0c 6400 5300 2905  |.j...|._.d.S.).
+00000530: 4e29 01da 0670 7265 6669 78da 0464 6973  N)...prefix..dis
+00000540: 6bda 0562 6c6f 636b e901 0000 0029 0d72  k..block.....).r
+00000550: 0600 0000 da08 7465 6d70 6669 6c65 da12  ......tempfile..
+00000560: 5465 6d70 6f72 6172 7944 6972 6563 746f  TemporaryDirecto
+00000570: 7279 da06 746d 7064 6972 da02 6f73 7203  ry..tmpdir..osr.
+00000580: 0000 00da 046a 6f69 6eda 046e 616d 65da  .....join..name.
+00000590: 0a6d 6f75 6e74 706f 696e 74da 056d 6b64  .mountpoint..mkd
+000005a0: 6972 7202 0000 005a 0950 6172 7469 7469  irr....Z.Partiti
+000005b0: 6f6e 7212 0000 0029 02da 0473 656c 6672  onr....)...selfr
+000005c0: 1100 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
+000005d0: 0000 00da 0573 6574 5570 2000 0000 730e  .....setUp ...s.
+000005e0: 0000 0008 140e 0114 010c 0104 0116 010a  ................
+000005f0: ff7a 0a42 6173 652e 7365 7455 7063 0100  .z.Base.setUpc..
+00000600: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000610: 0000 4300 0000 7318 0000 007c 006a 00a0  ..C...s....|.j..
+00000620: 01a1 0001 007c 006a 02a0 03a1 0001 0064  .....|.j.......d
+00000630: 0053 00a9 014e 2904 7212 0000 00da 0775  .S...N).r......u
+00000640: 6e6d 6f75 6e74 7217 0000 00da 0763 6c65  nmountr......cle
+00000650: 616e 7570 a901 721d 0000 0072 0b00 0000  anup..r....r....
+00000660: 720b 0000 0072 0c00 0000 da08 7465 6172  r....r......tear
+00000670: 446f 776e 3c00 0000 7304 0000 000a 010e  Down<...s.......
+00000680: 017a 0d42 6173 652e 7465 6172 446f 776e  .z.Base.tearDown
+00000690: 4e29 11da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+000006a0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000006b0: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+000006c0: da08 756e 6974 7465 7374 da06 736b 6970  ..unittest..skip
+000006d0: 4966 7218 0000 0072 0300 0000 da06 6973  Ifr....r......is
+000006e0: 6669 6c65 7204 0000 00da 0863 616e 5f73  filer......can_s
+000006f0: 7564 6fda 0a73 6b69 7055 6e6c 6573 7372  udo..skipUnlessr
+00000700: 0700 0000 7208 0000 00da 0e68 6173 5f63  ....r......has_c
+00000710: 6170 6162 696c 6974 7972 1e00 0000 7223  apabilityr....r#
+00000720: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
+00000730: 0000 720c 0000 0072 0e00 0000 1a00 0000  ..r....r........
+00000740: 732e 0000 0008 0004 0204 040e 0102 ff04  s...............
+00000750: 030a 0102 0102 fe04 040a 0102 0102 fe04  ................
+00000760: 040a 0102 0102 fe04 0408 0102 0102 fe12  ................
+00000770: 040c 0972 0e00 0000 6300 0000 0000 0000  ...r....c.......
+00000780: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
+00000790: 0073 1400 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+000007a0: 6402 8400 5a03 6403 5300 2904 da0d 5465  d...Z.d.S.)...Te
+000007b0: 7374 5061 7274 6974 696f 6e63 0100 0000  stPartitionc....
+000007c0: 0000 0000 0000 0000 0300 0000 0800 0000  ................
+000007d0: 4300 0000 73c2 0000 007c 00a0 007c 006a  C...s....|...|.j
+000007e0: 01a0 02a1 00a1 0101 007c 006a 01a0 03a1  .........|.j....
+000007f0: 0001 007c 006a 01a0 04a1 0001 0074 0564  ...|.j.......t.d
+00000800: 0183 018f 0c7d 017c 01a0 06a1 007d 0257  .....}.|.....}.W
+00000810: 0064 0204 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+00000820: 2577 0101 0001 0001 0059 0001 007c 00a0  %w.......Y...|..
+00000830: 077c 006a 087c 02a1 0201 007c 00a0 097c  .|.j.|.....|...|
+00000840: 006a 087c 006a 01a0 02a1 00a1 0201 007c  .j.|.j.........|
+00000850: 006a 01a0 0aa1 0001 0074 0564 0183 018f  .j.......t.d....
+00000860: 0c7d 017c 01a0 06a1 007d 0257 0064 0204  .}.|.....}.W.d..
+00000870: 0004 0083 0301 006e 0831 0073 5377 0101  .......n.1.sSw..
+00000880: 0001 0001 0059 0001 007c 00a0 0b7c 006a  .....Y...|...|.j
+00000890: 087c 02a1 0201 0064 0253 0029 037a 1754  .|.....d.S.).z.T
+000008a0: 6573 7420 7468 6520 6261 7369 6320 776f  est the basic wo
+000008b0: 726b 666c 6f77 720f 0000 004e 290c da0c  rkflowr....N)...
+000008c0: 6173 7365 7274 4973 4e6f 6e65 7212 0000  assertIsNoner...
+000008d0: 005a 0e67 6574 5f6d 6f75 6e74 706f 696e  .Z.get_mountpoin
+000008e0: 74da 046d 6b66 7372 1000 0000 da04 6f70  t..mkfsr......op
+000008f0: 656e da04 7265 6164 da08 6173 7365 7274  en..read..assert
+00000900: 496e 721b 0000 00da 0b61 7373 6572 7445  Inr......assertE
+00000910: 7175 616c 7220 0000 00da 0b61 7373 6572  qualr .....asser
+00000920: 744e 6f74 496e a903 721d 0000 00da 1070  tNotIn..r......p
+00000930: 726f 635f 6d6f 756e 7473 5f66 696c 65da  roc_mounts_file.
+00000940: 0b70 726f 635f 6d6f 756e 7473 720b 0000  .proc_mountsr...
+00000950: 0072 0b00 0000 720c 0000 00da 0a74 6573  .r....r......tes
+00000960: 745f 6261 7369 6342 0000 0073 1a00 0000  t_basicB...s....
+00000970: 1002 0a01 0a01 0a01 0a01 1cff 0e02 1401  ................
+00000980: 0a01 0a01 0a01 1cff 1202 7a18 5465 7374  ..........z.Test
+00000990: 5061 7274 6974 696f 6e2e 7465 7374 5f62  Partition.test_b
+000009a0: 6173 6963 4e29 0472 2400 0000 7225 0000  asicN).r$...r%..
+000009b0: 0072 2600 0000 7239 0000 0072 0b00 0000  .r&...r9...r....
+000009c0: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+000009d0: 2e00 0000 4100 0000 7304 0000 0008 000c  ....A...s.......
+000009e0: 0172 2e00 0000 6300 0000 0000 0000 0000  .r....c.........
+000009f0: 0000 0000 0000 0007 0000 0000 0000 0073  ...............s
+00000a00: da00 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00000a10: 8700 6601 6402 6403 8408 5a04 6404 6405  ..f.d.d...Z.d.d.
+00000a20: 8400 5a05 6506 a007 6508 6406 8301 6407  ..Z.e...e.d...d.
+00000a30: a102 6506 a007 6509 a00a 650b 6a0c 6408  ..e...e...e.j.d.
+00000a40: 1700 a101 0c00 6409 a102 6506 a007 6509  ......d...e...e.
+00000a50: a00a 640a a101 0c00 640b a102 640c 640d  ..d.....d...d.d.
+00000a60: 8400 8301 8301 8301 5a0d 6506 a007 6509  ........Z.e...e.
+00000a70: a00a 650b 6a0c 6408 1700 a101 0c00 6409  ..e.j.d.......d.
+00000a80: a102 6506 a00e 6508 6406 8301 640e a102  ..e...e.d...d...
+00000a90: 640f 6410 8400 8301 8301 5a0f 6506 a007  d.d.......Z.e...
+00000aa0: 6509 a00a 650b 6a0c 6408 1700 a101 0c00  e...e.j.d.......
+00000ab0: 6409 a102 6411 6412 8400 8301 5a10 6413  d...d.d.....Z.d.
+00000ac0: 6414 8400 5a11 6415 6416 8400 5a12 6417  d...Z.d.d...Z.d.
+00000ad0: 6418 8400 5a13 8700 0400 5a14 5300 2919  d...Z.....Z.S.).
+00000ae0: da16 5465 7374 5061 7274 6974 696f 6e4d  ..TestPartitionM
+00000af0: 6b66 734d 6f75 6e74 7a3e 0a20 2020 2054  kfsMountz>.    T
+00000b00: 6573 7473 2074 6861 7420 6173 7375 6d65  ests that assume
+00000b10: 2061 2066 696c 6573 7973 7465 6d20 616e   a filesystem an
+00000b20: 6420 6d6f 756e 7465 6420 7061 7274 6974  d mounted partit
+00000b30: 696f 6e0a 2020 2020 6301 0000 0000 0000  ion.    c.......
+00000b40: 0000 0000 0001 0000 0004 0000 0003 0000  ................
+00000b50: 0073 4a00 0000 7400 8300 a001 a100 0100  .sJ...t.........
+00000b60: 7c00 6a02 a003 a100 0100 7c00 6a02 a004  |.j.......|.j...
+00000b70: a100 0100 7405 6a06 a007 7c00 6a08 6401  ....t.j...|.j.d.
+00000b80: a102 7c00 5f09 740a 6a0b 9b00 6402 7c00  ..|._.t.j...d.|.
+00000b90: 6a09 9b00 6403 9d04 7c00 5f0c 6400 5300  j...d...|._.d.S.
+00000ba0: 2904 4eda 0466 696c 657a 1c20 2d63 2027  ).N..filez. -c '
+00000bb0: 696d 706f 7274 2074 696d 653b 2066 203d  import time; f =
+00000bc0: 206f 7065 6e28 227a 1822 2c20 2277 2229   open("z.", "w")
+00000bd0: 3b20 7469 6d65 2e73 6c65 6570 2836 3029  ; time.sleep(60)
+00000be0: 2729 0dda 0573 7570 6572 721e 0000 0072  ')...superr....r
+00000bf0: 1200 0000 7230 0000 0072 1000 0000 7218  ....r0...r....r.
+00000c00: 0000 0072 0300 0000 7219 0000 0072 1b00  ...r....r....r..
+00000c10: 0000 da0c 7573 655f 6d6e 745f 6669 6c65  ....use_mnt_file
+00000c20: da03 7379 73da 0a65 7865 6375 7461 626c  ..sys..executabl
+00000c30: 65da 0b75 7365 5f6d 6e74 5f63 6d64 7222  e..use_mnt_cmdr"
+00000c40: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
+00000c50: 720b 0000 0072 0c00 0000 721e 0000 0057  r....r....r....W
+00000c60: 0000 0073 1000 0000 0a01 0a01 0a01 1201  ...s............
+00000c70: 0802 0401 06ff 08ff 7a1c 5465 7374 5061  ........z.TestPa
+00000c80: 7274 6974 696f 6e4d 6b66 734d 6f75 6e74  rtitionMkfsMount
+00000c90: 2e73 6574 5570 6301 0000 0000 0000 0000  .setUpc.........
+00000ca0: 0000 0002 0000 0008 0000 0003 0000 0073  ...............s
+00000cb0: 3e00 0000 7400 6a01 8800 6a02 6401 6402  >...t.j...j.d.d.
+00000cc0: 8d02 7d01 7c01 a003 a100 0100 8800 a004  ..}.|...........
+00000cd0: 7405 6a06 8700 6601 6403 6404 8408 6405  t.j...f.d.d...d.
+00000ce0: 6406 6406 6407 8d04 6408 a102 0100 7c01  d.d.d...d.....|.
+00000cf0: 5300 2909 4e54 a901 da04 7375 646f 6300  S.).NT....sudoc.
+00000d00: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000d10: 0000 0013 0000 0073 0e00 0000 7400 6a01  .......s....t.j.
+00000d20: a002 8800 6a03 a101 5300 721f 0000 0029  ....j...S.r....)
+00000d30: 0472 1800 0000 7203 0000 00da 0665 7869  .r....r......exi
+00000d40: 7374 7372 3d00 0000 720b 0000 0072 2200  stsr=...r....r".
+00000d50: 0000 720b 0000 0072 0c00 0000 da08 3c6c  ..r....r......<l
+00000d60: 616d 6264 613e 6700 0000 7302 0000 000e  ambda>g...s.....
+00000d70: 007a 3f54 6573 7450 6172 7469 7469 6f6e  .z?TestPartition
+00000d80: 4d6b 6673 4d6f 756e 742e 7275 6e5f 7072  MkfsMount.run_pr
+00000d90: 6f63 6573 735f 746f 5f75 7365 5f6d 6e74  ocess_to_use_mnt
+00000da0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00000db0: 613e 7214 0000 0067 9a99 9999 9999 b93f  a>r....g.......?
+00000dc0: 2903 da07 7469 6d65 6f75 74da 0566 6972  )...timeout..fir
+00000dd0: 7374 da04 7374 6570 7a26 4669 6c65 2077  st..stepz&File w
+00000de0: 6173 206e 6f74 2063 7265 6174 6564 2077  as not created w
+00000df0: 6974 6869 6e20 6d6f 756e 7470 6f69 6e74  ithin mountpoint
+00000e00: 2907 7204 0000 00da 0a53 7562 5072 6f63  ).r......SubProc
+00000e10: 6573 7372 4000 0000 da05 7374 6172 74da  essr@.....start.
+00000e20: 0a61 7373 6572 7454 7275 6572 0500 0000  .assertTruer....
+00000e30: da08 7761 6974 5f66 6f72 2902 721d 0000  ..wait_for).r...
+00000e40: 00da 0470 726f 6372 0b00 0000 7222 0000  ...procr....r"..
+00000e50: 0072 0c00 0000 da16 7275 6e5f 7072 6f63  .r......run_proc
+00000e60: 6573 735f 746f 5f75 7365 5f6d 6e74 6200  ess_to_use_mntb.
+00000e70: 0000 7318 0000 0010 0108 0104 0104 010a  ..s.............
+00000e80: 0102 0102 0102 0104 fc02 0604 f904 097a  ...............z
+00000e90: 2d54 6573 7450 6172 7469 7469 6f6e 4d6b  -TestPartitionMk
+00000ea0: 6673 4d6f 756e 742e 7275 6e5f 7072 6f63  fsMount.run_proc
+00000eb0: 6573 735f 746f 5f75 7365 5f6d 6e74 5a04  ess_to_use_mntZ.
+00000ec0: 6c73 6f66 7a15 7265 7175 6972 6573 2072  lsofz.requires r
+00000ed0: 756e 6e69 6e67 206c 736f 667a 0620 2d63  unning lsofz. -c
+00000ee0: 2027 277a 2c72 6571 7569 7265 7320 7275   ''z,requires ru
+00000ef0: 6e6e 696e 6720 5079 7468 6f6e 2061 7320  nning Python as 
+00000f00: 6120 7072 6976 696c 6567 6564 2075 7365  a privileged use
+00000f10: 727a 076b 696c 6c20 2d6c 7a2a 7265 7175  rz.kill -lz*requ
+00000f20: 6972 6573 2072 756e 6e69 6e67 206b 696c  ires running kil
+00000f30: 6c20 6173 2061 2070 7269 7669 6c65 6765  l as a privilege
+00000f40: 6420 7573 6572 6301 0000 0000 0000 0000  d userc.........
+00000f50: 0000 0004 0000 0008 0000 0043 0000 0073  ...........C...s
+00000f60: ae00 0000 7400 6401 8301 8f0c 7d01 7c01  ....t.d.....}.|.
+00000f70: a001 a100 7d02 5700 6402 0400 0400 8303  ....}.W.d.......
+00000f80: 0100 6e08 3100 7313 7701 0100 0100 0100  ..n.1.s.w.......
+00000f90: 5900 0100 7c00 a002 7c00 6a03 7c02 a102  Y...|...|.j.|...
+00000fa0: 0100 7c00 a004 a100 7d03 7c00 a005 7c00  ..|.....}.|...|.
+00000fb0: 6a06 a007 a100 a101 0100 7c00 a002 7c03  j.........|...|.
+00000fc0: a008 a100 6403 6404 6702 6405 a103 0100  ....d.d.g.d.....
+00000fd0: 7400 6401 8301 8f0c 7d01 7c01 a001 a100  t.d.....}.|.....
+00000fe0: 7d02 5700 6402 0400 0400 8303 0100 6e08  }.W.d.........n.
+00000ff0: 3100 7349 7701 0100 0100 0100 5900 0100  1.sIw.......Y...
+00001000: 7c00 a009 7c00 6a03 7c02 a102 0100 6402  |...|.j.|.....d.
+00001010: 5300 2906 7a1a 5465 7374 2066 6f72 6365  S.).z.Test force
+00001020: 2d75 6e6d 6f75 6e74 2066 6561 7475 7265  -unmount feature
+00001030: 720f 0000 004e 69f7 ffff ffe9 8900 0000  r....Ni.........
+00001040: 7a47 556e 6578 7065 6374 6564 2072 6574  zGUnexpected ret
+00001050: 7572 6e20 636f 6465 2077 6865 6e20 7472  urn code when tr
+00001060: 7969 6e67 2074 6f20 6b69 6c6c 2070 726f  ying to kill pro
+00001070: 6365 7373 2075 7369 6e67 2074 6865 206d  cess using the m
+00001080: 6f75 6e74 706f 696e 7429 0a72 3100 0000  ountpoint).r1...
+00001090: 7232 0000 0072 3300 0000 721b 0000 0072  r2...r3...r....r
+000010a0: 4f00 0000 724c 0000 0072 1200 0000 7220  O...rL...r....r 
+000010b0: 0000 00da 0470 6f6c 6c72 3500 0000 a904  .....pollr5.....
+000010c0: 721d 0000 0072 3700 0000 7238 0000 0072  r....r7...r8...r
+000010d0: 4e00 0000 720b 0000 0072 0b00 0000 720c  N...r....r....r.
+000010e0: 0000 00da 1274 6573 745f 666f 7263 655f  .....test_force_
+000010f0: 756e 6d6f 756e 7470 0000 0073 1e00 0000  unmountp...s....
+00001100: 0a0a 0a01 1cff 0e02 0801 1001 0403 0601  ................
+00001110: 0601 0201 04fd 0a06 0a01 1cff 1202 7a29  ..............z)
+00001120: 5465 7374 5061 7274 6974 696f 6e4d 6b66  TestPartitionMkf
+00001130: 734d 6f75 6e74 2e74 6573 745f 666f 7263  sMount.test_forc
+00001140: 655f 756e 6d6f 756e 747a 1872 6571 7569  e_unmountz.requi
+00001150: 7265 7320 6e6f 7420 6861 7669 6e67 206c  res not having l
+00001160: 736f 6663 0100 0000 0000 0000 0000 0000  sofc............
+00001170: 0400 0000 0800 0000 4300 0000 7368 0000  ........C...sh..
+00001180: 0074 0064 0183 018f 0c7d 017c 01a0 01a1  .t.d.....}.|....
+00001190: 007d 0257 0064 0204 0004 0083 0301 006e  .}.W.d.........n
+000011a0: 0831 0073 1377 0101 0001 0001 0059 0001  .1.s.w.......Y..
+000011b0: 007c 00a0 027c 006a 037c 02a1 0201 007c  .|...|.j.|.....|
+000011c0: 00a0 04a1 007d 037c 00a0 0574 066a 077c  .....}.|...t.j.|
+000011d0: 006a 086a 09a1 0201 007c 036a 0a64 0364  .j.j.....|.j.d.d
+000011e0: 048d 0101 0064 0253 0029 057a 3d43 6865  .....d.S.).z=Che
+000011f0: 636b 7320 7468 6174 2061 2066 6f72 6365  cks that a force
+00001200: 2d75 6e6d 6f75 6e74 2077 696c 6c20 6661  -unmount will fa
+00001210: 696c 206f 6e20 7379 7374 656d 7320 7769  il on systems wi
+00001220: 7468 6f75 7420 6c73 6f66 720f 0000 004e  thout lsofr....N
+00001230: 7214 0000 00a9 0172 4700 0000 290b 7231  r......rG...).r1
+00001240: 0000 0072 3200 0000 7233 0000 0072 1b00  ...r2...r3...r..
+00001250: 0000 724f 0000 00da 0c61 7373 6572 7452  ..rO.....assertR
+00001260: 6169 7365 7372 0200 0000 da0e 5061 7274  aisesr......Part
+00001270: 6974 696f 6e45 7272 6f72 7212 0000 0072  itionErrorr....r
+00001280: 2000 0000 7205 0000 0072 5200 0000 720b   ...r....rR...r.
+00001290: 0000 0072 0b00 0000 720c 0000 00da 1a74  ...r....r......t
+000012a0: 6573 745f 666f 7263 655f 756e 6d6f 756e  est_force_unmoun
+000012b0: 745f 6e6f 5f6c 736f 668b 0000 0073 0e00  t_no_lsof....s..
+000012c0: 0000 0a07 0a01 1cff 0e02 0801 1201 1001  ................
+000012d0: 7a31 5465 7374 5061 7274 6974 696f 6e4d  z1TestPartitionM
+000012e0: 6b66 734d 6f75 6e74 2e74 6573 745f 666f  kfsMount.test_fo
+000012f0: 7263 655f 756e 6d6f 756e 745f 6e6f 5f6c  rce_unmount_no_l
+00001300: 736f 6663 0100 0000 0000 0000 0000 0000  sofc............
+00001310: 0500 0000 0900 0000 4300 0000 73e8 0000  ........C...s...
+00001320: 0074 0064 0183 018f 0c7d 017c 01a0 01a1  .t.d.....}.|....
+00001330: 007d 0257 0064 0204 0004 0083 0301 006e  .}.W.d.........n
+00001340: 0831 0073 1377 0101 0001 0001 0059 0001  .1.s.w.......Y..
+00001350: 007c 00a0 027c 006a 037c 02a1 0201 007c  .|...|.j.|.....|
+00001360: 00a0 04a1 007d 0374 056a 066a 0764 0374  .....}.t.j.j.d.t
+00001370: 086a 0964 048d 028f 3301 0074 056a 066a  .j.d....3..t.j.j
+00001380: 0764 0574 0a64 048d 028f 1b7d 047c 00a0  .d.t.d.....}.|..
+00001390: 0b74 0c6a 0d7c 006a 0e6a 0fa1 0201 007c  .t.j.|.j.j.....|
+000013a0: 046a 1064 067c 006a 0317 0064 0764 088d  .j.d.|.j...d.d..
+000013b0: 0201 0057 0064 0204 0004 0083 0301 006e  ...W.d.........n
+000013c0: 0831 0073 5377 0101 0001 0001 0059 0001  .1.sSw.......Y..
+000013d0: 0057 0064 0204 0004 0083 0301 006e 0831  .W.d.........n.1
+000013e0: 0073 6277 0101 0001 0001 0059 0001 007c  .sbw.......Y...|
+000013f0: 006a 0ea0 0fa1 0001 007c 036a 1164 0964  .j.......|.j.d.d
+00001400: 0a8d 0101 0064 0253 0029 0b7a 3e43 6865  .....d.S.).z>Che
+00001410: 636b 7320 5061 7274 6974 696f 6e45 7272  cks PartitionErr
+00001420: 6f72 2069 7320 7261 6973 6564 2069 6620  or is raised if 
+00001430: 7468 6572 6527 7320 6e6f 206c 736f 6620  there's no lsof 
+00001440: 746f 2067 6574 2070 6964 7372 0f00 0000  to get pidsr....
+00001450: 4e7a 2361 766f 6361 646f 2e75 7469 6c73  Nz#avocado.utils
+00001460: 2e70 6172 7469 7469 6f6e 2e70 726f 6365  .partition.proce
+00001470: 7373 2e72 756e a901 5a0b 7369 6465 5f65  ss.run..Z.side_e
+00001480: 6666 6563 747a 2d61 766f 6361 646f 2e75  ffectz-avocado.u
+00001490: 7469 6c73 2e70 6172 7469 7469 6f6e 2e70  tils.partition.p
+000014a0: 726f 6365 7373 2e73 7973 7465 6d5f 6f75  rocess.system_ou
+000014b0: 7470 7574 7a05 6c73 6f66 2054 7243 0000  tputz.lsof TrC..
+000014c0: 0072 1400 0000 7254 0000 0029 1272 3100  .r....rT...).r1.
+000014d0: 0000 7232 0000 0072 3300 0000 721b 0000  ..r2...r3...r...
+000014e0: 0072 4f00 0000 7228 0000 00da 046d 6f63  .rO...r(.....moc
+000014f0: 6bda 0570 6174 6368 7204 0000 00da 0843  k..patchr......C
+00001500: 6d64 4572 726f 72da 074f 5345 7272 6f72  mdError..OSError
+00001510: 7255 0000 0072 0200 0000 7256 0000 0072  rU...r....rV...r
+00001520: 1200 0000 7220 0000 005a 1261 7373 6572  ....r ...Z.asser
+00001530: 745f 6361 6c6c 6564 5f77 6974 6872 0500  t_called_withr..
+00001540: 0000 2905 721d 0000 0072 3700 0000 7238  ..).r....r7...r8
+00001550: 0000 0072 4e00 0000 5a14 6d6f 636b 6564  ...rN...Z.mocked
+00001560: 5f73 7973 7465 6d5f 6f75 7470 7574 720b  _system_outputr.
+00001570: 0000 0072 0b00 0000 720c 0000 00da 2074  ...r....r..... t
+00001580: 6573 745f 666f 7263 655f 756e 6d6f 756e  est_force_unmoun
+00001590: 745f 6765 745f 7069 6473 5f66 6169 6c99  t_get_pids_fail.
+000015a0: 0000 0073 2a00 0000 0a06 0a01 1cff 0e02  ...s*...........
+000015b0: 0801 0601 0601 08ff 0603 0401 06ff 0202  ................
+000015c0: 1201 0401 0a01 08ff 1cfc 0280 1cfd 0a0a  ................
+000015d0: 1001 7a37 5465 7374 5061 7274 6974 696f  ..z7TestPartitio
+000015e0: 6e4d 6b66 734d 6f75 6e74 2e74 6573 745f  nMkfsMount.test_
+000015f0: 666f 7263 655f 756e 6d6f 756e 745f 6765  force_unmount_ge
+00001600: 745f 7069 6473 5f66 6169 6c63 0100 0000  t_pids_failc....
+00001610: 0000 0000 0000 0000 0300 0000 0800 0000  ................
+00001620: 4300 0000 7362 0000 0074 0064 0183 018f  C...sb...t.d....
+00001630: 0c7d 017c 01a0 01a1 007d 0257 0064 0204  .}.|.....}.W.d..
+00001640: 0004 0083 0301 006e 0831 0073 1377 0101  .......n.1.s.w..
+00001650: 0001 0001 0059 0001 007c 00a0 027c 006a  .....Y...|...|.j
+00001660: 037c 02a1 0201 007c 00a0 0474 056a 067c  .|.....|...t.j.|
+00001670: 006a 076a 08a1 0201 007c 00a0 027c 006a  .j.j.....|...|.j
+00001680: 037c 02a1 0201 0064 0253 0029 037a 2843  .|.....d.S.).z(C
+00001690: 6865 636b 2074 6865 2061 7474 656d 7074  heck the attempt
+000016a0: 2066 6f72 2073 6563 6f6e 6420 6d6f 756e   for second moun
+000016b0: 7420 6661 696c 7372 0f00 0000 4e29 0972  t failsr....N).r
+000016c0: 3100 0000 7232 0000 0072 3300 0000 721b  1...r2...r3...r.
+000016d0: 0000 0072 5500 0000 7202 0000 0072 5600  ...rU...r....rV.
+000016e0: 0000 7212 0000 0072 1000 0000 7236 0000  ..r....r....r6..
+000016f0: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00001700: da11 7465 7374 5f64 6f75 626c 655f 6d6f  ..test_double_mo
+00001710: 756e 74b0 0000 0073 0c00 0000 0a02 0a01  unt....s........
+00001720: 1cff 0e02 1201 1201 7a28 5465 7374 5061  ........z(TestPa
+00001730: 7274 6974 696f 6e4d 6b66 734d 6f75 6e74  rtitionMkfsMount
+00001740: 2e74 6573 745f 646f 7562 6c65 5f6d 6f75  .test_double_mou
+00001750: 6e74 6301 0000 0000 0000 0000 0000 0003  ntc.............
+00001760: 0000 0008 0000 0043 0000 0073 d200 0000  .......C...s....
+00001770: 7400 6401 8301 8f0c 7d01 7c01 a001 a100  t.d.....}.|.....
+00001780: 7d02 5700 6402 0400 0400 8303 0100 6e08  }.W.d.........n.
+00001790: 3100 7313 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
+000017a0: 7c00 a002 7c00 6a03 7c02 a102 0100 7c00  |...|.j.|.....|.
+000017b0: 6a04 a005 a100 0100 7400 6401 8301 8f0c  j.......t.d.....
+000017c0: 7d01 7c01 a001 a100 7d02 5700 6402 0400  }.|.....}.W.d...
+000017d0: 0400 8303 0100 6e08 3100 7337 7701 0100  ......n.1.s7w...
+000017e0: 0100 0100 5900 0100 7c00 a006 7c00 6a03  ....Y...|...|.j.
+000017f0: 7c02 a102 0100 7c00 6a04 a005 a100 0100  |.....|.j.......
+00001800: 7400 6401 8301 8f0c 7d01 7c01 a001 a100  t.d.....}.|.....
+00001810: 7d02 5700 6402 0400 0400 8303 0100 6e08  }.W.d.........n.
+00001820: 3100 735b 7701 0100 0100 0100 5900 0100  1.s[w.......Y...
+00001830: 7c00 a006 7c00 6a03 7c02 a102 0100 6402  |...|.j.|.....d.
+00001840: 5300 2903 7a1f 4368 6563 6b20 646f 7562  S.).z.Check doub
+00001850: 6c65 2075 6e6d 6f75 6e74 2077 6f72 6b73  le unmount works
+00001860: 2077 656c 6c72 0f00 0000 4e29 0772 3100   wellr....N).r1.
+00001870: 0000 7232 0000 0072 3300 0000 721b 0000  ..r2...r3...r...
+00001880: 0072 1200 0000 7220 0000 0072 3500 0000  .r....r ...r5...
+00001890: 7236 0000 0072 0b00 0000 720b 0000 0072  r6...r....r....r
+000018a0: 0c00 0000 da12 7465 7374 5f64 6f75 626c  ......test_doubl
+000018b0: 655f 756d 6f75 6e74 b800 0000 731c 0000  e_umount....s...
+000018c0: 000a 020a 011c ff0e 020a 010a 010a 011c  ................
+000018d0: ff0e 020a 010a 010a 011c ff12 027a 2954  .............z)T
+000018e0: 6573 7450 6172 7469 7469 6f6e 4d6b 6673  estPartitionMkfs
+000018f0: 4d6f 756e 742e 7465 7374 5f64 6f75 626c  Mount.test_doubl
+00001900: 655f 756d 6f75 6e74 6301 0000 0000 0000  e_umountc.......
+00001910: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
+00001920: 0073 5400 0000 7400 6401 8301 8f0c 7d01  .sT...t.d.....}.
+00001930: 7c01 a001 a100 7d02 5700 6402 0400 0400  |.....}.W.d.....
+00001940: 8303 0100 6e08 3100 7313 7701 0100 0100  ....n.1.s.w.....
+00001950: 0100 5900 0100 7c00 a002 7c00 6a03 7c02  ..Y...|...|.j.|.
+00001960: a102 0100 7c00 a004 7405 6a06 7c00 6a07  ....|...t.j.|.j.
+00001970: 6a08 a102 0100 6402 5300 2903 7a24 4368  j.....d.S.).z$Ch
+00001980: 6563 6b20 666f 726d 6174 206f 6e20 6d6f  eck format on mo
+00001990: 756e 7465 6420 6465 7669 6365 2066 6169  unted device fai
+000019a0: 6c73 720f 0000 004e 2909 7231 0000 0072  lsr....N).r1...r
+000019b0: 3200 0000 7233 0000 0072 1b00 0000 7255  2...r3...r....rU
+000019c0: 0000 0072 0200 0000 7256 0000 0072 1200  ...r....rV...r..
+000019d0: 0000 7230 0000 0072 3600 0000 720b 0000  ..r0...r6...r...
+000019e0: 0072 0b00 0000 720c 0000 00da 1374 6573  .r....r......tes
+000019f0: 745f 666f 726d 6174 5f6d 6f75 6e74 6564  t_format_mounted
+00001a00: c600 0000 730a 0000 000a 020a 011c ff0e  ....s...........
+00001a10: 0216 017a 2a54 6573 7450 6172 7469 7469  ...z*TestPartiti
+00001a20: 6f6e 4d6b 6673 4d6f 756e 742e 7465 7374  onMkfsMount.test
+00001a30: 5f66 6f72 6d61 745f 6d6f 756e 7465 6429  _format_mounted)
+00001a40: 1572 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
+00001a50: 7227 0000 0072 1e00 0000 724f 0000 0072  r'...r....rO...r
+00001a60: 2800 0000 7229 0000 0072 0d00 0000 7204  (...r)...r....r.
+00001a70: 0000 0072 2b00 0000 723e 0000 0072 3f00  ...r+...r>...r?.
+00001a80: 0000 7253 0000 0072 2c00 0000 7257 0000  ..rS...r,...rW..
+00001a90: 0072 5d00 0000 725e 0000 0072 5f00 0000  .r]...r^...r_...
+00001aa0: 7260 0000 00da 0d5f 5f63 6c61 7373 6365  r`.....__classce
+00001ab0: 6c6c 5f5f 720b 0000 0072 0b00 0000 7241  ll__r....r....rA
+00001ac0: 0000 0072 0c00 0000 723a 0000 0051 0000  ...r....r:...Q..
+00001ad0: 0073 3600 0000 0800 0402 0c04 080b 0e0e  .s6.............
+00001ae0: 0401 1001 0201 02fe 0404 0c01 02ff 0e03  ................
+00001af0: 0413 1001 0201 02fe 0e04 0c01 0409 1001  ................
+00001b00: 0201 02fe 0a04 0813 0808 100e 723a 0000  ............r:..
+00001b10: 007a 092f 6574 632f 6d74 6162 7a1d 6d61  .z./etc/mtabz.ma
+00001b20: 634f 5320 646f 6573 206e 6f74 2068 6176  cOS does not hav
+00001b30: 6520 2f65 7463 2f6d 7461 6263 0000 0000  e /etc/mtabc....
+00001b40: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00001b50: 4000 0000 7318 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00001b60: 0264 015a 0364 0264 0384 005a 0464 0453  .d.Z.d.d...Z.d.S
+00001b70: 0029 05da 0c54 6573 744d 7461 624c 6f63  .)...TestMtabLoc
+00001b80: 6b7a 300a 2020 2020 556e 6974 2074 6573  kz0.    Unit tes
+00001b90: 7473 2066 6f72 2061 766f 6361 646f 2e75  ts for avocado.u
+00001ba0: 7469 6c73 2e70 6172 7469 7469 6f6e 0a20  tils.partition. 
+00001bb0: 2020 2063 0100 0000 0000 0000 0000 0000     c............
+00001bc0: 0100 0000 0900 0000 4300 0000 738e 0000  ........C...s...
+00001bd0: 0074 00a0 01a1 008f 3901 0074 026a 03a0  .t......9..t.j..
+00001be0: 0464 0174 026a 036a 0567 0064 02a2 0164  .d.t.j.j.g.d...d
+00001bf0: 038d 01a1 028f 1201 007c 00a0 0674 006a  .........|...t.j
+00001c00: 0774 00a0 01a1 006a 08a1 0201 0057 0064  .t.....j.....W.d
+00001c10: 0404 0004 0083 0301 006e 1031 0073 2877  .........n.1.s(w
+00001c20: 0101 0001 0001 0059 0001 0057 0064 0404  .......Y...W.d..
+00001c30: 0004 0083 0301 0064 0453 0057 0064 0404  .......d.S.W.d..
+00001c40: 0004 0083 0301 0064 0453 0031 0073 4077  .......d.S.1.s@w
+00001c50: 0101 0001 0001 0059 0001 0064 0453 0029  .......Y...d.S.)
+00001c60: 057a 3643 6865 636b 2064 6f75 626c 652d  .z6Check double-
+00001c70: 6c6f 636b 2072 6169 7365 7320 6578 6365  lock raises exce
+00001c80: 7074 696f 6e20 6166 7465 7220 3630 7320  ption after 60s 
+00001c90: 2869 6e20 302e 3173 297a 2061 766f 6361  (in 0.1s)z avoca
+00001ca0: 646f 2e75 7469 6c73 2e66 696c 656c 6f63  do.utils.fileloc
+00001cb0: 6b2e 7469 6d65 2e74 696d 6529 0372 1400  k.time.time).r..
+00001cc0: 0000 e902 0000 00e9 3e00 0000 7258 0000  ........>...rX..
+00001cd0: 004e 2909 7202 0000 005a 084d 7461 624c  .N).r....Z.MtabL
+00001ce0: 6f63 6b72 2800 0000 7259 0000 0072 5a00  ockr(...rY...rZ.
+00001cf0: 0000 5a09 4d61 6769 634d 6f63 6b72 5500  ..Z.MagicMockrU.
+00001d00: 0000 7256 0000 00da 095f 5f65 6e74 6572  ..rV.....__enter
+00001d10: 5f5f 7222 0000 0072 0b00 0000 720b 0000  __r"...r....r...
+00001d20: 0072 0c00 0000 da09 7465 7374 5f6c 6f63  .r......test_loc
+00001d30: 6bd5 0000 0073 1800 0000 0a02 0601 0201  k....s..........
+00001d40: 1001 06fe 0404 0c01 06ff 1efc 0eff 0201  ................
+00001d50: 22ff 7a16 5465 7374 4d74 6162 4c6f 636b  ".z.TestMtabLock
+00001d60: 2e74 6573 745f 6c6f 636b 4e29 0572 2400  .test_lockN).r$.
+00001d70: 0000 7225 0000 0072 2600 0000 7227 0000  ..r%...r&...r'..
+00001d80: 0072 6600 0000 720b 0000 0072 0b00 0000  .rf...r....r....
+00001d90: 720b 0000 0072 0c00 0000 7262 0000 00ce  r....r....rb....
+00001da0: 0000 0073 0600 0000 0800 0403 0c04 7262  ...s..........rb
+00001db0: 0000 00da 085f 5f6d 6169 6e5f 5f29 1872  .....__main__).r
+00001dc0: 2700 0000 7218 0000 0072 3e00 0000 7215  '...r....r>...r.
+00001dd0: 0000 005a 0d75 6e69 7474 6573 742e 6d6f  ...Z.unittest.mo
+00001de0: 636b 7228 0000 00da 0d61 766f 6361 646f  ckr(.....avocado
+00001df0: 2e75 7469 6c73 7202 0000 0072 0300 0000  .utilsr....r....
+00001e00: 7207 0000 0072 0400 0000 7205 0000 005a  r....r....r....Z
+00001e10: 0f73 656c 6674 6573 7473 2e75 7469 6c73  .selftests.utils
+00001e20: 7206 0000 0072 0d00 0000 da08 5465 7374  r....r......Test
+00001e30: 4361 7365 720e 0000 0072 2e00 0000 723a  Caser....r....r:
+00001e40: 0000 0072 2900 0000 722a 0000 0072 6200  ...r)...r*...rb.
+00001e50: 0000 7224 0000 00da 046d 6169 6e72 0b00  ..r$.....mainr..
+00001e60: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+00001e70: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001e80: 2400 0000 0400 0806 0801 0801 0801 0c02  $...............
+00001e90: 0c01 1001 0c01 0803 1208 1027 1010 147d  ...........'...}
+00001ea0: 1401 0812 0c01 04ff                      ........
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_path.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_path.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1338 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 3a05 0000  o.......i&.b:...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 3a05 0000  o.......nKec:...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6502 6a05 8303 5a06 6507 6405  ..d.e.j...Z.e.d.
 00000060: 6b02 7221 6502 a008 a100 0100 6401 5300  k.r!e.......d.S.
 00000070: 6401 5300 2906 e900 0000 004e 2901 da04  d.S.)......N)...
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_pci.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_pci.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1476 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 c405 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 c405 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6501 6a04  ..G.d.d...d.e.j.
 00000050: 8303 5a05 6506 6405 6b02 721d 6501 a007  ..Z.e.d.k.r.e...
 00000060: a100 0100 6401 5300 6401 5300 2906 e900  ....d.S.d.S.)...
 00000070: 0000 004e 2901 da03 7063 6963 0000 0000  ...N)...pcic....
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_pmem.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_pmem.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 340 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 5401 0000  o.......i&.bT...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 5401 0000  o.......nKecT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6501 6a04  ..G.d.d...d.e.j.
 00000050: 8303 5a05 6506 6405 6b02 721d 6501 a007  ..Z.e.d.k.r.e...
 00000060: a100 0100 6401 5300 6401 5300 2906 e900  ....d.S.d.S.)...
 00000070: 0000 004e 2901 da04 706d 656d 6300 0000  ...N)...pmemc...
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_process.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_process.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 31526 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 267b 0000  o.......i&.b&{..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 267b 0000  o.......nKec&{..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6403 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_script.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_script.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 541 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 1d02 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 1d02 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6501 6a04 8303 5a05 6506 6405  ..d.e.j...Z.e.d.
 00000060: 6b02 7221 6501 a007 a100 0100 6401 5300  k.r!e.......d.S.
 00000070: 6401 5300 2906 e900 0000 004e 2901 da06  d.S.)......N)...
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_service.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_service.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 12716 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 ac31 0000  o.......i&.b.1..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 ac31 0000  o.......nKec.1..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6505  ..d.d.l.m.Z...e.
 00000050: 8300 0100 4700 6404 6405 8400 6405 6501  ....G.d.d...d.e.
 00000060: 6a06 8303 5a07 4700 6406 6407 8400 6407  j...Z.G.d.d...d.
 00000070: 6501 6a06 8303 5a08 4700 6408 6409 8400  e.j...Z.G.d.d...
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_software_manager.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_software_manager.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 1215 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 bf04 0000  o.......i&.b....
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 bf04 0000  o.......nKec....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6509 8300 0100  m.Z.m.Z...e.....
 00000070: 6405 6406 8400 5a0a 6501 a00b 6500 a00c  d.d...Z.e...e...
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_ssh.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_ssh.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2408 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 6809 0000  o.......i&.bh...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 6809 0000  o.......nKech...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 4700  d.l.m.Z.m.Z...G.
 00000050: 6403 6404 8400 6404 6502 6a06 8303 5a07  d.d...d.e.j...Z.
 00000060: 6508 6405 6b02 7223 6502 a009 a100 0100  e.d.k.r#e.......
 00000070: 6401 5300 6401 5300 2906 e900 0000 004e  d.S.d.S.)......N
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_stacktrace.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_stacktrace.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 2932 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 740b 0000  o.......i&.bt...
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 740b 0000  o.......nKect...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 8302 5a06 4700 6406 6407 8400 6407 8302  ..Z.G.d.d...d...
 00000070: 5a07 4700 6408 6409 8400 6409 6508 8303  Z.G.d.d...d.e...
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/__pycache__/test_vmimage.cpython-310.pyc` & `avocado-framework-99.0/selftests/unit/utils/__pycache__/test_vmimage.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 11 13:32:25 2022 UTC, .py size: 32272 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6926 cc62 107e 0000  o.......i&.b.~..
+00000000: 6f0d 0d0a 0000 0000 6e4b 6563 107e 0000  o.......nKec.~..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6507 8300 0100  d.l.m.Z...e.....
 00000060: 4700 6405 6406 8400 6406 6501 6a08 8303  G.d.d...d.e.j...
 00000070: 5a09 4700 6407 6408 8400 6408 6501 6a08  Z.G.d.d...d.e.j.
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_ar.py` & `avocado-framework-99.0/selftests/unit/utils/test_ar.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_archive.py` & `avocado-framework-99.0/selftests/unit/utils/test_archive.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_astring.py` & `avocado-framework-99.0/selftests/unit/utils/test_astring.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_cloudinit.py` & `avocado-framework-99.0/selftests/unit/utils/test_cloudinit.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_cpu.py` & `avocado-framework-99.0/selftests/unit/utils/test_cpu.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/i386` & `avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/i386`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/s390x` & `avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/s390x`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/s390x_2` & `avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/s390x_2`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/s390x_3` & `avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/s390x_3`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_cpu.py.data/x86_64` & `avocado-framework-99.0/selftests/unit/utils/test_cpu.py.data/x86_64`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_data_structures.py` & `avocado-framework-99.0/selftests/unit/utils/test_data_structures.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_datadrainer.py` & `avocado-framework-99.0/selftests/unit/utils/test_datadrainer.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_diff_validator.py` & `avocado-framework-99.0/selftests/unit/utils/test_diff_validator.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_disk.py` & `avocado-framework-99.0/selftests/unit/utils/test_disk.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_distro.py` & `avocado-framework-99.0/selftests/unit/utils/test_distro.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_filelock.py` & `avocado-framework-99.0/selftests/unit/utils/test_filelock.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_gdb.py` & `avocado-framework-99.0/selftests/unit/utils/test_gdb.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_genio.py` & `avocado-framework-99.0/selftests/unit/utils/test_genio.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_iso9660.py` & `avocado-framework-99.0/selftests/unit/utils/test_iso9660.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,21 +66,14 @@
                 "sample.iso",
             )
         )
         self.iso = None
         prefix = temp_dir_prefix(self)
         self.tmpdir = tempfile.TemporaryDirectory(prefix=prefix)
 
-    @unittest.skipIf(
-        os.uname()[4] == "s390x",
-        (
-            "Endianess issues on pycdlib, see "
-            "https://github.com/clalancette/pycdlib/issues/39"
-        ),
-    )
     def test_basic_workflow(self):
         """
         Check the basic Iso9660 workflow
         """
         self.assertEqual(self.iso.read("file"), b"file content\n")
         dst = os.path.join(self.tmpdir.name, "file")
         self.iso.copy(os.path.join("Dir", "in_dir_file"), dst)
@@ -92,19 +85,14 @@
         not process.can_sudo("mount"),
         "This test requires mount to run under sudo or root",
     )
     @unittest.skipUnless(
         process.has_capability("cap_sys_admin"),
         "Capability to mount is required (cap_sys_admin)",
     )
-    @unittest.skipIf(
-        os.getenv("TRAVIS")
-        and os.getenv("TRAVIS_CPU_ARCH") in ["arm64", "ppc64le", "s390x"],
-        "TRAVIS Environment is unsuitable for these tests",
-    )
     def test_mnt_dir_workflow(self):
         """
         Check the mnt_dir functionality
         """
         base = self.iso.mnt_dir
         dir_path = os.path.join(base, "Dir")
         self.assertTrue(os.path.isdir(dir_path))
@@ -162,19 +150,14 @@
     """
 
     @unittest.skipIf(not process.can_sudo("mount"), "This test requires sudo or root")
     @unittest.skipUnless(
         process.has_capability("cap_sys_admin"),
         "Capability to mount is required (cap_sys_admin)",
     )
-    @unittest.skipIf(
-        os.getenv("TRAVIS")
-        and os.getenv("TRAVIS_CPU_ARCH") in ["arm64", "ppc64le", "s390x"],
-        "TRAVIS Environment is unsuitable for these tests",
-    )
     def setUp(self):
         super().setUp()
         self.iso = iso9660.Iso9660Mount(self.iso_path)
 
 
 class PyCDLib(BaseIso9660, unittest.TestCase):
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_kernel.py` & `avocado-framework-99.0/selftests/unit/utils/test_kernel.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_linux_modules.py` & `avocado-framework-99.0/selftests/unit/utils/test_linux_modules.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_linux_modules.py.data/lsmod` & `avocado-framework-99.0/selftests/unit/utils/test_linux_modules.py.data/lsmod`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_linux_modules.py.data/proc_modules` & `avocado-framework-99.0/selftests/unit/utils/test_linux_modules.py.data/proc_modules`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_memory.py` & `avocado-framework-99.0/selftests/unit/utils/test_memory.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_network.py` & `avocado-framework-99.0/selftests/unit/utils/test_network.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_output.py` & `avocado-framework-99.0/selftests/unit/utils/test_output.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_partition.py` & `avocado-framework-99.0/selftests/unit/utils/test_partition.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,19 +44,14 @@
         utils_path.find_command("mkfs.ext2", False),
         "mkfs.ext2 utility must be available",
     )
     @unittest.skipUnless(
         process.has_capability("cap_sys_admin"),
         "Capability to mount is required (cap_sys_admin)",
     )
-    @unittest.skipIf(
-        os.getenv("TRAVIS")
-        and os.getenv("TRAVIS_CPU_ARCH") in ["arm64", "ppc64le", "s390x"],
-        "TRAVIS Environment is unsuitable for these tests",
-    )
     def setUp(self):
         prefix = temp_dir_prefix(self)
         self.tmpdir = tempfile.TemporaryDirectory(prefix=prefix)
         self.mountpoint = os.path.join(self.tmpdir.name, "disk")
         os.mkdir(self.mountpoint)
         self.disk = partition.Partition(
             os.path.join(self.tmpdir.name, "block"), 1, self.mountpoint
```

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_path.py` & `avocado-framework-99.0/selftests/unit/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_pci.py` & `avocado-framework-99.0/selftests/unit/utils/test_pci.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_process.py` & `avocado-framework-99.0/selftests/unit/utils/test_process.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_script.py` & `avocado-framework-99.0/selftests/unit/utils/test_script.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_service.py` & `avocado-framework-99.0/selftests/unit/utils/test_service.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_software_manager.py` & `avocado-framework-99.0/selftests/unit/utils/test_software_manager.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_ssh.py` & `avocado-framework-99.0/selftests/unit/utils/test_ssh.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_stacktrace.py` & `avocado-framework-99.0/selftests/unit/utils/test_stacktrace.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/unit/utils/test_vmimage.py` & `avocado-framework-99.0/selftests/unit/utils/test_vmimage.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/selftests/utils.py` & `avocado-framework-99.0/selftests/utils.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-98.0/setup.py` & `avocado-framework-99.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -347,14 +347,15 @@
                 "avocado-runner-dry-run = avocado.plugins.runners.dry_run:main",
                 "avocado-runner-exec-test = avocado.plugins.runners.exec_test:main",
                 "avocado-runner-python-unittest = avocado.plugins.runners.python_unittest:main",
                 "avocado-runner-avocado-instrumented = avocado.plugins.runners.avocado_instrumented:main",
                 "avocado-runner-tap = avocado.plugins.runners.tap:main",
                 "avocado-runner-asset = avocado.plugins.runners.asset:main",
                 "avocado-runner-package = avocado.plugins.runners.package:main",
+                "avocado-runner-podman-image = avocado.plugins.runners.podman_image:main",
                 "avocado-runner-sysinfo = avocado.plugins.runners.sysinfo:main",
                 "avocado-software-manager = avocado.utils.software_manager.main:main",
                 "avocado-external-runner = scripts.external_runner:main",
             ],
             "avocado.plugins.init": [
                 "xunit = avocado.plugins.xunit:XUnitInit",
                 "jsonresult = avocado.plugins.jsonresult:JSONInit",
@@ -389,14 +390,15 @@
                 "sysinfo = avocado.plugins.sysinfo:SysInfo",
                 "plugins = avocado.plugins.plugins:Plugins",
                 "diff = avocado.plugins.diff:Diff",
                 "vmimage = avocado.plugins.vmimage:VMimage",
                 "assets = avocado.plugins.assets:Assets",
                 "jobs = avocado.plugins.jobs:Jobs",
                 "replay = avocado.plugins.replay:Replay",
+                "cache = avocado.plugins.cache:Cache",
             ],
             "avocado.plugins.job.prepost": [
                 "jobscripts = avocado.plugins.jobscripts:JobScripts",
                 "teststmpdir = avocado.plugins.teststmpdir:TestsTmpDir",
                 "human = avocado.plugins.human:HumanJob",
                 "testlogsui = avocado.plugins.testlogs:TestLogsUI",
             ],
@@ -439,20 +441,25 @@
                 "tap = avocado.plugins.runners.tap:TAPRunner",
                 "noop = avocado.plugins.runners.noop:NoOpRunner",
                 "dry-run = avocado.plugins.runners.dry_run:DryRunRunner",
                 "exec-test = avocado.plugins.runners.exec_test:ExecTestRunner",
                 "python-unittest = avocado.plugins.runners.python_unittest:PythonUnittestRunner",
                 "asset = avocado.plugins.runners.asset:AssetRunner",
                 "package = avocado.plugins.runners.package:PackageRunner",
+                "podman-image = avocado.plugins.runners.podman_image:PodmanImageRunner",
                 "sysinfo = avocado.plugins.runners.sysinfo:SysinfoRunner",
             ],
             "avocado.plugins.spawner": [
                 "process = avocado.plugins.spawners.process:ProcessSpawner",
                 "podman = avocado.plugins.spawners.podman:PodmanSpawner",
             ],
+            "avocado.plugins.cache": [
+                "vmimage = avocado.plugins.vmimage:VMimageCache",
+                "requirement = avocado.plugins.requirement_cache:RequirementCache",
+            ],
         },
         zip_safe=False,
         test_suite="selftests",
         python_requires=">=3.6",
         cmdclass={
             "clean": Clean,
             "develop": Develop,
```

