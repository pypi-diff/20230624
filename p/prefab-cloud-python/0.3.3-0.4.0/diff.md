# Comparing `tmp/prefab_cloud_python-0.3.3.tar.gz` & `tmp/prefab_cloud_python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefab_cloud_python-0.3.3.tar", max compression
+gzip compressed data, was "prefab_cloud_python-0.4.0.tar", max compression
```

## Comparing `prefab_cloud_python-0.3.3.tar` & `prefab_cloud_python-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1054 2023-06-13 00:50:55.374694 prefab_cloud_python-0.3.3/LICENSE.txt
--rw-r--r--   0        0        0      768 2023-05-08 23:50:45.418057 prefab_cloud_python-0.3.3/README.md
--rw-r--r--   0        0        0      117 2023-05-08 23:50:45.419706 prefab_cloud_python-0.3.3/prefab_cloud_python/__init__.py
--rw-r--r--   0        0        0     3496 2023-06-21 23:13:52.879273 prefab_cloud_python-0.3.3/prefab_cloud_python/_processors.py
--rw-r--r--   0        0        0     3581 2023-06-21 23:13:52.879890 prefab_cloud_python-0.3.3/prefab_cloud_python/client.py
--rw-r--r--   0        0        0     7240 2023-06-21 23:20:26.954698 prefab_cloud_python-0.3.3/prefab_cloud_python/config_client.py
--rw-r--r--   0        0        0     2288 2023-06-12 23:26:42.577338 prefab_cloud_python-0.3.3/prefab_cloud_python/config_loader.py
--rw-r--r--   0        0        0     4963 2023-04-12 22:57:29.416107 prefab_cloud_python-0.3.3/prefab_cloud_python/config_parser.py
--rw-r--r--   0        0        0     1476 2023-05-08 23:50:45.420741 prefab_cloud_python-0.3.3/prefab_cloud_python/config_resolver.py
--rw-r--r--   0        0        0     1107 2023-05-08 23:50:45.421081 prefab_cloud_python-0.3.3/prefab_cloud_python/config_value_unwrapper.py
--rw-r--r--   0        0        0     3305 2023-05-08 23:50:45.421401 prefab_cloud_python-0.3.3/prefab_cloud_python/context.py
--rw-r--r--   0        0        0     4010 2023-06-12 23:26:42.577562 prefab_cloud_python-0.3.3/prefab_cloud_python/criteria_evaluator.py
--rw-r--r--   0        0        0     1344 2023-06-12 23:26:42.577722 prefab_cloud_python-0.3.3/prefab_cloud_python/feature_flag_client.py
--rw-r--r--   0        0        0     2367 2023-06-21 23:13:52.881090 prefab_cloud_python-0.3.3/prefab_cloud_python/log_path_collector.py
--rw-r--r--   0        0        0     2497 2023-06-21 23:13:52.881814 prefab_cloud_python-0.3.3/prefab_cloud_python/logger_client.py
--rw-r--r--   0        0        0     5843 2023-06-21 23:13:52.882117 prefab_cloud_python-0.3.3/prefab_cloud_python/options.py
--rw-r--r--   0        0        0     1594 2023-06-21 23:13:52.882438 prefab_cloud_python-0.3.3/prefab_cloud_python/read_write_lock.py
--rw-r--r--   0        0        0     1099 2023-05-08 23:50:45.422222 prefab_cloud_python-0.3.3/prefab_cloud_python/weighted_value_resolver.py
--rw-r--r--   0        0        0      443 2023-05-25 23:50:08.502938 prefab_cloud_python-0.3.3/prefab_cloud_python/yaml_parser.py
--rw-r--r--   0        0        0    13403 2023-06-21 23:13:52.882990 prefab_cloud_python-0.3.3/prefab_pb2.py
--rw-r--r--   0        0        0      159 2023-06-13 22:44:30.791631 prefab_cloud_python-0.3.3/prefab_pb2_grpc.py
--rw-r--r--   0        0        0      998 2023-06-21 23:24:28.100953 prefab_cloud_python-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 prefab_cloud_python-0.3.3/setup.py
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 prefab_cloud_python-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-06-13 00:50:55.374694 prefab_cloud_python-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      768 2023-05-08 23:50:45.418057 prefab_cloud_python-0.4.0/README.md
+-rw-r--r--   0        0        0      117 2023-05-08 23:50:45.419706 prefab_cloud_python-0.4.0/prefab_cloud_python/__init__.py
+-rw-r--r--   0        0        0     3496 2023-06-24 01:10:49.542721 prefab_cloud_python-0.4.0/prefab_cloud_python/_processors.py
+-rw-r--r--   0        0        0     3581 2023-06-24 01:10:49.543366 prefab_cloud_python-0.4.0/prefab_cloud_python/client.py
+-rw-r--r--   0        0        0     7240 2023-06-24 01:10:49.543746 prefab_cloud_python-0.4.0/prefab_cloud_python/config_client.py
+-rw-r--r--   0        0        0     2266 2023-06-24 16:09:08.590771 prefab_cloud_python-0.4.0/prefab_cloud_python/config_loader.py
+-rw-r--r--   0        0        0     4963 2023-04-12 22:57:29.416107 prefab_cloud_python-0.4.0/prefab_cloud_python/config_parser.py
+-rw-r--r--   0        0        0     1476 2023-05-08 23:50:45.420741 prefab_cloud_python-0.4.0/prefab_cloud_python/config_resolver.py
+-rw-r--r--   0        0        0     1107 2023-05-08 23:50:45.421081 prefab_cloud_python-0.4.0/prefab_cloud_python/config_value_unwrapper.py
+-rw-r--r--   0        0        0     3305 2023-06-24 16:07:27.651479 prefab_cloud_python-0.4.0/prefab_cloud_python/context.py
+-rw-r--r--   0        0        0     4010 2023-06-12 23:26:42.577562 prefab_cloud_python-0.4.0/prefab_cloud_python/criteria_evaluator.py
+-rw-r--r--   0        0        0     1344 2023-06-12 23:26:42.577722 prefab_cloud_python-0.4.0/prefab_cloud_python/feature_flag_client.py
+-rw-r--r--   0        0        0     2367 2023-06-24 01:10:49.544803 prefab_cloud_python-0.4.0/prefab_cloud_python/log_path_collector.py
+-rw-r--r--   0        0        0     2497 2023-06-24 01:10:49.545616 prefab_cloud_python-0.4.0/prefab_cloud_python/logger_client.py
+-rw-r--r--   0        0        0     5843 2023-06-24 01:10:49.545891 prefab_cloud_python-0.4.0/prefab_cloud_python/options.py
+-rw-r--r--   0        0        0     1594 2023-06-24 01:10:49.546277 prefab_cloud_python-0.4.0/prefab_cloud_python/read_write_lock.py
+-rw-r--r--   0        0        0     1099 2023-05-08 23:50:45.422222 prefab_cloud_python-0.4.0/prefab_cloud_python/weighted_value_resolver.py
+-rw-r--r--   0        0        0      964 2023-06-24 16:09:08.590977 prefab_cloud_python-0.4.0/prefab_cloud_python/yaml_parser.py
+-rw-r--r--   0        0        0    17491 2023-06-24 16:22:04.471681 prefab_cloud_python-0.4.0/prefab_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-24 16:15:57.299152 prefab_cloud_python-0.4.0/prefab_pb2_grpc.py
+-rw-r--r--   0        0        0      998 2023-06-24 16:25:41.892367 prefab_cloud_python-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 prefab_cloud_python-0.4.0/setup.py
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 prefab_cloud_python-0.4.0/PKG-INFO
```

### Comparing `prefab_cloud_python-0.3.3/LICENSE.txt` & `prefab_cloud_python-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/README.md` & `prefab_cloud_python-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/_processors.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/_processors.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/client.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/config_client.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/config_client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/config_loader.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/config_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,16 @@
 
     def __load_config_from(self, dir):
         envs = self.options.prefab_envs
         envs.insert(0, "default")
         loaded_config = {}
         for env in envs:
             loaded_config.update(
-                ConfigLoader.__load_glob(
-                    os.path.join(dir, ".prefab.%s.config.yaml" % env)
-                )
+                self.__load_glob(os.path.join(dir, ".prefab.%s.config.yaml" % env))
             )
         return loaded_config
 
-    def __load_glob(filepath):
+    def __load_glob(self, filepath):
         rtn = {}
         for file in glob.glob(filepath):
-            rtn = rtn | YamlParser(file).data
+            rtn = rtn | YamlParser(file, self.base_client).data
         return rtn
```

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/config_parser.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/config_parser.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/config_resolver.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/config_resolver.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/config_value_unwrapper.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/config_value_unwrapper.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/context.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/context.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/criteria_evaluator.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/criteria_evaluator.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/feature_flag_client.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/feature_flag_client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/log_path_collector.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/log_path_collector.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/logger_client.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/logger_client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/options.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/options.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/read_write_lock.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/prefab_cloud_python/weighted_value_resolver.py` & `prefab_cloud_python-0.4.0/prefab_cloud_python/weighted_value_resolver.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.3.3/pyproject.toml` & `prefab_cloud_python-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prefab-cloud-python"
-version = "0.3.3"
+version = "0.4.0"
 description = "Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud"
 license = "MIT"
 authors = ["Michael Berkowitz <michael.berkowitz@gmail.com>"]
 maintainers = ["Michael Berkowitz <michael.berkowitz@gmail.com>"]
 readme = "README.md"
 homepage = "https://www.prefab.cloud"
 repository = "https://github.com/prefab-cloud/prefab-cloud-python"
```

### Comparing `prefab_cloud_python-0.3.3/setup.py` & `prefab_cloud_python-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pyyaml>=6.0.0,<7.0.0',
  'sseclient-py>=1.7.2,<2.0.0',
  'structlog>=22.3,<23.0',
  'urllib3>=1.26.16,<3']
 
 setup_kwargs = {
     'name': 'prefab-cloud-python',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': 'Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud',
     'long_description': '# prefab-cloud-python\n\nPython client for prefab.cloud, providing Config, FeatureFlags as a Service\n\n**Note: This library is under active development and not quite ready for production usage**\n\n[Sign up to be notified when this library releases](https://forms.gle/2qsjMFvjGnkTnA9T8)\n\n## Example usage\n\n```python\nfrom prefab_cloud_python import Client, Options\n\noptions = Options(\n    prefab_api_key="your-prefab-api-key"\n)\n\ncontext = {\n  "user": {\n    "team_id": 432,\n    "id": 123,\n    "subscription_level": \'pro\',\n    "email": "alice@example.com"\n  }\n}\n\nclient = Client(options)\n\nresult = client.enabled("my-first-feature-flag", context=context)\n\nprint("my-first-feature-flag is:", result)\n```\n\nSee full documentation https://docs.prefab.cloud/docs/python-sdk/python\n',
     'author': 'Michael Berkowitz',
     'author_email': 'michael.berkowitz@gmail.com',
     'maintainer': 'Michael Berkowitz',
     'maintainer_email': 'michael.berkowitz@gmail.com',
     'url': 'https://www.prefab.cloud',
```

### Comparing `prefab_cloud_python-0.3.3/PKG-INFO` & `prefab_cloud_python-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefab-cloud-python
-Version: 0.3.3
+Version: 0.4.0
 Summary: Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud
 Home-page: https://www.prefab.cloud
 License: MIT
 Author: Michael Berkowitz
 Author-email: michael.berkowitz@gmail.com
 Maintainer: Michael Berkowitz
 Maintainer-email: michael.berkowitz@gmail.com
```

