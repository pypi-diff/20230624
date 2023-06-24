# Comparing `tmp/krutils-0.20230621.1233.tar.gz` & `tmp/krutils-0.20230624.2226.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230621.1233.tar", last modified: Wed Jun 21 03:33:04 2023, max compression
+gzip compressed data, was "krutils-0.20230624.2226.tar", last modified: Sat Jun 24 13:26:31 2023, max compression
```

## Comparing `krutils-0.20230621.1233.tar` & `krutils-0.20230624.2226.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 03:33:04.487017 krutils-0.20230621.1233/
--rw-rw-rw-   0        0        0      526 2023-06-21 03:33:04.487017 krutils-0.20230621.1233/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230621.1233/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 03:33:04.452060 krutils-0.20230621.1233/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230621.1233/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230621.1233/krutils/CONST.py
--rw-rw-rw-   0        0        0      115 2023-06-07 14:26:39.000000 krutils-0.20230621.1233/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230621.1233/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0     2956 2023-06-20 05:26:47.000000 krutils-0.20230621.1233/krutils/futils.py
--rw-rw-rw-   0        0        0    12812 2023-06-09 06:11:45.000000 krutils-0.20230621.1233/krutils/logger.py
--rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230621.1233/krutils/logger2.py
--rw-rw-rw-   0        0        0    18188 2023-06-07 14:23:27.000000 krutils-0.20230621.1233/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:33:04.468432 krutils-0.20230621.1233/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-06-21 03:33:04.000000 krutils-0.20230621.1233/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-21 03:33:04.000000 krutils-0.20230621.1233/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 03:33:04.000000 krutils-0.20230621.1233/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-21 03:33:04.000000 krutils-0.20230621.1233/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 03:33:04.000000 krutils-0.20230621.1233/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 03:33:04.487017 krutils-0.20230621.1233/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-06-21 03:33:03.000000 krutils-0.20230621.1233/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:33:04.482021 krutils-0.20230621.1233/test/
--rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230621.1233/test/test_futils.py
--rw-rw-rw-   0        0        0      231 2023-06-07 14:23:57.000000 krutils-0.20230621.1233/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:26:31.934631 krutils-0.20230624.2226/
+-rw-rw-rw-   0        0        0      526 2023-06-24 13:26:31.932382 krutils-0.20230624.2226/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230624.2226/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 13:26:31.853721 krutils-0.20230624.2226/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230624.2226/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230624.2226/krutils/CONST.py
+-rw-rw-rw-   0        0        0      115 2023-06-07 14:26:39.000000 krutils-0.20230624.2226/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230624.2226/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0     2956 2023-06-20 05:26:47.000000 krutils-0.20230624.2226/krutils/futils.py
+-rw-rw-rw-   0        0        0    13839 2023-06-24 13:23:13.000000 krutils-0.20230624.2226/krutils/logger.py
+-rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230624.2226/krutils/logger2.py
+-rw-rw-rw-   0        0        0    18188 2023-06-07 14:23:27.000000 krutils-0.20230624.2226/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:26:31.910912 krutils-0.20230624.2226/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-06-24 13:26:31.000000 krutils-0.20230624.2226/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-24 13:26:31.000000 krutils-0.20230624.2226/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:26:31.000000 krutils-0.20230624.2226/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-24 13:26:31.000000 krutils-0.20230624.2226/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-24 13:26:31.000000 krutils-0.20230624.2226/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:26:31.934631 krutils-0.20230624.2226/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-06-24 13:26:29.000000 krutils-0.20230624.2226/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:26:31.930360 krutils-0.20230624.2226/test/
+-rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230624.2226/test/test_futils.py
+-rw-rw-rw-   0        0        0      321 2023-06-24 13:23:59.000000 krutils-0.20230624.2226/test/test_logger.py
```

### Comparing `krutils-0.20230621.1233/PKG-INFO` & `krutils-0.20230624.2226/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230621.1233
+Version: 0.20230624.2226
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230621.1233/krutils/CONST.py` & `krutils-0.20230624.2226/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230621.1233/krutils/_dbmgr.py` & `krutils-0.20230624.2226/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230621.1233/krutils/futils.py` & `krutils-0.20230624.2226/krutils/futils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230621.1233/krutils/logger.py` & `krutils-0.20230624.2226/krutils/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,22 +85,28 @@
         except Exception as e:
             v = nv
 
         # print (f'v[{v}]')
 
         return v
 
-    def find_config_file_path(self, start_path: str) -> str:
+    def find_config_file_path(self, start_path: str, settings) -> str:
         ''' logger 설정 파일을 찾는다 '''
 
         import os
 
         curr_dir = os.path.dirname(start_path)
         CONFIG_FILE_NAME = 'logger.json'
 
+        if (settings != None and
+            len(settings) > 0   ):
+            CONFIG_FILE_NAME = settings
+
+        # print('find setting file[' + CONFIG_FILE_NAME + '] from [' + curr_dir + ']')
+
         config_file_path = ""
         for ii in range(5):
             # print("seeking..[{0}]th : {1}".format(ii, curr_dir))
 
             if (os.path.isfile(CONFIG_FILE_NAME) == True):      # 가상환경에서는 디렉토리정보가 없다!!?
                 config_file_path = CONFIG_FILE_NAME
                 # print("찾았다!", config_file_path)
@@ -140,19 +146,25 @@
             return None
 
         # config 객체 매핑하자
         parsed_config = _logger_config()
 
         parsed_config.CONFIG_FILE_PATH = config_file_path
 
-        parsed_config.CURR_DEBUG_LEVEL = self.get_log_level_index(self.nvl_dict(config_json, 'LOG_LEVEL', parsed_config.CURR_DEBUG_LEVEL))
-        parsed_config.DEBUG_CONSOLE_PRINT_YN = self.nvl_dict(config_json, 'LOG_CONSOLE_YN', parsed_config.DEBUG_CONSOLE_PRINT_YN)
-        parsed_config.DEBUG_FILE_PRINT_YN = self.nvl_dict(config_json, 'LOG_FILE_YN', parsed_config.DEBUG_FILE_PRINT_YN)
-        parsed_config.DEBUG_FILE_DIR_PATH = self.nvl_dict(config_json, 'LOG_DIR_PATH', parsed_config.DEBUG_FILE_DIR_PATH)
-        parsed_config.DEBUG_FILE_FILE_NAME = self.nvl_dict(config_json, 'LOG_FILE_NAME', parsed_config.DEBUG_FILE_FILE_NAME)
+        if config_json['LOGGING'] != None:
+            # parsed_config.CURR_DEBUG_LEVEL = self.get_log_level_index(self.nvl_dict(config_json, 'LOG_LEVEL', parsed_config.CURR_DEBUG_LEVEL))
+            # parsed_config.DEBUG_CONSOLE_PRINT_YN = self.nvl_dict(config_json, 'LOG_CONSOLE_YN', parsed_config.DEBUG_CONSOLE_PRINT_YN)
+            # parsed_config.DEBUG_FILE_PRINT_YN = self.nvl_dict(config_json, 'LOG_FILE_YN', parsed_config.DEBUG_FILE_PRINT_YN)
+            # parsed_config.DEBUG_FILE_DIR_PATH = self.nvl_dict(config_json, 'LOG_DIR_PATH', parsed_config.DEBUG_FILE_DIR_PATH)
+            # parsed_config.DEBUG_FILE_FILE_NAME = self.nvl_dict(config_json, 'LOG_FILE_NAME', parsed_config.DEBUG_FILE_FILE_NAME)
+            parsed_config.CURR_DEBUG_LEVEL = self.get_log_level_index(self.nvl_dict(config_json['LOGGING'], 'LOG_LEVEL', parsed_config.CURR_DEBUG_LEVEL))
+            parsed_config.DEBUG_CONSOLE_PRINT_YN = self.nvl_dict(config_json['LOGGING'], 'LOG_CONSOLE_YN', parsed_config.DEBUG_CONSOLE_PRINT_YN)
+            parsed_config.DEBUG_FILE_PRINT_YN = self.nvl_dict(config_json['LOGGING'], 'LOG_FILE_YN', parsed_config.DEBUG_FILE_PRINT_YN)
+            parsed_config.DEBUG_FILE_DIR_PATH = self.nvl_dict(config_json['LOGGING'], 'LOG_DIR_PATH', parsed_config.DEBUG_FILE_DIR_PATH)
+            parsed_config.DEBUG_FILE_FILE_NAME = self.nvl_dict(config_json['LOGGING'], 'LOG_FILE_NAME', parsed_config.DEBUG_FILE_FILE_NAME)
 
         # print(parsed_config.__dict__)
         return parsed_config
 
 
 
 
@@ -338,24 +350,24 @@
         * LOG_CONSOLE_YN : Y*/N
         * LOG_FILE_YN : Y/N*
         * LOG_DIR_PATH : log directory path(None is default)
         * LOG_FILE_NAME : log file name(None is default)
 
     '''
 
-    def __init__(self, ____file__: str):
+    def __init__(self, ____file__: str, settings=''):
 
         # logger에 필요한 변수와 기능이 담겨있는 super 클래스를 초기화 한다.
         super().__init__()
 
         caller_path = ____file__
 
         # 인자로 받은 호출자 경로로 부터 root까지 탐색하며 config 파일을 찾는다.
         # 존재시 설정을 덮어 씌운다
-        cfp = _logger_util().find_config_file_path(caller_path)
+        cfp = _logger_util().find_config_file_path(caller_path, settings)
 
         if (cfp != None and len(cfp.strip()) > 0):
             parsed_config = _logger_util().parse_config_file(cfp)
 
             if (parsed_config != None):
                 self.config = parsed_config
                 self.config.CONFIG_FILE_PATH = cfp
```

### Comparing `krutils-0.20230621.1233/krutils/logger2.py` & `krutils-0.20230624.2226/krutils/logger2.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230621.1233/krutils/utils.py` & `krutils-0.20230624.2226/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230621.1233/krutils.egg-info/PKG-INFO` & `krutils-0.20230624.2226/krutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230621.1233
+Version: 0.20230624.2226
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230621.1233/setup.py` & `krutils-0.20230624.2226/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230621.1233",
+    version="0.20230624.2226",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

