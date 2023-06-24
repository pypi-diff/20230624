# Comparing `tmp/mercury-sync-0.3.2.tar.gz` & `tmp/mercury-sync-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.3.2.tar", last modified: Sat Jun 24 06:01:55 2023, max compression
+gzip compressed data, was "mercury-sync-0.3.3.tar", last modified: Sat Jun 24 21:43:40 2023, max compression
```

## Comparing `mercury-sync-0.3.2.tar` & `mercury-sync-0.3.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/models/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/models/ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/service/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    29990 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/service/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/mercury_sync/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/types/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/mercury_sync/types/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:01:55.484555 mercury-sync-0.3.2/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 06:01:55.000000 mercury-sync-0.3.2/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-24 06:01:55.000000 mercury-sync-0.3.2/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 06:01:55.000000 mercury-sync-0.3.2/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 06:01:55.000000 mercury-sync-0.3.2/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 06:01:55.000000 mercury-sync-0.3.2/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 06:01:55.488555 mercury-sync-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-24 06:01:52.000000 mercury-sync-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/models/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/models/ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/service/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32685 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/service/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/mercury_sync/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/types/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/mercury_sync/types/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:43:40.088667 mercury-sync-0.3.3/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-24 21:43:40.000000 mercury-sync-0.3.3/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-24 21:43:40.000000 mercury-sync-0.3.3/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:43:40.000000 mercury-sync-0.3.3/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 21:43:40.000000 mercury-sync-0.3.3/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 21:43:40.000000 mercury-sync-0.3.3/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:43:40.092667 mercury-sync-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-24 21:43:37.000000 mercury-sync-0.3.3/setup.py
```

### Comparing `mercury-sync-0.3.2/LICENSE` & `mercury-sync-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/PKG-INFO` & `mercury-sync-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.2
+Version: 0.3.3
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.2/README.md` & `mercury-sync-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.3.3/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.3.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.3.3/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.3.3/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.3.3/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/env/env.py` & `mercury-sync-0.3.3/mercury_sync/env/env.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,27 +12,33 @@
 
 
 PrimaryType = Union[str, int, float, bytes, bool]
 
 
 class Env(BaseModel):
     MERCURY_SYNC_BOOT_WAIT: StrictStr='5s'
-    MERCURY_SYNC_MAX_SUSPECT_TIMEOUT: StrictStr='10s'
+    MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD=3
+    MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=7
+    MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER: StrictInt=10
+    MERCURY_SYNC_INITIAL_NODES_COUNT: StrictInt=3
     MERCURY_SYNC_HEALTH_CHECK_TIMEOUT: StrictStr='1s'
     MERCURY_SYNC_REGISTRATION_TIMEOUT: StrictStr='1m'
     MERCURY_SYNC_HEALTH_POLL_INTERVAL: StrictFloat='0.2s'
     MERCURY_SYNC_INDIRECT_CHECK_NODES: StrictInt=1
     MERCURY_SYNC_CLEANUP_INTERVAL: StrictStr='10s'
     MERCURY_SYNC_MAX_CONCURRENCY: StrictInt=2048
     MERCURY_SYNC_AUTH_SECRET: StrictStr
 
     @classmethod
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
         return {
-            'MERCURY_SYNC_MAX_SUSPECT_TIMEOUT': str,
+            'MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD': int,
+            'MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER': int,
+            'MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER': int,
+            'MERCURY_SYNC_INITIAL_NODES_COUNT': int,
             'MERCURY_SYNC_BOOT_WAIT': str,
             'MERCURY_SYNC_REGISTRATION_TIMEOUT': str,
             'MERCURY_SYNC_HEALTH_POLL_INTERVAL': str,
             'MERCURY_SYNC_INDIRECT_CHECK_NODES': int,
             'MERCURY_SYNC_CLEANUP_INTERVAL': str,
             'MERCURY_SYNC_MAX_CONCURRENCY': int,
             'MERCURY_SYNC_AUTH_SECRET': str
```

### Comparing `mercury-sync-0.3.2/mercury_sync/env/load_env.py` & `mercury-sync-0.3.3/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/env/time_parser.py` & `mercury-sync-0.3.3/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.3.3/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.3.3/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/service/controller.py` & `mercury-sync-0.3.3/mercury_sync/service/controller.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/service/monitor.py` & `mercury-sync-0.3.3/mercury_sync/service/monitor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
+import math
 import random
 import time
-import traceback
 from collections import defaultdict, deque
 from mercury_sync.env import Env, load_env
 from mercury_sync.env.time_parser import TimeParser
 from mercury_sync.hooks.client_hook import client
 from mercury_sync.hooks.server_hook import server
 from mercury_sync.models.healthcheck import HealthCheck, HealthStatus
 from mercury_sync.models.ticket import Ticket
@@ -65,268 +65,313 @@
 
         self._healthchecks: Dict[str, asyncio.Task] = {}
         self._registered: Dict[int, Tuple[str, int]] = {}
         self._running = False
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
         self._poll_interval = TimeParser(env.MERCURY_SYNC_HEALTH_POLL_INTERVAL).time
         self._poll_timeout = TimeParser(env.MERCURY_SYNC_HEALTH_CHECK_TIMEOUT).time
-        self._max_suspect_timeout = TimeParser(env.MERCURY_SYNC_MAX_SUSPECT_TIMEOUT).time
         self._check_nodes_count = env.MERCURY_SYNC_INDIRECT_CHECK_NODES
 
+        self.min_suspect_multiplier = env.MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER
+        self.max_suspect_multiplier = env.MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER 
+        self._min_suspect_node_count = env.MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD
+        self._local_health_multiplier = self.max_suspect_multiplier
+
         self._local_health_monitor: Optional[asyncio.Task] = None
-        self._monitoring: Dict[Tuple[str, int], bool] = defaultdict(lambda: False)
+        self._confirmed_suspicions: Dict[Tuple[str, int], int] = {}
         self._waiter: Optional[asyncio.Future] = None
         self._active_checks_queue: Deque[asyncio.Task] = deque()
-        self._failed_nodes: Deque[Tuple[str, int]] = deque()
-        self._suspect_nodes: Dict[Tuple[str, int], List[int]] = {}
-        self._removed_nodes: Dict[Tuple[str, int], List[int]] = {}
+        self._degraded_nodes: Deque[Tuple[str, int]] = deque()
+        self._suspect_nodes: Deque[Tuple[str, int]] = deque()
 
-        self._active_probes: Dict[Tuple[str, int], bool] = {}
         self._failed_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
         self._suspect_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._investigating_nodes: Dict[Tuple[str, int], Dict[Tuple[str, int]]] = defaultdict(dict)
+        self._node_statuses: Dict[Tuple[str, int], HealthStatus] = {}
+        self._healthy_statuses = [
+            'healthy'
+        ]
+
+        self._unhealthy_statuses = [
+            'degraded',
+            'suspect',
+            'failed'
+        ]
 
     @server()
-    async def update_active(
+    async def send_indirect_check(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
         
+        source_host = healthcheck.source_host
+        source_port = healthcheck.source_port
+
         target_host = healthcheck.target_host
         target_port = healthcheck.target_port
 
-        if self._suspect_nodes.get((target_host, target_port)):
-            del self._suspect_nodes[(target_host, target_port)]
-
-        if target_host != self.host and target_port != self.port:
-            self._monitoring[(target_host, target_port)] = True
+        try:
 
-            await self.push_new_node(
+            investigation_update = self._acknowledge_indirect_probe(
+                source_host,
+                source_port,
                 target_host,
-                target_port,
-                self.host,
-                self.port,
-                self.status,
-                error_context=self.error_context
+                target_port
             )
 
-        return HealthCheck(
-            host=healthcheck.source_host,
-            port=healthcheck.source_port,
-            source_host=self.host,
-            source_port=self.port,
-            status=self.status,
-            error=self.error_context
-        )
-
-    @server()
-    async def update_suspect(
-        self,
-        shard_id: int,
-        healthcheck: HealthCheck
-    ) -> Call[HealthCheck]:
-        
-        target_host = healthcheck.target_host
-        target_port = healthcheck.target_port
-        shard_ids = healthcheck.shard_ids
-
-        self._suspect_nodes[(target_host, target_port)] = shard_ids
-        self._monitoring[(target_host, target_port)] = False
-
-        return HealthCheck(
-            host=healthcheck.source_host,
-            port=healthcheck.source_port,
-            source_host=self.host,
-            source_port=self.port,
-            status=self.status,
-            error=self.error_context
-        )
-
 
-    @server()
-    async def send_indirect_check(
-        self,
-        shard_id: int,
-        healthcheck: HealthCheck
-    ) -> Call[HealthCheck]:
-        try:
-
-            investigation_update = self._push_investigating_update(
-                host=healthcheck.source_host,
-                port=healthcheck.source_port,
-                target_host=healthcheck.target_host,
-                target_port=healthcheck.target_port,
-                timeout=self._poll_timeout
-            )
+            self._node_statuses[(target_host, target_port)] = healthcheck.target_status
 
             indirect_probe = asyncio.wait_for(
                 self.push_health_update(
-                    healthcheck.target_host,
-                    healthcheck.target_port,
-                    healthcheck.status,
+                    target_host,
+                    target_port,
+                    self.status,
                     error_context=healthcheck.error
                 ),
-                timeout=self._poll_timeout
+                timeout=self._poll_timeout * (self._local_health_multiplier + 1)
             )
 
             for task in asyncio.as_completed([
                 investigation_update,
                 indirect_probe
             ]):
                 result: Union[Tuple[int, HealthCheck], None] = await task
 
                 if isinstance(result, tuple):
 
                     _, response = result
 
+                    self._local_health_multiplier = max(
+                        0, 
+                        self._local_health_multiplier - 1
+                    )
+
+                    self._node_statuses[(target_host, target_port)]  = response.status
+
+                    # We've received a refutation
                     return HealthCheck(
                         host=healthcheck.source_host,
-                        port=healthcheck.source_port,   
+                        port=healthcheck.source_port,
+                        target_status=response.status,   
                         source_host=response.source_host,
                         source_port=response.source_port,
                         status=response.status,
                         error=response.error
                     )
 
         except asyncio.TimeoutError:
 
-            self._monitoring[(healthcheck.target_host, healthcheck.target_port)] = False
-
+            # Our suspicion is correct!
             return HealthCheck(
                 host=healthcheck.source_host,
                 port=healthcheck.source_port,
-                source_host=healthcheck.target_host,
-                source_port=healthcheck.target_port,
-                status='suspect',
-                error='timeout'
+                source_host=target_host,
+                source_port=target_port,
+                target_status=healthcheck.status, 
+                status=self.status
             )
         
-
     @server()
     async def register_new_node(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
         host = healthcheck.source_host
         port = healthcheck.source_port
 
         not_self = host != self.host and port != self.port
-
+        
         if not_self:
 
             suspect_tasks = dict(self._suspect_tasks)
             suspect_task = suspect_tasks.get((host, port))
 
             if suspect_task:
                 await cancel(suspect_task)
                 del suspect_tasks[(host, port)]
                 
                 self._suspect_tasks = suspect_tasks
+
+            self._node_statuses[(host, port)] =  'healthy'
             
             await self.extend_client(
                 HealthCheck(
                     host=host,
                     port=port,
                     source_host=self.host,
                     source_port=self.port,
                     status=healthcheck.status,
                     error=healthcheck.error
                 )
             )
 
-            self._monitoring[(host, port)] = True
-
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
             error=self.error_context,
             status=self.status
         )
+    
+    @server()
+    async def update_acknowledged(
+        self,
+        shard_id: int,
+        healthcheck: HealthCheck
+    ) -> Call[HealthCheck]:
+        
+        source_host = healthcheck.source_host
+        source_port = healthcheck.source_port
+        target_host = healthcheck.target_host
+        target_port = healthcheck.target_port
+
+        self._investigating_nodes[(target_host, target_port)].update({
+            (source_host, source_port): healthcheck.status
+        })
+
+        return HealthCheck(
+            host=source_host,
+            port=source_port,
+            source_host=self.host,
+            source_port=self.port,
+            status=self.status
+        )
         
     @server()
     async def register_health_update(
         self,
         shard_id: int,
         healthcheck: HealthCheck
     ) -> Call[HealthCheck]:
         
         source_host = healthcheck.source_host
         source_port = healthcheck.source_port
 
-        monitor_exists_status = self._monitoring.get((source_host, source_port))
+        target_host = healthcheck.target_host
+        target_port = healthcheck.target_port
+
+        if target_host and target_port: 
+            self._node_statuses[(target_host, target_port)] = healthcheck.target_status
+
+        local_node_status = self._node_statuses.get((source_host, source_port))
 
         suspect_tasks = dict(self._suspect_tasks)
-        suspect_task = suspect_tasks.get((source_host, source_port))
+        suspect_task = suspect_tasks.pop((source_host, source_port), None)
 
         if suspect_task:
             await cancel(suspect_task)
-            del suspect_tasks[(source_host, source_port)]
 
             self._suspect_tasks = suspect_tasks
-        
-        if healthcheck.status == 'investigating':
-
-            target_host = healthcheck.target_host
-            target_port =healthcheck.target_port
 
-            self._investigating_nodes[(target_host, target_port)].update({
-                (source_host, source_port): healthcheck.status
-            })
+            
+        if healthcheck.target_status == 'suspect' or healthcheck.target_status == 'degraded':
 
-        if not monitor_exists_status:
+            self._local_health_multiplier = min(
+                self._local_health_multiplier + 1,
+                self.max_suspect_multiplier
+            )
 
             monitoring = [
-                address for address, monitoring_status in self._monitoring.items() if monitoring_status
+                address for address, status in self._node_statuses.items() if status in self._healthy_statuses
             ]
+
+            # Send our refutation
+            self._active_checks_queue.extend([
+                asyncio.create_task(
+                    self._run_healthcheck(
+                        host,
+                        port,
+                        target_host=healthcheck.target_host,
+                        target_port=healthcheck.target_port
+                    )
+                ) for host, port in monitoring
+            ])
+
+        status_unhealthy = local_node_status == 'failed' or local_node_status == 'suspect'
+            
+        if local_node_status is None or status_unhealthy:
             
-            for host, port in monitoring:
+            monitoring = [
+                address for address, status in self._node_statuses.items() if status == 'healthy'
+            ]
 
-                await self.push_new_node(
+            await asyncio.gather(*[
+                self.push_new_node(
                     host,
                     port,
                     source_host,
                     source_port,
                     healthcheck.status,
                     error_context=healthcheck.error
-                )
+                ) for host, port in monitoring
+            ])
 
-        if monitor_exists_status is None:
+            self._active_checks_queue.extend([
+                asyncio.create_task(
+                    self._run_healthcheck(
+                        host,
+                        port,
+                    )
+                ) for host, port in monitoring
+            ])
+
+        if local_node_status is None:
 
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
 
-            self._monitoring[(source_host, source_port)] = True
-
-        elif monitor_exists_status is False:
-
+        elif status_unhealthy:
             await self.refresh_clients(
                 HealthCheck(
                     host=source_host,
                     port=source_port,
                     source_host=self.host,
                     source_port=self.port,
                     status=healthcheck.status,
                     error=healthcheck.error
                 )
             )
 
-            self._monitoring[(source_host, source_port)] = True
+        is_buddy = target_host is None and target_port is None
+
+        # Send our refutation
+        if local_node_status == 'suspect' and healthcheck.status == 'healthy' and is_buddy:
+
+            self._node_statuses[(source_host, source_port)] = 'healthy'
+            source_address = (source_host, source_port)
+            monitoring = [
+                address for address, status in self._node_statuses.items() if status in self._healthy_statuses and address != source_address
+            ]
+
+
+            self._active_checks_queue.extend([
+                asyncio.create_task(
+                    self._run_healthcheck(
+                        host,
+                        port,
+                        target_host=source_host,
+                        target_port=source_port
+                    )
+                ) for host, port in monitoring if host != source_host and port != source_port
+            ])
+
+        self._node_statuses[(source_host, source_port)] = healthcheck.status
 
         return HealthCheck(
             host=healthcheck.source_host,
             port=healthcheck.source_port,
             source_host=self.host,
             source_port=self.port,
             error=self.error_context,
@@ -339,42 +384,54 @@
         host: str,
         port: int,
         health_status: HealthStatus,
         target_host: Optional[str]=None,
         target_port: Optional[str]=None,
         error_context: Optional[str]=None
     ) -> Call[HealthCheck]:
+        
+        target_status = self._node_statuses[(host, port)]
+        if target_host and target_port:
+            target_status = self._node_statuses[(target_host, target_port)]
+
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
             target_host=target_host,
             target_port=target_port,
+            target_status=target_status,
             error=error_context,
             status=health_status
         )
     
     @client('register_health_update', as_tcp=True)
     async def push_tcp_health_update(
         self,
         host: str,
         port: int,
         health_status: HealthStatus,
         target_host: Optional[str]=None,
         target_port: Optional[str]=None,
         error_context: Optional[str]=None
     ) -> Call[HealthCheck]:
+        
+        target_status = self._node_statuses[(host, port)]
+        if target_host and target_port:
+            target_status = self._node_statuses[(target_host, target_port)]
+
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
             target_host=target_host,
             target_port=target_port,
+            target_status=target_status,
             error=error_context,
             status=health_status
         )
     
     @client('register_new_node')
     async def push_new_node(
         self,
@@ -390,81 +447,61 @@
             port=port,
             source_host=source_host,
             source_port=source_port,
             error=error_context,
             status=health_status
         )
     
-    @client('send_indirect_check')
-    async def request_indirect_check(
+    @client('update_acknowledged')
+    async def push_acknowledge_check(
         self,
         host: str,
         port: int,
         target_host: str,
         target_port: int,
         health_status: HealthStatus,
+        timeout: float,
         error_context: Optional[str]=None
-
     ) -> Call[HealthCheck]:
+        
+        await asyncio.sleep(0.8 * timeout)
+
         return HealthCheck(
             host=host,
             port=port,
-            target_host=target_host,
-            target_port=target_port,
             source_host=self.host,
             source_port=self.port,
-            error=error_context,
-            status=health_status
-        )
-    
-    @client('update_suspect')
-    async def submit_suspect_node(
-        self,
-        host: str,
-        port: int,
-        target_host: str,
-        target_port: int,
-        shard_ids: List[int],
-        health_status: HealthStatus,
-        error_context: Optional[str]=None
-
-    ) -> Call[HealthCheck]:
-        return HealthCheck(
-            host=host,
-            port=port,
             target_host=target_host,
             target_port=target_port,
-            shard_ids=shard_ids,
-            source_host=self.host,
-            source_port=self.port,
-            error=error_context,
-            status=health_status
+            status=health_status,
+            error=error_context
         )
     
-    @client('update_active')
-    async def submit_active_node(
+    @client('send_indirect_check')
+    async def request_indirect_check(
         self,
         host: str,
         port: int,
         target_host: str,
         target_port: int,
         health_status: HealthStatus,
         error_context: Optional[str]=None
+
     ) -> Call[HealthCheck]:
         return HealthCheck(
             host=host,
             port=port,
             target_host=target_host,
             target_port=target_port,
+            target_status=self._node_statuses[(target_host, target_port)],
             source_host=self.host,
             source_port=self.port,
             error=error_context,
             status=health_status
         )
-        
     
     async def start(self):
 
         await self.start_server()
         await asyncio.sleep(self.boot_wait)
 
     async def register(
@@ -486,177 +523,219 @@
                     cert_path=self.cert_path,
                     key_path=self.key_path
                 )
             ),
             timeout=self.registration_timeout
         )
 
-        self._monitoring[(host, port)] = True
+        self._node_statuses[(host, port)] = 'healthy'
 
         self.status = 'healthy'
         self._running = True
         
         self._healthchecks[(host, port)] = asyncio.create_task(
             self.start_health_monitor()
         )
         
         self.confirmation_task = asyncio.create_task(
             self.cleanup_pending_checks()
         )
+
+    def _calculate_min_suspect_timeout(self):
+        nodes_count = len({
+            address: status for address, status in self._node_statuses.items() if status != 'failed'
+        }) + 1
+
+        return round(
+            self.min_suspect_multiplier * math.log10(nodes_count) * self._poll_interval,
+            2
+        )
+
+    def _calculate_max_suspect_timeout(self, min_suspect_timeout: float):
+        
+        return round(
+            self.max_suspect_multiplier * min_suspect_timeout,
+            2
+        )
+
+    def _calculate_suspicion_timeout(
+        self,
+        suspect_node_address: Tuple[str, int]
+    ):
+
+        min_suspect_timeout = self._calculate_min_suspect_timeout()
+        
+        max_suspect_timeout = self._calculate_max_suspect_timeout(min_suspect_timeout)
+
+        confirmed_suspect_count = max(
+            0,
+            self._confirmed_suspicions[suspect_node_address] - 1
+        )
+
+        timeout_modifier = math.log(
+            confirmed_suspect_count + 1
+        )/math.log(self._min_suspect_node_count + 1)
+
+        timeout_difference = max_suspect_timeout - min_suspect_timeout
+
+        return max(
+            min_suspect_timeout,
+            max_suspect_timeout - (timeout_difference * timeout_modifier)
+        )
     
-    async def _push_investigating_update(
+    async def _acknowledge_indirect_probe(
         self,
         host: str,
         port: int,
         target_host: str,
-        target_port: int,
-        timeout: float
+        target_port: int
     ):
         try:
-            await asyncio.sleep(0.8 * timeout)
-
-            await asyncio.wait_for(
-                self.push_health_update(
-                    host=host,
-                    port=port,
-                    target_host=target_host,
-                    target_port=target_port,
-                    health_status='investigating',
+            
+            timeout = self._poll_timeout * (self._local_health_multiplier + 1)
+            response: Tuple[int, HealthCheck] = await asyncio.wait_for(
+                self.push_acknowledge_check(
+                    host,
+                    port,
+                    target_host,
+                    target_port,
+                    self.status,
+                    timeout,
                     error_context=self.error_context
                 ),
-                timeout=self._poll_timeout
+                timeout=timeout
+            )
+
+            _, healthcheck = response
+            source_host, source_port = healthcheck.source_host, healthcheck.source_port
+
+            self._node_statuses[(source_host, source_port)] = healthcheck.status
+
+            self._local_health_multiplier = max(
+                0, 
+                self._local_health_multiplier - 1
             )
 
         except asyncio.TimeoutError:
-            if not self._active_probes.get((host, port)):
-                self._active_probes[(host, port)] = True
-                self._failed_nodes.append((
+            self._local_health_multiplier = min(
+                self._local_health_multiplier + 1, 
+                self.max_suspect_multiplier
+            )
+
+            if self._node_statuses[(host, port)] not in self._unhealthy_statuses:
+                self._node_statuses[(host, port)] = 'degraded'
+
+                self._degraded_nodes.append((
                     host,
                     port
                 ))
 
                 self._failed_tasks[(host, port)] = asyncio.create_task(
                     self._probe_timed_out_node()
                 )
-            
-            self._monitoring[(host, port)] = False
-    
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
-                self._monitoring[(node_host, node_port)] = False
-
-                self._failed_tasks[(node_host, node_port)] = asyncio.create_task(
-                    self._probe_timed_out_node()
-                )
 
-    async def _run_healthcheck(self, host: str, port: int):
+    async def _run_healthcheck(
+        self, 
+        host: str, 
+        port: int,
+        target_host: Optional[str]=None,
+        target_port: Optional[str]=None
+    ):
 
         try:
 
-            await asyncio.wait_for(
+            response: Tuple[int, HealthCheck] = await asyncio.wait_for(
                 self.push_health_update(
                     host,
                     port,
                     self.status,
+                    target_host=target_host,
+                    target_port=target_port,
                     error_context=self.error_context
                 ),
-                timeout=self._poll_timeout
+                timeout=self._poll_timeout * (self._local_health_multiplier + 1)
+            )
+
+            _, healthcheck = response
+            source_host, source_port = healthcheck.source_host, healthcheck.source_port
+
+            self._node_statuses[(source_host, source_port)] = healthcheck.status
+
+            self._local_health_multiplier = max(
+                0, 
+                self._local_health_multiplier - 1
             )
 
         except asyncio.TimeoutError:
-            if not self._active_probes.get((host, port)):
-                self.status = 'investigating'
+            self._local_health_multiplier = min(
+                self._local_health_multiplier + 1, 
+                self.max_suspect_multiplier
+            )
 
-                self._active_probes[(host, port)] = True
-                self._failed_nodes.append((
+            if self._node_statuses[(host, port)] not in self._unhealthy_statuses:
+                self._node_statuses[(host, port)] = 'degraded'
+
+                self._degraded_nodes.append((
                     host,
                     port
                 ))
 
                 self._failed_tasks[(host, port)] = asyncio.create_task(
                     self._probe_timed_out_node()
                 )
-            
-            self._monitoring[(host, port)] = False
 
     async def _probe_timed_out_node(self):
-
-        host, port = self._failed_nodes.pop()
+        
+        suspect_host, suspect_port = self._degraded_nodes.pop()
         
         confirmation_members = self._get_confirmation_members()
 
         healthchecks, suspect_count = await self._request_indirect_probe(
-            host,
-            port,
+            suspect_host,
+            suspect_port,
             confirmation_members
         )
 
-        indirect_ack_count = len(self._investigating_nodes[(host, port)])
+        self._confirmed_suspicions[(suspect_host, suspect_port)] = len([
+            check for _, check in healthchecks if check.target_status == 'suspect'
+        ])
 
-        if len(confirmation_members) > indirect_ack_count:
-            # If we have received more results from other
-            # nodes than nacks we may be a degraded node.
-            self.status = 'degraded'
+        indirect_ack_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
 
-        elif suspect_count >= len(confirmation_members):
+        missing_ack_count = len(confirmation_members) - indirect_ack_count
+        
+        next_health_multiplier = self._local_health_multiplier + missing_ack_count - indirect_ack_count
+        if next_health_multiplier < 0:
+            self._local_health_multiplier = 0
 
-            self._suspect_nodes[(host, port)] = [
-                shard_id for shard_id, _ in healthchecks
-            ]
+        else:
+            self._local_health_multiplier = min(
+                next_health_multiplier, 
+                self.max_suspect_multiplier
+            )
 
-            await asyncio.gather(*[
-                asyncio.wait_for(
-                    self.submit_suspect_node(
-                        node_host,
-                        node_port,
-                        host,
-                        port,
-                        self._suspect_nodes.get(
-                            (host, port),
-                            []
-                        ),
-                        self.status,
-                        error_context=self.error_context
-                    ),
-                    timeout=self._poll_timeout
-                ) for node_host, node_port in confirmation_members
-            ], return_exceptions=True)
+        if suspect_count >= len(confirmation_members):
+
+            self._node_statuses[(suspect_host, suspect_port)] = 'suspect'
+            self._suspect_nodes.append((suspect_host, suspect_port))
 
-            self._suspect_tasks[(host, port)] = asyncio.create_task(
+            self._suspect_tasks[(suspect_host, suspect_port)] = asyncio.create_task(
                 self._start_suspect_monitor()
             )
 
         else:
-            self._monitoring[(host, port)] = True 
-
-            await self._update_suspect_nodes(
-                confirmation_members,
-                self._investigating_nodes[(host, port)]
-            )
+            self._node_statuses[(suspect_host, suspect_port)] = 'healthy' 
+            self.status = 'healthy'
 
-        del self._investigating_nodes[(host, port)]
+        if self._investigating_nodes.get((suspect_host, suspect_port)):
+            del self._investigating_nodes[(suspect_host, suspect_port)]
             
     def _get_confirmation_members(self) -> List[Tuple[str, int]]:
         confirmation_members = [
-            address for address, monitoring_status in self._monitoring.items() if monitoring_status
+            address for address, status in self._node_statuses.items() if status in self._healthy_statuses
         ]
 
         confirmation_candidates_count = len(confirmation_members) 
 
         if confirmation_candidates_count < self._check_nodes_count:
             self._check_nodes_count = confirmation_candidates_count
 
@@ -707,18 +786,17 @@
                         port,
                         self.status,
                         error_context=self.error_context
                     )
                 )
             )
 
-
         check_tasks: Tuple[List[asyncio.Task], List[asyncio.Task]] = await asyncio.wait(
             requested_checks, 
-            timeout=self._poll_timeout * 2
+            timeout=self._poll_timeout * (self._local_health_multiplier + 1)
         )
 
         completed, pending = check_tasks
 
         healthchecks: List[Call[HealthCheck]]  = await asyncio.gather(*completed)
 
         sorted_checks: List[Call[HealthCheck]] = list(sorted(
@@ -726,22 +804,22 @@
             key=lambda check: check[0]
         ))
 
         suspect = [
             (
                 shard_id,
                 check
-            ) for shard_id, check in sorted_checks if check.status == 'suspect'
+            ) for shard_id, check in sorted_checks if check.target_status == 'suspect'
         ]
 
         healthy = [
             (
                 shard_id,
                 check
-            ) for shard_id, check in sorted_checks if check.status == 'healthy' or check.status == 'investigating'
+            ) for shard_id, check in sorted_checks if check.target_status == 'healthy'
         ]
 
         suspect_checks: List[Call[HealthCheck]] = []
         for suspect_shard_id, suspect_check in suspect:
 
             newer_count = 0
             for healthy_shard_id, _ in healthy:
@@ -757,201 +835,196 @@
         suspect_count = len(suspect_checks) + len(pending)
         
         await asyncio.gather(*[
             cancel(pending_check) for pending_check in pending
         ])
 
         return healthchecks, suspect_count
+    
+    async def _propagate_state_update(
+        self,
+        target_host: str,
+        target_port: int
+    ):
+        monitoring = [
+            address for address, status in self._node_statuses.items() if status in self._healthy_statuses
+        ]
+
+        for host, port in monitoring:
+            await self.push_health_update(
+                host,
+                port,
+                self.status,
+                target_host=target_host,
+                target_port=target_port
+            )
 
     async def run_forever(self):
         self._waiter = asyncio.Future()
         await self._waiter
 
     async def start_health_monitor(self):
         
         monitor_idx = 0
 
         while self._running:
 
             monitors = [
-                address for address, monitoring_status in self._monitoring.items() if monitoring_status
+                address for address, status in self._node_statuses.items() if status == 'healthy'
             ]
 
             host: Union[str, None] = None
             port: Union[int, None] = None
 
             if len(monitors) > 0:
-                monitor_idx = monitor_idx%len(monitors)
+
+                monitors_count = len(monitors)
+                monitor_idx = monitor_idx%monitors_count
                 host, port = monitors[monitor_idx]
 
-            if self._monitoring.get((host, port)):
+            if self._node_statuses.get((host, port)):
         
                 self._active_checks_queue.append(
                     asyncio.create_task(
                         self._run_healthcheck(
                             host,
                             port
                         )
                     )
                 )
 
+            if monitor_idx%monitors_count == 0:
+                self.status = 'healthy'
+
             monitor_idx += 1
 
-            await asyncio.sleep(self._poll_interval)      
+            await asyncio.sleep(
+                self._poll_interval * (self._local_health_multiplier + 1)
+            )      
 
     async def _start_suspect_monitor(self):
 
         elapsed = 0
         start = time.monotonic()
 
+    
         if len(self._suspect_nodes) < 1:
             return
         
-        address, suspect_shard_id = self._suspect_nodes.popitem()
+        address = self._suspect_nodes.pop()
         suspect_host, suspect_port = address
-        
-        if self._active_probes.get((suspect_host, suspect_port)):
-            del self._active_probes[(suspect_host, suspect_port)]
 
         confirmation_task = self._failed_tasks.get((suspect_host, suspect_port))
         if confirmation_task:
             await cancel(confirmation_task)
             confirmation_task.cancel()
 
-        node_revived = False
+        node_status = self._node_statuses[(suspect_host, suspect_port)]
 
-        while elapsed < self._max_suspect_timeout:
-            
+        suspicion_timeout = self._calculate_suspicion_timeout(address)
+
+        while elapsed < suspicion_timeout and node_status == 'suspect':
+                
             confirmation_members = self._get_confirmation_members()
 
             healthchecks, suspect_count = await self._request_indirect_probe(
                 suspect_host,
                 suspect_port,
                 confirmation_members
             )
 
-            indirect_ack_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
+            self._confirmed_suspicions[(suspect_host, suspect_port)] = len([
+                check for _, check in healthchecks if check.target_status == 'suspect'
+            ])
 
-            suspect_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
+            indirect_ack_count = len(self._investigating_nodes[(suspect_host, suspect_port)])
 
-            if len(confirmation_members) > indirect_ack_count:
-                # If we have received more results from other
-                # nodes than nacks we may be a degraded node.
-                self.status = 'degraded'
-
-            elif suspect_count >= len(confirmation_members):
-                # All members have confirmed suspect.
-
-                self._suspect_nodes[(suspect_host, suspect_port)] = [
-                    shard_id for shard_id, _ in healthchecks
-                ]
-
-                await asyncio.gather(*[
-                    asyncio.wait_for(
-                        self.submit_suspect_node(
-                            node_host,
-                            node_port,
-                            suspect_host,
-                            suspect_port,
-                            self._suspect_nodes.get(
-                                (suspect_host, suspect_port),
-                                []
-                            ),
-                            self.status,
-                            error_context=self.error_context
-                        ),
-                        timeout=self._poll_timeout
-                    ) for node_host, node_port in confirmation_members
-                ], return_exceptions=True)
+            missing_ack_count = len(confirmation_members) - indirect_ack_count
+            
+            next_health_multiplier = self._local_health_multiplier + missing_ack_count - indirect_ack_count
+            if next_health_multiplier < 0:
+                self._local_health_multiplier = 0
 
             else:
+                self._local_health_multiplier = min(
+                    next_health_multiplier, 
+                    self.max_suspect_multiplier
+                )
+
+            if suspect_count < len(confirmation_members):
                 # We had a majority confirmation the node was healthy.
 
-                self._monitoring[(suspect_host, suspect_port)] = True 
+                self._node_statuses[(suspect_host, suspect_port)] = 'healthy'
 
-                monitoring = [
-                    address for address, monitoring_status in self._monitoring.items() if monitoring_status
-                ]
-
-                for host, port in monitoring:
-                    if self._suspect_nodes.get((host, port)) is None:
-                        await self.submit_active_node(
-                            host,
-                            port,
-                            suspect_host,
-                            suspect_port,
-                            health_status='healthy'
-                        )
+                await self._propagate_state_update(
+                    suspect_host,
+                    suspect_port
+                )
 
                 await self.refresh_clients(
                     HealthCheck(
                         host=suspect_host,
                         port=suspect_port,
                         source_host=self.host,
                         source_port=self.port,
-                        status='healthy'
+                        status=self.status
                     )
                 )
 
-                await self._update_suspect_nodes(
-                    confirmation_members,
-                    self._investigating_nodes[(suspect_host, suspect_port)]
-                )
-                
-                self._monitoring[(suspect_host, suspect_port)] = True
-
-                node_revived = True
-                break
+            if self._investigating_nodes.get((suspect_host, suspect_port)):
+                del self._investigating_nodes[(suspect_host, suspect_port)]
 
-            del self._investigating_nodes[(suspect_host, suspect_port)]
+            await asyncio.sleep(
+                self._poll_interval * (self._local_health_multiplier + 1)
+            ) 
 
-            await asyncio.sleep(self._poll_interval) 
             elapsed = time.monotonic() - start
         
-        if node_revived is False:
-            self._removed_nodes[(suspect_host, suspect_port)] = suspect_shard_id
-
-        if self.status == 'investigating':
-            self.status = 'healthy'
+        if self._node_statuses[(suspect_host, suspect_port)] == 'suspect':
+            self._node_statuses[(suspect_host, suspect_port)] = 'failed'
+            await self._propagate_state_update(
+                    suspect_host,
+                    suspect_port
+                )
 
     async def cleanup_pending_checks(self):
 
         while self._running:
 
             for pending_check in list(self._active_checks_queue):
                 if pending_check.done() or pending_check.cancelled():
                     self._active_checks_queue.remove(pending_check)
 
-            monitoring = dict(self._monitoring)
-            for host, port in self._removed_nodes:
-
-                if monitoring.get((host, port)) is False:
-                    await self.remove_clients(
-                        HealthCheck(
-                            host=host,
-                            port=port,
-                            source_host=self.host,
-                            source_port=self.port,
-                            status='removed'
-                        )
-                    )
+            failed_nodes = [
+                address for address, status in self._node_statuses.items() if status == 'failed'
+            ]
 
-                    del monitoring[(host, port)]
+            for host, port in failed_nodes:
 
-            self._removed_nodes.clear()
-            self._monitoring = monitoring
+                await self.remove_clients(
+                    HealthCheck(
+                        host=host,
+                        port=port,
+                        source_host=self.host,
+                        source_port=self.port,
+                        status='failed'
+                    )
+                )
 
             await asyncio.sleep(self._cleanup_interval)
-
     
     async def shutdown(self):
         self._running = False
         self._local_health_monitor.cancel()
 
         await asyncio.gather(*[
+            cancel(check) for check in self._active_checks_queue
+        ])
+
+        await asyncio.gather(*[
             cancel(remote_check) for remote_check in self._healthchecks.values()
         ])
 
         await cancel(self._local_health_monitor)
         
         await cancel(self._cleanup_task)
```

### Comparing `mercury-sync-0.3.2/mercury_sync/service/service.py` & `mercury-sync-0.3.3/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.3.3/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.3.3/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.3.3/mercury_sync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.2
+Version: 0.3.3
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.2/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.3.3/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.2/setup.py` & `mercury-sync-0.3.3/setup.py`

 * *Files identical despite different names*

