# Comparing `tmp/jaaql-monitor-1.2.73.tar.gz` & `tmp/jaaql-monitor-1.2.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.73.tar", last modified: Fri Jun 23 18:07:57 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.74.tar", last modified: Fri Jun 23 23:48:59 2023, max compression
```

## Comparing `jaaql-monitor-1.2.73.tar` & `jaaql-monitor-1.2.74.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 18:07:57.636523 jaaql-monitor-1.2.73/
--rw-rw-rw-   0        0        0    18124 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.73/LICENSE.txt
--rw-rw-rw-   0        0        0     1454 2023-06-23 18:07:57.635523 jaaql-monitor-1.2.73/PKG-INFO
--rw-rw-rw-   0        0        0     1075 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.73/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 18:07:57.634523 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1454 2023-06-23 18:07:57.000000 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-23 18:07:57.000000 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 18:07:57.000000 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-23 18:07:57.000000 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-23 18:07:57.000000 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-23 18:07:57.635523 jaaql-monitor-1.2.73/monitor/
--rw-rw-rw-   0        0        0        0 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.73/monitor/__init__.py
--rw-rw-rw-   0        0        0    31823 2023-06-23 18:07:46.000000 jaaql-monitor-1.2.73/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-06-23 18:07:49.000000 jaaql-monitor-1.2.73/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-06-23 18:07:57.636523 jaaql-monitor-1.2.73/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.73/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 23:48:59.431678 jaaql-monitor-1.2.74/
+-rw-rw-rw-   0        0        0    18124 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.74/LICENSE.txt
+-rw-rw-rw-   0        0        0     1454 2023-06-23 23:48:59.431678 jaaql-monitor-1.2.74/PKG-INFO
+-rw-rw-rw-   0        0        0     1075 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.74/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 23:48:59.429679 jaaql-monitor-1.2.74/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1454 2023-06-23 23:48:59.000000 jaaql-monitor-1.2.74/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-23 23:48:59.000000 jaaql-monitor-1.2.74/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 23:48:59.000000 jaaql-monitor-1.2.74/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-23 23:48:59.000000 jaaql-monitor-1.2.74/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 23:48:59.000000 jaaql-monitor-1.2.74/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 23:48:59.430677 jaaql-monitor-1.2.74/monitor/
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.74/monitor/__init__.py
+-rw-rw-rw-   0        0        0    31752 2023-06-23 23:48:37.000000 jaaql-monitor-1.2.74/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-06-23 23:48:51.000000 jaaql-monitor-1.2.74/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 23:48:59.431678 jaaql-monitor-1.2.74/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.74/setup.py
```

### Comparing `jaaql-monitor-1.2.73/LICENSE.txt` & `jaaql-monitor-1.2.74/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.73/PKG-INFO` & `jaaql-monitor-1.2.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.73
+Version: 1.2.74
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `jaaql-monitor-1.2.73/README.md` & `jaaql-monitor-1.2.74/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.73/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.74/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.73
+Version: 1.2.74
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `jaaql-monitor-1.2.73/monitor/main.py` & `jaaql-monitor-1.2.74/monitor/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -649,37 +649,14 @@
 
         parameter_file = args[arg_idx + 1]
 
         for line in open(parameter_file, "r").readlines():
             state.parameters[line.split("=")[0]] = "=".join(line.split("=")[1:])
 
     for arg, arg_idx in zip(args, range(len(args))):
-        if arg not in ARGS__folder_config:
-            continue
-
-        if arg_idx == len(args) - 1:
-            print_error(state, "The folder config flag is the last argument. You need to supply a file")
-
-        configuration_folder = args[arg_idx + 1]
-
-        for config_file in os.listdir(configuration_folder):
-            full_file_name = os.path.join(configuration_folder, config_file)
-            if config_file.endswith(".email-credentials.txt"):
-                configuration_name = config_file[0:-len(".email-credentials.txt")]
-            elif config_file.endswith(".credentials.txt"):
-                configuration_name = config_file[0:-len(".credentials.txt")]
-            else:
-                raise JAAQLMonitorException("Unrecognised file extension for file " + full_file_name)
-
-            if configuration_name in state.connections:
-                print_error(state, "The configuration with name '" + configuration_name + "' already exists")
-
-            state.connections[configuration_name] = full_file_name
-
-    for arg, arg_idx in zip(args, range(len(args))):
         if arg not in ARGS__encoded_config and arg not in ARGS__config:
             continue
 
         if arg_idx == len(args) - 1:
             print_error(state, "The config flag is the last argument. You need to supply a file")
 
         configuration_name = args[arg_idx + 1]
@@ -703,14 +680,37 @@
             db = None
             if len(content_split) == 4:
                 db = b64d(content_split[3]).decode()
 
             state.connection_info[configuration_name] = ConnectionInfo(b64d(content_split[0]).decode(), b64d(content_split[1]).decode(),
                                                                        b64d(content_split[2]).decode(), db, state.override_url)
 
+    for arg, arg_idx in zip(args, range(len(args))):
+        if arg not in ARGS__folder_config:
+            continue
+
+        if arg_idx == len(args) - 1:
+            print_error(state, "The folder config flag is the last argument. You need to supply a file")
+
+        configuration_folder = args[arg_idx + 1]
+
+        for config_file in os.listdir(configuration_folder):
+            full_file_name = os.path.join(configuration_folder, config_file)
+            if config_file.endswith(".email-credentials.txt"):
+                configuration_name = config_file[0:-len(".email-credentials.txt")]
+            elif config_file.endswith(".credentials.txt"):
+                configuration_name = config_file[0:-len(".credentials.txt")]
+            else:
+                raise JAAQLMonitorException("Unrecognised file extension for file " + full_file_name)
+
+            if configuration_name in state.connections:
+                continue  # Allow this
+
+            state.connections[configuration_name] = full_file_name
+
     deal_with_input(state, file_content)
 
 
 def initialise(file_name: str, file_content: str, configs: list[[str, str]], encoded_configs: list[[str, str, str, str, str | None]],
                override_url: str, folder_name: str = None):
     args = [ARGS__single_query[0]]
```

### Comparing `jaaql-monitor-1.2.73/setup.py` & `jaaql-monitor-1.2.74/setup.py`

 * *Files identical despite different names*

