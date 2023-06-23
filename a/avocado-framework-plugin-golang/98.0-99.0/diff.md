# Comparing `tmp/avocado-framework-plugin-golang-98.0.tar.gz` & `tmp/avocado-framework-plugin-golang-99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocado-framework-plugin-golang-98.0.tar", last modified: Thu Jul 14 20:53:49 2022, max compression
+gzip compressed data, was "avocado-framework-plugin-golang-99.0.tar", last modified: Thu Nov 10 19:12:47 2022, max compression
```

## Comparing `avocado-framework-plugin-golang-98.0.tar` & `avocado-framework-plugin-golang-99.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:49.970615 avocado-framework-plugin-golang-98.0/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       16 2019-07-19 21:00:45.000000 avocado-framework-plugin-golang-98.0/MANIFEST.in
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      241 2022-07-14 20:53:49.970615 avocado-framework-plugin-golang-98.0/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        5 2022-07-14 20:50:57.000000 avocado-framework-plugin-golang-98.0/VERSION
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:49.969615 avocado-framework-plugin-golang-98.0/avocado_framework_plugin_golang.egg-info/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      241 2022-07-14 20:53:49.000000 avocado-framework-plugin-golang-98.0/avocado_framework_plugin_golang.egg-info/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      410 2022-07-14 20:53:49.000000 avocado-framework-plugin-golang-98.0/avocado_framework_plugin_golang.egg-info/SOURCES.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2022-07-14 20:53:49.000000 avocado-framework-plugin-golang-98.0/avocado_framework_plugin_golang.egg-info/dependency_links.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      222 2022-07-14 20:53:49.000000 avocado-framework-plugin-golang-98.0/avocado_framework_plugin_golang.egg-info/entry_points.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       24 2022-07-14 20:53:49.000000 avocado-framework-plugin-golang-98.0/avocado_framework_plugin_golang.egg-info/requires.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       15 2022-07-14 20:53:49.000000 avocado-framework-plugin-golang-98.0/avocado_framework_plugin_golang.egg-info/top_level.txt
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:49.970615 avocado-framework-plugin-golang-98.0/avocado_golang/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3386 2022-07-11 13:32:25.000000 avocado-framework-plugin-golang-98.0/avocado_golang/golang.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     2407 2022-07-11 13:32:25.000000 avocado-framework-plugin-golang-98.0/avocado_golang/runner.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       38 2022-07-14 20:53:49.970615 avocado-framework-plugin-golang-98.0/setup.cfg
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1636 2022-07-11 13:32:25.000000 avocado-framework-plugin-golang-98.0/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:47.576156 avocado-framework-plugin-golang-99.0/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       16 2019-07-19 21:00:45.000000 avocado-framework-plugin-golang-99.0/MANIFEST.in
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      241 2022-11-10 19:12:47.576156 avocado-framework-plugin-golang-99.0/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        5 2022-11-10 19:09:51.000000 avocado-framework-plugin-golang-99.0/VERSION
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:47.576156 avocado-framework-plugin-golang-99.0/avocado_framework_plugin_golang.egg-info/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      241 2022-11-10 19:12:47.000000 avocado-framework-plugin-golang-99.0/avocado_framework_plugin_golang.egg-info/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      410 2022-11-10 19:12:47.000000 avocado-framework-plugin-golang-99.0/avocado_framework_plugin_golang.egg-info/SOURCES.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2022-11-10 19:12:47.000000 avocado-framework-plugin-golang-99.0/avocado_framework_plugin_golang.egg-info/dependency_links.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      222 2022-11-10 19:12:47.000000 avocado-framework-plugin-golang-99.0/avocado_framework_plugin_golang.egg-info/entry_points.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       24 2022-11-10 19:12:47.000000 avocado-framework-plugin-golang-99.0/avocado_framework_plugin_golang.egg-info/requires.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       15 2022-11-10 19:12:47.000000 avocado-framework-plugin-golang-99.0/avocado_framework_plugin_golang.egg-info/top_level.txt
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:47.576156 avocado-framework-plugin-golang-99.0/avocado_golang/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3386 2022-11-04 17:27:10.000000 avocado-framework-plugin-golang-99.0/avocado_golang/golang.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2395 2022-11-04 17:27:10.000000 avocado-framework-plugin-golang-99.0/avocado_golang/runner.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2022-11-10 19:12:47.576156 avocado-framework-plugin-golang-99.0/setup.cfg
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1636 2022-11-04 17:27:10.000000 avocado-framework-plugin-golang-99.0/setup.py
```

### Comparing `avocado-framework-plugin-golang-98.0/avocado_golang/golang.py` & `avocado-framework-plugin-golang-99.0/avocado_golang/golang.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-golang-98.0/avocado_golang/runner.py` & `avocado-framework-plugin-golang-99.0/avocado_golang/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import subprocess
-import time
 
 from avocado_golang.golang import GO_BIN
 
 from avocado.core.nrunner.app import BaseRunnerApp
-from avocado.core.nrunner.runner import RUNNER_RUN_STATUS_INTERVAL, BaseRunner
+from avocado.core.nrunner.runner import BaseRunner
 from avocado.core.utils import messages
 
 
 class GolangRunner(BaseRunner):
     """Runner for Golang tests.
 
     When creating the Runnable, use the following attributes:
@@ -61,17 +60,19 @@
         process = subprocess.Popen(
             cmd,
             stdin=subprocess.DEVNULL,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
 
-        while process.poll() is None:
-            time.sleep(RUNNER_RUN_STATUS_INTERVAL)
-            yield messages.RunningMessage.get()
+        def poll_proc():
+            return process.poll() is not None
+
+        yield self.prepare_status("started")
+        yield from self.running_loop(poll_proc)
 
         result = "pass" if process.returncode == 0 else "fail"
         yield messages.StdoutMessage.get(process.stdout.read())
         yield messages.StderrMessage.get(process.stderr.read())
         yield messages.FinishedMessage.get(result, returncode=process.returncode)
```

### Comparing `avocado-framework-plugin-golang-98.0/setup.py` & `avocado-framework-plugin-golang-99.0/setup.py`

 * *Files identical despite different names*

