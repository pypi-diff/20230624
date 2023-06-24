# Comparing `tmp/mercury-sync-0.3.0.tar.gz` & `tmp/mercury-sync-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.3.0.tar", last modified: Fri Jun 23 15:18:59 2023, max compression
+gzip compressed data, was "mercury-sync-0.3.1.tar", last modified: Sat Jun 24 00:25:44 2023, max compression
```

## Comparing `mercury-sync-0.3.0.tar` & `mercury-sync-0.3.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.392506 mercury-sync-0.3.0/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/models/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/models/ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/service/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/service/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/mercury_sync/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/types/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/types/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-23 15:18:59.000000 mercury-sync-0.3.0/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-23 15:18:59.000000 mercury-sync-0.3.0/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:18:59.000000 mercury-sync-0.3.0/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 15:18:59.000000 mercury-sync-0.3.0/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 15:18:59.000000 mercury-sync-0.3.0/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/models/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/models/ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18901 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/service/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23296 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/service/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/mercury_sync/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/types/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/types/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 00:25:44.000000 mercury-sync-0.3.1/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-24 00:25:44.000000 mercury-sync-0.3.1/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:25:44.000000 mercury-sync-0.3.1/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 00:25:44.000000 mercury-sync-0.3.1/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 00:25:44.000000 mercury-sync-0.3.1/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/setup.py
```

### Comparing `mercury-sync-0.3.0/LICENSE` & `mercury-sync-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/PKG-INFO` & `mercury-sync-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.0
+Version: 0.3.1
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.0/README.md` & `mercury-sync-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.3.1/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.3.1/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.3.1/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.3.1/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/env/env.py` & `mercury-sync-0.3.1/mercury_sync/env/env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/env/load_env.py` & `mercury-sync-0.3.1/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/env/time_parser.py` & `mercury-sync-0.3.1/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.3.1/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.3.1/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/service/controller.py` & `mercury-sync-0.3.1/mercury_sync/service/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,16 @@
     List, 
     Literal, 
     Union, 
     Dict,
     get_args,
     Callable,
     AsyncIterable,
-    Tuple,
-    Deque
+    Tuple
 )
-from .service import Service
 
 
 def handle_worker_loop_stop(signame, loop: asyncio.AbstractEventLoop):
     loop.stop()
 
 
 def handle_loop_stop(signame, executor: Union[ProcessPoolExecutor, ThreadPoolExecutor]):
@@ -497,14 +495,33 @@
             await connection.close()
 
         return await self.extend_client(
             remote,
             cert_path=cert_path,
             key_path=key_path
         )
+    
+    async def remove_clients(
+        self,
+        remote: Message 
+    ):
+        
+        existing_udp_connections = self._udp_queue[(remote.host, remote.port)]
+        existing_tcp_connections = self._tcp_queue[(remote.host, remote.port)]
+
+        while existing_udp_connections.empty() is False:
+            connection: MercurySyncUDPConnection = await existing_udp_connections.get()
+            await connection.close()
+
+        while existing_tcp_connections.empty() is False:
+            connection: MercurySyncUDPConnection = await existing_tcp_connections.get()
+            await connection.close()
+
+        del self._udp_queue[(remote.host, remote.port)]
+        del self._tcp_queue[(remote.host, remote.port)]
 
     async def send(
         self,
         event_name: str,
         message: Message
     ):
         connection: MercurySyncUDPConnection = await self._udp_queue[(message.host, message.port)].get()
```

### Comparing `mercury-sync-0.3.0/mercury_sync/service/monitor.py` & `mercury-sync-0.3.1/mercury_sync/service/monitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,37 +95,49 @@
 
         if self._suspect_nodes.get((target_host, target_port)):
             del self._suspect_nodes[(target_host, target_port)]
 
         if target_host != self.host and target_port != self.port:
             self._monitoring[(target_host, target_port)] = True
 
+            await self.push_new_node(
+                target_host,
+                target_port,
+                self.host,
+                self.port,
+                self.health,
+                error_context=self.error_context
+            )
+
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
             status=self.health,
             error=self.error_context
         )
 
     @server()
-    async def update_failed(
+    async def update_suspect(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
         
         target_host = healthcheck.target_host
         target_port = healthcheck.target_port
         shard_ids = healthcheck.shard_ids
 
-        if self._suspect_nodes.get((target_host, target_port)) is None:
+        self._suspect_nodes[(target_host, target_port)] = shard_ids
 
-            self._suspect_nodes[(target_host, target_port)] = shard_ids
+        if self._suspect_tasks.get((target_host, target_port)) is None:
+            self._suspect_tasks[(target_host, target_port)] = asyncio.create_task(
+                self._start_suspect_monitor()
+            )
 
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
             status=self.health,
@@ -156,19 +168,22 @@
                 source_host=response.source_host,
                 source_port=response.source_port,
                 status=response.status,
                 error=response.error
             )
 
         except asyncio.TimeoutError:
+
+            self._monitoring[(healthcheck.target_host, healthcheck.target_port)] = False
+
             return HealthCheck(
                 host=healthcheck.source_host,
                 port=healthcheck.source_port,
-                source_host=self.host,
-                source_port=self.port,
+                source_host=healthcheck.target_host,
+                source_port=healthcheck.target_port,
                 status='suspect',
                 error='timeout'
             )
         
 
     @server()
     async def register_new_node(
@@ -179,39 +194,39 @@
         host = healthcheck.source_host
         port = healthcheck.source_port
 
         not_self = host != self.host and port != self.port
 
         if not_self:
 
-            if self._suspect_nodes.get((
-                healthcheck.source_host, 
-                healthcheck.source_port
-            )):
-                del self._suspect_nodes[(
-                    healthcheck.source_host,
-                    healthcheck.source_port
-                )]
+            suspect_tasks = dict(self._suspect_tasks)
+            suspect_task = suspect_tasks.get((host, port))
+
+            if suspect_task:
+                await cancel(suspect_task)
+                del suspect_tasks[(host, port)]
+                
+                self._suspect_tasks = suspect_tasks
 
             await self.extend_client(
                 HealthCheck(
-                    host=healthcheck.source_host,
-                    port=healthcheck.source_port,
+                    host=host,
+                    port=port,
                     source_host=self.host,
                     source_port=self.port,
                     status=healthcheck.status,
                     error=healthcheck.error
                 )
             )
 
-            self._monitoring[(healthcheck.source_host, healthcheck.source_port)] = True
+            self._monitoring[(host, port)] = True
 
         return HealthCheck(
-            host=healthcheck.source_host,
-            port=healthcheck.source_port,
+            host=host,
+            port=port,
             source_host=self.host,
             source_port=self.port,
             error=self.error_context,
             status=self.health
         )
         
 
@@ -221,37 +236,69 @@
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
         
         source_host = healthcheck.source_host
         source_port = healthcheck.source_port
 
-        if not self._monitoring.get((source_host, source_port)):
+        monitor_exists_status = self._monitoring.get((source_host, source_port))
+
+        suspect_tasks = dict(self._suspect_tasks)
+        suspect_task = suspect_tasks.get((source_host, source_port))
+
+        if suspect_task:
+            await cancel(suspect_task)
+            del suspect_tasks[(source_host, source_port)]
+
+            self._suspect_tasks = suspect_tasks
+
+        if not monitor_exists_status:
+
+            monitoring = [
+                address for address, monitoring_status in self._monitoring.items() if monitoring_status
+            ]
+            
+            for host, port in monitoring:
+
+                await self.push_new_node(
+                    host,
+                    port,
+                    source_host,
+                    source_port,
+                    healthcheck.status,
+                    error_context=healthcheck.error
+                )
+
+        if monitor_exists_status is None:
+
             await self.extend_client(
                 HealthCheck(
                     host=source_host,
                     port=source_port,
                     source_host=self.host,
                     source_port=self.port,
                     status=healthcheck.status,
                     error=healthcheck.error
                 )
             )
 
-            monitoring = dict(self._monitoring)
-            for host, port in monitoring:
+            self._monitoring[(source_host, source_port)] = True
 
-                await self.push_new_node(
-                    host,
-                    port,
-                    source_host,
-                    source_port,
-                    healthcheck.status,
-                    error_context=healthcheck.error
+        elif monitor_exists_status is False:
+
+            await self.refresh_clients(
+                HealthCheck(
+                    host=source_host,
+                    port=source_port,
+                    source_host=self.host,
+                    source_port=self.port,
+                    status=healthcheck.status,
+                    error=healthcheck.error
                 )
+            )
 
             self._monitoring[(source_host, source_port)] = True
 
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
@@ -314,15 +361,15 @@
             target_port=target_port,
             source_host=self.host,
             source_port=self.port,
             error=error_context,
             status=health_status
         )
     
-    @client('update_failed')
+    @client('update_suspect')
     async def submit_suspect_node(
         self,
         host: str,
         port: int,
         target_host: str,
         target_port: int,
         shard_ids: List[int],
@@ -399,14 +446,37 @@
         self._healthchecks[(host, port)] = asyncio.create_task(
             self.start_health_monitor()
         )
         
         self.confirmation_task = asyncio.create_task(
             self.cleanup_pending_checks()
         )
+    
+    async def _update_suspect_nodes(
+        self,
+        confirmation_members: List[Tuple[str, int]],
+        successful_requests: Dict[Tuple[str, int], int]
+    ):
+        for node_host, node_port in confirmation_members:
+
+            request_failed = successful_requests.get((node_host, node_port)) is None
+            not_active_probe = self._active_probes.get((node_host, node_port)) is None
+
+            if request_failed and not_active_probe:
+                self._active_probes[(node_host, node_port)] = True
+                self._failed_nodes.append((
+                    node_host,
+                    node_port
+                ))
+
+                self._monitoring[(node_host, node_port)] = False
+
+                self._failed_tasks[(node_host, node_port)] = asyncio.create_task(
+                    self._probe_timed_out_node()
+                )
 
     async def _run_healthcheck(self, host: str, port: int):
 
         try:
 
             await asyncio.wait_for(
                 self.push_health_update(
@@ -425,40 +495,20 @@
                     host,
                     port
                 ))
 
                 self._failed_tasks[(host, port)] = asyncio.create_task(
                     self._probe_timed_out_node()
                 )
-                
+            
             self._monitoring[(host, port)] = False
 
-    async def _update_suspect_nodes(
-        self,
-        confirmation_members: List[Tuple[str, int]],
-        successful_requests: Dict[Tuple[str, int], int]
-    ):
-        for node_host, node_port in confirmation_members:
-
-            request_failed = successful_requests.get((node_host, node_port)) is None
-            not_active_probe = self._active_probes.get((node_host, node_port)) is None
-
-            if request_failed and not_active_probe:
-                self._active_probes[(node_host, node_port)] = True
-                self._failed_nodes.append((
-                    node_host,
-                    node_port
-                ))
-
-                self._failed_tasks[(node_host, node_port)] = asyncio.create_task(
-                    self._probe_timed_out_node()
-                )
-
     async def _probe_timed_out_node(self):
 
+
         host, port = self._failed_nodes.pop()
 
         confirmation_members = list(filter(
             lambda address: address[0] != host and address[1] != port,
             self._monitoring.keys()
         ))
 
@@ -472,14 +522,18 @@
                 confirmation_members, 
                 1
             )[0] for _ in range(
                 self._check_nodes_count
             )
         ]
 
+        if len(confirmation_members) < 1:
+            self._monitoring[(host, port)] = True
+            return
+
         check_tasks: Tuple[List[asyncio.Task], List[asyncio.Task]] = await asyncio.wait([
             asyncio.create_task(
                 self.request_indirect_check(
                     node_host,
                     node_port,
                     host,
                     port,
@@ -532,50 +586,57 @@
 
             await self._update_suspect_nodes(
                 confirmation_members,
                 successful_requests
             )
 
             self._suspect_tasks[(host, port)] = asyncio.create_task(
-                self.start_timed_out_monitor()
+                self._start_suspect_monitor()
             )
 
         else:
             self._monitoring[(host, port)] = True 
 
     async def run_forever(self):
         self._waiter = asyncio.Future()
         await self._waiter
 
     async def start_health_monitor(self):
         
+        monitor_idx = 0
+
         while self._running:
 
-            monitors = list(self._monitoring.keys())
+            monitors = [
+                address for address, monitoring_status in self._monitoring.items() if monitoring_status
+            ]
+
             host: Union[str, None] = None
             port: Union[int, None] = None
 
             if len(monitors) > 0:
-
-                host, port = random.sample(monitors, 1)[0]
+                monitor_idx = monitor_idx%len(monitors)
+                host, port = monitors[monitor_idx]
 
             if self._monitoring.get((host, port)):
         
                 self._active_checks_queue.append(
                     asyncio.create_task(
                         self._run_healthcheck(
                             host,
                             port
                         )
                     )
                 )
 
+            monitor_idx += 1
+
             await asyncio.sleep(self._poll_interval)      
 
-    async def start_timed_out_monitor(self):
+    async def _start_suspect_monitor(self):
 
         elapsed = 0
         start = time.monotonic()
 
         if len(self._suspect_nodes) < 1:
             return
         
@@ -601,15 +662,18 @@
                         suspect_port,
                         self.health,
                         error_context=self.error_context
                     ),
                     timeout=self._poll_timeout
                 )
 
-                monitoring = dict(self._monitoring)
+                monitoring = [
+                    address for address, monitoring_status in self._monitoring.items() if monitoring_status
+                ]
+
                 for host, port in monitoring:
                     if self._suspect_nodes.get((host, port)) is None:
                         await self.submit_active_node(
                             host,
                             port,
                             healthcheck.source_host,
                             healthcheck.source_port,
@@ -637,22 +701,45 @@
                 pass
 
             await asyncio.sleep(self._poll_interval) 
             elapsed = time.monotonic() - start
         
         if node_revived is False:
             self._removed_nodes[(suspect_host, suspect_port)] = suspect_shard_id
-    
+
     async def cleanup_pending_checks(self):
-        for pending_check in list(self._active_checks_queue):
-            if pending_check.done() or pending_check.cancelled():
-                self._active_checks_queue.remove(pending_check)
 
-                await asyncio.sleep(self._cleanup_interval)
+        while self._running:
+
+            for pending_check in list(self._active_checks_queue):
+                if pending_check.done() or pending_check.cancelled():
+                    self._active_checks_queue.remove(pending_check)
+
+            monitoring = dict(self._monitoring)
+            for host, port in self._removed_nodes:
+
+                if monitoring.get((host, port)) is False:
+                    await self.remove_clients(
+                        HealthCheck(
+                            host=host,
+                            port=port,
+                            source_host=self.host,
+                            source_port=self.port,
+                            status='removed'
+                        )
+                    )
+
+                    del monitoring[(host, port)]
 
+            self._removed_nodes.clear()
+            self._monitoring = monitoring
+
+            await asyncio.sleep(self._cleanup_interval)
+
+    
     async def shutdown(self):
         self._running = False
         self._local_health_monitor.cancel()
 
         await asyncio.gather(*[
             cancel(remote_check) for remote_check in self._healthchecks.values()
         ])
```

### Comparing `mercury-sync-0.3.0/mercury_sync/service/service.py` & `mercury-sync-0.3.1/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.3.1/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.3.1/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.3.1/mercury_sync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.0
+Version: 0.3.1
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.0/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.3.1/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.0/setup.py` & `mercury-sync-0.3.1/setup.py`

 * *Files identical despite different names*

