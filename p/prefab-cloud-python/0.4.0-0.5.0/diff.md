# Comparing `tmp/prefab_cloud_python-0.4.0.tar.gz` & `tmp/prefab_cloud_python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefab_cloud_python-0.4.0.tar", max compression
+gzip compressed data, was "prefab_cloud_python-0.5.0.tar", max compression
```

## Comparing `prefab_cloud_python-0.4.0.tar` & `prefab_cloud_python-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1054 2023-06-13 00:50:55.374694 prefab_cloud_python-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0      768 2023-05-08 23:50:45.418057 prefab_cloud_python-0.4.0/README.md
--rw-r--r--   0        0        0      117 2023-05-08 23:50:45.419706 prefab_cloud_python-0.4.0/prefab_cloud_python/__init__.py
--rw-r--r--   0        0        0     3496 2023-06-24 01:10:49.542721 prefab_cloud_python-0.4.0/prefab_cloud_python/_processors.py
--rw-r--r--   0        0        0     3581 2023-06-24 01:10:49.543366 prefab_cloud_python-0.4.0/prefab_cloud_python/client.py
--rw-r--r--   0        0        0     7240 2023-06-24 01:10:49.543746 prefab_cloud_python-0.4.0/prefab_cloud_python/config_client.py
--rw-r--r--   0        0        0     2266 2023-06-24 16:09:08.590771 prefab_cloud_python-0.4.0/prefab_cloud_python/config_loader.py
--rw-r--r--   0        0        0     4963 2023-04-12 22:57:29.416107 prefab_cloud_python-0.4.0/prefab_cloud_python/config_parser.py
--rw-r--r--   0        0        0     1476 2023-05-08 23:50:45.420741 prefab_cloud_python-0.4.0/prefab_cloud_python/config_resolver.py
--rw-r--r--   0        0        0     1107 2023-05-08 23:50:45.421081 prefab_cloud_python-0.4.0/prefab_cloud_python/config_value_unwrapper.py
--rw-r--r--   0        0        0     3305 2023-06-24 16:07:27.651479 prefab_cloud_python-0.4.0/prefab_cloud_python/context.py
--rw-r--r--   0        0        0     4010 2023-06-12 23:26:42.577562 prefab_cloud_python-0.4.0/prefab_cloud_python/criteria_evaluator.py
--rw-r--r--   0        0        0     1344 2023-06-12 23:26:42.577722 prefab_cloud_python-0.4.0/prefab_cloud_python/feature_flag_client.py
--rw-r--r--   0        0        0     2367 2023-06-24 01:10:49.544803 prefab_cloud_python-0.4.0/prefab_cloud_python/log_path_collector.py
--rw-r--r--   0        0        0     2497 2023-06-24 01:10:49.545616 prefab_cloud_python-0.4.0/prefab_cloud_python/logger_client.py
--rw-r--r--   0        0        0     5843 2023-06-24 01:10:49.545891 prefab_cloud_python-0.4.0/prefab_cloud_python/options.py
--rw-r--r--   0        0        0     1594 2023-06-24 01:10:49.546277 prefab_cloud_python-0.4.0/prefab_cloud_python/read_write_lock.py
--rw-r--r--   0        0        0     1099 2023-05-08 23:50:45.422222 prefab_cloud_python-0.4.0/prefab_cloud_python/weighted_value_resolver.py
--rw-r--r--   0        0        0      964 2023-06-24 16:09:08.590977 prefab_cloud_python-0.4.0/prefab_cloud_python/yaml_parser.py
--rw-r--r--   0        0        0    17491 2023-06-24 16:22:04.471681 prefab_cloud_python-0.4.0/prefab_pb2.py
--rw-r--r--   0        0        0      159 2023-06-24 16:15:57.299152 prefab_cloud_python-0.4.0/prefab_pb2_grpc.py
--rw-r--r--   0        0        0      998 2023-06-24 16:25:41.892367 prefab_cloud_python-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 prefab_cloud_python-0.4.0/setup.py
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 prefab_cloud_python-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-06-13 00:50:55.374694 prefab_cloud_python-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      768 2023-05-08 23:50:45.418057 prefab_cloud_python-0.5.0/README.md
+-rw-r--r--   0        0        0      117 2023-05-08 23:50:45.419706 prefab_cloud_python-0.5.0/prefab_cloud_python/__init__.py
+-rw-r--r--   0        0        0     3502 2023-06-24 16:32:43.359485 prefab_cloud_python-0.5.0/prefab_cloud_python/_processors.py
+-rw-r--r--   0        0        0     3920 2023-06-24 16:32:43.359605 prefab_cloud_python-0.5.0/prefab_cloud_python/client.py
+-rw-r--r--   0        0        0     7485 2023-06-24 16:32:43.359725 prefab_cloud_python-0.5.0/prefab_cloud_python/config_client.py
+-rw-r--r--   0        0        0     2266 2023-06-24 16:27:49.007188 prefab_cloud_python-0.5.0/prefab_cloud_python/config_loader.py
+-rw-r--r--   0        0        0     4963 2023-04-12 22:57:29.416107 prefab_cloud_python-0.5.0/prefab_cloud_python/config_parser.py
+-rw-r--r--   0        0        0     1476 2023-05-08 23:50:45.420741 prefab_cloud_python-0.5.0/prefab_cloud_python/config_resolver.py
+-rw-r--r--   0        0        0     1107 2023-05-08 23:50:45.421081 prefab_cloud_python-0.5.0/prefab_cloud_python/config_value_unwrapper.py
+-rw-r--r--   0        0        0     3305 2023-06-24 16:07:27.651479 prefab_cloud_python-0.5.0/prefab_cloud_python/context.py
+-rw-r--r--   0        0        0      173 2023-06-24 16:32:43.359796 prefab_cloud_python-0.5.0/prefab_cloud_python/context_shape.py
+-rw-r--r--   0        0        0     2023 2023-06-24 16:32:43.359874 prefab_cloud_python-0.5.0/prefab_cloud_python/context_shape_aggregator.py
+-rw-r--r--   0        0        0     4010 2023-06-12 23:26:42.577562 prefab_cloud_python-0.5.0/prefab_cloud_python/criteria_evaluator.py
+-rw-r--r--   0        0        0     1344 2023-06-12 23:26:42.577722 prefab_cloud_python-0.5.0/prefab_cloud_python/feature_flag_client.py
+-rw-r--r--   0        0        0     2368 2023-06-24 16:32:43.359956 prefab_cloud_python-0.5.0/prefab_cloud_python/log_path_aggregator.py
+-rw-r--r--   0        0        0     2504 2023-06-24 16:32:43.360067 prefab_cloud_python-0.5.0/prefab_cloud_python/logger_client.py
+-rw-r--r--   0        0        0     5931 2023-06-24 16:32:43.360183 prefab_cloud_python-0.5.0/prefab_cloud_python/options.py
+-rw-r--r--   0        0        0     1612 2023-06-24 16:32:43.360281 prefab_cloud_python-0.5.0/prefab_cloud_python/read_write_lock.py
+-rw-r--r--   0        0        0     1099 2023-05-08 23:50:45.422222 prefab_cloud_python-0.5.0/prefab_cloud_python/weighted_value_resolver.py
+-rw-r--r--   0        0        0      964 2023-06-24 16:27:49.008894 prefab_cloud_python-0.5.0/prefab_cloud_python/yaml_parser.py
+-rw-r--r--   0        0        0    17491 2023-06-24 16:29:04.175755 prefab_cloud_python-0.5.0/prefab_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-24 16:28:27.795273 prefab_cloud_python-0.5.0/prefab_pb2_grpc.py
+-rw-r--r--   0        0        0      998 2023-06-24 16:32:43.360386 prefab_cloud_python-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 prefab_cloud_python-0.5.0/setup.py
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 prefab_cloud_python-0.5.0/PKG-INFO
```

### Comparing `prefab_cloud_python-0.4.0/LICENSE.txt` & `prefab_cloud_python-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/README.md` & `prefab_cloud_python-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/_processors.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/_processors.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 def clean_event_dict(_, __, event_dict):
     event_dict.pop("pathname")
     event_dict.pop("func_name")
     event_dict.pop("config_client")
     event_dict.pop("log_prefix")
     event_dict.pop("log_boundary")
-    event_dict.pop("log_path_collector")
-    if "skip_collector" in event_dict:
-        event_dict.pop("skip_collector")
+    event_dict.pop("log_path_aggregator")
+    if "skip_aggregator" in event_dict:
+        event_dict.pop("skip_aggregator")
     if "internal_path" in event_dict:
         event_dict.pop("internal_path")
     return event_dict
 
 
 def set_location(_, __, event_dict):
     if "internal_path" in event_dict:
@@ -61,16 +61,16 @@
 
 def log_or_drop(_, method, event_dict):
     location = event_dict["location"]
     config_client = event_dict["config_client"]
     closest_log_level = get_severity(location, config_client)
     called_method_level = python_to_prefab_log_levels[method]
 
-    if event_dict["log_path_collector"] and not event_dict["skip_collector"]:
-        event_dict["log_path_collector"].push(
+    if event_dict["log_path_aggregator"] and not event_dict["skip_aggregator"]:
+        event_dict["log_path_aggregator"].push(
             event_dict["location"], Prefab.LogLevel.Name(called_method_level)
         )
 
     if closest_log_level > called_method_level:
         raise DropEvent
 
     return event_dict
```

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/client.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import functools
 from .context import Context
 from .config_client import ConfigClient
 from .feature_flag_client import FeatureFlagClient
-from .log_path_collector import LogPathCollector
+from .context_shape_aggregator import ContextShapeAggregator
+from .log_path_aggregator import LogPathAggregator
 from .logger_client import LoggerClient
 import base64
 import prefab_pb2 as Prefab
 import uuid
 import urllib3
 
 
@@ -14,22 +15,30 @@
     max_sleep_sec = 10
     base_sleep_sec = 0.5
     no_default_provided = "NO_DEFAULT_PROVIDED"
 
     def __init__(self, options):
         self.options = options
         self.instance_hash = str(uuid.uuid4())
-        self.log_path_collector = LogPathCollector(
+        self.log_path_aggregator = LogPathAggregator(
             self, self.options.collect_max_paths, self.options.collect_sync_interval
         )
         self.logger = LoggerClient(
-            self.options.log_prefix, self.options.log_boundary, self.log_path_collector
+            self.options.log_prefix, self.options.log_boundary, self.log_path_aggregator
         )
-        self.log_path_collector.client = self
-        self.log_path_collector.start_periodic_sync()
+        self.log_path_aggregator.client = self
+
+        self.context_shape_aggregator = ContextShapeAggregator(
+            self, self.options.collect_max_shapes, self.options.collect_sync_interval
+        )
+
+        if not options.is_local_only():
+            self.log_path_aggregator.start_periodic_sync()
+            self.context_shape_aggregator.start_periodic_sync()
+
         self.namespace = options.namespace
         self.api_url = options.prefab_api_url
         self.grpc_url = options.prefab_grpc_url
         if options.is_local_only():
             self.logger.log_internal("info", "Prefab running in local-only mode")
         else:
             self.logger.log_internal(
```

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/config_client.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/config_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,32 +58,39 @@
         else:
             self.load_checkpoint()
             self.start_checkpointing_thread()
             self.start_streaming()
 
     def get(self, key, default="NO_DEFAULT_PROVIDED", context=Context.get_current()):
         value = self.__get(key, None, {}, context=context)
+
+        if isinstance(context, Context):
+            self.base_client.context_shape_aggregator.push(context)
+        elif not isinstance(context, str):
+            self.base_client.context_shape_aggregator.push(Context(context))
+
         if value is not None:
             return ConfigValueUnwrapper.unwrap(value, key, context)
         else:
             return self.handle_default(key, default)
 
     def __get(self, key, lookup_key, properties, context=Context.get_current()):
         try:
-            with self.init_lock.read_locked():
-                return self.config_resolver.get(key, context=context)
+            self.init_lock.acquire_read(self.options.connection_timeout_seconds)
         except Exception:
             if self.options.on_connection_failure == "RAISE":
                 raise InitializationTimeoutException(
                     self.options.connection_timeout_seconds, key
                 )
-            self.base_client.logger.warn(
-                f"Couldn't initialize in {self.options.connection_timeout_seconds}. Key {key}. Returning what we have."
+            self.base_client.logger.log_internal(
+                "warn",
+                f"Couldn't initialize in {self.options.connection_timeout_seconds}. Key {key}. Returning what we have.",
             )
             self.init_lock.release_write()
+        finally:
             return self.config_resolver.get(key, context=context)
 
     def handle_default(self, key, default):
         if default != "NO_DEFAULT_PROVIDED":
             return default
         if self.options.on_no_default == "RAISE":
             raise MissingDefaultException(key)
```

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/config_loader.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/config_loader.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/config_parser.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/config_parser.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/config_resolver.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/config_resolver.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/config_value_unwrapper.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/config_value_unwrapper.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/context.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/context.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/criteria_evaluator.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/criteria_evaluator.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/feature_flag_client.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/feature_flag_client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/log_path_collector.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/log_path_aggregator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 from collections import defaultdict
 import prefab_pb2 as Prefab
 import threading
 
 
-class LogPathCollector:
+class LogPathAggregator:
     def __init__(self, client, max_paths, sync_interval):
         self.client = client
         self.max_paths = max_paths
         self.sync_interval = sync_interval or 8
 
         self.start_at = time.time()
         self.paths = defaultdict(int)
```

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/logger_client.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/logger_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,19 +30,19 @@
         bootstrap_log_level = os.environ.get("PREFAB_LOG_CLIENT_BOOTSTRAP_LOG_LEVEL")
         if bootstrap_log_level is not None:
             return bootstrap_log_level.upper()
         return default
 
 
 class LoggerClient:
-    def __init__(self, log_prefix=None, log_boundary=None, log_path_collector=None):
+    def __init__(self, log_prefix=None, log_boundary=None, log_path_aggregator=None):
         self.log_prefix = log_prefix
         self.log_boundary = log_boundary
         self.config_client = BootstrappingConfigClient()
-        self.log_path_collector = log_path_collector
+        self.log_path_aggregator = log_path_aggregator
 
     def debug(self, msg):
         self.configured_logger().debug(msg)
 
     def info(self, msg):
         self.configured_logger().info(msg)
 
@@ -53,15 +53,15 @@
         self.configured_logger().error(msg)
 
     def critical(self, msg):
         self.configured_logger().critical(msg)
 
     def log_internal(self, level, msg, path=None):
         internal_logger = self.configured_logger().bind(
-            skip_collector=True, internal_path=path
+            skip_aggregator=True, internal_path=path
         )
         getattr(internal_logger, level)(msg)
 
     def set_config_client(self, config_client):
         self.config_client = config_client
 
     def add_config_client(self, _, __, event_dict):
@@ -69,10 +69,10 @@
         return event_dict
 
     def configured_logger(self):
         return structlog.get_logger().bind(
             config_client=self.config_client,
             log_prefix=self.log_prefix,
             log_boundary=self.log_boundary,
-            log_path_collector=self.log_path_collector,
-            skip_collector=False,
+            log_path_aggregator=self.log_path_aggregator,
+            skip_aggregator=False,
         )
```

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/options.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         prefab_config_classpath_dir=".",
         prefab_envs=[],
         http_secure=None,
         on_no_default="RAISE",
         on_connection_failure="RETURN",
         collect_logs=True,
         collect_max_paths=1000,
+        collect_max_shapes=10_000,
         collect_sync_interval=None,
     ):
         self.prefab_datasources = Options.__validate_datasource(prefab_datasources)
         self.__set_api_key(api_key or os.environ.get("PREFAB_API_KEY"))
         self.__set_api_url(
             prefab_api_url
             or os.environ.get("PREFAB_API_URL")
@@ -78,14 +79,15 @@
         self.stats = None
         self.shared_cache = None
         self.__set_url_for_api_cdn()
         self.__set_on_no_default(on_no_default)
         self.__set_on_connection_failure(on_connection_failure)
         self.__set_log_collection(collect_logs, collect_max_paths, self.is_local_only())
         self.collect_sync_interval = collect_sync_interval
+        self.collect_max_shapes = collect_max_shapes
 
     def is_local_only(self):
         return self.prefab_datasources == "LOCAL_ONLY"
 
     def __set_url_for_api_cdn(self):
         if self.prefab_datasources == "LOCAL_ONLY":
             self.url_for_api_cdn = None
```

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/read_write_lock.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/read_write_lock.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     only one "write lock." """
 
     def __init__(self):
         self._read_ready = threading.Condition(threading.Lock())
         self._readers = 0
         self._write_locked = False
 
-    def acquire_read(self):
+    def acquire_read(self, timeout=1):
         """Acquire a read lock. Blocks only if a thread has
         acquired the write lock."""
-        self._read_ready.acquire()
+        self._read_ready.acquire(timeout)
         try:
             self._readers += 1
         finally:
             self._read_ready.release()
 
     def release_read(self):
         """Release a read lock."""
```

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/weighted_value_resolver.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/weighted_value_resolver.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/prefab_cloud_python/yaml_parser.py` & `prefab_cloud_python-0.5.0/prefab_cloud_python/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/prefab_pb2.py` & `prefab_cloud_python-0.5.0/prefab_pb2.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.4.0/pyproject.toml` & `prefab_cloud_python-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prefab-cloud-python"
-version = "0.4.0"
+version = "0.5.0"
 description = "Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud"
 license = "MIT"
 authors = ["Michael Berkowitz <michael.berkowitz@gmail.com>"]
 maintainers = ["Michael Berkowitz <michael.berkowitz@gmail.com>"]
 readme = "README.md"
 homepage = "https://www.prefab.cloud"
 repository = "https://github.com/prefab-cloud/prefab-cloud-python"
```

### Comparing `prefab_cloud_python-0.4.0/setup.py` & `prefab_cloud_python-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pyyaml>=6.0.0,<7.0.0',
  'sseclient-py>=1.7.2,<2.0.0',
  'structlog>=22.3,<23.0',
  'urllib3>=1.26.16,<3']
 
 setup_kwargs = {
     'name': 'prefab-cloud-python',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud',
     'long_description': '# prefab-cloud-python\n\nPython client for prefab.cloud, providing Config, FeatureFlags as a Service\n\n**Note: This library is under active development and not quite ready for production usage**\n\n[Sign up to be notified when this library releases](https://forms.gle/2qsjMFvjGnkTnA9T8)\n\n## Example usage\n\n```python\nfrom prefab_cloud_python import Client, Options\n\noptions = Options(\n    prefab_api_key="your-prefab-api-key"\n)\n\ncontext = {\n  "user": {\n    "team_id": 432,\n    "id": 123,\n    "subscription_level": \'pro\',\n    "email": "alice@example.com"\n  }\n}\n\nclient = Client(options)\n\nresult = client.enabled("my-first-feature-flag", context=context)\n\nprint("my-first-feature-flag is:", result)\n```\n\nSee full documentation https://docs.prefab.cloud/docs/python-sdk/python\n',
     'author': 'Michael Berkowitz',
     'author_email': 'michael.berkowitz@gmail.com',
     'maintainer': 'Michael Berkowitz',
     'maintainer_email': 'michael.berkowitz@gmail.com',
     'url': 'https://www.prefab.cloud',
```

### Comparing `prefab_cloud_python-0.4.0/PKG-INFO` & `prefab_cloud_python-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefab-cloud-python
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud
 Home-page: https://www.prefab.cloud
 License: MIT
 Author: Michael Berkowitz
 Author-email: michael.berkowitz@gmail.com
 Maintainer: Michael Berkowitz
 Maintainer-email: michael.berkowitz@gmail.com
```

