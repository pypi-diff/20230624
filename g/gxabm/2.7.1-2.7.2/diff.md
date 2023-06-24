# Comparing `tmp/gxabm-2.7.1.tar.gz` & `tmp/gxabm-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.7.1.tar", last modified: Tue Jun 20 16:58:13 2023, max compression
+gzip compressed data, was "gxabm-2.7.2.tar", last modified: Sat Jun 24 18:45:00 2023, max compression
```

## Comparing `gxabm-2.7.1.tar` & `gxabm-2.7.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-20 16:58:13.709203 gxabm-2.7.1/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.1/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-20 16:58:13.708827 gxabm-2.7.1/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.1/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-20 16:58:13.699522 gxabm-2.7.1/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        6 2023-06-20 16:57:31.000000 gxabm-2.7.1/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.1/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.1/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-20 16:58:13.705106 gxabm-2.7.1/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.1/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    19882 2023-06-13 14:43:19.000000 gxabm-2.7.1/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.1/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     9068 2023-06-13 14:43:19.000000 gxabm-2.7.1/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.7.1/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     7902 2023-06-13 14:43:19.000000 gxabm-2.7.1/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.7.1/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.1/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.7.1/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.1/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)    11467 2023-06-13 14:43:19.000000 gxabm-2.7.1/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.1/abm/lib/invocation.py
--rw-r--r--   0 suderman   (502) staff       (20)     5049 2023-06-20 16:56:58.000000 gxabm-2.7.1/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.1/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.1/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-13 14:43:19.000000 gxabm-2.7.1/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.1/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.1/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-20 16:58:13.706230 gxabm-2.7.1/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      691 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-06-20 16:58:13.709335 gxabm-2.7.1/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.1/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-20 16:58:13.707894 gxabm-2.7.1/test/
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.1/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.1/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.1/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.1/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.1/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-24 18:45:00.049835 gxabm-2.7.2/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.2/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-24 18:45:00.049650 gxabm-2.7.2/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.2/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-24 18:45:00.040247 gxabm-2.7.2/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        6 2023-06-24 18:44:37.000000 gxabm-2.7.2/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.2/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.2/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-24 18:45:00.046479 gxabm-2.7.2/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.2/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    19882 2023-06-13 14:43:19.000000 gxabm-2.7.2/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.2/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     9068 2023-06-13 14:43:19.000000 gxabm-2.7.2/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2023-06-24 18:27:14.000000 gxabm-2.7.2/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7902 2023-06-13 14:43:19.000000 gxabm-2.7.2/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.7.2/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.2/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.7.2/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.2/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)    11689 2023-06-24 18:44:37.000000 gxabm-2.7.2/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.2/abm/lib/invocation.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5049 2023-06-20 16:56:58.000000 gxabm-2.7.2/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.2/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.2/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-13 14:43:19.000000 gxabm-2.7.2/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.2/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.2/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-24 18:45:00.047428 gxabm-2.7.2/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      691 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-06-24 18:45:00.049888 gxabm-2.7.2/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.2/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-24 18:45:00.049060 gxabm-2.7.2/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.2/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.2/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.2/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.2/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.2/test/workflow.py
```

### Comparing `gxabm-2.7.1/PKG-INFO` & `gxabm-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.7.1
+Version: 2.7.2
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.7.1/README.md` & `gxabm-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/__main__.py` & `gxabm-2.7.2/abm/__main__.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/benchmark.py` & `gxabm-2.7.2/abm/lib/benchmark.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/cloudlaunch.py` & `gxabm-2.7.2/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/common.py` & `gxabm-2.7.2/abm/lib/common.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/config.py` & `gxabm-2.7.2/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/dataset.py` & `gxabm-2.7.2/abm/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/experiment.py` & `gxabm-2.7.2/abm/lib/experiment.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/folder.py` & `gxabm-2.7.2/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/helm.py` & `gxabm-2.7.2/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/history.py` & `gxabm-2.7.2/abm/lib/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,19 @@
     if '--contents' in args:
         contents = True
         args.remove('--contents')
     if len(args) == 0:
         print("ERROR: No history ID provided.")
         return
     gi = connect(context)
-    history = gi.histories.show_history(args[0], contents=contents)
+    hid = find_history(gi, args[0])
+    if hid is None:
+        print(f"ERROR: No such history {args[0]}")
+        return
+    history = gi.histories.show_history(hid, contents=contents)
     print(json.dumps(history, indent=4))
 
 
 def find(context: Context, args: list):
     if len(args) == 0:
         print("ERROR: No history ID provided")
         return
@@ -123,16 +127,16 @@
         args.remove('--no-wait')
     if  '-n' in args:
         wait = False
         args.remove('-w')
     if len(args) == 0:
         print("ERROR: no history ID specified")
         return
-    hid = args[0]
     gi = connect(context)
+    hid = find_history(gi, args[0])
     jeha_id = gi.histories.export_history(hid, gzip=True, wait=wait)
     # global GALAXY_SERVER
     export_url = "unknown"
     if wait:
         export_url = f"{context.GALAXY_SERVER}/history/export_archive?id={args[0]}&jeha_id={jeha_id}"
         print(f"The history can be imported from {export_url}")
         history = gi.histories.show_history(hid, contents=False)
@@ -150,25 +154,25 @@
 
 
 def publish(context: Context, args: list):
     if len(args) == 0:
         print("ERROR: No history ID provided.")
         return
     gi = connect(context)
-    result = gi.histories.update_history(args[0], published=True)
+    result = gi.histories.update_history(find_history(gi, args[0]), published=True)
     print(f"Published: {result['published']}")
 
 
 def rename(context: Context, args: list):
     if len(args) != 2:
         print("ERROR: Invalid command")
         print("USAGE: rename ID 'new history name'")
         return
     gi = connect(context)
-    result = gi.histories.update_history(args[0], name=args[1])
+    result = gi.histories.update_history(find_history(gi, args[0]), name=args[1])
     print(f"History renamed to {result['name']}")
 
 
 def _import(context: Context, args: list):
     gi = connect(context)
     result = gi.histories.import_history(url=args[0])
     id = result['id']
@@ -268,15 +272,15 @@
     print(f"Deleted history {args[0]}")
 
 
 def copy(context:Context, args:list):
     if len(args) != 2:
         print("ERROR: Invalid parameters. Provide a history ID and new history name.")
         return
-    id = args[0]
+    id = find_history(args[0])
     name = args[1]
 
     gi = connect(context)
     new_history = gi.histories.create_history(name)
     datasets = gi.datasets.get_datasets(history_id=id)
     for dataset in datasets:
         gi.histories.copy_dataset(new_history['id'], dataset['id'])
@@ -314,29 +318,29 @@
         replace = True
         args.remove('-r')
     if len(args) < 2:
         print("ERROR: Invalid command. Please provide the history ID and one or more tags.")
         return
 
     gi = connect(context)
-    hid = args.pop(0)
+    hid = find_history(gi, args.pop(0))
     if not replace:
         history = gi.histories.show_history(hid, contents=False)
         args += history['tags']
     gi.histories.update_history(hid, tags=args)
     print(f"Set history tags to: {', '.join(args)}")
 
 def summarize(context: Context, args: list):
     if len(args) == 0:
         print("ERROR: Provide one or more history ID values.")
         return
     gi = connect(context)
     all_jobs = []
     while len(args) > 0:
-        hid = args.pop(0)
+        hid = find_history(gi, args.pop(0))
         history = gi.histories.show_history(history_id=hid)
         jobs = gi.jobs.get_jobs(history_id=hid)
         for job in jobs:
             job['invocation_id'] = ''
             job['history_id'] = hid
             job['history_name'] = history['name']
             job['workflow_id'] = ''
```

### Comparing `gxabm-2.7.1/abm/lib/invocation.py` & `gxabm-2.7.2/abm/lib/invocation.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/job.py` & `gxabm-2.7.2/abm/lib/job.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/kubectl.py` & `gxabm-2.7.2/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/library.py` & `gxabm-2.7.2/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/menu.yml` & `gxabm-2.7.2/abm/lib/menu.yml`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/users.py` & `gxabm-2.7.2/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/abm/lib/workflow.py` & `gxabm-2.7.2/abm/lib/workflow.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/gxabm.egg-info/PKG-INFO` & `gxabm-2.7.2/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.7.1
+Version: 2.7.2
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.7.1/gxabm.egg-info/SOURCES.txt` & `gxabm-2.7.2/gxabm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/setup.py` & `gxabm-2.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/test/check_tools.py` & `gxabm-2.7.2/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/test/metrics.py` & `gxabm-2.7.2/test/metrics.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.1/test/workflow.py` & `gxabm-2.7.2/test/workflow.py`

 * *Files identical despite different names*

