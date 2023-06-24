# Comparing `tmp/mercury-sync-0.3.1.tar.gz` & `tmp/mercury-sync-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.3.1.tar", last modified: Sat Jun 24 00:25:44 2023, max compression
+gzip compressed data, was "mercury-sync-0.3.2.tar", last modified: Sat Jun 24 06:01:55 2023, max compression
```

## Comparing `mercury-sync-0.3.1.tar` & `mercury-sync-0.3.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/models/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/models/ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18901 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/service/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    23296 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/service/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/mercury_sync/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/types/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/mercury_sync/types/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:25:44.919989 mercury-sync-0.3.1/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 00:25:44.000000 mercury-sync-0.3.1/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-24 00:25:44.000000 mercury-sync-0.3.1/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:25:44.000000 mercury-sync-0.3.1/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 00:25:44.000000 mercury-sync-0.3.1/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 00:25:44.000000 mercury-sync-0.3.1/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 00:25:44.923989 mercury-sync-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-24 00:25:37.000000 mercury-sync-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/models/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/models/ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/service/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29990 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/service/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/mercury_sync/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/types/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/types/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 06:01:55.000000 mercury-sync-0.3.2/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-24 06:01:55.000000 mercury-sync-0.3.2/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 06:01:55.000000 mercury-sync-0.3.2/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 06:01:55.000000 mercury-sync-0.3.2/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 06:01:55.000000 mercury-sync-0.3.2/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/setup.py
```

### Comparing `mercury-sync-0.3.1/LICENSE` & `mercury-sync-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/PKG-INFO` & `mercury-sync-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.1
+Version: 0.3.2
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.1/README.md` & `mercury-sync-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.3.2/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,15 +164,25 @@
                 cert_path=cert_path,
                 key_path=key_path
             ) 
 
         if self.connected is False and worker_socket is None:
             self._server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self._server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            self._server_socket.bind((self.host, self.port))
+
+            while True:
+
+                try:
+
+                    self._server_socket.bind((self.host, self.port))
+                    break
+
+                except Exception:
+                    self.port += 1
+ 
 
             self._server_socket
 
             self._server_socket.setblocking(False)
 
         elif self.connected is False:
             self._server_socket = worker_socket
@@ -294,19 +304,27 @@
         address: Tuple[str, int]
     ) -> Tuple[int, Dict[str, Any]]:
         
         async with self._semaphore:
             self._last_call.append(event_name)
 
             client_transport = self._client_transports.get(address)
+            if client_transport is None:
+                await self.connect_client(
+                    address,
+                    cert_path=self._client_cert_path,
+                    key_path=self._client_key_path
+                )
+
+                client_transport = self._client_transports.get(address)
 
             item = pickle.dumps(
                 (
                     'request',
-                    next(self.id_generator),
+                    self.id_generator.generate(),
                     event_name,
                     data,
                     self.host,
                     self.port
                 ),
                 protocol=pickle.HIGHEST_PROTOCOL
             )
@@ -348,29 +366,29 @@
             client_transport = self._client_transports.get(address)
 
 
             if self._stream is False:
                 item = pickle.dumps(
                     (
                         'stream_connect',
-                        next(self.id_generator),
+                        self.id_generator.generate(),
                         event_name,
                         data,
                         self.host,
                         self.port
                     ),
                     protocol=pickle.HIGHEST_PROTOCOL
                 )
 
 
             else:
                 item = pickle.dumps(
                     (
                         'stream',
-                        next(self.id_generator),
+                        self.id_generator.generate(),
                         event_name,
                         data,
                         self.host,
                         self.port
                     ),
                     protocol=pickle.HIGHEST_PROTOCOL
                 )
@@ -390,15 +408,15 @@
                 self.queue[event_name].pop()
 
                 self._stream = True
 
                 item = pickle.dumps(
                     (
                         'stream',
-                        next(self.id_generator),
+                        self.id_generator.generate(),
                         event_name,
                         data,
                         self.host,
                         self.port
                     ),
                     pickle.HIGHEST_PROTOCOL
                 )
@@ -605,15 +623,15 @@
         transport: asyncio.Transport
     ) -> Coroutine[Any, Any, None]:
         response: Message = await coroutine
 
         item = pickle.dumps(
             (
                 'response', 
-                next(self.id_generator),
+                self.id_generator.generate(),
                 event_name,
                 response.to_data(), 
                 self.host,
                 self.port
             ),
             protocol=pickle.HIGHEST_PROTOCOL
         )
@@ -630,15 +648,15 @@
         transport: asyncio.Transport       
     ) -> Coroutine[Any, Any, None]:
   
         async for response in coroutine:
             item = pickle.dumps(
                 (
                     'response', 
-                    next(self.id_generator),
+                    self.id_generator.generate(),
                     event_name,
                     response.to_data(), 
                     self.host,
                     self.port
                 ),
                 protocol=pickle.HIGHEST_PROTOCOL
             )
@@ -653,15 +671,15 @@
         event_name: str,
         transport: asyncio.Transport            
     ) -> Coroutine[Any, Any, None]:
         message = Message()
         item = pickle.dumps(
             (
                 'response', 
-                next(self.id_generator),
+                self.id_generator.generate(),
                 event_name,
                 message.to_data(), 
                 self.host,
                 self.port
             ),
             protocol=pickle.HIGHEST_PROTOCOL
         )
@@ -680,15 +698,15 @@
         error = Message(
             error=error_message
         )
 
         item = pickle.dumps(
             (
                 'response', 
-                next(self.id_generator),
+                self.id_generator.generate(),
                 None,
                 error.to_data(), 
                 self.host,
                 self.port
             ),
             protocol=pickle.HIGHEST_PROTOCOL
         )
```

### Comparing `mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.3.2/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.3.2/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.3.2/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/env/env.py` & `mercury-sync-0.3.2/mercury_sync/env/env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/env/load_env.py` & `mercury-sync-0.3.2/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/env/time_parser.py` & `mercury-sync-0.3.2/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.3.2/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.3.2/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/service/controller.py` & `mercury-sync-0.3.2/mercury_sync/service/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,14 +443,18 @@
         ):
       
             await udp_connection.connect_async(
                 cert_path=cert_path,
                 key_path=key_path
             )
 
+            await tcp_connection.connect_async(
+                cert_path=cert_path,
+                key_path=key_path
+            )
 
             await self._udp_queue[(remote.host, remote.port)].put(udp_connection)
             await self._tcp_queue[(remote.host, remote.port)].put(tcp_connection)
 
             self._host_map[remote.__class__.__name__][udp_connection] = (
                 remote_copy.host, 
                 remote_copy.port
@@ -462,18 +466,18 @@
             )
 
         for tcp_connection, remote_copy in zip(
             tcp_pool,
             remote_pool
         ):
             await tcp_connection.connect_client(
-                    (remote_copy.host, remote_copy.port + 1),
-                    cert_path=cert_path,
-                    key_path=key_path
-                )
+                (remote_copy.host, remote_copy.port + 1),
+                cert_path=cert_path,
+                key_path=key_path
+            )
             
         self._udp_pool.extend(udp_pool)
         self._tcp_pool.extend(tcp_pool)
 
         return port
     
     async def refresh_clients(
@@ -547,15 +551,14 @@
         return shard_id, response_data
     
     async def send_tcp(
         self,
         event_name: str,
         message: Message
     ):
-
         connection: MercurySyncTCPConnection = await self._tcp_queue[(message.host, message.port)].get()
         (host, port) = self._host_map.get(message.__class__.__name__).get(connection)
         address = (
             host,
             port + 1
         )
```

### Comparing `mercury-sync-0.3.1/mercury_sync/service/monitor.py` & `mercury-sync-0.3.2/mercury_sync/service/monitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,15 +52,17 @@
             cert_path=cert_path,
             key_path=key_path,
             workers=workers,
             env=env,
             engine=engine
         )
 
-        self.health: HealthStatus = 'initializing'
+        self.status: HealthStatus = 'initializing'
+        
+
         self.error_context: Optional[str] = None
         self.registration_timeout = TimeParser(env.MERCURY_SYNC_REGISTRATION_TIMEOUT).time
         self.boot_wait = TimeParser(env.MERCURY_SYNC_BOOT_WAIT).time
 
         self._healthchecks: Dict[str, asyncio.Task] = {}
         self._registered: Dict[int, Tuple[str, int]] = {}
         self._running = False
@@ -78,14 +80,15 @@
         self._suspect_nodes: Dict[Tuple[str, int], List[int]] = {}
         self._removed_nodes: Dict[Tuple[str, int], List[int]] = {}
 
         self._active_probes: Dict[Tuple[str, int], bool] = {}
         self._failed_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
         self._suspect_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
         self._cleanup_task: Union[asyncio.Task, None] = None
+        self._investigating_nodes: Dict[Tuple[str, int], Dict[Tuple[str, int]]] = defaultdict(dict)
 
     @server()
     async def update_active(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
@@ -100,24 +103,24 @@
             self._monitoring[(target_host, target_port)] = True
 
             await self.push_new_node(
                 target_host,
                 target_port,
                 self.host,
                 self.port,
-                self.health,
+                self.status,
                 error_context=self.error_context
             )
 
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
-            status=self.health,
+            status=self.status,
             error=self.error_context
         )
 
     @server()
     async def update_suspect(
         self,
         shard_id: int,
@@ -125,55 +128,70 @@
     ) -> Call[HealthCheck]:
         
         target_host = healthcheck.target_host
         target_port = healthcheck.target_port
         shard_ids = healthcheck.shard_ids
 
         self._suspect_nodes[(target_host, target_port)] = shard_ids
-
-        if self._suspect_tasks.get((target_host, target_port)) is None:
-            self._suspect_tasks[(target_host, target_port)] = asyncio.create_task(
-                self._start_suspect_monitor()
-            )
+        self._monitoring[(target_host, target_port)] = False
 
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
-            status=self.health,
+            status=self.status,
             error=self.error_context
         )
 
 
     @server()
     async def send_indirect_check(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
         try:
-            _, response = await asyncio.wait_for(
+
+            investigation_update = self._push_investigating_update(
+                host=healthcheck.source_host,
+                port=healthcheck.source_port,
+                target_host=healthcheck.target_host,
+                target_port=healthcheck.target_port,
+                timeout=self._poll_timeout
+            )
+
+            indirect_probe = asyncio.wait_for(
                 self.push_health_update(
                     healthcheck.target_host,
                     healthcheck.target_port,
                     healthcheck.status,
                     error_context=healthcheck.error
                 ),
                 timeout=self._poll_timeout
             )
 
-            return HealthCheck(
-                host=healthcheck.source_host,
-                port=healthcheck.source_port,
-                source_host=response.source_host,
-                source_port=response.source_port,
-                status=response.status,
-                error=response.error
-            )
+            for task in asyncio.as_completed([
+                investigation_update,
+                indirect_probe
+            ]):
+                result: Union[Tuple[int, HealthCheck], None] = await task
+
+                if isinstance(result, tuple):
+
+                    _, response = result
+
+                    return HealthCheck(
+                        host=healthcheck.source_host,
+                        port=healthcheck.source_port,   
+                        source_host=response.source_host,
+                        source_port=response.source_port,
+                        status=response.status,
+                        error=response.error
+                    )
 
         except asyncio.TimeoutError:
 
             self._monitoring[(healthcheck.target_host, healthcheck.target_port)] = False
 
             return HealthCheck(
                 host=healthcheck.source_host,
@@ -202,15 +220,15 @@
             suspect_task = suspect_tasks.get((host, port))
 
             if suspect_task:
                 await cancel(suspect_task)
                 del suspect_tasks[(host, port)]
                 
                 self._suspect_tasks = suspect_tasks
-
+            
             await self.extend_client(
                 HealthCheck(
                     host=host,
                     port=port,
                     source_host=self.host,
                     source_port=self.port,
                     status=healthcheck.status,
@@ -222,18 +240,17 @@
 
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
             error=self.error_context,
-            status=self.health
+            status=self.status
         )
         
-
     @server()
     async def register_health_update(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
         
@@ -246,14 +263,23 @@
         suspect_task = suspect_tasks.get((source_host, source_port))
 
         if suspect_task:
             await cancel(suspect_task)
             del suspect_tasks[(source_host, source_port)]
 
             self._suspect_tasks = suspect_tasks
+        
+        if healthcheck.status == 'investigating':
+
+            target_host = healthcheck.target_host
+            target_port =healthcheck.target_port
+
+            self._investigating_nodes[(target_host, target_port)].update({
+                (source_host, source_port): healthcheck.status
+            })
 
         if not monitor_exists_status:
 
             monitoring = [
                 address for address, monitoring_status in self._monitoring.items() if monitoring_status
             ]
             
@@ -300,30 +326,55 @@
 
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
             error=self.error_context,
-            status=self.health
+            status=self.status
         )
 
     @client('register_health_update')
     async def push_health_update(
         self,
         host: str,
         port: int,
         health_status: HealthStatus,
+        target_host: Optional[str]=None,
+        target_port: Optional[str]=None,
         error_context: Optional[str]=None
     ) -> Call[HealthCheck]:
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
+            target_host=target_host,
+            target_port=target_port,
+            error=error_context,
+            status=health_status
+        )
+    
+    @client('register_health_update', as_tcp=True)
+    async def push_tcp_health_update(
+        self,
+        host: str,
+        port: int,
+        health_status: HealthStatus,
+        target_host: Optional[str]=None,
+        target_port: Optional[str]=None,
+        error_context: Optional[str]=None
+    ) -> Call[HealthCheck]:
+        return HealthCheck(
+            host=host,
+            port=port,
+            source_host=self.host,
+            source_port=self.port,
+            target_host=target_host,
+            target_port=target_port,
             error=error_context,
             status=health_status
         )
     
     @client('register_new_node')
     async def push_new_node(
         self,
@@ -405,14 +456,15 @@
             target_host=target_host,
             target_port=target_port,
             source_host=self.host,
             source_port=self.port,
             error=error_context,
             status=health_status
         )
+        
     
     async def start(self):
 
         await self.start_server()
         await asyncio.sleep(self.boot_wait)
 
     async def register(
@@ -425,36 +477,73 @@
             asyncio.create_task(
                 self.start_client(
                     HealthCheck(
                         host=host,
                         port=port,
                         source_host=self.host,
                         source_port=self.port,
-                        status=self.health
+                        status=self.status
                     ),
                     cert_path=self.cert_path,
                     key_path=self.key_path
                 )
             ),
             timeout=self.registration_timeout
         )
 
         self._monitoring[(host, port)] = True
 
-        self.health = 'healthy'
+        self.status = 'healthy'
         self._running = True
         
         self._healthchecks[(host, port)] = asyncio.create_task(
             self.start_health_monitor()
         )
         
         self.confirmation_task = asyncio.create_task(
             self.cleanup_pending_checks()
         )
     
+    async def _push_investigating_update(
+        self,
+        host: str,
+        port: int,
+        target_host: str,
+        target_port: int,
+        timeout: float
+    ):
+        try:
+            await asyncio.sleep(0.8 * timeout)
+
+            await asyncio.wait_for(
+                self.push_health_update(
+                    host=host,
+                    port=port,
+                    target_host=target_host,
+                    target_port=target_port,
+                    health_status='investigating',
+                    error_context=self.error_context
+                ),
+                timeout=self._poll_timeout
+            )
+
+        except asyncio.TimeoutError:
+            if not self._active_probes.get((host, port)):
+                self._active_probes[(host, port)] = True
+                self._failed_nodes.append((
+                    host,
+                    port
+                ))
+
+                self._failed_tasks[(host, port)] = asyncio.create_task(
+                    self._probe_timed_out_node()
+                )
+            
+            self._monitoring[(host, port)] = False
+    
     async def _update_suspect_nodes(
         self,
         confirmation_members: List[Tuple[str, int]],
         successful_requests: Dict[Tuple[str, int], int]
     ):
         for node_host, node_port in confirmation_members:
 
@@ -478,127 +567,204 @@
 
         try:
 
             await asyncio.wait_for(
                 self.push_health_update(
                     host,
                     port,
-                    self.health,
+                    self.status,
                     error_context=self.error_context
                 ),
                 timeout=self._poll_timeout
             )
 
         except asyncio.TimeoutError:
             if not self._active_probes.get((host, port)):
+                self.status = 'investigating'
+
                 self._active_probes[(host, port)] = True
                 self._failed_nodes.append((
                     host,
                     port
                 ))
 
                 self._failed_tasks[(host, port)] = asyncio.create_task(
                     self._probe_timed_out_node()
                 )
             
             self._monitoring[(host, port)] = False
 
     async def _probe_timed_out_node(self):
 
-
         host, port = self._failed_nodes.pop()
+        
+        confirmation_members = self._get_confirmation_members()
 
-        confirmation_members = list(filter(
-            lambda address: address[0] != host and address[1] != port,
-            self._monitoring.keys()
-        ))
-
-        confirmation_candidates_count = len(confirmation_members) 
-
-        if confirmation_candidates_count < self._check_nodes_count:
-            self._check_nodes_count = confirmation_candidates_count
-
-        confirmation_members = [
-            random.sample(
-                confirmation_members, 
-                1
-            )[0] for _ in range(
-                self._check_nodes_count
-            )
-        ]
-
-        if len(confirmation_members) < 1:
-            self._monitoring[(host, port)] = True
-            return
-
-        check_tasks: Tuple[List[asyncio.Task], List[asyncio.Task]] = await asyncio.wait([
-            asyncio.create_task(
-                self.request_indirect_check(
-                    node_host,
-                    node_port,
-                    host,
-                    port,
-                    self.health,
-                    error_context=self.error_context
-                )
-            ) for node_host, node_port in confirmation_members
-        ], timeout=self._poll_timeout * 2)
-
-        completed, pending = check_tasks
+        healthchecks, suspect_count = await self._request_indirect_probe(
+            host,
+            port,
+            confirmation_members
+        )
 
-        healthchecks: List[Call[HealthCheck]]  = await asyncio.gather(*completed)
+        indirect_ack_count = len(self._investigating_nodes[(host, port)])
 
-        suspect_count = len([
-            response for _, response in healthchecks if response.status == 'suspect'
-        ]) + len(pending)
+        if len(confirmation_members) > indirect_ack_count:
+            # If we have received more results from other
+            # nodes than nacks we may be a degraded node.
+            self.status = 'degraded'
 
-        await asyncio.gather(*[
-            cancel(pending_check) for pending_check in pending
-        ])
+        elif suspect_count >= len(confirmation_members):
 
-        if suspect_count == len(confirmation_members):
             self._suspect_nodes[(host, port)] = [
                 shard_id for shard_id, _ in healthchecks
             ]
 
-            responses = await asyncio.gather(*[
+            await asyncio.gather(*[
                 asyncio.wait_for(
                     self.submit_suspect_node(
                         node_host,
                         node_port,
                         host,
                         port,
                         self._suspect_nodes.get(
                             (host, port),
                             []
                         ),
-                        self.health,
+                        self.status,
                         error_context=self.error_context
                     ),
                     timeout=self._poll_timeout
                 ) for node_host, node_port in confirmation_members
             ], return_exceptions=True)
 
-            successful_requests: Dict[Tuple[str, int], int] = {}
-            for response in responses:
-                if isinstance(response, tuple):
-                    shard_id, healthcheck = response
-                    successful_requests[(healthcheck.source_host, healthcheck.source_port)] = shard_id
+            self._suspect_tasks[(host, port)] = asyncio.create_task(
+                self._start_suspect_monitor()
+            )
+
+        else:
+            self._monitoring[(host, port)] = True 
 
             await self._update_suspect_nodes(
                 confirmation_members,
-                successful_requests
+                self._investigating_nodes[(host, port)]
             )
 
-            self._suspect_tasks[(host, port)] = asyncio.create_task(
-                self._start_suspect_monitor()
-            )
+        del self._investigating_nodes[(host, port)]
+            
+    def _get_confirmation_members(self) -> List[Tuple[str, int]]:
+        confirmation_members = [
+            address for address, monitoring_status in self._monitoring.items() if monitoring_status
+        ]
 
+        confirmation_candidates_count = len(confirmation_members) 
+
+        if confirmation_candidates_count < self._check_nodes_count:
+            self._check_nodes_count = confirmation_candidates_count
+
+        confirmation_members = random.sample(
+            confirmation_members, 
+            self._check_nodes_count
+        )
+
+        return confirmation_members
+
+    async def _request_indirect_probe(
+        self,
+        host: str,
+        port: int,
+        confirmation_members: List[Tuple[str, int]]
+    ) -> Tuple[List[Call[HealthCheck]], int]:
+
+        if len(confirmation_members) < 1:
+            requested_checks = [
+                asyncio.create_task(
+                    self.push_tcp_health_update(
+                        host,
+                        port,
+                        self.status,
+                        error_context=self.error_context
+                    )
+                )
+            ]
+        
         else:
-            self._monitoring[(host, port)] = True 
+            requested_checks = [
+                asyncio.create_task(
+                    self.request_indirect_check(
+                        node_host,
+                        node_port,
+                        host,
+                        port,
+                        self.status,
+                        error_context=self.error_context
+                    )
+                ) for node_host, node_port in confirmation_members
+            ]
+
+            requested_checks.append(
+                asyncio.create_task(
+                    self.push_tcp_health_update(
+                        host,
+                        port,
+                        self.status,
+                        error_context=self.error_context
+                    )
+                )
+            )
+
+
+        check_tasks: Tuple[List[asyncio.Task], List[asyncio.Task]] = await asyncio.wait(
+            requested_checks, 
+            timeout=self._poll_timeout * 2
+        )
+
+        completed, pending = check_tasks
+
+        healthchecks: List[Call[HealthCheck]]  = await asyncio.gather(*completed)
+
+        sorted_checks: List[Call[HealthCheck]] = list(sorted(
+            healthchecks,
+            key=lambda check: check[0]
+        ))
+
+        suspect = [
+            (
+                shard_id,
+                check
+            ) for shard_id, check in sorted_checks if check.status == 'suspect'
+        ]
+
+        healthy = [
+            (
+                shard_id,
+                check
+            ) for shard_id, check in sorted_checks if check.status == 'healthy' or check.status == 'investigating'
+        ]
+
+        suspect_checks: List[Call[HealthCheck]] = []
+        for suspect_shard_id, suspect_check in suspect:
+
+            newer_count = 0
+            for healthy_shard_id, _ in healthy:
+                if suspect_shard_id > healthy_shard_id:
+                    newer_count += 1
+
+            if newer_count >= len(healthy):
+                suspect_checks.append((
+                    suspect_shard_id,
+                    suspect_check
+                ))
+
+        suspect_count = len(suspect_checks) + len(pending)
+        
+        await asyncio.gather(*[
+            cancel(pending_check) for pending_check in pending
+        ])
+
+        return healthchecks, suspect_count
 
     async def run_forever(self):
         self._waiter = asyncio.Future()
         await self._waiter
 
     async def start_health_monitor(self):
         
@@ -651,65 +817,106 @@
             await cancel(confirmation_task)
             confirmation_task.cancel()
 
         node_revived = False
 
         while elapsed < self._max_suspect_timeout:
             
-            try:
-                _, healthcheck = await asyncio.wait_for(
-                    self.push_health_update(
-                        suspect_host,
-                        suspect_port,
-                        self.health,
-                        error_context=self.error_context
-                    ),
-                    timeout=self._poll_timeout
-                )
+            confirmation_members = self._get_confirmation_members()
+
+            healthchecks, suspect_count = await self._request_indirect_probe(
+                suspect_host,
+                suspect_port,
+                confirmation_members
+            )
+
+            indirect_ack_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
+
+            suspect_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
+
+            if len(confirmation_members) > indirect_ack_count:
+                # If we have received more results from other
+                # nodes than nacks we may be a degraded node.
+                self.status = 'degraded'
+
+            elif suspect_count >= len(confirmation_members):
+                # All members have confirmed suspect.
+
+                self._suspect_nodes[(suspect_host, suspect_port)] = [
+                    shard_id for shard_id, _ in healthchecks
+                ]
+
+                await asyncio.gather(*[
+                    asyncio.wait_for(
+                        self.submit_suspect_node(
+                            node_host,
+                            node_port,
+                            suspect_host,
+                            suspect_port,
+                            self._suspect_nodes.get(
+                                (suspect_host, suspect_port),
+                                []
+                            ),
+                            self.status,
+                            error_context=self.error_context
+                        ),
+                        timeout=self._poll_timeout
+                    ) for node_host, node_port in confirmation_members
+                ], return_exceptions=True)
+
+            else:
+                # We had a majority confirmation the node was healthy.
+
+                self._monitoring[(suspect_host, suspect_port)] = True 
 
                 monitoring = [
                     address for address, monitoring_status in self._monitoring.items() if monitoring_status
                 ]
 
                 for host, port in monitoring:
                     if self._suspect_nodes.get((host, port)) is None:
                         await self.submit_active_node(
                             host,
                             port,
-                            healthcheck.source_host,
-                            healthcheck.source_port,
-                            health_status=healthcheck.status,
-                            error_context=healthcheck.error
+                            suspect_host,
+                            suspect_port,
+                            health_status='healthy'
                         )
 
                 await self.refresh_clients(
                     HealthCheck(
                         host=suspect_host,
                         port=suspect_port,
                         source_host=self.host,
                         source_port=self.port,
-                        status=healthcheck.status,
-                        error=healthcheck.error
+                        status='healthy'
                     )
                 )
-                    
+
+                await self._update_suspect_nodes(
+                    confirmation_members,
+                    self._investigating_nodes[(suspect_host, suspect_port)]
+                )
+                
                 self._monitoring[(suspect_host, suspect_port)] = True
 
                 node_revived = True
                 break
 
-            except asyncio.TimeoutError:
-                pass
+            del self._investigating_nodes[(suspect_host, suspect_port)]
 
             await asyncio.sleep(self._poll_interval) 
             elapsed = time.monotonic() - start
         
         if node_revived is False:
             self._removed_nodes[(suspect_host, suspect_port)] = suspect_shard_id
 
+        if self.status == 'investigating':
+            self.status = 'healthy'
+
     async def cleanup_pending_checks(self):
 
         while self._running:
 
             for pending_check in list(self._active_checks_queue):
                 if pending_check.done() or pending_check.cancelled():
                     self._active_checks_queue.remove(pending_check)
```

### Comparing `mercury-sync-0.3.1/mercury_sync/service/service.py` & `mercury-sync-0.3.2/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.3.2/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.3.2/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.3.2/mercury_sync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.1
+Version: 0.3.2
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.1/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.3.2/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.1/setup.py` & `mercury-sync-0.3.2/setup.py`

 * *Files identical despite different names*

