# Comparing `tmp/bullmq-1.1.0.tar.gz` & `tmp/bullmq-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-1.1.0.tar", last modified: Fri Jun 23 19:17:12 2023, max compression
+gzip compressed data, was "bullmq-1.2.0.tar", last modified: Sat Jun 24 16:26:41 2023, max compression
```

## Comparing `bullmq-1.1.0.tar` & `bullmq-1.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:17:12.299510 bullmq-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-23 19:17:12.299510 bullmq-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-23 19:15:56.000000 bullmq-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:17:12.287510 bullmq-1.1.0/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-23 19:17:08.000000 bullmq-1.1.0/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:17:12.299510 bullmq-1.1.0/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/addJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/changePriority-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveToActive-10.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveToFinished-13.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/pause-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/promote-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/retryJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:17:12.299510 bullmq-1.1.0/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:17:12.287510 bullmq-1.1.0/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-23 19:17:12.000000 bullmq-1.1.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-23 19:17:12.000000 bullmq-1.1.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:17:12.000000 bullmq-1.1.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 19:17:12.000000 bullmq-1.1.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 19:17:12.000000 bullmq-1.1.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-23 19:17:12.299510 bullmq-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-23 19:15:56.000000 bullmq-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:26:41.742303 bullmq-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-24 16:26:41.742303 bullmq-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-24 16:25:13.000000 bullmq-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:26:41.734303 bullmq-1.2.0/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-24 16:26:39.000000 bullmq-1.2.0/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:26:41.742303 bullmq-1.2.0/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/addJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/changePriority-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveToActive-10.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveToFinished-13.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/pause-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/promote-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/retryJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:26:41.742303 bullmq-1.2.0/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:26:41.734303 bullmq-1.2.0/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-24 16:26:41.000000 bullmq-1.2.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-24 16:26:41.000000 bullmq-1.2.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 16:26:41.000000 bullmq-1.2.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-24 16:26:41.000000 bullmq-1.2.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 16:26:41.000000 bullmq-1.2.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-24 16:26:41.742303 bullmq-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-24 16:25:13.000000 bullmq-1.2.0/setup.py
```

### Comparing `bullmq-1.1.0/PKG-INFO` & `bullmq-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.1.0
+Version: 1.2.0
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.1.0/README.md` & `bullmq-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/backoffs.py` & `bullmq-1.2.0/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/addJob-9.lua` & `bullmq-1.2.0/bullmq/commands/addJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/changeDelay-3.lua` & `bullmq-1.2.0/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/changePriority-5.lua` & `bullmq-1.2.0/bullmq/commands/changePriority-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-1.2.0/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/drain-4.lua` & `bullmq-1.2.0/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/getCounts-1.lua` & `bullmq-1.2.0/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/getRanges-1.lua` & `bullmq-1.2.0/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/getState-8.lua` & `bullmq-1.2.0/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/getStateV2-8.lua` & `bullmq-1.2.0/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/isFinished-3.lua` & `bullmq-1.2.0/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-1.2.0/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-1.2.0/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/moveToActive-10.lua` & `bullmq-1.2.0/bullmq/commands/moveToActive-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/moveToDelayed-8.lua` & `bullmq-1.2.0/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/moveToFinished-13.lua` & `bullmq-1.2.0/bullmq/commands/moveToFinished-13.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-1.2.0/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/obliterate-2.lua` & `bullmq-1.2.0/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/pause-5.lua` & `bullmq-1.2.0/bullmq/commands/pause-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/promote-7.lua` & `bullmq-1.2.0/bullmq/commands/promote-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/removeJob-1.lua` & `bullmq-1.2.0/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/removeRepeatable-2.lua` & `bullmq-1.2.0/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/reprocessJob-6.lua` & `bullmq-1.2.0/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/retryJob-9.lua` & `bullmq-1.2.0/bullmq/commands/retryJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/commands/retryJobs-6.lua` & `bullmq-1.2.0/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/event_emitter.py` & `bullmq-1.2.0/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/job.py` & `bullmq-1.2.0/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/queue.py` & `bullmq-1.2.0/bullmq/queue.py`

 * *Files 10% similar despite different names*

```diff
@@ -122,14 +122,35 @@
         responses = await self.scripts.getCounts(current_types)
         counts = {}
 
         for index, val in enumerate(responses):
             counts[current_types[index]] = val or 0
         return counts
 
+    def getActive(self, start = 0, end=-1):
+        return self.getJobs(['active'], start, end, True)
+
+    def getCompleted(self, start = 0, end=-1):
+        return self.getJobs(['completed'], start, end, False)
+
+    def getDelayed(self, start = 0, end=-1):
+        return self.getJobs(['delayed'], start, end, True)
+
+    def getFailed(self, start = 0, end=-1):
+        return self.getJobs(['completed'], start, end, False)
+
+    def getPrioritized(self, start = 0, end=-1):
+        return self.getJobs(['prioritized'], start, end, True)
+
+    def getWaiting(self, start = 0, end=-1):
+        return self.getJobs(['waiting'], start, end, True)
+
+    def getWaitingChildren(self, start = 0, end=-1):
+        return self.getJobs(['waiting-children'], start, end, True)
+
     async def getJobs(self, types, start=0, end=-1, asc:bool=False):
         current_types = self.sanitizeJobTypes(types)
         job_ids = await self.scripts.getRanges(current_types, start, end, asc)
         tasks = [asyncio.create_task(Job.fromId(self, i)) for i in job_ids]   
         job_set, _ = await asyncio.wait(tasks, return_when=asyncio.ALL_COMPLETED)
         jobs = [extract_result(job_task) for job_task in job_set]
         jobs_len = len(jobs)
@@ -141,14 +162,15 @@
             pivot_job = jobs[index]
 
             for i in range(index,jobs_len):
                 current_job = jobs[i]
                 if current_job and current_job.id == job_id:
                     jobs[index] = current_job
                     jobs[i] = pivot_job
+                    continue
 
         return jobs
 
     def sanitizeJobTypes(self, types):
         current_types = list(types)
 
         if len(types) > 0:
```

### Comparing `bullmq-1.1.0/bullmq/redis_connection.py` & `bullmq-1.2.0/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/scripts.py` & `bullmq-1.2.0/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/timer.py` & `bullmq-1.2.0/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/types/job_options.py` & `bullmq-1.2.0/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/types/worker_options.py` & `bullmq-1.2.0/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq/worker.py` & `bullmq-1.2.0/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/bullmq.egg-info/PKG-INFO` & `bullmq-1.2.0/bullmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.1.0
+Version: 1.2.0
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.1.0/bullmq.egg-info/SOURCES.txt` & `bullmq-1.2.0/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-1.1.0/setup.py` & `bullmq-1.2.0/setup.py`

 * *Files identical despite different names*

