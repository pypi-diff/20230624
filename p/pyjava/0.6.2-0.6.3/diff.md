# Comparing `tmp/pyjava-0.6.2.tar.gz` & `tmp/pyjava-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjava-0.6.2.tar", last modified: Fri Jun 23 14:50:16 2023, max compression
+gzip compressed data, was "pyjava-0.6.3.tar", last modified: Sat Jun 24 13:07:12 2023, max compression
```

## Comparing `pyjava-0.6.2.tar` & `pyjava-0.6.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.843610 pyjava-0.6.2/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-06-23 14:50:16.843610 pyjava-0.6.2/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      448 2023-04-11 04:53:45.000000 pyjava-0.6.2/README.md
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.839610 pyjava-0.6.2/pyjava/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2612 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.839610 pyjava-0.6.2/pyjava/api/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      688 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/api/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16024 2023-05-26 04:03:49.000000 pyjava-0.6.2/pyjava/api/mlsql.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4524 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/api/serve.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.839610 pyjava-0.6.2/pyjava/cache/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/cache/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      489 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/cache/code_cache.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42222 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/cloudpickle.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7048 2023-04-17 05:24:46.000000 pyjava-0.6.2/pyjava/daemon.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.843610 pyjava-0.6.2/pyjava/data/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/data/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1185 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/data/datasource.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.843610 pyjava-0.6.2/pyjava/datatype/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/datatype/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    64554 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/datatype/types.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2190 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/rayfix.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30195 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/serializers.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.843610 pyjava-0.6.2/pyjava/storage/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/storage/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2825 2023-04-24 06:01:20.000000 pyjava-0.6.2/pyjava/storage/streaming_tar.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.843610 pyjava-0.6.2/pyjava/udf/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6176 2023-06-23 14:39:18.000000 pyjava-0.6.2/pyjava/udf/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3990 2023-06-23 13:03:45.000000 pyjava-0.6.2/pyjava/utils.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      828 2023-06-23 14:49:59.000000 pyjava-0.6.2/pyjava/version.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6457 2023-04-18 03:10:44.000000 pyjava-0.6.2/pyjava/worker.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.839610 pyjava-0.6.2/pyjava.egg-info/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-06-23 14:50:16.000000 pyjava-0.6.2/pyjava.egg-info/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      596 2023-06-23 14:50:16.000000 pyjava-0.6.2/pyjava.egg-info/SOURCES.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-06-23 14:50:16.000000 pyjava-0.6.2/pyjava.egg-info/dependency_links.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        7 2023-06-23 14:50:16.000000 pyjava-0.6.2/pyjava.egg-info/top_level.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       79 2023-06-23 14:50:16.843610 pyjava-0.6.2/setup.cfg
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2955 2023-04-11 04:53:45.000000 pyjava-0.6.2/setup.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:07:12.358324 pyjava-0.6.3/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-06-24 13:07:12.358324 pyjava-0.6.3/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      448 2023-04-11 04:53:45.000000 pyjava-0.6.3/README.md
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:07:12.322324 pyjava-0.6.3/pyjava/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2612 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:07:12.322324 pyjava-0.6.3/pyjava/api/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      688 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/api/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16024 2023-05-26 04:03:49.000000 pyjava-0.6.3/pyjava/api/mlsql.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4524 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/api/serve.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:07:12.322324 pyjava-0.6.3/pyjava/cache/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/cache/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      489 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/cache/code_cache.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42222 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/cloudpickle.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7048 2023-04-17 05:24:46.000000 pyjava-0.6.3/pyjava/daemon.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:07:12.322324 pyjava-0.6.3/pyjava/data/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/data/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1185 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/data/datasource.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:07:12.322324 pyjava-0.6.3/pyjava/datatype/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/datatype/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    64554 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/datatype/types.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2190 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/rayfix.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30195 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/serializers.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:07:12.322324 pyjava-0.6.3/pyjava/storage/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.3/pyjava/storage/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2825 2023-04-24 06:01:20.000000 pyjava-0.6.3/pyjava/storage/streaming_tar.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:07:12.358324 pyjava-0.6.3/pyjava/udf/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5526 2023-06-24 12:14:47.000000 pyjava-0.6.3/pyjava/udf/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1555 2023-06-24 13:03:57.000000 pyjava-0.6.3/pyjava/udf/store.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3990 2023-06-23 13:03:45.000000 pyjava-0.6.3/pyjava/utils.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      828 2023-06-24 13:07:00.000000 pyjava-0.6.3/pyjava/version.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6457 2023-04-18 03:10:44.000000 pyjava-0.6.3/pyjava/worker.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-24 13:07:12.322324 pyjava-0.6.3/pyjava.egg-info/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-06-24 13:07:12.000000 pyjava-0.6.3/pyjava.egg-info/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      616 2023-06-24 13:07:12.000000 pyjava-0.6.3/pyjava.egg-info/SOURCES.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-06-24 13:07:12.000000 pyjava-0.6.3/pyjava.egg-info/dependency_links.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        7 2023-06-24 13:07:12.000000 pyjava-0.6.3/pyjava.egg-info/top_level.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       79 2023-06-24 13:07:12.358324 pyjava-0.6.3/setup.cfg
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2955 2023-04-11 04:53:45.000000 pyjava-0.6.3/setup.py
```

### Comparing `pyjava-0.6.2/PKG-INFO` & `pyjava-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjava
-Version: 0.6.2
+Version: 0.6.3
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyjava-0.6.2/pyjava/__init__.py` & `pyjava-0.6.3/pyjava/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/api/__init__.py` & `pyjava-0.6.3/pyjava/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/api/mlsql.py` & `pyjava-0.6.3/pyjava/api/mlsql.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/api/serve.py` & `pyjava-0.6.3/pyjava/api/serve.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/cloudpickle.py` & `pyjava-0.6.3/pyjava/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/daemon.py` & `pyjava-0.6.3/pyjava/daemon.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/data/datasource.py` & `pyjava-0.6.3/pyjava/data/datasource.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/datatype/types.py` & `pyjava-0.6.3/pyjava/datatype/types.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/rayfix.py` & `pyjava-0.6.3/pyjava/rayfix.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/serializers.py` & `pyjava-0.6.3/pyjava/serializers.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/storage/streaming_tar.py` & `pyjava-0.6.3/pyjava/storage/streaming_tar.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/udf/__init__.py` & `pyjava-0.6.3/pyjava/udf/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,25 +38,16 @@
         if len(custom_resources) > 0:
             udf_worker_conf["resources"] = dict(custom_resources)
 
         udf_name  = conf["UDF_CLIENT"] if "UDF_CLIENT" in conf else "UNKNOW MODEL"
         standalone = conf.get("standalone", "false") == "true"
         model_refs = []
         if "modelServers" in conf and not standalone:
-            model_servers = RayContext.parse_servers(conf["modelServers"])  
-            print_flush(f"MODEL[{udf_name}] Transfer model from {model_servers[0].host}:{model_servers[0].port} to Ray Object Store")                       
-            time1 = time.time()            
-            count = 0           
-            for item in RayContext.collect_from(model_servers):
-                if count % 1000 == 0:
-                    print_flush(f"MODEL[{udf_name}] , current count: {count}")
-                count += 1    
-                model_refs.append(ray.put(item))            
-            time2 = time.time()
-            print_flush(f"MODEL[{udf_name}] Successful to put the model in Ray, time taken:{time2-time1}s. The total refs: {count}") 
+            from .store import transfer_to_ob
+            transfer_to_ob(udf_name, conf,model_refs)
         
         self.actors = dict(
             [(index,
               UDFWorker.options(**udf_worker_conf).remote(model_refs, conf, self.init_func,
                                                           self.apply_func)) for index in
              range(self.num)])
         self._idle_actors = [index for index in range(self.num)]
```

### Comparing `pyjava-0.6.2/pyjava/utils.py` & `pyjava-0.6.3/pyjava/utils.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava/version.py` & `pyjava-0.6.3/pyjava/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
```

### Comparing `pyjava-0.6.2/pyjava/worker.py` & `pyjava-0.6.3/pyjava/worker.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.2/pyjava.egg-info/PKG-INFO` & `pyjava-0.6.3/pyjava.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjava
-Version: 0.6.2
+Version: 0.6.3
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyjava-0.6.2/pyjava.egg-info/SOURCES.txt` & `pyjava-0.6.3/pyjava.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 pyjava/cache/code_cache.py
 pyjava/data/__init__.py
 pyjava/data/datasource.py
 pyjava/datatype/__init__.py
 pyjava/datatype/types.py
 pyjava/storage/__init__.py
 pyjava/storage/streaming_tar.py
-pyjava/udf/__init__.py
+pyjava/udf/__init__.py
+pyjava/udf/store.py
```

### Comparing `pyjava-0.6.2/setup.py` & `pyjava-0.6.3/setup.py`

 * *Files identical despite different names*

