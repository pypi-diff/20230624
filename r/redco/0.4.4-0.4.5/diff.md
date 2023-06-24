# Comparing `tmp/redco-0.4.4.tar.gz` & `tmp/redco-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redco-0.4.4.tar", last modified: Mon Jun  5 13:15:21 2023, max compression
+gzip compressed data, was "redco-0.4.5.tar", last modified: Sat Jun 24 20:55:07 2023, max compression
```

## Comparing `redco-0.4.4.tar` & `redco-0.4.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.670000 redco-0.4.4/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.4/LICENSE
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-06-05 13:15:21.670000 redco-0.4.4/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-13 23:56:05.000000 redco-0.4.4/README.md
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.660000 redco-0.4.4/redco/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.4/redco/__init__.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.660000 redco-0.4.4/redco/datasets/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.4/redco/datasets/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-04-19 06:51:00.000000 redco-0.4.4/redco/datasets/dataset.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-04-19 06:51:00.000000 redco-0.4.4/redco/datasets/jsonl_dataset.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.660000 redco-0.4.4/redco/deployers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.4/redco/deployers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2065 2023-04-19 06:51:00.000000 redco-0.4.4/redco/deployers/data_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8110 2023-05-29 01:02:59.000000 redco-0.4.4/redco/deployers/deployer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.4/redco/deployers/log_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.660000 redco-0.4.4/redco/deployers/model_parallel_utils/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.4/redco/deployers/model_parallel_utils/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5546 2023-05-29 00:52:43.000000 redco-0.4.4/redco/deployers/model_parallel_utils/mesh_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1854 2023-05-29 01:00:49.000000 redco-0.4.4/redco/deployers/model_parallel_utils/partition_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.4/redco/deployers/opt_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.670000 redco-0.4.4/redco/predictors/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.4/redco/predictors/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4263 2023-06-02 00:28:54.000000 redco-0.4.4/redco/predictors/predictor.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.4/redco/predictors/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.670000 redco-0.4.4/redco/trainers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.4/redco/trainers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12128 2023-06-02 00:28:54.000000 redco-0.4.4/redco/trainers/trainer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.4/redco/trainers/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.660000 redco-0.4.4/redco.egg-info/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-06-05 13:15:21.000000 redco-0.4.4/redco.egg-info/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-06-05 13:15:21.000000 redco-0.4.4/redco.egg-info/SOURCES.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-06-05 13:15:21.000000 redco-0.4.4/redco.egg-info/dependency_links.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-06-05 13:15:21.000000 redco-0.4.4/redco.egg-info/requires.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-06-05 13:15:21.000000 redco-0.4.4/redco.egg-info/top_level.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-06-05 13:15:21.670000 redco-0.4.4/setup.cfg
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-06-05 13:12:00.000000 redco-0.4.4/setup.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.5/LICENSE
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-06-24 20:55:07.360000 redco-0.4.5/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-13 23:56:05.000000 redco-0.4.5/README.md
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.5/redco/__init__.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/datasets/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.5/redco/datasets/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-06-20 03:18:51.000000 redco-0.4.5/redco/datasets/dataset.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-06-15 02:34:05.000000 redco-0.4.5/redco/datasets/jsonl_dataset.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/deployers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.5/redco/deployers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2064 2023-06-22 04:36:30.000000 redco-0.4.5/redco/deployers/data_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8110 2023-05-29 01:02:59.000000 redco-0.4.5/redco/deployers/deployer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.5/redco/deployers/log_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/deployers/model_parallel_utils/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.5/redco/deployers/model_parallel_utils/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5527 2023-06-22 04:36:30.000000 redco-0.4.5/redco/deployers/model_parallel_utils/mesh_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1854 2023-05-29 01:00:49.000000 redco-0.4.5/redco/deployers/model_parallel_utils/partition_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.5/redco/deployers/opt_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/predictors/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.5/redco/predictors/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4263 2023-06-20 20:03:17.000000 redco-0.4.5/redco/predictors/predictor.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.5/redco/predictors/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/trainers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.5/redco/trainers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12128 2023-06-02 00:28:54.000000 redco-0.4.5/redco/trainers/trainer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.5/redco/trainers/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco.egg-info/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-06-24 20:55:06.000000 redco-0.4.5/redco.egg-info/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-06-24 20:55:07.000000 redco-0.4.5/redco.egg-info/SOURCES.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-06-24 20:55:06.000000 redco-0.4.5/redco.egg-info/dependency_links.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-06-24 20:55:07.000000 redco-0.4.5/redco.egg-info/requires.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-06-24 20:55:07.000000 redco-0.4.5/redco.egg-info/top_level.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-06-24 20:55:07.360000 redco-0.4.5/setup.cfg
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-06-24 20:54:53.000000 redco-0.4.5/setup.py
```

### Comparing `redco-0.4.4/LICENSE` & `redco-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/PKG-INFO` & `redco-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.4
+Version: 0.4.5
 Summary: UNKNOWN
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `redco-0.4.4/README.md` & `redco-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/__init__.py` & `redco-0.4.5/redco/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/datasets/__init__.py` & `redco-0.4.5/redco/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/datasets/dataset.py` & `redco-0.4.5/redco/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/datasets/jsonl_dataset.py` & `redco-0.4.5/redco/datasets/jsonl_dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/deployers/__init__.py` & `redco-0.4.5/redco/deployers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/deployers/data_utils.py` & `redco-0.4.5/redco/deployers/data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import tqdm
-
 import jax
 import jax.numpy as jnp
 from flax.training.common_utils import shard
 
 
 def get_dataloader(examples, batch_size, collate_fn, do_shard):
     def make_jnp(value):
```

### Comparing `redco-0.4.4/redco/deployers/deployer.py` & `redco-0.4.5/redco/deployers/deployer.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/deployers/log_utils.py` & `redco-0.4.5/redco/deployers/log_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/deployers/model_parallel_utils/__init__.py` & `redco-0.4.5/redco/deployers/model_parallel_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/deployers/model_parallel_utils/mesh_utils.py` & `redco-0.4.5/redco/deployers/model_parallel_utils/mesh_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import numpy as np
-
 import jax
-from jax.experimental.maps import Mesh
 from jax.experimental.pjit import pjit
-from jax.experimental.pjit import PartitionSpec as P
+from jax.sharding import Mesh
+from jax.sharding import PartitionSpec as P
 from flax.core.frozen_dict import FrozenDict, unfreeze
 from flax.traverse_util import flatten_dict
 import optax
 
 from .partition_utils import set_partitions
```

### Comparing `redco-0.4.4/redco/deployers/model_parallel_utils/partition_utils.py` & `redco-0.4.5/redco/deployers/model_parallel_utils/partition_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/deployers/opt_utils.py` & `redco-0.4.5/redco/deployers/opt_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/predictors/__init__.py` & `redco-0.4.5/redco/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/predictors/predictor.py` & `redco-0.4.5/redco/predictors/predictor.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/predictors/utils.py` & `redco-0.4.5/redco/predictors/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/trainers/__init__.py` & `redco-0.4.5/redco/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/trainers/trainer.py` & `redco-0.4.5/redco/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco/trainers/utils.py` & `redco-0.4.5/redco/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/redco.egg-info/PKG-INFO` & `redco-0.4.5/redco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.4
+Version: 0.4.5
 Summary: UNKNOWN
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `redco-0.4.4/redco.egg-info/SOURCES.txt` & `redco-0.4.5/redco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redco-0.4.4/setup.py` & `redco-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="redco",
-    version="0.4.4",
+    version="0.4.5",
     author="Bowen Tan",
     packages=find_packages(),
     install_requires=['jax', 'flax', 'optax', 'numpy'],
     include_package_data=True,
     python_requires=">=3.8",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

