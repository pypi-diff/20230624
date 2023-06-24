# Comparing `tmp/ovos-backend-client-0.1.0a5.tar.gz` & `tmp/ovos-backend-client-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-backend-client-0.1.0a5.tar", last modified: Wed Jun 21 18:03:26 2023, max compression
+gzip compressed data, was "ovos-backend-client-0.1.0a6.tar", last modified: Sat Jun 24 14:10:45 2023, max compression
```

## Comparing `ovos-backend-client-0.1.0a5.tar` & `ovos-backend-client-0.1.0a6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/ovos_backend_client/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/ovos_backend_client/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    40915 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/backends/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)    38679 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/backends/personal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/ovos_backend_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 18:03:26.000000 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-21 18:03:26.000000 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:03:26.000000 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-21 18:03:26.000000 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 18:03:26.000000 ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:03:26.160849 ovos-backend-client-0.1.0a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-21 18:03:25.000000 ovos-backend-client-0.1.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:10:45.688252 ovos-backend-client-0.1.0a6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-24 14:10:45.688252 ovos-backend-client-0.1.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:10:45.688252 ovos-backend-client-0.1.0a6/ovos_backend_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33568 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:10:45.688252 ovos-backend-client-0.1.0a6/ovos_backend_client/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40817 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/backends/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38679 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/backends/personal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15977 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16539 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/ovos_backend_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:10:45.688252 ovos-backend-client-0.1.0a6/ovos_backend_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-24 14:10:45.000000 ovos-backend-client-0.1.0a6/ovos_backend_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-24 14:10:45.000000 ovos-backend-client-0.1.0a6/ovos_backend_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:10:45.000000 ovos-backend-client-0.1.0a6/ovos_backend_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-24 14:10:45.000000 ovos-backend-client-0.1.0a6/ovos_backend_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-24 14:10:45.000000 ovos-backend-client-0.1.0a6/ovos_backend_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:10:45.688252 ovos-backend-client-0.1.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-24 14:10:44.000000 ovos-backend-client-0.1.0a6/setup.py
```

### Comparing `ovos-backend-client-0.1.0a5/CHANGELOG.md` & `ovos-backend-client-0.1.0a6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Changelog
 
-## [0.1.0a5](https://github.com/OpenVoiceOS/ovos-backend-client/tree/0.1.0a5) (2023-06-21)
+## [0.1.0a6](https://github.com/OpenVoiceOS/ovos-backend-client/tree/0.1.0a6) (2023-06-24)
 
-[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.0a4...0.1.0a5)
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.0a5...0.1.0a6)
+
+**Merged pull requests:**
+
+- Import more xdg functions from ovos\_config rather than ovos\_utils [\#44](https://github.com/OpenVoiceOS/ovos-backend-client/pull/44) ([PureTryOut](https://github.com/PureTryOut))
+
+## [V0.1.0a5](https://github.com/OpenVoiceOS/ovos-backend-client/tree/V0.1.0a5) (2023-06-21)
+
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.0a4...V0.1.0a5)
 
 **Merged pull requests:**
 
 - Import xdg functions from ovos\_config rather than ovos\_utils [\#43](https://github.com/OpenVoiceOS/ovos-backend-client/pull/43) ([PureTryOut](https://github.com/PureTryOut))
 
 ## [V0.1.0a4](https://github.com/OpenVoiceOS/ovos-backend-client/tree/V0.1.0a4) (2023-06-08)
```

### Comparing `ovos-backend-client-0.1.0a5/README.md` & `ovos-backend-client-0.1.0a6/README.md`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/api.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from ovos_utils import timed_lru_cache
 from ovos_utils.log import LOG
 
 import json
 import os
 from os import makedirs
 from os.path import isfile
-from ovos_config.config import Configuration
-from ovos_utils.configuration import get_xdg_config_save_path
+from ovos_config.config import Configuration, get_xdg_config_save_path
 from ovos_backend_client.backends import OfflineBackend, \
     PersonalBackend, BackendType, get_backend_config, API_REGISTRY
 from ovos_backend_client.database import SkillSettingsModel
 from ovos_backend_client.settings import get_local_settings
 
 
 class BaseApi:
```

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/backends/__init__.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/backends/base.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/backends/base.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/backends/offline.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/backends/offline.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 import time
 from os import listdir, makedirs, remove
 from os.path import isfile, join
 from tempfile import NamedTemporaryFile
 from uuid import uuid4
 
 import requests
-from ovos_config.config import Configuration
-from ovos_config.config import update_mycroft_config
-from ovos_config.locations import USER_CONFIG
+from ovos_config.config import Configuration, update_mycroft_config, get_xdg_config_save_path
+from ovos_config.locations import USER_CONFIG, get_xdg_data_save_path, xdg_data_home
 from ovos_utils import timed_lru_cache
-from ovos_utils.configuration import get_xdg_config_save_path, get_xdg_data_save_path
 from ovos_utils.network_utils import get_external_ip
 from ovos_utils.smtp_utils import send_smtp
-from ovos_utils.xdg_utils import xdg_data_home
 from ovos_utils.log import LOG
 from ovos_backend_client.backends.base import AbstractBackend, BackendType
 from ovos_backend_client.database import JsonMetricDatabase, JsonWakeWordDatabase, \
     SkillSettingsModel, OAuthTokenDatabase, OAuthApplicationDatabase, DeviceModel, JsonUtteranceDatabase
 from ovos_backend_client.identity import IdentityManager
 from ovos_backend_client.settings import get_local_settings
```

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/backends/personal.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/backends/personal.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/cloud.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/cloud.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/config.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/config.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/database.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import enum
 import json
 from copy import deepcopy
 
 from json_database import JsonStorageXDG, JsonDatabaseXDG
-from ovos_config.config import Configuration
-from ovos_utils.configuration import get_xdg_config_save_path, get_xdg_base
+from ovos_config.config import Configuration, get_xdg_config_save_path
+from ovos_config.locations import get_xdg_config_save_path
+from ovos_config.meta import get_xdg_base
 
 from ovos_backend_client.identity import IdentityManager
 
 
 class AudioTag(str, enum.Enum):
     UNTAGGED = "untagged"
     WAKE_WORD = "wake_word"
```

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/identity.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/identity.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/pairing.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/pairing.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client/settings.py` & `ovos-backend-client-0.1.0a6/ovos_backend_client/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import re
 from copy import deepcopy
 from os import makedirs
 from os.path import dirname, expanduser, join, isfile, isdir
 
 from json_database import JsonStorage
 from ovos_config import Configuration
+from ovos_config.config import get_xdg_config_save_path
+from ovos_config.locations import get_xdg_data_save_path, get_xdg_data_dirs
 from ovos_utils import camel_case_split
-from ovos_utils.configuration import get_xdg_config_save_path, get_xdg_data_save_path, get_xdg_data_dirs
 from ovos_backend_client.database import SkillSettingsModel
 import ovos_backend_client.api as _api
 
 
 def get_display_name(skill_name: str):
     """Splits camelcase and removes leading/trailing "skill"."""
     skill_name = skill_name.replace("_", " ").replace("-", " ")
```

### Comparing `ovos-backend-client-0.1.0a5/ovos_backend_client.egg-info/SOURCES.txt` & `ovos-backend-client-0.1.0a6/ovos_backend_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a5/setup.py` & `ovos-backend-client-0.1.0a6/setup.py`

 * *Files identical despite different names*

