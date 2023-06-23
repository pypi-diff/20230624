# Comparing `tmp/avocado-framework-plugin-robot-98.0.tar.gz` & `tmp/avocado-framework-plugin-robot-99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocado-framework-plugin-robot-98.0.tar", last modified: Thu Jul 14 20:54:10 2022, max compression
+gzip compressed data, was "avocado-framework-plugin-robot-99.0.tar", last modified: Thu Nov 10 19:13:09 2022, max compression
```

## Comparing `avocado-framework-plugin-robot-98.0.tar` & `avocado-framework-plugin-robot-99.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:10.508745 avocado-framework-plugin-robot-98.0/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       16 2019-07-19 21:00:45.000000 avocado-framework-plugin-robot-98.0/MANIFEST.in
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      249 2022-07-14 20:54:10.508745 avocado-framework-plugin-robot-98.0/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        5 2022-07-14 20:50:57.000000 avocado-framework-plugin-robot-98.0/VERSION
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:10.507745 avocado-framework-plugin-robot-98.0/avocado_framework_plugin_robot.egg-info/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      249 2022-07-14 20:54:10.000000 avocado-framework-plugin-robot-98.0/avocado_framework_plugin_robot.egg-info/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      401 2022-07-14 20:54:10.000000 avocado-framework-plugin-robot-98.0/avocado_framework_plugin_robot.egg-info/SOURCES.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2022-07-14 20:54:10.000000 avocado-framework-plugin-robot-98.0/avocado_framework_plugin_robot.egg-info/dependency_links.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      213 2022-07-14 20:54:10.000000 avocado-framework-plugin-robot-98.0/avocado_framework_plugin_robot.egg-info/entry_points.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       44 2022-07-14 20:54:10.000000 avocado-framework-plugin-robot-98.0/avocado_framework_plugin_robot.egg-info/requires.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       14 2022-07-14 20:54:10.000000 avocado-framework-plugin-robot-98.0/avocado_framework_plugin_robot.egg-info/top_level.txt
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:10.508745 avocado-framework-plugin-robot-98.0/avocado_robot/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2550 2022-07-11 13:32:25.000000 avocado-framework-plugin-robot-98.0/avocado_robot/robot.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4191 2022-07-11 13:32:25.000000 avocado-framework-plugin-robot-98.0/avocado_robot/runner.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       38 2022-07-14 20:54:10.508745 avocado-framework-plugin-robot-98.0/setup.cfg
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1611 2022-07-11 13:32:25.000000 avocado-framework-plugin-robot-98.0/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:09.356257 avocado-framework-plugin-robot-99.0/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       16 2019-07-19 21:00:45.000000 avocado-framework-plugin-robot-99.0/MANIFEST.in
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      249 2022-11-10 19:13:09.356257 avocado-framework-plugin-robot-99.0/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        5 2022-11-10 19:09:51.000000 avocado-framework-plugin-robot-99.0/VERSION
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:09.356257 avocado-framework-plugin-robot-99.0/avocado_framework_plugin_robot.egg-info/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      249 2022-11-10 19:13:09.000000 avocado-framework-plugin-robot-99.0/avocado_framework_plugin_robot.egg-info/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      401 2022-11-10 19:13:09.000000 avocado-framework-plugin-robot-99.0/avocado_framework_plugin_robot.egg-info/SOURCES.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2022-11-10 19:13:09.000000 avocado-framework-plugin-robot-99.0/avocado_framework_plugin_robot.egg-info/dependency_links.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      213 2022-11-10 19:13:09.000000 avocado-framework-plugin-robot-99.0/avocado_framework_plugin_robot.egg-info/entry_points.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       44 2022-11-10 19:13:09.000000 avocado-framework-plugin-robot-99.0/avocado_framework_plugin_robot.egg-info/requires.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       14 2022-11-10 19:13:09.000000 avocado-framework-plugin-robot-99.0/avocado_framework_plugin_robot.egg-info/top_level.txt
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:09.356257 avocado-framework-plugin-robot-99.0/avocado_robot/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2550 2022-11-04 17:27:10.000000 avocado-framework-plugin-robot-99.0/avocado_robot/robot.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3549 2022-11-04 17:27:10.000000 avocado-framework-plugin-robot-99.0/avocado_robot/runner.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2022-11-10 19:13:09.356257 avocado-framework-plugin-robot-99.0/setup.cfg
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1611 2022-11-04 17:27:10.000000 avocado-framework-plugin-robot-99.0/setup.py
```

### Comparing `avocado-framework-plugin-robot-98.0/avocado_robot/robot.py` & `avocado-framework-plugin-robot-99.0/avocado_robot/robot.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-robot-98.0/avocado_robot/runner.py` & `avocado-framework-plugin-robot-99.0/avocado_robot/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,19 @@
 """
 Avocado nrunner for Robot Framework tests
 """
 
 import io
 import multiprocessing
 import tempfile
-import time
 
 from robot import run
 
 from avocado.core.nrunner.app import BaseRunnerApp
-from avocado.core.nrunner.runner import (
-    RUNNER_RUN_CHECK_INTERVAL,
-    RUNNER_RUN_STATUS_INTERVAL,
-    BaseRunner,
-)
+from avocado.core.nrunner.runner import BaseRunner
 from avocado.core.utils import messages
 
 
 class RobotRunner(BaseRunner):
 
     name = "robot"
     description = "Runner for Robot Framework tests"
@@ -96,29 +91,15 @@
 
         queue = multiprocessing.SimpleQueue()
         process = multiprocessing.Process(
             target=self._run, args=(file_name, suite_name, test_name, queue)
         )
         process.start()
         yield messages.StartedMessage.get()
-
-        most_current_execution_state_time = None
-        while queue.empty():
-            time.sleep(RUNNER_RUN_CHECK_INTERVAL)
-            now = time.monotonic()
-            if most_current_execution_state_time is not None:
-                next_execution_state_mark = (
-                    most_current_execution_state_time + RUNNER_RUN_STATUS_INTERVAL
-                )
-            if (
-                most_current_execution_state_time is None
-                or now > next_execution_state_mark
-            ):
-                most_current_execution_state_time = now
-                yield messages.RunningMessage.get()
+        yield from self.running_loop(lambda: not queue.empty())
 
         status = queue.get()
         yield messages.StdoutMessage.get(status["stdout"])
         yield messages.StderrMessage.get(status["stderr"])
         yield messages.FinishedMessage.get(status["result"])
```

### Comparing `avocado-framework-plugin-robot-98.0/setup.py` & `avocado-framework-plugin-robot-99.0/setup.py`

 * *Files identical despite different names*

