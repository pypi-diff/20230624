# Comparing `tmp/dbt-upsolver-1.5.24.tar.gz` & `tmp/dbt-upsolver-1.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-upsolver-1.5.24.tar", last modified: Mon Jun  5 16:01:33 2023, max compression
+gzip compressed data, was "dbt-upsolver-1.5.25.tar", last modified: Sat Jun 24 12:41:15 2023, max compression
```

## Comparing `dbt-upsolver-1.5.24.tar` & `dbt-upsolver-1.5.25.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/adapters/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/connection_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/copy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/target_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/transformation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/include/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/connection.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/materializedview.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/create_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/render_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.968070 dbt-upsolver-1.5.25/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.968070 dbt-upsolver-1.5.25/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/adapters/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/connection_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/target_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/transformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.968070 dbt-upsolver-1.5.25/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/include/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/connection.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/materializedview.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/alter_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/create_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/expextations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/render_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/setup.py
```

### Comparing `dbt-upsolver-1.5.24/LICENSE` & `dbt-upsolver-1.5.25/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/PKG-INFO` & `dbt-upsolver-1.5.25/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 1.5.24
+Version: 1.5.25
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -135,16 +135,16 @@
 ```sh
 dbt run --select <model name>
 ```
 ### Supported dbt commands:
 
 | COMMAND | STATE |
 | ------ | ------ |
-| docs| not supported |
-| source | not supported |
+| docs| supported |
+| source | supported |
 | init | supported |
 | clean | supported |
 | debug | supported |
 | deps | supported |
 | list| not supported |
 | ls | not supported |
 | build | supported |
@@ -153,22 +153,28 @@
 | compile | supported |
 | parse | supported |
 | test | not supported |
 | seed | not supported |
 | run-operation | supported |
 
 ### Supported Upsolver SQLake functionality:
-| COMMAND | STATE | MATERIALIZED |
-| ------ | ------ | ------ |
-| SQL compute cluster| not supported | - |
-| SQL connections| supported | connection |
-| SQL copy job | supported | incremental |
-| SQL merge job | supported | incremental |
-| SQL insert job | supported | incremental |
-| SQL materialized views | supported | materializedview |
+| FUNCTION | STATE | MATERIALIZED | CONFIGURATION PROPERTIES
+| ------ | ------ | ------ | ------ |
+| Create compute cluster| not supported | - | - |
+| [Create connection](https://docs.upsolver.com/sqlake/sql-command-reference/sql-connections/create-connection) | supported | connection | connection_type(S3/Kafka/Snowflake ...), [connection_options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-connections/create-connection#connection-options) |
+| [Create copy job](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/copy-from) | supported | incremental, incremental_strategy: 'copy' | source(S3/Kafka/Snowflake ...) , target_type(Datalake/Snowflake), [options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/copy-from#job-options) |
+| [Create merge job](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/merge) | supported | incremental, incremental_strategy: 'merge'| target_type(S3/Datalake/Snowflake ...), target_connection, target_table_alias, target_schema, [options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/merge#job-options) |
+| [Create insert job](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/insert) | supported | incremental, incremental_strategy: 'insert'| target_type(S3/Datalake/Snowflake ...), target_connection, target_table_alias, target_schema, [options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/insert#job-options) |
+| [Create materialized views](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/sql-materialized-views) | supported | materializedview |
+| [Expectations](https://docs.upsolver.com/sqlake/how-to-guides/managing-data-quality-ingesting-data-with-expectations) | supported | incremental, incremental_strategy: 'copy' | model constraints and column constraints [in the yml file](https://docs.getdbt.com/reference/resource-properties/constraints) |
+| [MAP_COLUMNS_BY_NAME](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/insert/map_columns_by_name) | supported | incremental, incremental_strategy: ‘insert’ | map_columns_by_name(True/False) |
+| [Upsert with INSERT](https://docs.upsolver.com/sqlake/quickstarts/upsert-data-to-your-target-table#upsert-with-insert) | supported | incremental, incremental_strategy: ‘insert’ | primary_key|
+| [Upsert with MERGE](https://docs.upsolver.com/sqlake/quickstarts/upsert-data-to-your-target-table#upsert-with-insert)| supported | incremental, incremental_strategy: ‘merge’ | primary_key |
+| [PARTITIONED BY](https://docs.upsolver.com/sqlake/sql-command-reference/sql-tables/create-table#partition-clause) | supported | incremental | partition_by |
+
 
 ## SQL connections
 Connections are used to provide Upsolver with the proper credentials to bring your data into SQLake as well as to write out your transformed data to various services. More details on ["Upsolver SQL connections"](https://docs.upsolver.com/sqlake/sql-command-reference/sql-connections)
 As a dbt model connection is a model with materialized='connection'
 ```sql
 {{ config(
         materialized='connection',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbt-upsolver-1.5.24/README.md` & `dbt-upsolver-1.5.25/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -113,16 +113,16 @@
 ```sh
 dbt run --select <model name>
 ```
 ### Supported dbt commands:
 
 | COMMAND | STATE |
 | ------ | ------ |
-| docs| not supported |
-| source | not supported |
+| docs| supported |
+| source | supported |
 | init | supported |
 | clean | supported |
 | debug | supported |
 | deps | supported |
 | list| not supported |
 | ls | not supported |
 | build | supported |
@@ -131,22 +131,28 @@
 | compile | supported |
 | parse | supported |
 | test | not supported |
 | seed | not supported |
 | run-operation | supported |
 
 ### Supported Upsolver SQLake functionality:
-| COMMAND | STATE | MATERIALIZED |
-| ------ | ------ | ------ |
-| SQL compute cluster| not supported | - |
-| SQL connections| supported | connection |
-| SQL copy job | supported | incremental |
-| SQL merge job | supported | incremental |
-| SQL insert job | supported | incremental |
-| SQL materialized views | supported | materializedview |
+| FUNCTION | STATE | MATERIALIZED | CONFIGURATION PROPERTIES
+| ------ | ------ | ------ | ------ |
+| Create compute cluster| not supported | - | - |
+| [Create connection](https://docs.upsolver.com/sqlake/sql-command-reference/sql-connections/create-connection) | supported | connection | connection_type(S3/Kafka/Snowflake ...), [connection_options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-connections/create-connection#connection-options) |
+| [Create copy job](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/copy-from) | supported | incremental, incremental_strategy: 'copy' | source(S3/Kafka/Snowflake ...) , target_type(Datalake/Snowflake), [options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/copy-from#job-options) |
+| [Create merge job](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/merge) | supported | incremental, incremental_strategy: 'merge'| target_type(S3/Datalake/Snowflake ...), target_connection, target_table_alias, target_schema, [options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/merge#job-options) |
+| [Create insert job](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/insert) | supported | incremental, incremental_strategy: 'insert'| target_type(S3/Datalake/Snowflake ...), target_connection, target_table_alias, target_schema, [options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/insert#job-options) |
+| [Create materialized views](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/sql-materialized-views) | supported | materializedview |
+| [Expectations](https://docs.upsolver.com/sqlake/how-to-guides/managing-data-quality-ingesting-data-with-expectations) | supported | incremental, incremental_strategy: 'copy' | model constraints and column constraints [in the yml file](https://docs.getdbt.com/reference/resource-properties/constraints) |
+| [MAP_COLUMNS_BY_NAME](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/insert/map_columns_by_name) | supported | incremental, incremental_strategy: ‘insert’ | map_columns_by_name(True/False) |
+| [Upsert with INSERT](https://docs.upsolver.com/sqlake/quickstarts/upsert-data-to-your-target-table#upsert-with-insert) | supported | incremental, incremental_strategy: ‘insert’ | primary_key|
+| [Upsert with MERGE](https://docs.upsolver.com/sqlake/quickstarts/upsert-data-to-your-target-table#upsert-with-insert)| supported | incremental, incremental_strategy: ‘merge’ | primary_key |
+| [PARTITIONED BY](https://docs.upsolver.com/sqlake/sql-command-reference/sql-tables/create-table#partition-clause) | supported | incremental | partition_by |
+
 
 ## SQL connections
 Connections are used to provide Upsolver with the proper credentials to bring your data into SQLake as well as to write out your transformed data to various services. More details on ["Upsolver SQL connections"](https://docs.upsolver.com/sqlake/sql-command-reference/sql-connections)
 As a dbt model connection is a model with materialized='connection'
 ```sql
 {{ config(
         materialized='connection',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbt-upsolver-1.5.24/dbt/adapters/upsolver/connections.py` & `dbt-upsolver-1.5.25/dbt/adapters/upsolver/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/connection_options.py` & `dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/connection_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/copy_options.py` & `dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/copy_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/target_options.py` & `dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/target_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/transformation_options.py` & `dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/transformation_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/adapters/upsolver/relation.py` & `dbt-upsolver-1.5.25/dbt/adapters/upsolver/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/catalog.sql` & `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/connection.sql` & `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/connection.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql` & `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-{% macro get_create_copy_job_sql(job_identifier, sql, into_relation, sync, options, source, target_type) -%}
+{% macro get_create_copy_job_sql(job_identifier,
+                                 sql,
+                                 into_relation,
+                                 sync, options,
+                                 source, target_type,
+                                 raw_constraints,
+                                 raw_columns) -%}
 
     {%- set connection_identifier = adapter.get_connection_from_sql(sql) -%}
     {%- set job_options, source_options = adapter.separate_options(options, source) -%}
     {%- if target_type != 'datalake' -%}
       {%- set target_options = adapter.enrich_options(options, target_type, 'target_options') -%}
       {%- set target_type = target_type -%}
     {%- else -%}
@@ -16,9 +22,10 @@
     {%- endif -%}
     JOB {{job_identifier}}
     {{ render_options(job_options, 'create') }}
     {{ render_options(target_options, 'create') }}
     AS COPY FROM {{source}} {{connection_identifier}}
     {{ render_options(source_options, 'create') }}
     INTO {{target_type}} {{into_relation}}
+    {{ get_add_constraints(row_constraints=raw_columns+raw_constraints) }}
 
 {%- endmacro %}
```

### Comparing `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql` & `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql` & `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/incremental.sql` & `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/incremental.sql`

 * *Files 24% similar despite different names*

```diff
@@ -9,28 +9,33 @@
   {%- set target_type = adapter.get(model_config, 'target_type', 'datalake').lower() -%}
   {%- set target_table_alias = adapter.get(model_config, 'target_table_alias', identifier) -%}
   {%- set delete_condition = adapter.get(model_config, 'delete_condition', False) -%}
   {%- set partition_by = adapter.get(model_config, 'partition_by', []) -%}
   {%- set primary_key = adapter.get(model_config, 'primary_key', []) -%}
   {%- set map_columns_by_name = adapter.get(model_config, 'map_columns_by_name', False) -%}
   {%- set job_identifier = identifier + '_job' %}
+  {%- set model_constraints = adapter.render_raw_model_constraints(raw_constraints=model['constraints']) -%}
+  {%- set column_constraints = adapter.render_raw_columns_constraints(raw_columns=model['columns']) -%}
+
+  {{ get_validate_constraints(model_constraints, column_constraints, incremental_strategy, target_type) }}
 
   {%- set old_relation = adapter.get_relation(identifier=job_identifier,
                                               schema=schema,
                                               database=database) -%}
   {%- set target_relation = api.Relation.create(identifier=job_identifier,
                                                 schema=schema,
                                                 database=database,
                                                 type='incremental') -%}
 
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
   {{ log("model[config]: " ~ model['config'] ) }}
-
+  {{ log("model['columns']): " ~ model['columns'] ) }}
+  {{ log("model['constraints']: " ~ model['constraints'] ) }}
 
   {% if target_type  == 'datalake' %}
     {%- set target_connection = adapter.get(model_config, 'target_connection', database) -%}
     {%- set target_schema = adapter.get(model_config, 'target_schema', schema) -%}
     {%- set table_relation = api.Relation.create(identifier=target_table_alias,
                                                  schema=target_schema,
                                                  database=target_connection,
@@ -45,29 +50,30 @@
     {%- set into_relation = target_connection + '.' + target_schema + '.' + target_table_alias -%}
   {%- endif %}
 
   {%- if old_relation -%}
     {%- call statement('main') -%}
       {{ get_alter_job_sql(job_identifier, options, incremental_strategy, source) }}
     {%- endcall %}
+    {{ get_add_expectations_if_not_exists_sql(job_identifier, rendered_constraints = column_constraints + model_constraints) }}
   {%- else -%}
     {%- call statement('main') -%}
       {%- if incremental_strategy == 'merge' -%}
         {{ get_create_merge_job_sql(job_identifier, into_relation, sync,
                                     options, primary_key, delete_condition,
                                     target_type) }}
       {%- elif incremental_strategy == 'insert' -%}
         {{ get_create_insert_job_sql(job_identifier,
                                     into_relation, sync, options,
                                     map_columns_by_name, target_type) }}
 
       {%- else  -%}
         {{ get_create_copy_job_sql(job_identifier, sql,
                                    into_relation, sync, options, source,
-                                   target_type) }}
+                                   target_type, model_constraints, column_constraints) }}
 
       {%- endif -%}
     {%- endcall -%}
   {%- endif -%}
 
   {%- do persist_docs(target_relation, model) -%}
   {%- do persist_docs(table_relation, model) -%}
```

### Comparing `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/materializedview.sql` & `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/ater_job.sql` & `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/alter_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/create_table.sql` & `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/create_table.sql`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 {% macro get_create_table_if_not_exists_sql(target_relation, partition_by, primary_key, options) -%}
 
 {%- set old_relation = adapter.get_relation(identifier=target_relation.identifier,
                                             schema=target_relation.schema,
                                             database=target_relation.database) -%}
 
-  {%- set columns_with_types = adapter.get_columns_names_with_types(partition_by + primary_key) -%}
-  {%- set columns_partitioned_by  = adapter.get_columns_names(partition_by) -%}
-  {%- set columns_primary_key  = adapter.get_columns_names(primary_key) -%}
+  {%- set raw_columns = adapter.render_columns(raw_columns_from_config=partition_by+primary_key, raw_columns_from_columns=model['columns']) -%}
+  {%- set columns_partitioned_by  = adapter.render_columns_names(partition_by) -%}
+  {%- set columns_primary_key  = adapter.render_columns_names(primary_key) -%}
   {%- set enriched_options = adapter.enrich_options(options, 'datalake', 'target_options') -%}
   {%- set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') -%}
 
   {%- if old_relation -%}
     ALTER TABLE {{target_relation}}
     {{ render_options(enriched_editable_options, 'alter') }}
   {%- else -%}
     CREATE TABLE {{ target_relation }}
-    ({{ columns_with_types }})
+    ({{ raw_columns }})
     {%- if partition_by %}
     PARTITIONED BY
       {{ columns_partitioned_by }}
     {%- endif -%}
     {%- if primary_key %}
     PRIMARY KEY
       {{ columns_primary_key }}
```

### Comparing `dbt-upsolver-1.5.24/dbt_upsolver.egg-info/PKG-INFO` & `dbt-upsolver-1.5.25/dbt_upsolver.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 1.5.24
+Version: 1.5.25
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -135,16 +135,16 @@
 ```sh
 dbt run --select <model name>
 ```
 ### Supported dbt commands:
 
 | COMMAND | STATE |
 | ------ | ------ |
-| docs| not supported |
-| source | not supported |
+| docs| supported |
+| source | supported |
 | init | supported |
 | clean | supported |
 | debug | supported |
 | deps | supported |
 | list| not supported |
 | ls | not supported |
 | build | supported |
@@ -153,22 +153,28 @@
 | compile | supported |
 | parse | supported |
 | test | not supported |
 | seed | not supported |
 | run-operation | supported |
 
 ### Supported Upsolver SQLake functionality:
-| COMMAND | STATE | MATERIALIZED |
-| ------ | ------ | ------ |
-| SQL compute cluster| not supported | - |
-| SQL connections| supported | connection |
-| SQL copy job | supported | incremental |
-| SQL merge job | supported | incremental |
-| SQL insert job | supported | incremental |
-| SQL materialized views | supported | materializedview |
+| FUNCTION | STATE | MATERIALIZED | CONFIGURATION PROPERTIES
+| ------ | ------ | ------ | ------ |
+| Create compute cluster| not supported | - | - |
+| [Create connection](https://docs.upsolver.com/sqlake/sql-command-reference/sql-connections/create-connection) | supported | connection | connection_type(S3/Kafka/Snowflake ...), [connection_options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-connections/create-connection#connection-options) |
+| [Create copy job](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/copy-from) | supported | incremental, incremental_strategy: 'copy' | source(S3/Kafka/Snowflake ...) , target_type(Datalake/Snowflake), [options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/copy-from#job-options) |
+| [Create merge job](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/merge) | supported | incremental, incremental_strategy: 'merge'| target_type(S3/Datalake/Snowflake ...), target_connection, target_table_alias, target_schema, [options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/merge#job-options) |
+| [Create insert job](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/insert) | supported | incremental, incremental_strategy: 'insert'| target_type(S3/Datalake/Snowflake ...), target_connection, target_table_alias, target_schema, [options](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/insert#job-options) |
+| [Create materialized views](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/sql-materialized-views) | supported | materializedview |
+| [Expectations](https://docs.upsolver.com/sqlake/how-to-guides/managing-data-quality-ingesting-data-with-expectations) | supported | incremental, incremental_strategy: 'copy' | model constraints and column constraints [in the yml file](https://docs.getdbt.com/reference/resource-properties/constraints) |
+| [MAP_COLUMNS_BY_NAME](https://docs.upsolver.com/sqlake/sql-command-reference/sql-jobs/create-job/sql-transformation-jobs/insert/map_columns_by_name) | supported | incremental, incremental_strategy: ‘insert’ | map_columns_by_name(True/False) |
+| [Upsert with INSERT](https://docs.upsolver.com/sqlake/quickstarts/upsert-data-to-your-target-table#upsert-with-insert) | supported | incremental, incremental_strategy: ‘insert’ | primary_key|
+| [Upsert with MERGE](https://docs.upsolver.com/sqlake/quickstarts/upsert-data-to-your-target-table#upsert-with-insert)| supported | incremental, incremental_strategy: ‘merge’ | primary_key |
+| [PARTITIONED BY](https://docs.upsolver.com/sqlake/sql-command-reference/sql-tables/create-table#partition-clause) | supported | incremental | partition_by |
+
 
 ## SQL connections
 Connections are used to provide Upsolver with the proper credentials to bring your data into SQLake as well as to write out your transformed data to various services. More details on ["Upsolver SQL connections"](https://docs.upsolver.com/sqlake/sql-command-reference/sql-connections)
 As a dbt model connection is a model with materialized='connection'
 ```sql
 {{ config(
         materialized='connection',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbt-upsolver-1.5.24/dbt_upsolver.egg-info/SOURCES.txt` & `dbt-upsolver-1.5.25/dbt_upsolver.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 dbt/include/upsolver/macros/catalog.sql
 dbt/include/upsolver/macros/materializations/connection.sql
 dbt/include/upsolver/macros/materializations/materializedview.sql
 dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
 dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
 dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
 dbt/include/upsolver/macros/materializations/incremental/incremental.sql
-dbt/include/upsolver/macros/materializations/utils/ater_job.sql
+dbt/include/upsolver/macros/materializations/utils/alter_job.sql
 dbt/include/upsolver/macros/materializations/utils/create_table.sql
+dbt/include/upsolver/macros/materializations/utils/expextations.sql
 dbt/include/upsolver/macros/materializations/utils/render_options.sql
 dbt_upsolver.egg-info/PKG-INFO
 dbt_upsolver.egg-info/SOURCES.txt
 dbt_upsolver.egg-info/dependency_links.txt
 dbt_upsolver.egg-info/not-zip-safe
 dbt_upsolver.egg-info/requires.txt
 dbt_upsolver.egg-info/top_level.txt
```

### Comparing `dbt-upsolver-1.5.24/setup.py` & `dbt-upsolver-1.5.25/setup.py`

 * *Files identical despite different names*

