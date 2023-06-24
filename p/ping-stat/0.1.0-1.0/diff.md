# Comparing `tmp/ping_stat-0.1.0.tar.gz` & `tmp/ping_stat-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ping_stat-0.1.0.tar", max compression
+gzip compressed data, was "ping_stat-1.0.tar", max compression
```

## Comparing `ping_stat-0.1.0.tar` & `ping_stat-1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1544 2023-06-22 16:48:49.808440 ping_stat-0.1.0/ping_stat/__about__.py
--rw-r--r--   0        0        0     1037 2023-06-22 16:48:49.815008 ping_stat-0.1.0/ping_stat/__init__.py
--rw-r--r--   0        0        0     1278 2023-06-22 16:48:49.729175 ping_stat-0.1.0/ping_stat/config/__init__.py
--rw-r--r--   0        0        0      326 2023-04-02 08:42:22.092769 ping_stat-0.1.0/ping_stat/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      352 2023-06-01 04:46:00.553303 ping_stat-0.1.0/ping_stat/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      324 2023-02-23 16:32:27.461202 ping_stat-0.1.0/ping_stat/config/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2301 2023-06-15 05:30:30.703332 ping_stat-0.1.0/ping_stat/config/__pycache__/arguments.cpython-310.pyc
--rw-r--r--   0        0        0     3463 2023-06-01 04:46:00.555305 ping_stat-0.1.0/ping_stat/config/__pycache__/arguments.cpython-311.pyc
--rw-r--r--   0        0        0     2297 2023-02-27 09:50:04.201840 ping_stat-0.1.0/ping_stat/config/__pycache__/arguments.cpython-39.pyc
--rw-r--r--   0        0        0     4112 2023-06-22 16:48:49.777274 ping_stat-0.1.0/ping_stat/config/arguments.py
--rw-r--r--   0        0        0     3160 2023-06-22 16:48:49.763246 ping_stat-0.1.0/ping_stat/errors/__init__.py
--rw-r--r--   0        0        0     2358 2023-06-15 19:03:47.561769 ping_stat-0.1.0/ping_stat/errors/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3629 2023-06-02 05:08:20.217606 ping_stat-0.1.0/ping_stat/errors/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2778 2023-06-15 19:03:47.577465 ping_stat-0.1.0/ping_stat/errors/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     3545 2023-06-02 05:08:20.235604 ping_stat-0.1.0/ping_stat/errors/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     4137 2023-06-22 16:48:49.787878 ping_stat-0.1.0/ping_stat/errors/utils.py
--rw-r--r--   0        0        0     1930 2023-06-22 16:48:49.803907 ping_stat-0.1.0/ping_stat/logging/__init__.py
--rw-r--r--   0        0        0      892 2023-04-02 08:42:22.090773 ping_stat-0.1.0/ping_stat/logging/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1360 2023-06-01 04:46:00.551307 ping_stat-0.1.0/ping_stat/logging/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      890 2023-04-02 08:14:15.270788 ping_stat-0.1.0/ping_stat/logging/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      180 2023-03-14 19:26:03.082000 ping_stat-0.1.0/ping_stat/logging/foo.log
--rw-r--r--   0        0        0     1277 2023-06-22 16:48:49.792876 ping_stat-0.1.0/ping_stat/models/__init__.py
--rw-r--r--   0        0        0      351 2023-06-02 05:06:45.827767 ping_stat-0.1.0/ping_stat/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1281 2023-06-22 16:48:49.782281 ping_stat-0.1.0/ping_stat/models/gui/__init__.py
--rw-r--r--   0        0        0      359 2023-06-02 05:06:45.829767 ping_stat-0.1.0/ping_stat/models/gui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3278 2023-06-22 16:48:49.747722 ping_stat-0.1.0/ping_stat/models/gui/windows/__init__.py
--rw-r--r--   0        0        0     4074 2023-06-02 05:06:45.833767 ping_stat-0.1.0/ping_stat/models/gui/windows/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1682 2023-06-02 05:12:15.437344 ping_stat-0.1.0/ping_stat/models/gui/windows/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0     1877 2023-06-22 16:48:49.766626 ping_stat-0.1.0/ping_stat/models/gui/windows/errors.py
--rw-r--r--   0        0        0   246779 2023-04-02 08:45:40.170572 ping_stat-0.1.0/ping_stat/public_suffix_list.dat
--rw-r--r--   0        0        0     6837 2023-06-22 16:48:49.757245 ping_stat-0.1.0/ping_stat/utils/__init__.py
--rw-r--r--   0        0        0     6098 2023-06-15 19:03:47.506569 ping_stat-0.1.0/ping_stat/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    10547 2023-06-01 11:40:10.456269 ping_stat-0.1.0/ping_stat/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5093 2023-04-02 08:25:16.381419 ping_stat-0.1.0/ping_stat/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      935 2023-05-09 21:39:30.727683 ping_stat-0.1.0/ping_stat/utils/__pycache__/decorators.cpython-310.pyc
--rw-r--r--   0        0        0     1475 2023-06-01 04:46:02.369903 ping_stat-0.1.0/ping_stat/utils/__pycache__/decorators.cpython-311.pyc
--rw-r--r--   0        0        0      931 2023-02-27 10:40:31.335441 ping_stat-0.1.0/ping_stat/utils/__pycache__/decorators.cpython-39.pyc
--rw-r--r--   0        0        0     2649 2023-05-10 01:37:31.804216 ping_stat-0.1.0/ping_stat/utils/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0    12036 2023-06-15 20:24:34.010801 ping_stat-0.1.0/ping_stat/utils/__pycache__/network.cpython-310.pyc
--rw-r--r--   0        0        0    17527 2023-06-01 11:02:53.798848 ping_stat-0.1.0/ping_stat/utils/__pycache__/network.cpython-311.pyc
--rw-r--r--   0        0        0     1854 2023-06-22 16:48:49.819964 ping_stat-0.1.0/ping_stat/utils/decorators.py
--rw-r--r--   0        0        0     3544 2023-06-22 16:48:49.772142 ping_stat-0.1.0/ping_stat/utils/helpers.py
--rw-r--r--   0        0        0    15417 2023-06-22 16:48:49.798389 ping_stat-0.1.0/ping_stat/utils/network.py
--rw-r--r--   0        0        0   246779 2023-04-02 08:25:16.111400 ping_stat-0.1.0/ping_stat/utils/public_suffix_list.dat
--rw-r--r--   0        0        0     8248 2023-06-22 16:48:49.734174 ping_stat-0.1.0/ping_stat/utils/workers/__init__.py
--rw-r--r--   0        0        0     7409 2023-06-15 20:13:57.392927 ping_stat-0.1.0/ping_stat/utils/workers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    12364 2023-06-01 13:12:40.618319 ping_stat-0.1.0/ping_stat/utils/workers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2269 2023-06-22 16:48:49.740201 ping_stat-0.1.0/ping_stat/utils/workers/gui.py
--rw-r--r--   0        0        0      604 2023-06-22 16:47:14.503418 ping_stat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 ping_stat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1587 2023-06-23 23:16:57.458552 ping_stat-1.0/ping_stat/__about__.py
+-rw-r--r--   0        0        0       67 2023-06-22 19:22:53.439672 ping_stat-1.0/ping_stat/__constants__.py
+-rw-r--r--   0        0        0     1077 2023-06-22 17:51:09.767348 ping_stat-1.0/ping_stat/__init__.py
+-rw-r--r--   0        0        0     1278 2023-06-22 16:48:49.729175 ping_stat-1.0/ping_stat/config/__init__.py
+-rw-r--r--   0        0        0      326 2023-04-02 08:42:22.092769 ping_stat-1.0/ping_stat/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      352 2023-06-22 17:49:38.330695 ping_stat-1.0/ping_stat/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      324 2023-02-23 16:32:27.461202 ping_stat-1.0/ping_stat/config/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2301 2023-06-15 05:30:30.703332 ping_stat-1.0/ping_stat/config/__pycache__/arguments.cpython-310.pyc
+-rw-r--r--   0        0        0     3463 2023-06-22 17:49:38.335138 ping_stat-1.0/ping_stat/config/__pycache__/arguments.cpython-311.pyc
+-rw-r--r--   0        0        0     2297 2023-02-27 09:50:04.201840 ping_stat-1.0/ping_stat/config/__pycache__/arguments.cpython-39.pyc
+-rw-r--r--   0        0        0     4112 2023-06-22 16:48:49.777274 ping_stat-1.0/ping_stat/config/arguments.py
+-rw-r--r--   0        0        0     3160 2023-06-22 16:48:49.763246 ping_stat-1.0/ping_stat/errors/__init__.py
+-rw-r--r--   0        0        0     2358 2023-06-15 19:03:47.561769 ping_stat-1.0/ping_stat/errors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3629 2023-06-22 17:49:38.560869 ping_stat-1.0/ping_stat/errors/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2778 2023-06-15 19:03:47.577465 ping_stat-1.0/ping_stat/errors/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     3545 2023-06-22 17:49:38.564776 ping_stat-1.0/ping_stat/errors/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     4137 2023-06-22 16:48:49.787878 ping_stat-1.0/ping_stat/errors/utils.py
+-rw-r--r--   0        0        0     1930 2023-06-22 16:48:49.803907 ping_stat-1.0/ping_stat/logging/__init__.py
+-rw-r--r--   0        0        0      892 2023-04-02 08:42:22.090773 ping_stat-1.0/ping_stat/logging/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1360 2023-06-22 17:49:38.327765 ping_stat-1.0/ping_stat/logging/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      890 2023-04-02 08:14:15.270788 ping_stat-1.0/ping_stat/logging/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1041 2023-06-24 00:53:44.468144 ping_stat-1.0/ping_stat/main.py
+-rw-r--r--   0        0        0     1277 2023-06-22 16:48:49.792876 ping_stat-1.0/ping_stat/models/__init__.py
+-rw-r--r--   0        0        0      351 2023-06-02 05:06:45.827767 ping_stat-1.0/ping_stat/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1281 2023-06-22 16:48:49.782281 ping_stat-1.0/ping_stat/models/gui/__init__.py
+-rw-r--r--   0        0        0      359 2023-06-02 05:06:45.829767 ping_stat-1.0/ping_stat/models/gui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3278 2023-06-22 16:48:49.747722 ping_stat-1.0/ping_stat/models/gui/windows/__init__.py
+-rw-r--r--   0        0        0     4074 2023-06-02 05:06:45.833767 ping_stat-1.0/ping_stat/models/gui/windows/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1682 2023-06-02 05:12:15.437344 ping_stat-1.0/ping_stat/models/gui/windows/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     1877 2023-06-22 16:48:49.766626 ping_stat-1.0/ping_stat/models/gui/windows/errors.py
+-rw-r--r--   0        0        0     6837 2023-06-22 16:48:49.757245 ping_stat-1.0/ping_stat/utils/__init__.py
+-rw-r--r--   0        0        0     6098 2023-06-15 19:03:47.506569 ping_stat-1.0/ping_stat/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    10547 2023-06-22 17:49:38.508402 ping_stat-1.0/ping_stat/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5093 2023-04-02 08:25:16.381419 ping_stat-1.0/ping_stat/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      935 2023-05-09 21:39:30.727683 ping_stat-1.0/ping_stat/utils/__pycache__/decorators.cpython-310.pyc
+-rw-r--r--   0        0        0     1475 2023-06-22 17:49:38.513230 ping_stat-1.0/ping_stat/utils/__pycache__/decorators.cpython-311.pyc
+-rw-r--r--   0        0        0      931 2023-02-27 10:40:31.335441 ping_stat-1.0/ping_stat/utils/__pycache__/decorators.cpython-39.pyc
+-rw-r--r--   0        0        0     2649 2023-05-10 01:37:31.804216 ping_stat-1.0/ping_stat/utils/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0    12036 2023-06-15 20:24:34.010801 ping_stat-1.0/ping_stat/utils/__pycache__/network.cpython-310.pyc
+-rw-r--r--   0        0        0    20217 2023-06-23 22:45:53.082052 ping_stat-1.0/ping_stat/utils/__pycache__/network.cpython-311.pyc
+-rw-r--r--   0        0        0     1854 2023-06-22 16:48:49.819964 ping_stat-1.0/ping_stat/utils/decorators.py
+-rw-r--r--   0        0        0     3544 2023-06-22 16:48:49.772142 ping_stat-1.0/ping_stat/utils/helpers.py
+-rw-r--r--   0        0        0    15639 2023-06-23 08:44:14.162470 ping_stat-1.0/ping_stat/utils/network.py
+-rw-r--r--   0        0        0     8249 2023-06-22 19:24:29.126372 ping_stat-1.0/ping_stat/utils/workers/__init__.py
+-rw-r--r--   0        0        0     7409 2023-06-15 20:13:57.392927 ping_stat-1.0/ping_stat/utils/workers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12391 2023-06-22 19:24:30.202468 ping_stat-1.0/ping_stat/utils/workers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2269 2023-06-22 16:48:49.740201 ping_stat-1.0/ping_stat/utils/workers/gui.py
+-rw-r--r--   0        0        0     1465 2023-06-23 23:16:57.468943 ping_stat-1.0/pyproject.toml
+-rw-r--r--   0        0        0      519 2023-06-01 04:20:15.471933 ping_stat-1.0/README.md
+-rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 ping_stat-1.0/PKG-INFO
```

### Comparing `ping_stat-0.1.0/ping_stat/__about__.py` & `ping_stat-1.0/ping_stat/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 Project: PingPing
 Author: Inspyre Softworks - https://inspyre.techCreated: 2/23/2023 @ 9:09 AM
 File:
   Name: __about__
   Filepath: ping_stat
 """
 
+__AUTHOR__ = 'Inspyre Softworks'
+
 __PROG__ = 'PingPing'
 
 __DESCRIPTION__ = f'{__PROG__} is a simple ping-time monitoring service that can assist in monitoring for and ' \
                   f'documenting outages from your ISP.'
 
-__VERSION__ = '0.1.0_dev1'
+__VERSION__ = '1.0'
 
-__VERSION_FULL__ = f'{__PROG__} v{__VERSION__}'
+__VERSION_FULL__ = f'{__PROG__} v{__VERSION__} by {__AUTHOR__}'
 
 
 
 
 
 """
 The MIT License (MIT)
```

### Comparing `ping_stat-0.1.0/ping_stat/__init__.py` & `ping_stat-1.0/ping_stat/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from datetime import datetime
 from pypattyrn.behavioral.null import Null
 
 from rich.console import Console
 from ping_stat.logging import LOG_DEVICE
 from ping_stat.utils.workers import PingWorker
-
+from ping_stat.utils.network import Ping
 
 console = Console()
 
 
 
 
 # def ping_monitor(ping_object):
```

### Comparing `ping_stat-0.1.0/ping_stat/config/__init__.py` & `ping_stat-1.0/ping_stat/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/config/__pycache__/arguments.cpython-310.pyc` & `ping_stat-1.0/ping_stat/config/__pycache__/arguments.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/config/__pycache__/arguments.cpython-311.pyc` & `ping_stat-1.0/ping_stat/config/__pycache__/arguments.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,24 +1,24 @@
 magic:    0xa70d0d0a
-moddate:  0xe96cfc63 (Mon Feb 27 08:42:17 2023 UTC)
+moddate:  0x717b9464 (Thu Jun 22 16:48:49 2023 UTC)
 files sz: 4112
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a0501
       00640164046c066d075a086d095a0a6d0b5a0c0100020047006405840064
       066502a6030000ab0300000000000000005a0d0200650da6000000ab0000
       000000000000005a0e650ea00f0000000000000000000000000000000000
       000000a6000000ab0000000000000000005a1064075300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.tech\nCreated: 2/23/2023 @ 9:08 AM\nFile:\n  Name: arguments\n  Filepath: ping_ping/config\n')
+     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.tech\nCreated: 2/23/2023 @ 9:08 AM\nFile:\n  Name: arguments\n  Filepath: ping_stat/config\n')
                  4 STORE_NAME               0 (__doc__)
    
      9           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('ArgumentParser',))
                 10 IMPORT_NAME              1 (argparse)
                 12 IMPORT_FROM              2 (ArgumentParser)
                 14 STORE_NAME               2 (ArgumentParser)
@@ -29,26 +29,26 @@
                 22 IMPORT_NAME              3 (inspy_logger)
                 24 IMPORT_FROM              4 (LEVELS)
                 26 STORE_NAME               5 (LOG_LEVELS)
                 28 POP_TOP
    
     11          30 LOAD_CONST               1 (0)
                 32 LOAD_CONST               4 (('__PROG__', '__DESCRIPTION__', '__VERSION_FULL__'))
-                34 IMPORT_NAME              6 (ping_ping.__about__)
+                34 IMPORT_NAME              6 (ping_stat.__about__)
                 36 IMPORT_FROM              7 (__PROG__)
                 38 STORE_NAME               8 (PROG_NAME)
                 40 IMPORT_FROM              9 (__DESCRIPTION__)
                 42 STORE_NAME              10 (DESCRIPTION)
                 44 IMPORT_FROM             11 (__VERSION_FULL__)
                 46 STORE_NAME              12 (VERSION)
                 48 POP_TOP
    
     14          50 PUSH_NULL
                 52 LOAD_BUILD_CLASS
-                54 LOAD_CONST               5 (<code object PingPingArguments, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\config\arguments.py", line 14>)
+                54 LOAD_CONST               5 (<code object PingPingArguments, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\config\arguments.py", line 14>)
                 56 MAKE_FUNCTION            0
                 58 LOAD_CONST               6 ('PingPingArguments')
                 60 LOAD_NAME                2 (ArgumentParser)
                 62 PRECALL                  3
                 66 CALL                     3
                 76 STORE_NAME              13 (PingPingArguments)
    
@@ -63,15 +63,15 @@
                122 PRECALL                  0
                126 CALL                     0
                136 STORE_NAME              16 (ARGUMENTS)
    
    109         138 LOAD_CONST               7 (None)
                140 RETURN_VALUE
    consts
-      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.tech\nCreated: 2/23/2023 @ 9:08 AM\nFile:\n  Name: arguments\n  Filepath: ping_ping/config\n'
+      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.tech\nCreated: 2/23/2023 @ 9:08 AM\nFile:\n  Name: arguments\n  Filepath: ping_stat/config\n'
       0
       ('ArgumentParser',)
       ('LEVELS',)
       ('__PROG__', '__DESCRIPTION__', '__VERSION_FULL__')
       code
          argcount  : 0
          nlocals   : 0
@@ -86,15 +86,15 @@
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('PingPingArguments')
                       10 STORE_NAME               2 (__qualname__)
          
           15          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\config\arguments.py", line 15>)
+                      16 LOAD_CONST               1 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\config\arguments.py", line 15>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
                       22 LOAD_CLOSURE             0 (__class__)
                       24 COPY                     1
                       26 STORE_NAME               4 (__classcell__)
                       28 RETURN_VALUE
          consts
@@ -385,34 +385,34 @@
                   'Monitor your ping-time against the specified host server.'
                   'The time between ping requests'
                   2
                names      ('super', 'PingPingArguments', '__init__', 'PROG_NAME', 'prog', 'DESCRIPTION', 'description', 'add_argument', 'LOG_LEVELS', 'int', 'str', 'add_subparsers', 'ArgumentParser', 'add_parser')
                varnames   ('self', 'args', 'kwargs', 'sub_parsers', 'ttl_test_parser', 'monitor_parser')
                freevars   ('__class__',)
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\config\\arguments.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\config\\arguments.py'
                name       '__init__'
                firstlineno 15
                lnotab
                   0x040140021801180218010201020102010c010201020102f9120a180102
                   010201020102010c01020102f9120a18010201020102010c01020102fa12
                   0918010201020102010c01020102fa120a180102010c0102fd120630010e
                   02180102010201020102010c01020102f9120a180102010201020102010c
                   01020102f9120a2a010e02180102010201020102010c01020102f9
          names      ('__name__', '__module__', '__qualname__', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\config\\arguments.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\config\\arguments.py'
          name       'PingPingArguments'
          firstlineno 14
          lnotab 0x0c01
       'PingPingArguments'
       None
-   names      ('__doc__', 'argparse', 'ArgumentParser', 'inspy_logger', 'LEVELS', 'LOG_LEVELS', 'ping_ping.__about__', '__PROG__', 'PROG_NAME', '__DESCRIPTION__', 'DESCRIPTION', '__VERSION_FULL__', 'VERSION', 'PingPingArguments', 'args', 'parse_args', 'ARGUMENTS')
+   names      ('__doc__', 'argparse', 'ArgumentParser', 'inspy_logger', 'LEVELS', 'LOG_LEVELS', 'ping_stat.__about__', '__PROG__', 'PROG_NAME', '__DESCRIPTION__', 'DESCRIPTION', '__VERSION_FULL__', 'VERSION', 'PingPingArguments', 'args', 'parse_args', 'ARGUMENTS')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\config\\arguments.py'
+   filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\config\\arguments.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104080c010c0114031c5a14012804
```

### Comparing `ping_stat-0.1.0/ping_stat/config/__pycache__/arguments.cpython-39.pyc` & `ping_stat-1.0/ping_stat/config/__pycache__/arguments.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/config/arguments.py` & `ping_stat-1.0/ping_stat/config/arguments.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/errors/__init__.py` & `ping_stat-1.0/ping_stat/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/errors/__pycache__/__init__.cpython-310.pyc` & `ping_stat-1.0/ping_stat/errors/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/errors/__pycache__/__init__.cpython-311.pyc` & `ping_stat-1.0/ping_stat/errors/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc4787964 (Fri Jun  2 05:06:12 2023 UTC)
+moddate:  0x717b9464 (Thu Jun 22 16:48:49 2023 UTC)
 files sz: 3160
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -11,76 +11,76 @@
       065a060100020047006403840064046507a6030000ab0300000000000000
       005a08020047006405840064066508a6030000ab0300000000000000005a
       09020047006407840064086508a6030000ab0300000000000000005a0a02
       00470064098400640a6508a6030000ab0300000000000000005a0b640b53
       00
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 5/9/2023 @ 9:00 PM\nFile:\n  Name: errors\n  Filepath: ping_ping\n')
+     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 5/9/2023 @ 9:00 PM\nFile:\n  Name: errors\n  Filepath: ping_stat\n')
                  4 STORE_NAME               0 (__doc__)
    
      8           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('get_caller_module_name', 'get_caller_filename', 'get_caller_line_number', 'get_caller_function_name', 'get_caller_class_name'))
-                10 IMPORT_NAME              1 (ping_ping.errors.utils)
+                10 IMPORT_NAME              1 (ping_stat.errors.utils)
                 12 IMPORT_FROM              2 (get_caller_module_name)
                 14 STORE_NAME               2 (get_caller_module_name)
                 16 IMPORT_FROM              3 (get_caller_filename)
                 18 STORE_NAME               3 (get_caller_filename)
                 20 IMPORT_FROM              4 (get_caller_line_number)
                 22 STORE_NAME               4 (get_caller_line_number)
                 24 IMPORT_FROM              5 (get_caller_function_name)
                 26 STORE_NAME               5 (get_caller_function_name)
                 28 IMPORT_FROM              6 (get_caller_class_name)
                 30 STORE_NAME               6 (get_caller_class_name)
                 32 POP_TOP
    
     15          34 PUSH_NULL
                 36 LOAD_BUILD_CLASS
-                38 LOAD_CONST               3 (<code object PingPingError, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\__init__.py", line 15>)
+                38 LOAD_CONST               3 (<code object PingPingError, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\__init__.py", line 15>)
                 40 MAKE_FUNCTION            0
                 42 LOAD_CONST               4 ('PingPingError')
                 44 LOAD_NAME                7 (Exception)
                 46 PRECALL                  3
                 50 CALL                     3
                 60 STORE_NAME               8 (PingPingError)
    
     26          62 PUSH_NULL
                 64 LOAD_BUILD_CLASS
-                66 LOAD_CONST               5 (<code object RedundantWorkOrderError, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\__init__.py", line 26>)
+                66 LOAD_CONST               5 (<code object RedundantWorkOrderError, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\__init__.py", line 26>)
                 68 MAKE_FUNCTION            0
                 70 LOAD_CONST               6 ('RedundantWorkOrderError')
                 72 LOAD_NAME                8 (PingPingError)
                 74 PRECALL                  3
                 78 CALL                     3
                 88 STORE_NAME               9 (RedundantWorkOrderError)
    
     36          90 PUSH_NULL
                 92 LOAD_BUILD_CLASS
-                94 LOAD_CONST               7 (<code object WorkerAlreadyStartedError, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\__init__.py", line 36>)
+                94 LOAD_CONST               7 (<code object WorkerAlreadyStartedError, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\__init__.py", line 36>)
                 96 MAKE_FUNCTION            0
                 98 LOAD_CONST               8 ('WorkerAlreadyStartedError')
                100 LOAD_NAME                8 (PingPingError)
                102 PRECALL                  3
                106 CALL                     3
                116 STORE_NAME              10 (WorkerAlreadyStartedError)
    
     46         118 PUSH_NULL
                120 LOAD_BUILD_CLASS
-               122 LOAD_CONST               9 (<code object WorkerNotStartedError, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\__init__.py", line 46>)
+               122 LOAD_CONST               9 (<code object WorkerNotStartedError, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\__init__.py", line 46>)
                124 MAKE_FUNCTION            0
                126 LOAD_CONST              10 ('WorkerNotStartedError')
                128 LOAD_NAME                8 (PingPingError)
                130 PRECALL                  3
                134 CALL                     3
                144 STORE_NAME              11 (WorkerNotStartedError)
    
     58         146 LOAD_CONST              11 (None)
                148 RETURN_VALUE
    consts
-      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 5/9/2023 @ 9:00 PM\nFile:\n  Name: errors\n  Filepath: ping_ping\n'
+      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 5/9/2023 @ 9:00 PM\nFile:\n  Name: errors\n  Filepath: ping_stat\n'
       0
       ('get_caller_module_name', 'get_caller_filename', 'get_caller_line_number', 'get_caller_function_name', 'get_caller_class_name')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
@@ -100,15 +100,15 @@
          
           18          16 LOAD_CONST               5 ((None,))
                       18 LOAD_CONST               3 ('message')
                       20 LOAD_NAME                4 (str)
                       22 BUILD_TUPLE              2
                       24 LOAD_CLOSURE             0 (__class__)
                       26 BUILD_TUPLE              1
-                      28 LOAD_CONST               4 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\__init__.py", line 18>)
+                      28 LOAD_CONST               4 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\__init__.py", line 18>)
                       30 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       32 STORE_NAME               5 (__init__)
                       34 LOAD_CLOSURE             0 (__class__)
                       36 COPY                     1
                       38 STORE_NAME               6 (__classcell__)
                       40 RETURN_VALUE
          consts
@@ -162,24 +162,24 @@
                   'PingPingGUIError'
                   'An error occurred in the PingPing GUI'
                   'An error occurred in the PingPing program'
                names      ('get_caller_class_name', 'super', '__init__')
                varnames   ('self', 'message')
                freevars   ('__class__',)
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\__init__.py'
                name       '__init__'
                firstlineno 18
                lnotab 0x04012401040104010401
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\__init__.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\__init__.py'
          name       'PingPingError'
          firstlineno 15
          lnotab 0x0c010402
       'PingPingError'
       code
          argcount  : 0
          nlocals   : 0
@@ -203,15 +203,15 @@
                       18 LOAD_CONST               3 ('worker_name')
                       20 LOAD_NAME                4 (str)
                       22 LOAD_CONST               4 ('message')
                       24 LOAD_NAME                4 (str)
                       26 BUILD_TUPLE              4
                       28 LOAD_CLOSURE             0 (__class__)
                       30 BUILD_TUPLE              1
-                      32 LOAD_CONST               5 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\__init__.py", line 29>)
+                      32 LOAD_CONST               5 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\__init__.py", line 29>)
                       34 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       36 STORE_NAME               5 (__init__)
                       38 LOAD_CLOSURE             0 (__class__)
                       40 COPY                     1
                       42 STORE_NAME               6 (__classcell__)
                       44 RETURN_VALUE
          consts
@@ -265,24 +265,24 @@
                   None
                   'The specified worker already exists: '
                   '. '
                names      ('super', '__init__')
                varnames   ('self', 'worker_name', 'message', 'default_message')
                freevars   ('__class__',)
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\__init__.py'
                name       '__init__'
                firstlineno 29
                lnotab 0x04010a0104011001
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\__init__.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\__init__.py'
          name       'RedundantWorkOrderError'
          firstlineno 26
          lnotab 0x0c010402
       'RedundantWorkOrderError'
       code
          argcount  : 0
          nlocals   : 0
@@ -306,15 +306,15 @@
                       18 LOAD_CONST               3 ('worker_name')
                       20 LOAD_NAME                4 (str)
                       22 LOAD_CONST               4 ('message')
                       24 LOAD_NAME                4 (str)
                       26 BUILD_TUPLE              4
                       28 LOAD_CLOSURE             0 (__class__)
                       30 BUILD_TUPLE              1
-                      32 LOAD_CONST               5 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\__init__.py", line 39>)
+                      32 LOAD_CONST               5 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\__init__.py", line 39>)
                       34 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       36 STORE_NAME               5 (__init__)
                       38 LOAD_CLOSURE             0 (__class__)
                       40 COPY                     1
                       42 STORE_NAME               6 (__classcell__)
                       44 RETURN_VALUE
          consts
@@ -368,24 +368,24 @@
                   None
                   'The specified worker is already running: '
                   '. '
                names      ('super', '__init__')
                varnames   ('self', 'worker_name', 'message', 'default_message')
                freevars   ('__class__',)
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\__init__.py'
                name       '__init__'
                firstlineno 39
                lnotab 0x04010a0104011001
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\__init__.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\__init__.py'
          name       'WorkerAlreadyStartedError'
          firstlineno 36
          lnotab 0x0c010402
       'WorkerAlreadyStartedError'
       code
          argcount  : 0
          nlocals   : 0
@@ -409,15 +409,15 @@
                       18 LOAD_CONST               3 ('worker_name')
                       20 LOAD_NAME                4 (str)
                       22 LOAD_CONST               4 ('message')
                       24 LOAD_NAME                4 (str)
                       26 BUILD_TUPLE              4
                       28 LOAD_CLOSURE             0 (__class__)
                       30 BUILD_TUPLE              1
-                      32 LOAD_CONST               5 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\__init__.py", line 49>)
+                      32 LOAD_CONST               5 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\__init__.py", line 49>)
                       34 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       36 STORE_NAME               5 (__init__)
                       38 LOAD_CLOSURE             0 (__class__)
                       40 COPY                     1
                       42 STORE_NAME               6 (__classcell__)
                       44 RETURN_VALUE
          consts
@@ -471,30 +471,30 @@
                   None
                   'The specified worker is not running: '
                   '. '
                names      ('super', '__init__')
                varnames   ('self', 'worker_name', 'message', 'default_message')
                freevars   ('__class__',)
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\__init__.py'
                name       '__init__'
                firstlineno 49
                lnotab 0x04010a0104011001
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\__init__.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\__init__.py'
          name       'WorkerNotStartedError'
          firstlineno 46
          lnotab 0x0c010402
       'WorkerNotStartedError'
       None
-   names      ('__doc__', 'ping_ping.errors.utils', 'get_caller_module_name', 'get_caller_filename', 'get_caller_line_number', 'get_caller_function_name', 'get_caller_class_name', 'Exception', 'PingPingError', 'RedundantWorkOrderError', 'WorkerAlreadyStartedError', 'WorkerNotStartedError')
+   names      ('__doc__', 'ping_stat.errors.utils', 'get_caller_module_name', 'get_caller_filename', 'get_caller_line_number', 'get_caller_function_name', 'get_caller_class_name', 'Exception', 'PingPingError', 'RedundantWorkOrderError', 'WorkerAlreadyStartedError', 'WorkerNotStartedError')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\__init__.py'
+   filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104071c071c0b1c0a1c0a1c0c
```

### Comparing `ping_stat-0.1.0/ping_stat/errors/__pycache__/utils.cpython-310.pyc` & `ping_stat-1.0/ping_stat/errors/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/errors/__pycache__/utils.cpython-311.pyc` & `ping_stat-1.0/ping_stat/errors/__pycache__/utils.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,22 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0xed1f7964 (Thu Jun  1 22:47:09 2023 UTC)
+moddate:  0x717b9464 (Thu Jun 22 16:48:49 2023 UTC)
 files sz: 4137
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x970064005a00640164026c015a01640164026c025a0267006403a2015a
       03640484005a04640584005a05640684005a06640784005a07640884005a
       0864025300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 6/1/2023 @ 5:10 PM\nFile:\n  Name: utils\n  Filepath: ping_ping/errors\n')
+     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 6/1/2023 @ 5:10 PM\nFile:\n  Name: utils\n  Filepath: ping_stat/errors\n')
                  4 STORE_NAME               0 (__doc__)
    
      8           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
                 10 IMPORT_NAME              1 (inspect)
                 12 STORE_NAME               1 (inspect)
    
@@ -26,38 +26,38 @@
                 20 STORE_NAME               2 (os)
    
     12          22 BUILD_LIST               0
                 24 LOAD_CONST               3 (('get_caller_class_name', 'get_caller_filename', 'get_caller_function_name', 'get_caller_line_number', 'get_caller_module_name'))
                 26 LIST_EXTEND              1
                 28 STORE_NAME               3 (__all__)
    
-    21          30 LOAD_CONST               4 (<code object get_caller_function_name, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\utils.py", line 21>)
+    21          30 LOAD_CONST               4 (<code object get_caller_function_name, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\utils.py", line 21>)
                 32 MAKE_FUNCTION            0
                 34 STORE_NAME               4 (get_caller_function_name)
    
-    35          36 LOAD_CONST               5 (<code object get_caller_filename, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\utils.py", line 35>)
+    35          36 LOAD_CONST               5 (<code object get_caller_filename, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\utils.py", line 35>)
                 38 MAKE_FUNCTION            0
                 40 STORE_NAME               5 (get_caller_filename)
    
-    48          42 LOAD_CONST               6 (<code object get_caller_line_number, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\utils.py", line 48>)
+    48          42 LOAD_CONST               6 (<code object get_caller_line_number, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\utils.py", line 48>)
                 44 MAKE_FUNCTION            0
                 46 STORE_NAME               6 (get_caller_line_number)
    
-    62          48 LOAD_CONST               7 (<code object get_caller_module_name, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\utils.py", line 62>)
+    62          48 LOAD_CONST               7 (<code object get_caller_module_name, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\utils.py", line 62>)
                 50 MAKE_FUNCTION            0
                 52 STORE_NAME               7 (get_caller_module_name)
    
-    78          54 LOAD_CONST               8 (<code object get_caller_class_name, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\errors\utils.py", line 78>)
+    78          54 LOAD_CONST               8 (<code object get_caller_class_name, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\errors\utils.py", line 78>)
                 56 MAKE_FUNCTION            0
                 58 STORE_NAME               8 (get_caller_class_name)
    
    102          60 LOAD_CONST               2 (None)
                 62 RETURN_VALUE
    consts
-      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 6/1/2023 @ 5:10 PM\nFile:\n  Name: utils\n  Filepath: ping_ping/errors\n'
+      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 6/1/2023 @ 5:10 PM\nFile:\n  Name: utils\n  Filepath: ping_stat/errors\n'
       0
       None
       ('get_caller_class_name', 'get_caller_filename', 'get_caller_function_name', 'get_caller_line_number', 'get_caller_module_name')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
@@ -79,15 +79,15 @@
                       78 RETURN_VALUE
          consts
             '\n    Get the name of the calling function.\n\n    Go two frames back in the stack: one for this function call, and one for the caller.\n    Then, retrieve the name of the compiled function body from the code object.\n\n    Returns:\n        str: The name of the caller function.\n    '
          names      ('inspect', 'currentframe', 'f_back', 'f_code', 'co_name')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\utils.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\utils.py'
          name       'get_caller_function_name'
          firstlineno 21
          lnotab 0x020b
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 2
@@ -114,15 +114,15 @@
          consts
             '\n    Get the filename of the calling function.\n\n    Go two frames back in the stack: one for this function call, and one for the caller.\n\n    Returns:\n        str: The filename of the caller function.\n    '
             '__file__'
          names      ('inspect', 'currentframe', 'f_back', 'f_globals')
          varnames   ('frame',)
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\utils.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\utils.py'
          name       'get_caller_filename'
          firstlineno 35
          lnotab 0x020a3a01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
@@ -143,15 +143,15 @@
                       68 RETURN_VALUE
          consts
             '\n    Get the line number of the calling function.\n\n    Go two frames back in the stack: one for this function call, and one for the caller.\n    Then, retrieve the line number from the frame.\n\n    Returns:\n        int: The line number of the caller function.\n    '
          names      ('inspect', 'currentframe', 'f_back', 'f_lineno')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\utils.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\utils.py'
          name       'get_caller_line_number'
          firstlineno 48
          lnotab 0x020b
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
@@ -189,15 +189,15 @@
          consts
             "\n    Get the module name of the calling function.\n\n    Go two frames back in the stack: one for this function call, and one for the caller.\n    Then, get the module that contains the code of the frame.\n\n    Returns:\n        str: The name of the caller's module, or None if it couldn't be determined.\n    "
             None
          names      ('inspect', 'currentframe', 'f_back', 'getmodule', '__name__')
          varnames   ('frame', 'module')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\utils.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\utils.py'
          name       'get_caller_module_name'
          firstlineno 62
          lnotab 0x020b3a012801
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 4
@@ -257,19 +257,19 @@
             '\n   Get the name of the class of the calling function.\n\n   Go two frames back in the stack: one for this function call, and one for the caller.\n   Then, retrieve the class of the caller function from the frame.\n\n   Returns:\n       str: The name of the class of the caller function, or None if the function is not a method of a class.\n   '
             'self'
             None
          names      ('inspect', 'currentframe', 'f_back', 'getframeinfo', 'function', 'f_locals', 'get', 'hasattr', '__class__', '__name__')
          varnames   ('frame', 'method', 'instance')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\utils.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\utils.py'
          name       'get_caller_class_name'
          firstlineno 78
          lnotab 0x020b3a013201340324021802
    names      ('__doc__', 'inspect', 'os', '__all__', 'get_caller_function_name', 'get_caller_filename', 'get_caller_line_number', 'get_caller_module_name', 'get_caller_class_name')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\errors\\utils.py'
+   filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\errors\\utils.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010407080108030809060e060d060e06100618
```

### Comparing `ping_stat-0.1.0/ping_stat/errors/utils.py` & `ping_stat-1.0/ping_stat/errors/utils.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/logging/__init__.py` & `ping_stat-1.0/ping_stat/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/logging/__pycache__/__init__.cpython-310.pyc` & `ping_stat-1.0/ping_stat/logging/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/logging/__pycache__/__init__.cpython-311.pyc` & `ping_stat-1.0/ping_stat/logging/__pycache__/__init__.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x54392964 (Sun Apr  2 08:14:12 2023 UTC)
+moddate:  0x717b9464 (Thu Jun 22 16:48:49 2023 UTC)
 files sz: 1930
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -14,27 +14,27 @@
       0000000000000000000000a6000000ab0000000000000000005a0f650fa0
       100000000000000000000000000000000000000000640765059b009d02a6
       010000ab0100000000000000000100650fa0100000000000000000000000
       0000000000000000006407650f6a1100000000000000009b009d02a60100
       00ab0100000000000000000100640884005a1264095300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/26/2023 @ 1:34 AM\nFile:\n  Name: __init__.py\n  Filepath: ping_ping/logging\n')
+     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/26/2023 @ 1:34 AM\nFile:\n  Name: __init__.py\n  Filepath: ping_stat/logging\n')
                  4 STORE_NAME               0 (__doc__)
    
      8           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('ARGUMENTS',))
-                10 IMPORT_NAME              1 (ping_ping.config.arguments)
+                10 IMPORT_NAME              1 (ping_stat.config.arguments)
                 12 IMPORT_FROM              2 (ARGUMENTS)
                 14 STORE_NAME               2 (ARGUMENTS)
                 16 POP_TOP
    
      9          18 LOAD_CONST               1 (0)
                 20 LOAD_CONST               3 (('__PROG__',))
-                22 IMPORT_NAME              3 (ping_ping.__about__)
+                22 IMPORT_NAME              3 (ping_stat.__about__)
                 24 IMPORT_FROM              4 (__PROG__)
                 26 STORE_NAME               5 (PROG_NAME)
                 28 POP_TOP
    
     10          30 LOAD_CONST               1 (0)
                 32 LOAD_CONST               4 (('InspyLogger',))
                 34 IMPORT_NAME              6 (inspy_logger)
@@ -88,22 +88,22 @@
                222 LOAD_ATTR               17 (name)
                232 FORMAT_VALUE             0
                234 BUILD_STRING             2
                236 PRECALL                  1
                240 CALL                     1
                250 POP_TOP
    
-    28         252 LOAD_CONST               8 (<code object add_child, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\logging\__init__.py", line 28>)
+    28         252 LOAD_CONST               8 (<code object add_child, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\logging\__init__.py", line 28>)
                254 MAKE_FUNCTION            0
                256 STORE_NAME              18 (add_child)
    
     35         258 LOAD_CONST               9 (None)
                260 RETURN_VALUE
    consts
-      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/26/2023 @ 1:34 AM\nFile:\n  Name: __init__.py\n  Filepath: ping_ping/logging\n'
+      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/26/2023 @ 1:34 AM\nFile:\n  Name: __init__.py\n  Filepath: ping_stat/logging\n'
       0
       ('ARGUMENTS',)
       ('__PROG__',)
       ('InspyLogger',)
       ('RichHandler',)
       'debug'
       'Logger started for '
@@ -142,20 +142,20 @@
          consts
             None
             'Received logger '
          names      ('LOG_DEVICE', 'add_child', 'debug', 'name')
          varnames   ('name', '_')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\logging\\__init__.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\logging\\__init__.py'
          name       'add_child'
          firstlineno 28
          lnotab 0x020134013a02
       None
-   names      ('__doc__', 'ping_ping.config.arguments', 'ARGUMENTS', 'ping_ping.__about__', '__PROG__', 'PROG_NAME', 'inspy_logger', 'InspyLogger', 'rich.logging', 'RichHandler', 'ISL', 'device', 'LOG_DEVICE', 'started', 'start', 'LOGGER', 'debug', 'name', 'add_child')
+   names      ('__doc__', 'ping_stat.config.arguments', 'ARGUMENTS', 'ping_stat.__about__', '__PROG__', 'PROG_NAME', 'inspy_logger', 'InspyLogger', 'rich.logging', 'RichHandler', 'ISL', 'device', 'LOG_DEVICE', 'started', 'start', 'LOGGER', 'debug', 'name', 'add_child')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\logging\\__init__.py'
+   filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\logging\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104070c010c010c010c0418020e020e02280130033a030607
```

### Comparing `ping_stat-0.1.0/ping_stat/logging/__pycache__/__init__.cpython-39.pyc` & `ping_stat-1.0/ping_stat/logging/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/models/__init__.py` & `ping_stat-1.0/ping_stat/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/models/gui/__init__.py` & `ping_stat-1.0/ping_stat/models/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/models/gui/windows/__init__.py` & `ping_stat-1.0/ping_stat/models/gui/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/models/gui/windows/__pycache__/__init__.cpython-311.pyc` & `ping_stat-1.0/ping_stat/models/gui/windows/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/models/gui/windows/__pycache__/errors.cpython-311.pyc` & `ping_stat-1.0/ping_stat/models/gui/windows/__pycache__/errors.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/models/gui/windows/errors.py` & `ping_stat-1.0/ping_stat/models/gui/windows/errors.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/__init__.py` & `ping_stat-1.0/ping_stat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/__pycache__/__init__.cpython-310.pyc` & `ping_stat-1.0/ping_stat/utils/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/__pycache__/__init__.cpython-311.pyc` & `ping_stat-1.0/ping_stat/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x82837864 (Thu Jun  1 11:39:46 2023 UTC)
+moddate:  0x717b9464 (Thu Jun 22 16:48:49 2023 UTC)
 files sz: 6837
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -15,15 +15,15 @@
       00000000005a136513a01800000000000000000000000000000000000000
       00640a65136a1900000000000000009b009d02a6010000ab010000000000
       0000000100590064035a175b176e0864035a175b17770177007803590077
       01640b84005a1a090009000900090009006411640e84015a1b0200470064
       0f84006410a6020000ab0200000000000000005a1c64035300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/23/2023 @ 9:03 AM\nFile:\n  Name: __init__.py\n  Filepath: ping_ping/utils\n')
+     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/23/2023 @ 9:03 AM\nFile:\n  Name: __init__.py\n  Filepath: ping_stat/utils\n')
                  4 STORE_NAME               0 (__doc__)
    
      8           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('InspyLogger',))
                 10 IMPORT_NAME              1 (inspy_logger)
                 12 IMPORT_FROM              2 (InspyLogger)
                 14 STORE_NAME               2 (InspyLogger)
@@ -41,15 +41,15 @@
                 34 STORE_NAME               5 (ping)
                 36 IMPORT_FROM              6 (verbose_ping)
                 38 STORE_NAME               6 (verbose_ping)
                 40 POP_TOP
    
     11          42 LOAD_CONST               1 (0)
                 44 LOAD_CONST               5 (('add_child', 'PROG_NAME'))
-                46 IMPORT_NAME              7 (ping_ping.logging)
+                46 IMPORT_NAME              7 (ping_stat.logging)
                 48 IMPORT_FROM              8 (add_child)
                 50 STORE_NAME               9 (add_child_logger)
                 52 IMPORT_FROM             10 (PROG_NAME)
                 54 STORE_NAME              10 (PROG_NAME)
                 56 POP_TOP
    
     12          58 LOAD_CONST               1 (0)
@@ -62,15 +62,15 @@
     13          70 LOAD_CONST               1 (0)
                 72 LOAD_CONST               3 (None)
                 74 IMPORT_NAME             13 (inspect)
                 76 STORE_NAME              13 (inspect)
    
     14          78 LOAD_CONST               1 (0)
                 80 LOAD_CONST               7 (('validate_properties',))
-                82 IMPORT_NAME             14 (ping_ping.utils.decorators)
+                82 IMPORT_NAME             14 (ping_stat.utils.decorators)
                 84 IMPORT_FROM             15 (validate_properties)
                 86 STORE_NAME              15 (validate_properties)
                 88 POP_TOP
    
     15          90 LOAD_CONST               1 (0)
                 92 LOAD_CONST               8 (('mean', 'median'))
                 94 IMPORT_NAME             16 (statistics)
@@ -125,51 +125,51 @@
                230 RERAISE                  1
    
     21     >>  232 RERAISE                  0
            >>  234 COPY                     3
                236 POP_EXCEPT
                238 RERAISE                  1
    
-    26     >>  240 LOAD_CONST              11 (<code object get_ping_mean, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 26>)
+    26     >>  240 LOAD_CONST              11 (<code object get_ping_mean, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 26>)
                242 MAKE_FUNCTION            0
                244 STORE_NAME              26 (get_ping_mean)
    
     34         246 NOP
    
     35         248 NOP
    
     36         250 NOP
    
     37         252 NOP
    
     38         254 NOP
    
     32         256 LOAD_CONST              17 ((True, 5, True, True, True))
-               258 LOAD_CONST              14 (<code object gather_times, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 32>)
+               258 LOAD_CONST              14 (<code object gather_times, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 32>)
                260 MAKE_FUNCTION            1 (defaults)
                262 STORE_NAME              27 (gather_times)
    
     75         264 PUSH_NULL
                266 LOAD_BUILD_CLASS
-               268 LOAD_CONST              15 (<code object TTLTest, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 75>)
+               268 LOAD_CONST              15 (<code object TTLTest, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 75>)
                270 MAKE_FUNCTION            0
                272 LOAD_CONST              16 ('TTLTest')
                274 PRECALL                  2
                278 CALL                     2
                288 STORE_NAME              28 (TTLTest)
    
    229         290 LOAD_CONST               3 (None)
                292 RETURN_VALUE
    ExceptionTable:
      108 to 110 -> 114 [0]
      114 to 126 -> 234 [1] lasti
      128 to 212 -> 224 [1] lasti
      224 to 232 -> 234 [1] lasti
    consts
-      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/23/2023 @ 9:03 AM\nFile:\n  Name: __init__.py\n  Filepath: ping_ping/utils\n'
+      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/23/2023 @ 9:03 AM\nFile:\n  Name: __init__.py\n  Filepath: ping_stat/utils\n'
       0
       ('InspyLogger',)
       None
       ('ping', 'verbose_ping')
       ('add_child', 'PROG_NAME')
       ('RichHandler',)
       ('validate_properties',)
@@ -198,15 +198,15 @@
                       26 LOAD_CONST               2 (False)
                       28 BUILD_MAP                1
                       30 LOAD_FAST                2 (kwargs)
                       32 DICT_MERGE               1
                       34 CALL_FUNCTION_EX         1
                       36 STORE_FAST               3 (times)
          
-          28          38 LOAD_CONST               3 (<code object <listcomp>, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 28>)
+          28          38 LOAD_CONST               3 (<code object <listcomp>, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 28>)
                       40 MAKE_FUNCTION            0
                       42 LOAD_FAST                3 (times)
                       44 GET_ITER
                       46 PRECALL                  0
                       50 CALL                     0
                       60 STORE_FAST               4 (p_means)
          
@@ -242,23 +242,23 @@
                             44 JUMP_BACKWARD           20 (to 6)
                        >>   46 RETURN_VALUE
                consts
                names      ('mean',)
                varnames   ('.0', 'p_time')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       '<listcomp>'
                firstlineno 28
                lnotab 0x
          names      ('gather_times', 'mean')
          varnames   ('ping_object', 'args', 'kwargs', 'times', 'p_means')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
          name       'get_ping_mean'
          firstlineno 26
          lnotab 0x020124011801
       True
       5
       code
          argcount  : 6
@@ -444,15 +444,15 @@
             ' failed '
             ()
             0
          names      ('history', 'print', 'len', 'append')
          varnames   ('ping_object', 'count_timeout_time_for_fails', 'timeout', 'return_success_list', 'return_fail_list', 'format_fail_times', 'ping', 'ping_times', 'failed_pings', 'history', 'item', 'noun', 'ret')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
          name       'gather_times'
          firstlineno 32
          lnotab
             0x02080401040104010e014001120210012a0104012c0238020401260106
             01260104024402040104010e0104010e0226011002
       code
          argcount  : 0
@@ -524,216 +524,216 @@
           90          60 LOAD_NAME               12 (_TTLTest__timeout)
          
           91          62 LOAD_NAME               10 (_TTLTest__starting_at)
          
           92          64 LOAD_NAME                6 (_TTLTest__end_at)
          
           85          66 BUILD_TUPLE              6
-                      68 LOAD_CONST               8 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 85>)
+                      68 LOAD_CONST               8 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 85>)
                       70 MAKE_FUNCTION            1 (defaults)
                       72 STORE_NAME              13 (__init__)
          
          104          74 LOAD_NAME               14 (property)
          
          105          76 LOAD_CONST               9 ('return')
                       78 LOAD_NAME                4 (bool)
                       80 BUILD_TUPLE              2
-                      82 LOAD_CONST              10 (<code object auto_run, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 104>)
+                      82 LOAD_CONST              10 (<code object auto_run, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 104>)
                       84 MAKE_FUNCTION            4 (annotations)
          
          104          86 PRECALL                  0
                       90 CALL                     0
          
          105         100 STORE_NAME              15 (auto_run)
          
          108         102 LOAD_NAME               15 (auto_run)
                      104 LOAD_ATTR               16 (setter)
          
          109         114 LOAD_CONST              11 ('new')
                      116 LOAD_NAME                4 (bool)
                      118 BUILD_TUPLE              2
-                     120 LOAD_CONST              12 (<code object auto_run, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 108>)
+                     120 LOAD_CONST              12 (<code object auto_run, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 108>)
                      122 MAKE_FUNCTION            4 (annotations)
          
          108         124 PRECALL                  0
                      128 CALL                     0
          
          109         138 STORE_NAME              15 (auto_run)
          
          112         140 LOAD_NAME               14 (property)
          
-         113         142 LOAD_CONST              13 (<code object iterations, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 112>)
+         113         142 LOAD_CONST              13 (<code object iterations, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 112>)
                      144 MAKE_FUNCTION            0
          
          112         146 PRECALL                  0
                      150 CALL                     0
          
          113         160 STORE_NAME              17 (iterations)
          
          116         162 LOAD_NAME               17 (iterations)
                      164 LOAD_ATTR               16 (setter)
          
-         117         174 LOAD_CONST              14 (<code object iterations, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 116>)
+         117         174 LOAD_CONST              14 (<code object iterations, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 116>)
                      176 MAKE_FUNCTION            0
          
          116         178 PRECALL                  0
                      182 CALL                     0
          
          117         192 STORE_NAME              17 (iterations)
          
          123         194 LOAD_NAME               17 (iterations)
                      196 LOAD_ATTR               18 (deleter)
          
-         124         206 LOAD_CONST              15 (<code object iterations, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 123>)
+         124         206 LOAD_CONST              15 (<code object iterations, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 123>)
                      208 MAKE_FUNCTION            0
          
          123         210 PRECALL                  0
                      214 CALL                     0
          
          124         224 STORE_NAME              17 (iterations)
          
          127         226 LOAD_NAME               14 (property)
          
-         128         228 LOAD_CONST              16 (<code object history, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 127>)
+         128         228 LOAD_CONST              16 (<code object history, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 127>)
                      230 MAKE_FUNCTION            0
          
          127         232 PRECALL                  0
                      236 CALL                     0
          
          128         246 STORE_NAME              19 (history)
          
          131         248 LOAD_NAME               14 (property)
          
-         132         250 LOAD_CONST              17 (<code object timeout, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 131>)
+         132         250 LOAD_CONST              17 (<code object timeout, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 131>)
                      252 MAKE_FUNCTION            0
          
          131         254 PRECALL                  0
                      258 CALL                     0
          
          132         268 STORE_NAME              20 (timeout)
          
          135         270 LOAD_NAME               20 (timeout)
                      272 LOAD_ATTR               16 (setter)
          
-         136         282 LOAD_CONST              18 (<code object timeout, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 135>)
+         136         282 LOAD_CONST              18 (<code object timeout, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 135>)
                      284 MAKE_FUNCTION            0
          
          135         286 PRECALL                  0
                      290 CALL                     0
          
          136         300 STORE_NAME              20 (timeout)
          
          141         302 LOAD_NAME               20 (timeout)
                      304 LOAD_ATTR               18 (deleter)
          
-         142         314 LOAD_CONST              19 (<code object timeout, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 141>)
+         142         314 LOAD_CONST              19 (<code object timeout, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 141>)
                      316 MAKE_FUNCTION            0
          
          141         318 PRECALL                  0
                      322 CALL                     0
          
          142         332 STORE_NAME              20 (timeout)
          
          145         334 LOAD_NAME               14 (property)
          
          146         336 LOAD_CONST               9 ('return')
                      338 LOAD_NAME               21 (str)
                      340 BUILD_TUPLE              2
-                     342 LOAD_CONST              20 (<code object address, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 145>)
+                     342 LOAD_CONST              20 (<code object address, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 145>)
                      344 MAKE_FUNCTION            4 (annotations)
          
          145         346 PRECALL                  0
                      350 CALL                     0
          
          146         360 STORE_NAME              22 (address)
          
          149         362 LOAD_NAME               22 (address)
                      364 LOAD_ATTR               16 (setter)
          
-         150         374 LOAD_CONST              21 (<code object address, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 149>)
+         150         374 LOAD_CONST              21 (<code object address, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 149>)
                      376 MAKE_FUNCTION            0
          
          149         378 PRECALL                  0
                      382 CALL                     0
          
          150         392 STORE_NAME              22 (address)
          
          157         394 LOAD_NAME               22 (address)
                      396 LOAD_ATTR               18 (deleter)
          
-         158         406 LOAD_CONST              22 (<code object address, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 157>)
+         158         406 LOAD_CONST              22 (<code object address, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 157>)
                      408 MAKE_FUNCTION            0
          
          157         410 PRECALL                  0
                      414 CALL                     0
          
          158         424 STORE_NAME              22 (address)
          
          161         426 LOAD_NAME               14 (property)
          
-         162         428 LOAD_CONST              23 (<code object minimum_ttl, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 161>)
+         162         428 LOAD_CONST              23 (<code object minimum_ttl, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 161>)
                      430 MAKE_FUNCTION            0
          
          161         432 PRECALL                  0
                      436 CALL                     0
          
          162         446 STORE_NAME              23 (minimum_ttl)
          
          165         448 LOAD_NAME               23 (minimum_ttl)
                      450 LOAD_ATTR               16 (setter)
          
-         166         460 LOAD_CONST              24 (<code object minimum_ttl, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 165>)
+         166         460 LOAD_CONST              24 (<code object minimum_ttl, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 165>)
                      462 MAKE_FUNCTION            0
          
          165         464 PRECALL                  0
                      468 CALL                     0
          
          166         478 STORE_NAME              23 (minimum_ttl)
          
          172         480 LOAD_NAME               23 (minimum_ttl)
                      482 LOAD_ATTR               18 (deleter)
          
-         173         492 LOAD_CONST              25 (<code object minimum_ttl, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 172>)
+         173         492 LOAD_CONST              25 (<code object minimum_ttl, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 172>)
                      494 MAKE_FUNCTION            0
          
          172         496 PRECALL                  0
                      500 CALL                     0
          
          173         510 STORE_NAME              23 (minimum_ttl)
          
          176         512 LOAD_NAME               14 (property)
          
          177         514 LOAD_CONST               9 ('return')
                      516 LOAD_NAME               24 (int)
                      518 BUILD_TUPLE              2
-                     520 LOAD_CONST              26 (<code object starting_at, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 176>)
+                     520 LOAD_CONST              26 (<code object starting_at, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 176>)
                      522 MAKE_FUNCTION            4 (annotations)
          
          176         524 PRECALL                  0
                      528 CALL                     0
          
          177         538 STORE_NAME              25 (starting_at)
          
          180         540 LOAD_NAME               25 (starting_at)
                      542 LOAD_ATTR               16 (setter)
          
-         181         552 LOAD_CONST              27 (<code object starting_at, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 180>)
+         181         552 LOAD_CONST              27 (<code object starting_at, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 180>)
                      554 MAKE_FUNCTION            0
          
          180         556 PRECALL                  0
                      560 CALL                     0
          
          181         570 STORE_NAME              25 (starting_at)
          
-         188         572 LOAD_CONST              28 (<code object get_property_list, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 188>)
+         188         572 LOAD_CONST              28 (<code object get_property_list, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 188>)
                      574 MAKE_FUNCTION            0
                      576 STORE_NAME              26 (get_property_list)
          
          191         578 LOAD_CONST              30 ((None, None, None))
-                     580 LOAD_CONST              29 (<code object run, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 191>)
+                     580 LOAD_CONST              29 (<code object run, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 191>)
                      582 MAKE_FUNCTION            1 (defaults)
                      584 STORE_NAME              27 (run)
                      586 LOAD_CONST               3 (None)
                      588 RETURN_VALUE
          consts
             'TTLTest'
             False
@@ -800,15 +800,15 @@
                            172 RETURN_VALUE
                consts
                   None
                names      ('str', 'address', 'auto_run', 'end_at', 'iterations', 'starting_at', 'timeout', 'run')
                varnames   ('self', 'address', 'auto_run', 'iterations', 'timeout', 'starting_at', 'end_at')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       '__init__'
                firstlineno 85
                lnotab 0x020928010e010e010e010e010e020e012cff
             'return'
             code
                argcount  : 1
                nlocals   : 1
@@ -822,15 +822,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_TTLTest__auto_run',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'auto_run'
                firstlineno 104
                lnotab 0x0202
             'new'
             code
                argcount  : 2
                nlocals   : 2
@@ -846,15 +846,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('_TTLTest__auto_run',)
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'auto_run'
                firstlineno 108
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -867,15 +867,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_TTLTest__iterations',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'iterations'
                firstlineno 112
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -908,15 +908,15 @@
                consts
                   None
                   'iterations must be an integer'
                names      ('isinstance', 'int', 'TypeError', '_TTLTest__iterations')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'iterations'
                firstlineno 116
                lnotab 0x02022a011e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
@@ -932,15 +932,15 @@
                consts
                   None
                   5
                names      ('_TTLTest__iterations',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'iterations'
                firstlineno 123
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -953,15 +953,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_TTLTest__history',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'history'
                firstlineno 127
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -974,15 +974,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_TTLTest__timeout',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'timeout'
                firstlineno 131
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
@@ -1017,15 +1017,15 @@
                consts
                   None
                   'Timeout must be a number.'
                names      ('isinstance', 'int', 'float', 'TypeError', '_TTLTest__timeout')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'timeout'
                firstlineno 135
                lnotab 0x020238011e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
@@ -1041,15 +1041,15 @@
                consts
                   None
                   3
                names      ('_TTLTest__timeout',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'timeout'
                firstlineno 141
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -1067,15 +1067,15 @@
                             40 RETURN_VALUE
                consts
                   None
                names      ('str', '_TTLTest__test_addr')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'address'
                firstlineno 145
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
@@ -1129,15 +1129,15 @@
                consts
                   None
                   'Address must be a string!'
                names      ('print', 'dir', 'type', 'isinstance', 'str', 'TypeError', '_TTLTest__test_addr')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'address'
                firstlineno 149
                lnotab 0x0202380138012a011e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
@@ -1153,15 +1153,15 @@
                consts
                   None
                   'inspyre.tech'
                names      ('_TTLTest__test_addr',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'address'
                firstlineno 157
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1174,15 +1174,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_TTLTest__min_ttl',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'minimum_ttl'
                firstlineno 161
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
@@ -1217,15 +1217,15 @@
                consts
                   None
                   'minimum__ttl must be an integer'
                names      ('isinstance', 'int', 'TypeError', '_TTLTest__min_ttl')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'minimum_ttl'
                firstlineno 165
                lnotab 0x02022e011e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
@@ -1240,15 +1240,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('minimum_ttl',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'minimum_ttl'
                firstlineno 172
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1261,15 +1261,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_TTLTest__starting_at',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'starting_at'
                firstlineno 176
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -1302,30 +1302,30 @@
                consts
                   None
                   '"starting_at" must be an integer'
                names      ('isinstance', 'int', 'TypeError', '_TTLTest__starting_at')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'starting_at'
                firstlineno 180
                lnotab 0x02022a011e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x9700640184007401000000000000000000006a01000000000000000074
                   0400000000000000000000a6010000ab0100000000000000004400a60000
                   00ab0000000000000000005300
                188           0 RESUME                   0
                
-               189           2 LOAD_CONST               1 (<code object <listcomp>, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\__init__.py", line 189>)
+               189           2 LOAD_CONST               1 (<code object <listcomp>, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\__init__.py", line 189>)
                              4 MAKE_FUNCTION            0
                              6 LOAD_GLOBAL              1 (NULL + inspect)
                             18 LOAD_ATTR                1 (getmembers)
                             28 LOAD_GLOBAL              4 (TTLTest)
                             40 PRECALL                  1
                             44 CALL                     1
                             54 GET_ITER
@@ -1361,23 +1361,23 @@
                                   62 JUMP_BACKWARD           29 (to 6)
                              >>   64 RETURN_VALUE
                      consts
                      names      ('isinstance', 'property')
                      varnames   ('.0', 'name', 'value')
                      freevars   ()
                      cellvars   ()
-                     filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+                     filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                      name       '<listcomp>'
                      firstlineno 189
                      lnotab 0x
                names      ('inspect', 'getmembers', 'TTLTest')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'get_property_list'
                firstlineno 188
                lnotab 0x0201
             code
                argcount  : 4
                nlocals   : 13
                stacksize : 7
@@ -1613,40 +1613,40 @@
                   'FOUND'
                   ' seconds elapsed total. In '
                   ' tries.'
                names      ('address', 'timeout', 'starting_at', 'time', 'minimum_ttl', 'print', 'ping', '_TTLTest__history', 'append', 'len', 'history', 'startswith')
                varnames   ('self', 'address', 'timeout', 'starting_at', 'addr', 'cur_ttl', 'markA', 'mark1', 'res', 'mark2', 'markB', 'tries', 'item')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
                name       'run'
                firstlineno 191
                lnotab
                   0x0201120216010e02120216010e021802260212010a0126011e01380128
                   01260104010e01460240f5120d2602280112012a010c02
             (None, None, None)
          names      ('__name__', '__module__', '__qualname__', '_TTLTest__auto_run', 'bool', '__annotations__', '_TTLTest__end_at', '_TTLTest__history', '_TTLTest__iterations', '_TTLTest__min_ttl', '_TTLTest__starting_at', '_TTLTest__address', '_TTLTest__timeout', '__init__', 'property', 'auto_run', 'setter', 'iterations', 'deleter', 'history', 'timeout', 'str', 'address', 'minimum_ttl', 'int', 'starting_at', 'get_property_list', 'run')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
          name       'TTLTest'
          firstlineno 75
          lnotab
             0x0c010e0104010401040104010401040104040201020102010201020102
             f9081302010aff0e0102030c010aff0e010203020104ff0e0102030c0104
             ff0e0102060c0104ff0e010203020104ff0e010203020104ff0e0102030c
             0104ff0e0102050c0104ff0e01020302010aff0e0102030c0104ff0e0102
             070c0104ff0e010203020104ff0e0102030c0104ff0e0102060c0104ff0e
             01020302010aff0e0102030c0104ff0e0102070603
       'TTLTest'
       (True, 5, True, True, True)
-   names      ('__doc__', 'inspy_logger', 'InspyLogger', 'time', 'ping3', 'ping', 'verbose_ping', 'ping_ping.logging', 'add_child', 'add_child_logger', 'PROG_NAME', 'rich.logging', 'RichHandler', 'inspect', 'ping_ping.utils.decorators', 'validate_properties', 'statistics', 'mean', 'median', 'LOGGER', '_', 'ModuleNotFoundError', 'NameError', 'e', 'debug', 'name', 'get_ping_mean', 'gather_times', 'TTLTest')
+   names      ('__doc__', 'inspy_logger', 'InspyLogger', 'time', 'ping3', 'ping', 'verbose_ping', 'ping_stat.logging', 'add_child', 'add_child_logger', 'PROG_NAME', 'rich.logging', 'RichHandler', 'inspect', 'ping_stat.utils.decorators', 'validate_properties', 'statistics', 'mean', 'median', 'LOGGER', '_', 'ModuleNotFoundError', 'NameError', 'e', 'debug', 'name', 'get_ping_mean', 'gather_times', 'TTLTest')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\__init__.py'
+   filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020104070c010801100110010c0108010c011003020108020c011c
       014cfe08050608020102010201020102fa082b1a7f001b
```

### Comparing `ping_stat-0.1.0/ping_stat/utils/__pycache__/__init__.cpython-39.pyc` & `ping_stat-1.0/ping_stat/utils/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/__pycache__/decorators.cpython-310.pyc` & `ping_stat-1.0/ping_stat/utils/__pycache__/decorators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/__pycache__/decorators.cpython-311.pyc` & `ping_stat-1.0/ping_stat/utils/__pycache__/decorators.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,34 +1,34 @@
 magic:    0xa70d0d0a
-moddate:  0x9088fc63 (Mon Feb 27 10:40:16 2023 UTC)
+moddate:  0x717b9464 (Thu Jun 22 16:48:49 2023 UTC)
 files sz: 1854
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x970064005a00640164026c015a01640384005a0264025300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/27/2023 @ 4:37 AM\nFile:\n  Name: decorators.py\n  Filepath: ping_ping/utils\n')
+     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/27/2023 @ 4:37 AM\nFile:\n  Name: decorators.py\n  Filepath: ping_stat/utils\n')
                  4 STORE_NAME               0 (__doc__)
    
      8           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
                 10 IMPORT_NAME              1 (typing)
                 12 STORE_NAME               1 (typing)
    
-    11          14 LOAD_CONST               3 (<code object validate_properties, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\decorators.py", line 11>)
+    11          14 LOAD_CONST               3 (<code object validate_properties, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\decorators.py", line 11>)
                 16 MAKE_FUNCTION            0
                 18 STORE_NAME               2 (validate_properties)
    
     27          20 LOAD_CONST               2 (None)
                 22 RETURN_VALUE
    consts
-      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/27/2023 @ 4:37 AM\nFile:\n  Name: decorators.py\n  Filepath: ping_ping/utils\n'
+      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 2/27/2023 @ 4:37 AM\nFile:\n  Name: decorators.py\n  Filepath: ping_stat/utils\n'
       0
       None
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 9
          flags     : 3
@@ -82,15 +82,15 @@
                      188 PRECALL                  1
                      192 CALL                     1
                      202 STORE_FAST               4 (validator)
          
           17         204 LOAD_FAST                1 (name)
                      206 LOAD_FAST                4 (validator)
                      208 BUILD_TUPLE              2
-                     210 LOAD_CONST               2 (<code object setter, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\decorators.py", line 17>)
+                     210 LOAD_CONST               2 (<code object setter, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\decorators.py", line 17>)
                      212 MAKE_FUNCTION            1 (defaults)
                      214 STORE_FAST               5 (setter)
          
           22         216 LOAD_GLOBAL             17 (NULL + setattr)
                      228 LOAD_FAST                0 (cls)
                      230 LOAD_FAST                1 (name)
                      232 LOAD_GLOBAL              7 (NULL + property)
@@ -154,27 +154,27 @@
                   None
                   'value'
                   '_'
                names      ('validate', 'ValueError', 'errors', 'setattr')
                varnames   ('self', 'value', 'name', 'validator')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\decorators.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\decorators.py'
                name       'setter'
                firstlineno 17
                lnotab 0x02012e012801
          names      ('__dict__', 'items', 'isinstance', 'property', 'fset', 'typing', 'get_type_hints', 'Validator', 'setattr', 'fget')
          varnames   ('cls', 'name', 'prop', 'schema', 'validator', 'setter')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\decorators.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\decorators.py'
          name       'validate_properties'
          firstlineno 11
          lnotab 0x02013c01380138011e020c054a02
    names      ('__doc__', 'typing', 'validate_properties')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\decorators.py'
+   filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\decorators.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201040708030610
```

### Comparing `ping_stat-0.1.0/ping_stat/utils/__pycache__/decorators.cpython-39.pyc` & `ping_stat-1.0/ping_stat/utils/__pycache__/decorators.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/__pycache__/helpers.cpython-310.pyc` & `ping_stat-1.0/ping_stat/utils/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/__pycache__/network.cpython-310.pyc` & `ping_stat-1.0/ping_stat/utils/__pycache__/network.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/__pycache__/network.cpython-311.pyc` & `ping_stat-1.0/ping_stat/utils/__pycache__/network.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,1365 +1,1497 @@
 magic:    0xa70d0d0a
-moddate:  0xdbba5b64 (Wed May 10 15:40:11 2023 UTC)
-files sz: 13547
+moddate:  0x5e5b9564 (Fri Jun 23 08:44:14 2023 UTC)
+files sz: 15639
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
-      0x970064005a00640164026c016d025a026d015a010100640164036c036d
-      045a046d055a050100640164046c066d075a070100640164056c086d095a
-      096d0a5a0a0100640164066c0b6d0c5a0c6d0d5a0d0100640164076c0e6d
-      0f5a100100640164086c116d125a120100640164096c136d145a14010064
-      01640a6c156d165a16010002006516a6000000ab0000000000000000005a
-      17640b5a1802004700640c8400640da6020000ab0200000000000000005a
-      19640e5300
+      0x970064005a00640164026c016d025a030100640164036c046d055a056d
+      065a060100640164046c076d085a080100640164056c096d0a5a0a6d0b5a
+      0b0100640164066c0c6d0d5a0d0100640164076c0e5a0e640164086c0f6d
+      105a100100640164096c116d125a126d135a1301006401640a6c146d155a
+      1501006401640b6c166d175a176d165a16010002006510a6000000ab0000
+      000000000000005a18640c5a1902004700640d8400640ea6020000ab0200
+      000000000000005a1a64075300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 5/9/2023 @ 8:47 PM\nFile:\n  Name: network\n  Filepath: ping_ping/utils\n')
+     1           2 LOAD_CONST               0 ('\nPingPing: network\nModule Author: Inspyre Softworks (https://inspyre.tech)\nModule Created: 5/9/2023 @ 8:47 PM\nModule Path: ping_stat/utils\n\nThis module implements the network functionality for the PingPing project. It is responsible for performing\nnetwork operations, including the following:\n\n1. Pinging operations on a specific target (IP address or hostname).\n2. Generating network operation reports.\n3. Managing the state and execution of the PingWorker and PingMonitor classes.\n\nClasses:\n- Ping: This class represents a ping operation on a target. It has several configurable parameters like\n  target IP or hostname, timeout, and the number of times to perform the operation. It can also perform\n  the operation automatically upon initialization.\n\nAttributes:\n- console: An instance of the rich.console.Console class for console operations.\n- track_mean: A boolean value used for internal operations.\n\nUsage:\nfrom ping_stat.utils.network import Ping\n\n# Create an instance of the Ping class, automatically performing the operation upon initialization.\nping = Ping(target="google.com", auto_run=True)\n\n# Perform the operation manually and print the results.\nprint(ping.ping())\n\nDisclaimer:\nPlease use this tool only with the express permission of the target system\'s network administrator and\nexercise due care and responsibility in doing so. The author of this tool assumes no liability for any damage,\nlegal or otherwise, caused by its use. Pinging a target is not a passive operation and may be detected by\nintrusion detection systems or firewall logs. Irresponsible use of this tool could potentially cause a\ndenial of service to the target system\'s network services, or your own.\n')
                  4 STORE_NAME               0 (__doc__)
    
-     8           6 LOAD_CONST               1 (0)
-                 8 LOAD_CONST               2 (('sleep', 'time'))
-                10 IMPORT_NAME              1 (time)
-                12 IMPORT_FROM              2 (sleep)
-                14 STORE_NAME               2 (sleep)
-                16 IMPORT_FROM              1 (time)
-                18 STORE_NAME               1 (time)
-                20 POP_TOP
+    39           6 LOAD_CONST               1 (0)
+                 8 LOAD_CONST               2 (('ping',))
+                10 IMPORT_NAME              1 (ping3)
+                12 IMPORT_FROM              2 (ping)
+                14 STORE_NAME               3 (_ping)
+                16 POP_TOP
    
-     9          22 LOAD_CONST               1 (0)
-                24 LOAD_CONST               3 (('RedundantWorkOrderError', 'WorkerAlreadyStartedError'))
-                26 IMPORT_NAME              3 (ping_ping.errors)
-                28 IMPORT_FROM              4 (RedundantWorkOrderError)
-                30 STORE_NAME               4 (RedundantWorkOrderError)
-                32 IMPORT_FROM              5 (WorkerAlreadyStartedError)
-                34 STORE_NAME               5 (WorkerAlreadyStartedError)
-                36 POP_TOP
+    40          18 LOAD_CONST               1 (0)
+                20 LOAD_CONST               3 (('RedundantWorkOrderError', 'WorkerAlreadyStartedError'))
+                22 IMPORT_NAME              4 (ping_stat.errors)
+                24 IMPORT_FROM              5 (RedundantWorkOrderError)
+                26 STORE_NAME               5 (RedundantWorkOrderError)
+                28 IMPORT_FROM              6 (WorkerAlreadyStartedError)
+                30 STORE_NAME               6 (WorkerAlreadyStartedError)
+                32 POP_TOP
    
-    11          38 LOAD_CONST               1 (0)
-                40 LOAD_CONST               4 (('gather_times',))
-                42 IMPORT_NAME              6 (ping_ping.utils)
-                44 IMPORT_FROM              7 (gather_times)
-                46 STORE_NAME               7 (gather_times)
-                48 POP_TOP
+    42          34 LOAD_CONST               1 (0)
+                36 LOAD_CONST               4 (('gather_times',))
+                38 IMPORT_NAME              7 (ping_stat.utils)
+                40 IMPORT_FROM              8 (gather_times)
+                42 STORE_NAME               8 (gather_times)
+                44 POP_TOP
    
-    12          50 LOAD_CONST               1 (0)
-                52 LOAD_CONST               5 (('PingMonitor', 'PingWorker'))
-                54 IMPORT_NAME              8 (ping_ping.utils.workers)
-                56 IMPORT_FROM              9 (PingMonitor)
-                58 STORE_NAME               9 (PingMonitor)
-                60 IMPORT_FROM             10 (PingWorker)
-                62 STORE_NAME              10 (PingWorker)
-                64 POP_TOP
+    43          46 LOAD_CONST               1 (0)
+                48 LOAD_CONST               5 (('PingMonitor', 'PingWorker'))
+                50 IMPORT_NAME              9 (ping_stat.utils.workers)
+                52 IMPORT_FROM             10 (PingMonitor)
+                54 STORE_NAME              10 (PingMonitor)
+                56 IMPORT_FROM             11 (PingWorker)
+                58 STORE_NAME              11 (PingWorker)
+                60 POP_TOP
    
-    13          66 LOAD_CONST               1 (0)
-                68 LOAD_CONST               6 (('mean', 'median'))
-                70 IMPORT_NAME             11 (statistics)
-                72 IMPORT_FROM             12 (mean)
-                74 STORE_NAME              12 (mean)
-                76 IMPORT_FROM             13 (median)
-                78 STORE_NAME              13 (median)
-                80 POP_TOP
+    44          62 LOAD_CONST               1 (0)
+                64 LOAD_CONST               6 (('Null',))
+                66 IMPORT_NAME             12 (pypattyrn.behavioral.null)
+                68 IMPORT_FROM             13 (Null)
+                70 STORE_NAME              13 (Null)
+                72 POP_TOP
    
-    14          82 LOAD_CONST               1 (0)
-                84 LOAD_CONST               7 (('ping',))
-                86 IMPORT_NAME             14 (ping3)
-                88 IMPORT_FROM             15 (ping)
-                90 STORE_NAME              16 (_ping)
+    45          74 LOAD_CONST               1 (0)
+                76 LOAD_CONST               7 (None)
+                78 IMPORT_NAME             14 (queue)
+                80 STORE_NAME              14 (queue)
+   
+    46          82 LOAD_CONST               1 (0)
+                84 LOAD_CONST               8 (('Console',))
+                86 IMPORT_NAME             15 (rich.console)
+                88 IMPORT_FROM             16 (Console)
+                90 STORE_NAME              16 (Console)
                 92 POP_TOP
    
-    15          94 LOAD_CONST               1 (0)
-                96 LOAD_CONST               8 (('Null',))
-                98 IMPORT_NAME             17 (pypattyrn.behavioral.null)
-               100 IMPORT_FROM             18 (Null)
-               102 STORE_NAME              18 (Null)
-               104 POP_TOP
+    47          94 LOAD_CONST               1 (0)
+                96 LOAD_CONST               9 (('mean', 'median'))
+                98 IMPORT_NAME             17 (statistics)
+               100 IMPORT_FROM             18 (mean)
+               102 STORE_NAME              18 (mean)
+               104 IMPORT_FROM             19 (median)
+               106 STORE_NAME              19 (median)
+               108 POP_TOP
    
-    16         106 LOAD_CONST               1 (0)
-               108 LOAD_CONST               9 (('Thread',))
-               110 IMPORT_NAME             19 (threading)
-               112 IMPORT_FROM             20 (Thread)
-               114 STORE_NAME              20 (Thread)
-               116 POP_TOP
+    48         110 LOAD_CONST               1 (0)
+               112 LOAD_CONST              10 (('Thread',))
+               114 IMPORT_NAME             20 (threading)
+               116 IMPORT_FROM             21 (Thread)
+               118 STORE_NAME              21 (Thread)
+               120 POP_TOP
    
-    17         118 LOAD_CONST               1 (0)
-               120 LOAD_CONST              10 (('Console',))
-               122 IMPORT_NAME             21 (rich.console)
-               124 IMPORT_FROM             22 (Console)
-               126 STORE_NAME              22 (Console)
-               128 POP_TOP
+    49         122 LOAD_CONST               1 (0)
+               124 LOAD_CONST              11 (('sleep', 'time'))
+               126 IMPORT_NAME             22 (time)
+               128 IMPORT_FROM             23 (sleep)
+               130 STORE_NAME              23 (sleep)
+               132 IMPORT_FROM             22 (time)
+               134 STORE_NAME              22 (time)
+               136 POP_TOP
    
-    20         130 PUSH_NULL
-               132 LOAD_NAME               22 (Console)
-               134 PRECALL                  0
-               138 CALL                     0
-               148 STORE_NAME              23 (console)
+    52         138 PUSH_NULL
+               140 LOAD_NAME               16 (Console)
+               142 PRECALL                  0
+               146 CALL                     0
+               156 STORE_NAME              24 (console)
    
-    23         150 LOAD_CONST              11 (False)
-               152 STORE_NAME              24 (track_mean)
+    55         158 LOAD_CONST              12 (False)
+               160 STORE_NAME              25 (track_mean)
    
-    26         154 PUSH_NULL
-               156 LOAD_BUILD_CLASS
-               158 LOAD_CONST              12 (<code object Ping, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 26>)
-               160 MAKE_FUNCTION            0
-               162 LOAD_CONST              13 ('Ping')
-               164 PRECALL                  2
-               168 CALL                     2
-               178 STORE_NAME              25 (Ping)
+    58         162 PUSH_NULL
+               164 LOAD_BUILD_CLASS
+               166 LOAD_CONST              13 (<code object Ping, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 58>)
+               168 MAKE_FUNCTION            0
+               170 LOAD_CONST              14 ('Ping')
+               172 PRECALL                  2
+               176 CALL                     2
+               186 STORE_NAME              26 (Ping)
    
-   482         180 LOAD_CONST              14 (None)
-               182 RETURN_VALUE
+   537         188 LOAD_CONST               7 (None)
+               190 RETURN_VALUE
    consts
-      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.techCreated: 5/9/2023 @ 8:47 PM\nFile:\n  Name: network\n  Filepath: ping_ping/utils\n'
+      '\nPingPing: network\nModule Author: Inspyre Softworks (https://inspyre.tech)\nModule Created: 5/9/2023 @ 8:47 PM\nModule Path: ping_stat/utils\n\nThis module implements the network functionality for the PingPing project. It is responsible for performing\nnetwork operations, including the following:\n\n1. Pinging operations on a specific target (IP address or hostname).\n2. Generating network operation reports.\n3. Managing the state and execution of the PingWorker and PingMonitor classes.\n\nClasses:\n- Ping: This class represents a ping operation on a target. It has several configurable parameters like\n  target IP or hostname, timeout, and the number of times to perform the operation. It can also perform\n  the operation automatically upon initialization.\n\nAttributes:\n- console: An instance of the rich.console.Console class for console operations.\n- track_mean: A boolean value used for internal operations.\n\nUsage:\nfrom ping_stat.utils.network import Ping\n\n# Create an instance of the Ping class, automatically performing the operation upon initialization.\nping = Ping(target="google.com", auto_run=True)\n\n# Perform the operation manually and print the results.\nprint(ping.ping())\n\nDisclaimer:\nPlease use this tool only with the express permission of the target system\'s network administrator and\nexercise due care and responsibility in doing so. The author of this tool assumes no liability for any damage,\nlegal or otherwise, caused by its use. Pinging a target is not a passive operation and may be detected by\nintrusion detection systems or firewall logs. Irresponsible use of this tool could potentially cause a\ndenial of service to the target system\'s network services, or your own.\n'
       0
-      ('sleep', 'time')
+      ('ping',)
       ('RedundantWorkOrderError', 'WorkerAlreadyStartedError')
       ('gather_times',)
       ('PingMonitor', 'PingWorker')
-      ('mean', 'median')
-      ('ping',)
       ('Null',)
-      ('Thread',)
+      None
       ('Console',)
+      ('mean', 'median')
+      ('Thread',)
+      ('sleep', 'time')
       False
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 9
+         stacksize : 10
          flags     : 0
          code
             0x970065005a0164005a0264015a03640264036c046d055a050100020065
             056404a6010000ab0100000000000000005a0664055a0764065a0864075a
             0964085a0a64065a0b64095a0c640a5a0d67005a0e64055a0f64055a1002
             006511a6000000ab000000000000000000650764066509650a650c650d64
-            0664056609640b65126602640c84055a136514640d65156602640e8404a6
-            000000ab0000000000000000005a1665166a170000000000000000640f65
-            15660264108404a6000000ab0000000000000000005a16651464118400a6
-            000000ab0000000000000000005a186514640d6519660264128404a60000
-            00ab0000000000000000005a1a651a6a17000000000000000064138400a6
-            000000ab0000000000000000005a1a651464148400a6000000ab00000000
-            00000000005a1b651b6a17000000000000000064158400a6000000ab0000
-            000000000000005a1b651464168400a6000000ab0000000000000000005a
-            1c651464178400a6000000ab0000000000000000005a1d651d6a17000000
-            000000000064188400a6000000ab0000000000000000005a1d6514641984
-            00a6000000ab0000000000000000005a1865186a17000000000000000064
-            1a8400a6000000ab0000000000000000005a186514641b8400a6000000ab
-            0000000000000000005a1e651e6a170000000000000000641c8400a60000
-            00ab0000000000000000005a1e6514641d8400a6000000ab000000000000
-            0000005a1f651f6a170000000000000000641e8400a6000000ab00000000
-            00000000005a1f6514641f8400a6000000ab0000000000000000005a2065
-            14640d6521660264208404a6000000ab0000000000000000005a2265226a
-            17000000000000000064218400a6000000ab0000000000000000005a2265
-            1464228400a6000000ab0000000000000000005a23651464238400a60000
-            00ab0000000000000000005a2465246a17000000000000000064248400a6
-            000000ab0000000000000000005a2465246a250000000000000000642584
-            00a6000000ab0000000000000000005a24651464268400a6000000ab0000
-            000000000000005a26642d642784015a27642884005a28642984005a2964
-            2a84005a2a642b84005a2b642c84005a2c64065300
-          26           0 RESUME                   0
+            0664056405660a640b65126602640c84055a136514640d65156602640e84
+            04a6000000ab0000000000000000005a1665166a17000000000000000064
+            0f6515660264108404a6000000ab0000000000000000005a166514641184
+            00a6000000ab0000000000000000005a186514640d6519660264128404a6
+            000000ab0000000000000000005a1a651a6a170000000000000000641384
+            00a6000000ab0000000000000000005a1a6514640d6515660264148404a6
+            000000ab0000000000000000005a1b651b6a170000000000000000641584
+            00a6000000ab0000000000000000005a1b651464168400a6000000ab0000
+            000000000000005a1c651c6a17000000000000000064178400a6000000ab
+            0000000000000000005a1c651464188400a6000000ab0000000000000000
+            005a1d651464198400a6000000ab0000000000000000005a1e651e6a1700
+            00000000000000641a8400a6000000ab0000000000000000005a1e651464
+            1b8400a6000000ab0000000000000000005a1865186a1700000000000000
+            00641c8400a6000000ab0000000000000000005a186514641d8400a60000
+            00ab0000000000000000005a1f651f6a170000000000000000641e8400a6
+            000000ab0000000000000000005a1f6514641f8400a6000000ab00000000
+            00000000005a2065206a17000000000000000064208400a6000000ab0000
+            000000000000005a20651464218400a6000000ab0000000000000000005a
+            216514640d6522660264228404a6000000ab0000000000000000005a2365
+            236a17000000000000000064238400a6000000ab0000000000000000005a
+            23651464248400a6000000ab0000000000000000005a2465246a25000000
+            000000000064258400a6000000ab0000000000000000005a246514642684
+            00a6000000ab0000000000000000005a26651464278400a6000000ab0000
+            000000000000005a2765276a17000000000000000064288400a6000000ab
+            0000000000000000005a2765276a25000000000000000064298400a60000
+            00ab0000000000000000005a276514642a8400a6000000ab000000000000
+            0000005a286431642b84015a29642c84005a2a642d84005a2b642e84005a
+            2c642f84005a2d643084005a2e64065300
+          58           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Ping')
                        8 STORE_NAME               2 (__qualname__)
          
-          27          10 LOAD_CONST               1 ('\n    A class for performing ping operations on a target.\n\n    Disclaimer:\n        Please use this tool only with the express permission of the target system\'s network administrator,\n        and exercise due care and responsibility in doing so. The author of this tool assumes no liability for any damage,\n        legal or otherwise, caused by its use.\n\n    Note:\n        Pinging a target is not a passive operation and may be detected by intrusion detection systems or firewall logs.\n        Irresponsible use of this tool could potentially cause a denial of service to the target system\'s network\n        services, or your own.\n\n\n    Attributes:\n        target (str):\n            The IP address or hostname to ping.\n\n        auto_run (bool):\n            Whether to automatically ping the ping operation upon initialization.\n\n        timeout (float):\n            The time in seconds to wait for a response before timing out.\n\n        runs (int):\n            The number of times to send a ping request to the target.\n\n    Methods:\n        ping():\n            Runs the ping operation and returns a list of ping times (in milliseconds).\n\n    Usage:\n        ping = Ping(target="google.com", auto_run=True)\n        ping.ping()\n        # [15.132, 15.269, 15.265]\n    ')
+          59          10 LOAD_CONST               1 ('\n    A class for performing ping operations on a target.\n\n    Disclaimer:\n        Please use this tool only with the express permission of the target system\'s network administrator,\n        and exercise due care and responsibility in doing so. The author of this tool assumes no liability for any damage,\n        legal or otherwise, caused by its use.\n\n    Note:\n        Pinging a target is not a passive operation and may be detected by intrusion detection systems or firewall logs.\n        Irresponsible use of this tool could potentially cause a denial of service to the target system\'s network\n        services, or your own.\n\n\n    Attributes:\n        target (str):\n            The IP address or hostname to ping.\n\n        auto_run (bool):\n            Whether to automatically ping the ping operation upon initialization.\n\n        timeout (float):\n            The time in seconds to wait for a response before timing out.\n\n        runs (int):\n            The number of times to send a ping request to the target.\n\n    Methods:\n        ping():\n            Runs the ping operation and returns a list of ping times (in milliseconds).\n\n    Usage:\n        ping = Ping(target="google.com", auto_run=True)\n        ping.ping()\n        # [15.132, 15.269, 15.265]\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-          63          14 LOAD_CONST               2 (0)
+          95          14 LOAD_CONST               2 (0)
                       16 LOAD_CONST               3 (('add_child',))
-                      18 IMPORT_NAME              4 (ping_ping.logging)
+                      18 IMPORT_NAME              4 (ping_stat.logging)
                       20 IMPORT_FROM              5 (add_child)
                       22 STORE_NAME               5 (add_child)
                       24 POP_TOP
          
-          65          26 PUSH_NULL
+          97          26 PUSH_NULL
                       28 LOAD_NAME                5 (add_child)
                       30 LOAD_CONST               4 ('PingPing.Ping')
                       32 PRECALL                  1
                       36 CALL                     1
                       46 STORE_NAME               6 (_Ping__cls_log)
          
-          67          48 LOAD_CONST               5 (False)
+          99          48 LOAD_CONST               5 (False)
                       50 STORE_NAME               7 (_Ping__auto_run)
          
-          68          52 LOAD_CONST               6 (None)
+         100          52 LOAD_CONST               6 (None)
                       54 STORE_NAME               8 (_Ping__target)
          
-          69          56 LOAD_CONST               7 (5)
+         101          56 LOAD_CONST               7 (5)
                       58 STORE_NAME               9 (_Ping__timeout)
          
-          70          60 LOAD_CONST               8 (3)
+         102          60 LOAD_CONST               8 (3)
                       62 STORE_NAME              10 (_Ping__runs)
          
-          71          64 LOAD_CONST               6 (None)
+         103          64 LOAD_CONST               6 (None)
                       66 STORE_NAME              11 (_Ping__results)
          
-          72          68 LOAD_CONST               9 (1)
+         104          68 LOAD_CONST               9 (1)
                       70 STORE_NAME              12 (_Ping__interval)
          
-          73          72 LOAD_CONST              10 (256)
+         105          72 LOAD_CONST              10 (256)
                       74 STORE_NAME              13 (_Ping__size)
          
-          74          76 BUILD_LIST               0
+         106          76 BUILD_LIST               0
                       78 STORE_NAME              14 (_Ping__history)
          
-          75          80 LOAD_CONST               5 (False)
+         107          80 LOAD_CONST               5 (False)
                       82 STORE_NAME              15 (_Ping__monitoring)
          
-          76          84 LOAD_CONST               5 (False)
+         108          84 LOAD_CONST               5 (False)
                       86 STORE_NAME              16 (_Ping__continuous_ping)
          
-          81          88 PUSH_NULL
+         113          88 PUSH_NULL
                       90 LOAD_NAME               17 (Null)
                       92 PRECALL                  0
                       96 CALL                     0
          
-          82         106 LOAD_NAME                7 (_Ping__auto_run)
+         114         106 LOAD_NAME                7 (_Ping__auto_run)
+         
+         115         108 LOAD_CONST               6 (None)
+         
+         116         110 LOAD_NAME                9 (_Ping__timeout)
+         
+         117         112 LOAD_NAME               10 (_Ping__runs)
+         
+         118         114 LOAD_NAME               12 (_Ping__interval)
+         
+         119         116 LOAD_NAME               13 (_Ping__size)
+         
+         120         118 LOAD_CONST               6 (None)
+         
+         121         120 LOAD_CONST               5 (False)
          
-          83         108 LOAD_CONST               6 (None)
+         122         122 LOAD_CONST               5 (False)
          
-          84         110 LOAD_NAME                9 (_Ping__timeout)
+         110         124 BUILD_TUPLE             10
+                     126 LOAD_CONST              11 ('target')
          
-          85         112 LOAD_NAME               10 (_Ping__runs)
+         112         128 LOAD_NAME               18 (str)
          
-          86         114 LOAD_NAME               12 (_Ping__interval)
+         110         130 BUILD_TUPLE              2
+                     132 LOAD_CONST              12 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 110>)
+                     134 MAKE_FUNCTION            5 (defaults, annotations)
+                     136 STORE_NAME              19 (__init__)
          
-          87         116 LOAD_NAME               13 (_Ping__size)
+         187         138 LOAD_NAME               20 (property)
          
-          88         118 LOAD_CONST               6 (None)
+         188         140 LOAD_CONST              13 ('return')
+                     142 LOAD_NAME               21 (bool)
+                     144 BUILD_TUPLE              2
+                     146 LOAD_CONST              14 (<code object auto_run, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 187>)
+                     148 MAKE_FUNCTION            4 (annotations)
          
-          89         120 LOAD_CONST               5 (False)
+         187         150 PRECALL                  0
+                     154 CALL                     0
          
-          78         122 BUILD_TUPLE              9
-                     124 LOAD_CONST              11 ('target')
+         188         164 STORE_NAME              22 (auto_run)
          
-          80         126 LOAD_NAME               18 (str)
+         195         166 LOAD_NAME               22 (auto_run)
+                     168 LOAD_ATTR               23 (setter)
          
-          78         128 BUILD_TUPLE              2
-                     130 LOAD_CONST              12 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 78>)
-                     132 MAKE_FUNCTION            5 (defaults, annotations)
-                     134 STORE_NAME              19 (__init__)
+         196         178 LOAD_CONST              15 ('new')
+                     180 LOAD_NAME               21 (bool)
+                     182 BUILD_TUPLE              2
+                     184 LOAD_CONST              16 (<code object auto_run, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 195>)
+                     186 MAKE_FUNCTION            4 (annotations)
          
-         151         136 LOAD_NAME               20 (property)
+         195         188 PRECALL                  0
+                     192 CALL                     0
          
-         152         138 LOAD_CONST              13 ('return')
-                     140 LOAD_NAME               21 (bool)
-                     142 BUILD_TUPLE              2
-                     144 LOAD_CONST              14 (<code object auto_run, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 151>)
-                     146 MAKE_FUNCTION            4 (annotations)
+         196         202 STORE_NAME              22 (auto_run)
          
-         151         148 PRECALL                  0
-                     152 CALL                     0
+         213         204 LOAD_NAME               20 (property)
          
-         152         162 STORE_NAME              22 (auto_run)
+         214         206 LOAD_CONST              17 (<code object continuous_ping, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 213>)
+                     208 MAKE_FUNCTION            0
          
-         159         164 LOAD_NAME               22 (auto_run)
-                     166 LOAD_ATTR               23 (setter)
+         213         210 PRECALL                  0
+                     214 CALL                     0
          
-         160         176 LOAD_CONST              15 ('new')
-                     178 LOAD_NAME               21 (bool)
-                     180 BUILD_TUPLE              2
-                     182 LOAD_CONST              16 (<code object auto_run, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 159>)
-                     184 MAKE_FUNCTION            4 (annotations)
+         214         224 STORE_NAME              24 (continuous_ping)
          
-         159         186 PRECALL                  0
-                     190 CALL                     0
+         217         226 LOAD_NAME               20 (property)
          
-         160         200 STORE_NAME              22 (auto_run)
+         218         228 LOAD_CONST              13 ('return')
+                     230 LOAD_NAME               25 (int)
+                     232 BUILD_TUPLE              2
+                     234 LOAD_CONST              18 (<code object interval, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 217>)
+                     236 MAKE_FUNCTION            4 (annotations)
          
-         177         202 LOAD_NAME               20 (property)
+         217         238 PRECALL                  0
+                     242 CALL                     0
          
-         178         204 LOAD_CONST              17 (<code object continuous_ping, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 177>)
-                     206 MAKE_FUNCTION            0
+         218         252 STORE_NAME              26 (interval)
          
-         177         208 PRECALL                  0
-                     212 CALL                     0
+         221         254 LOAD_NAME               26 (interval)
+                     256 LOAD_ATTR               23 (setter)
          
-         178         222 STORE_NAME              24 (continuous_ping)
+         222         266 LOAD_CONST              19 (<code object interval, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 221>)
+                     268 MAKE_FUNCTION            0
          
-         181         224 LOAD_NAME               20 (property)
+         221         270 PRECALL                  0
+                     274 CALL                     0
          
-         182         226 LOAD_CONST              13 ('return')
-                     228 LOAD_NAME               25 (int)
-                     230 BUILD_TUPLE              2
-                     232 LOAD_CONST              18 (<code object interval, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 181>)
-                     234 MAKE_FUNCTION            4 (annotations)
+         222         284 STORE_NAME              26 (interval)
          
-         181         236 PRECALL                  0
-                     240 CALL                     0
+         228         286 LOAD_NAME               20 (property)
          
-         182         250 STORE_NAME              26 (interval)
+         229         288 LOAD_CONST              13 ('return')
+                     290 LOAD_NAME               21 (bool)
+                     292 BUILD_TUPLE              2
+                     294 LOAD_CONST              20 (<code object gui_mode, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 228>)
+                     296 MAKE_FUNCTION            4 (annotations)
          
-         185         252 LOAD_NAME               26 (interval)
-                     254 LOAD_ATTR               23 (setter)
+         228         298 PRECALL                  0
+                     302 CALL                     0
          
-         186         264 LOAD_CONST              19 (<code object interval, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 185>)
-                     266 MAKE_FUNCTION            0
+         229         312 STORE_NAME              27 (gui_mode)
          
-         185         268 PRECALL                  0
-                     272 CALL                     0
+         232         314 LOAD_NAME               27 (gui_mode)
+                     316 LOAD_ATTR               23 (setter)
          
-         186         282 STORE_NAME              26 (interval)
+         233         326 LOAD_CONST              21 (<code object gui_mode, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 232>)
+                     328 MAKE_FUNCTION            0
          
-         192         284 LOAD_NAME               20 (property)
+         232         330 PRECALL                  0
+                     334 CALL                     0
          
-         193         286 LOAD_CONST              20 (<code object packet_size, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 192>)
-                     288 MAKE_FUNCTION            0
+         233         344 STORE_NAME              27 (gui_mode)
          
-         192         290 PRECALL                  0
-                     294 CALL                     0
+         238         346 LOAD_NAME               20 (property)
          
-         193         304 STORE_NAME              27 (packet_size)
+         239         348 LOAD_CONST              22 (<code object packet_size, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 238>)
+                     350 MAKE_FUNCTION            0
          
-         196         306 LOAD_NAME               27 (packet_size)
-                     308 LOAD_ATTR               23 (setter)
+         238         352 PRECALL                  0
+                     356 CALL                     0
          
-         197         318 LOAD_CONST              21 (<code object packet_size, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 196>)
-                     320 MAKE_FUNCTION            0
+         239         366 STORE_NAME              28 (packet_size)
          
-         196         322 PRECALL                  0
-                     326 CALL                     0
+         242         368 LOAD_NAME               28 (packet_size)
+                     370 LOAD_ATTR               23 (setter)
          
-         197         336 STORE_NAME              27 (packet_size)
+         243         380 LOAD_CONST              23 (<code object packet_size, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 242>)
+                     382 MAKE_FUNCTION            0
          
-         207         338 LOAD_NAME               20 (property)
+         242         384 PRECALL                  0
+                     388 CALL                     0
          
-         208         340 LOAD_CONST              22 (<code object ping_worker, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 207>)
-                     342 MAKE_FUNCTION            0
+         243         398 STORE_NAME              28 (packet_size)
          
-         207         344 PRECALL                  0
-                     348 CALL                     0
+         253         400 LOAD_NAME               20 (property)
          
-         208         358 STORE_NAME              28 (ping_worker)
+         254         402 LOAD_CONST              24 (<code object ping_worker, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 253>)
+                     404 MAKE_FUNCTION            0
          
-         211         360 LOAD_NAME               20 (property)
+         253         406 PRECALL                  0
+                     410 CALL                     0
          
-         212         362 LOAD_CONST              23 (<code object target, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 211>)
-                     364 MAKE_FUNCTION            0
+         254         420 STORE_NAME              29 (ping_worker)
          
-         211         366 PRECALL                  0
-                     370 CALL                     0
+         257         422 LOAD_NAME               20 (property)
          
-         212         380 STORE_NAME              29 (target)
+         258         424 LOAD_CONST              25 (<code object target, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 257>)
+                     426 MAKE_FUNCTION            0
          
-         219         382 LOAD_NAME               29 (target)
-                     384 LOAD_ATTR               23 (setter)
+         257         428 PRECALL                  0
+                     432 CALL                     0
          
-         220         394 LOAD_CONST              24 (<code object target, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 219>)
-                     396 MAKE_FUNCTION            0
+         258         442 STORE_NAME              30 (target)
          
-         219         398 PRECALL                  0
-                     402 CALL                     0
+         265         444 LOAD_NAME               30 (target)
+                     446 LOAD_ATTR               23 (setter)
          
-         220         412 STORE_NAME              29 (target)
+         266         456 LOAD_CONST              26 (<code object target, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 265>)
+                     458 MAKE_FUNCTION            0
          
-         242         414 LOAD_NAME               20 (property)
+         265         460 PRECALL                  0
+                     464 CALL                     0
          
-         243         416 LOAD_CONST              25 (<code object continuous_ping, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 242>)
-                     418 MAKE_FUNCTION            0
+         266         474 STORE_NAME              30 (target)
          
-         242         420 PRECALL                  0
-                     424 CALL                     0
+         288         476 LOAD_NAME               20 (property)
          
-         243         434 STORE_NAME              24 (continuous_ping)
+         289         478 LOAD_CONST              27 (<code object continuous_ping, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 288>)
+                     480 MAKE_FUNCTION            0
          
-         246         436 LOAD_NAME               24 (continuous_ping)
-                     438 LOAD_ATTR               23 (setter)
+         288         482 PRECALL                  0
+                     486 CALL                     0
          
-         247         448 LOAD_CONST              26 (<code object continuous_ping, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 246>)
-                     450 MAKE_FUNCTION            0
+         289         496 STORE_NAME              24 (continuous_ping)
          
-         246         452 PRECALL                  0
-                     456 CALL                     0
+         292         498 LOAD_NAME               24 (continuous_ping)
+                     500 LOAD_ATTR               23 (setter)
          
-         247         466 STORE_NAME              24 (continuous_ping)
+         293         510 LOAD_CONST              28 (<code object continuous_ping, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 292>)
+                     512 MAKE_FUNCTION            0
          
-         253         468 LOAD_NAME               20 (property)
+         292         514 PRECALL                  0
+                     518 CALL                     0
          
-         254         470 LOAD_CONST              27 (<code object monitoring, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 253>)
-                     472 MAKE_FUNCTION            0
+         293         528 STORE_NAME              24 (continuous_ping)
          
-         253         474 PRECALL                  0
-                     478 CALL                     0
+         299         530 LOAD_NAME               20 (property)
          
-         254         488 STORE_NAME              30 (monitoring)
+         300         532 LOAD_CONST              29 (<code object monitoring, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 299>)
+                     534 MAKE_FUNCTION            0
          
-         257         490 LOAD_NAME               30 (monitoring)
-                     492 LOAD_ATTR               23 (setter)
+         299         536 PRECALL                  0
+                     540 CALL                     0
          
-         258         502 LOAD_CONST              28 (<code object monitoring, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 257>)
-                     504 MAKE_FUNCTION            0
+         300         550 STORE_NAME              31 (monitoring)
          
-         257         506 PRECALL                  0
-                     510 CALL                     0
+         303         552 LOAD_NAME               31 (monitoring)
+                     554 LOAD_ATTR               23 (setter)
          
-         258         520 STORE_NAME              30 (monitoring)
+         304         564 LOAD_CONST              30 (<code object monitoring, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 303>)
+                     566 MAKE_FUNCTION            0
          
-         264         522 LOAD_NAME               20 (property)
+         303         568 PRECALL                  0
+                     572 CALL                     0
          
-         265         524 LOAD_CONST              29 (<code object history, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 264>)
-                     526 MAKE_FUNCTION            0
+         304         582 STORE_NAME              31 (monitoring)
          
-         264         528 PRECALL                  0
-                     532 CALL                     0
+         310         584 LOAD_NAME               20 (property)
          
-         265         542 STORE_NAME              31 (history)
+         311         586 LOAD_CONST              31 (<code object history, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 310>)
+                     588 MAKE_FUNCTION            0
          
-         268         544 LOAD_NAME               31 (history)
-                     546 LOAD_ATTR               23 (setter)
+         310         590 PRECALL                  0
+                     594 CALL                     0
          
-         269         556 LOAD_CONST              30 (<code object history, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 268>)
-                     558 MAKE_FUNCTION            0
+         311         604 STORE_NAME              32 (history)
          
-         268         560 PRECALL                  0
-                     564 CALL                     0
+         314         606 LOAD_NAME               32 (history)
+                     608 LOAD_ATTR               23 (setter)
          
-         269         574 STORE_NAME              31 (history)
+         315         618 LOAD_CONST              32 (<code object history, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 314>)
+                     620 MAKE_FUNCTION            0
          
-         273         576 LOAD_NAME               20 (property)
+         314         622 PRECALL                  0
+                     626 CALL                     0
          
-         274         578 LOAD_CONST              31 (<code object latest, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 273>)
-                     580 MAKE_FUNCTION            0
+         315         636 STORE_NAME              32 (history)
          
-         273         582 PRECALL                  0
-                     586 CALL                     0
+         319         638 LOAD_NAME               20 (property)
          
-         274         596 STORE_NAME              32 (latest)
+         320         640 LOAD_CONST              33 (<code object latest, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 319>)
+                     642 MAKE_FUNCTION            0
          
-         280         598 LOAD_NAME               20 (property)
+         319         644 PRECALL                  0
+                     648 CALL                     0
          
-         281         600 LOAD_CONST              13 ('return')
-                     602 LOAD_NAME               33 (float)
-                     604 BUILD_TUPLE              2
-                     606 LOAD_CONST              32 (<code object timeout, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 280>)
-                     608 MAKE_FUNCTION            4 (annotations)
+         320         658 STORE_NAME              33 (latest)
          
-         280         610 PRECALL                  0
-                     614 CALL                     0
+         326         660 LOAD_NAME               20 (property)
          
-         281         624 STORE_NAME              34 (timeout)
+         327         662 LOAD_CONST              13 ('return')
+                     664 LOAD_NAME               34 (float)
+                     666 BUILD_TUPLE              2
+                     668 LOAD_CONST              34 (<code object timeout, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 326>)
+                     670 MAKE_FUNCTION            4 (annotations)
          
-         288         626 LOAD_NAME               34 (timeout)
-                     628 LOAD_ATTR               23 (setter)
+         326         672 PRECALL                  0
+                     676 CALL                     0
          
-         289         638 LOAD_CONST              33 (<code object timeout, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 288>)
-                     640 MAKE_FUNCTION            0
+         327         686 STORE_NAME              35 (timeout)
          
-         288         642 PRECALL                  0
-                     646 CALL                     0
+         334         688 LOAD_NAME               35 (timeout)
+                     690 LOAD_ATTR               23 (setter)
          
-         289         656 STORE_NAME              34 (timeout)
+         335         700 LOAD_CONST              35 (<code object timeout, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 334>)
+                     702 MAKE_FUNCTION            0
          
-         311         658 LOAD_NAME               20 (property)
+         334         704 PRECALL                  0
+                     708 CALL                     0
          
-         312         660 LOAD_CONST              34 (<code object results, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 311>)
-                     662 MAKE_FUNCTION            0
+         335         718 STORE_NAME              35 (timeout)
          
-         311         664 PRECALL                  0
-                     668 CALL                     0
+         357         720 LOAD_NAME               20 (property)
          
-         312         678 STORE_NAME              35 (results)
+         358         722 LOAD_CONST              36 (<code object queue, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 357>)
+                     724 MAKE_FUNCTION            0
          
-         315         680 LOAD_NAME               20 (property)
+         357         726 PRECALL                  0
+                     730 CALL                     0
          
-         316         682 LOAD_CONST              35 (<code object runs, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 315>)
-                     684 MAKE_FUNCTION            0
+         358         740 STORE_NAME              36 (queue)
          
-         315         686 PRECALL                  0
-                     690 CALL                     0
+         361         742 LOAD_NAME               36 (queue)
+                     744 LOAD_ATTR               37 (deleter)
          
-         316         700 STORE_NAME              36 (runs)
+         362         754 LOAD_CONST              37 (<code object queue, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 361>)
+                     756 MAKE_FUNCTION            0
          
-         323         702 LOAD_NAME               36 (runs)
-                     704 LOAD_ATTR               23 (setter)
+         361         758 PRECALL                  0
+                     762 CALL                     0
          
-         324         714 LOAD_CONST              36 (<code object runs, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 323>)
-                     716 MAKE_FUNCTION            0
+         362         772 STORE_NAME              36 (queue)
          
-         323         718 PRECALL                  0
-                     722 CALL                     0
+         365         774 LOAD_NAME               20 (property)
          
-         324         732 STORE_NAME              36 (runs)
+         366         776 LOAD_CONST              38 (<code object results, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 365>)
+                     778 MAKE_FUNCTION            0
          
-         354         734 LOAD_NAME               36 (runs)
-                     736 LOAD_ATTR               37 (deleter)
+         365         780 PRECALL                  0
+                     784 CALL                     0
          
-         355         746 LOAD_CONST              37 (<code object runs, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 354>)
-                     748 MAKE_FUNCTION            0
+         366         794 STORE_NAME              38 (results)
          
-         354         750 PRECALL                  0
-                     754 CALL                     0
+         369         796 LOAD_NAME               20 (property)
          
-         355         764 STORE_NAME              36 (runs)
+         370         798 LOAD_CONST              39 (<code object runs, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 369>)
+                     800 MAKE_FUNCTION            0
          
-         361         766 LOAD_NAME               20 (property)
+         369         802 PRECALL                  0
+                     806 CALL                     0
          
-         362         768 LOAD_CONST              38 (<code object status, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 361>)
-                     770 MAKE_FUNCTION            0
+         370         816 STORE_NAME              39 (runs)
          
-         361         772 PRECALL                  0
-                     776 CALL                     0
+         377         818 LOAD_NAME               39 (runs)
+                     820 LOAD_ATTR               23 (setter)
          
-         362         786 STORE_NAME              38 (status)
+         378         830 LOAD_CONST              40 (<code object runs, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 377>)
+                     832 MAKE_FUNCTION            0
          
-         376         788 LOAD_CONST              45 ((False,))
-                     790 LOAD_CONST              39 (<code object create_worker, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 376>)
-                     792 MAKE_FUNCTION            1 (defaults)
-                     794 STORE_NAME              39 (create_worker)
+         377         834 PRECALL                  0
+                     838 CALL                     0
          
-         386         796 LOAD_CONST              40 (<code object ping, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 386>)
-                     798 MAKE_FUNCTION            0
-                     800 STORE_NAME              40 (ping)
+         378         848 STORE_NAME              39 (runs)
          
-         435         802 LOAD_CONST              41 (<code object generate_report, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 435>)
-                     804 MAKE_FUNCTION            0
-                     806 STORE_NAME              41 (generate_report)
+         408         850 LOAD_NAME               39 (runs)
+                     852 LOAD_ATTR               37 (deleter)
          
-         454         808 LOAD_CONST              42 (<code object start, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 454>)
-                     810 MAKE_FUNCTION            0
-                     812 STORE_NAME              42 (start)
+         409         862 LOAD_CONST              41 (<code object runs, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 408>)
+                     864 MAKE_FUNCTION            0
          
-         468         814 LOAD_CONST              43 (<code object stop_monitoring, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 468>)
-                     816 MAKE_FUNCTION            0
-                     818 STORE_NAME              43 (stop_monitoring)
+         408         866 PRECALL                  0
+                     870 CALL                     0
          
-         473         820 LOAD_CONST              44 (<code object stop, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\network.py", line 473>)
-                     822 MAKE_FUNCTION            0
-                     824 STORE_NAME              44 (stop)
-                     826 LOAD_CONST               6 (None)
-                     828 RETURN_VALUE
+         409         880 STORE_NAME              39 (runs)
+         
+         415         882 LOAD_NAME               20 (property)
+         
+         416         884 LOAD_CONST              42 (<code object status, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 415>)
+                     886 MAKE_FUNCTION            0
+         
+         415         888 PRECALL                  0
+                     892 CALL                     0
+         
+         416         902 STORE_NAME              40 (status)
+         
+         430         904 LOAD_CONST              49 ((False,))
+                     906 LOAD_CONST              43 (<code object create_worker, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 430>)
+                     908 MAKE_FUNCTION            1 (defaults)
+                     910 STORE_NAME              41 (create_worker)
+         
+         440         912 LOAD_CONST              44 (<code object ping, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 440>)
+                     914 MAKE_FUNCTION            0
+                     916 STORE_NAME              42 (ping)
+         
+         489         918 LOAD_CONST              45 (<code object generate_report, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 489>)
+                     920 MAKE_FUNCTION            0
+                     922 STORE_NAME              43 (generate_report)
+         
+         508         924 LOAD_CONST              46 (<code object start, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 508>)
+                     926 MAKE_FUNCTION            0
+                     928 STORE_NAME              44 (start)
+         
+         522         930 LOAD_CONST              47 (<code object stop_monitoring, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 522>)
+                     932 MAKE_FUNCTION            0
+                     934 STORE_NAME              45 (stop_monitoring)
+         
+         528         936 LOAD_CONST              48 (<code object stop, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\network.py", line 528>)
+                     938 MAKE_FUNCTION            0
+                     940 STORE_NAME              46 (stop)
+                     942 LOAD_CONST               6 (None)
+                     944 RETURN_VALUE
          consts
             'Ping'
             '\n    A class for performing ping operations on a target.\n\n    Disclaimer:\n        Please use this tool only with the express permission of the target system\'s network administrator,\n        and exercise due care and responsibility in doing so. The author of this tool assumes no liability for any damage,\n        legal or otherwise, caused by its use.\n\n    Note:\n        Pinging a target is not a passive operation and may be detected by intrusion detection systems or firewall logs.\n        Irresponsible use of this tool could potentially cause a denial of service to the target system\'s network\n        services, or your own.\n\n\n    Attributes:\n        target (str):\n            The IP address or hostname to ping.\n\n        auto_run (bool):\n            Whether to automatically ping the ping operation upon initialization.\n\n        timeout (float):\n            The time in seconds to wait for a response before timing out.\n\n        runs (int):\n            The number of times to send a ping request to the target.\n\n    Methods:\n        ping():\n            Runs the ping operation and returns a list of ping times (in milliseconds).\n\n    Usage:\n        ping = Ping(target="google.com", auto_run=True)\n        ping.ping()\n        # [15.132, 15.269, 15.265]\n    '
             0
             ('add_child',)
             'PingPing.Ping'
             False
             None
             5
             3
             1
             256
             'target'
             code
-               argcount  : 11
-               nlocals   : 12
+               argcount  : 12
+               nlocals   : 13
                stacksize : 4
                flags     : 3
                code
                   0x97007c027c005f0000000000000000007c02a001000000000000000000
-                  00000000000000000000006401a6010000ab0100000000000000007d0b7c
-                  067c005f0200000000000000007c017c005f0300000000000000007c0ba0
+                  00000000000000000000006401a6010000ab0100000000000000007d0c7c
+                  067c005f0200000000000000007c017c005f0300000000000000007c0ca0
                   04000000000000000000000000000000000000000064027c006a03000000
                   00000000009b009d02a6010000ab01000000000000000001007c037c005f
-                  0500000000000000007c0ba0040000000000000000000000000000000000
+                  0500000000000000007c0ca0040000000000000000000000000000000000
                   00000064037c006a0500000000000000009b009d02a6010000ab01000000
-                  000000000001007c057c005f0600000000000000007c0ba0040000000000
+                  000000000001007c057c005f0600000000000000007c0ca0040000000000
                   00000000000000000000000000000064047c006a0600000000000000009b
                   009d02a6010000ab01000000000000000001007c047c005f070000000000
-                  0000007c0ba004000000000000000000000000000000000000000064057c
+                  0000007c0ca004000000000000000000000000000000000000000064057c
                   006a0800000000000000009b009d02a6010000ab01000000000000000001
-                  007c077c005f0900000000000000007c0ba0040000000000000000000000
+                  007c077c005f0900000000000000007c0ca0040000000000000000000000
                   00000000000000000064067c006a0900000000000000009b009d02a60100
                   00ab01000000000000000001007c0a7c005f0a000000000000000064077c
-                  005f0b00000000000000007c006a070000000000000000723f7c00a00c00
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  0000007c005f0b00000000000000007c09811c64087c005f0d0000000000
-                  000000741d000000000000000000007c00a6010000ab0100000000000000
-                  007c005f0f00000000000000006e0f64097c005f0d00000000000000006e
-                  0764077c005f0b00000000000000007c006a05000000000000000072167c
-                  00a0100000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000001006407530064075300
-                78           0 RESUME                   0
+                  005f0b000000000000000064077c005f0c00000000000000007c006a0700
+                  000000000000007257741b000000000000000000006a0e00000000000000
+                  00a6000000ab0000000000000000007c005f0c00000000000000007c00a0
+                  0f0000000000000000000000000000000000000000a6000000ab00000000
+                  00000000007c005f0b00000000000000007c09811c64087c005f10000000
+                  00000000007423000000000000000000007c00a6010000ab010000000000
+                  0000007c005f1200000000000000006e0f64097c005f1000000000000000
+                  006e0764077c005f0b00000000000000007c006a05000000000000000072
+                  167c00a0130000000000000000000000000000000000000000a6000000ab
+                  00000000000000000001006407530064075300
+               110           0 RESUME                   0
                
-               109           2 LOAD_FAST                2 (log_device)
+               142           2 LOAD_FAST                2 (log_device)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (log_device)
                
-               110          16 LOAD_FAST                2 (log_device)
+               143          16 LOAD_FAST                2 (log_device)
                             18 LOAD_METHOD              1 (add_child)
                             40 LOAD_CONST               1 ('PingPing.Ping.init')
                             42 PRECALL                  1
                             46 CALL                     1
-                            56 STORE_FAST              11 (log)
+                            56 STORE_FAST              12 (log)
                
-               112          58 LOAD_FAST                6 (runs)
+               145          58 LOAD_FAST                6 (runs)
                             60 LOAD_FAST                0 (self)
                             62 STORE_ATTR               2 (runs)
                
-               114          72 LOAD_FAST                1 (target)
+               147          72 LOAD_FAST                1 (target)
                             74 LOAD_FAST                0 (self)
                             76 STORE_ATTR               3 (target)
                
-               115          86 LOAD_FAST               11 (log)
+               148          86 LOAD_FAST               12 (log)
                             88 LOAD_METHOD              4 (debug)
                            110 LOAD_CONST               2 ('Ping target: ')
                            112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                3 (target)
                            124 FORMAT_VALUE             0
                            126 BUILD_STRING             2
                            128 PRECALL                  1
                            132 CALL                     1
                            142 POP_TOP
                
-               117         144 LOAD_FAST                3 (auto_run)
+               150         144 LOAD_FAST                3 (auto_run)
                            146 LOAD_FAST                0 (self)
                            148 STORE_ATTR               5 (auto_run)
                
-               118         158 LOAD_FAST               11 (log)
+               151         158 LOAD_FAST               12 (log)
                            160 LOAD_METHOD              4 (debug)
                            182 LOAD_CONST               3 ('Auto-run: ')
                            184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                5 (auto_run)
                            196 FORMAT_VALUE             0
                            198 BUILD_STRING             2
                            200 PRECALL                  1
                            204 CALL                     1
                            214 POP_TOP
                
-               120         216 LOAD_FAST                5 (timeout)
+               153         216 LOAD_FAST                5 (timeout)
                            218 LOAD_FAST                0 (self)
                            220 STORE_ATTR               6 (timeout)
                
-               121         230 LOAD_FAST               11 (log)
+               154         230 LOAD_FAST               12 (log)
                            232 LOAD_METHOD              4 (debug)
                            254 LOAD_CONST               4 ('Timeout: ')
                            256 LOAD_FAST                0 (self)
                            258 LOAD_ATTR                6 (timeout)
                            268 FORMAT_VALUE             0
                            270 BUILD_STRING             2
                            272 PRECALL                  1
                            276 CALL                     1
                            286 POP_TOP
                
-               123         288 LOAD_FAST                4 (continuous_ping)
+               156         288 LOAD_FAST                4 (continuous_ping)
                            290 LOAD_FAST                0 (self)
                            292 STORE_ATTR               7 (_Ping__continuous_ping)
                
-               124         302 LOAD_FAST               11 (log)
+               157         302 LOAD_FAST               12 (log)
                            304 LOAD_METHOD              4 (debug)
                            326 LOAD_CONST               5 ('Monitor mode active: ')
                            328 LOAD_FAST                0 (self)
                            330 LOAD_ATTR                8 (continuous_ping)
                            340 FORMAT_VALUE             0
                            342 BUILD_STRING             2
                            344 PRECALL                  1
                            348 CALL                     1
                            358 POP_TOP
                
-               126         360 LOAD_FAST                7 (interval)
+               159         360 LOAD_FAST                7 (interval)
                            362 LOAD_FAST                0 (self)
                            364 STORE_ATTR               9 (interval)
                
-               127         374 LOAD_FAST               11 (log)
+               160         374 LOAD_FAST               12 (log)
                            376 LOAD_METHOD              4 (debug)
                            398 LOAD_CONST               6 ('Ping interval: ')
                            400 LOAD_FAST                0 (self)
                            402 LOAD_ATTR                9 (interval)
                            412 FORMAT_VALUE             0
                            414 BUILD_STRING             2
                            416 PRECALL                  1
                            420 CALL                     1
                            430 POP_TOP
                
-               129         432 LOAD_FAST               10 (debug_mode)
+               162         432 LOAD_FAST               10 (debug_mode)
                            434 LOAD_FAST                0 (self)
                            436 STORE_ATTR              10 (_Ping__debug_mode)
                
-               131         446 LOAD_CONST               7 (None)
+               164         446 LOAD_CONST               7 (None)
                            448 LOAD_FAST                0 (self)
                            450 STORE_ATTR              11 (_Ping__ping_worker)
                
-               133         460 LOAD_FAST                0 (self)
-                           462 LOAD_ATTR                7 (_Ping__continuous_ping)
-                           472 POP_JUMP_FORWARD_IF_FALSE    63 (to 600)
-               
-               134         474 LOAD_FAST                0 (self)
-                           476 LOAD_METHOD             12 (create_worker)
-                           498 PRECALL                  0
-                           502 CALL                     0
-                           512 LOAD_FAST                0 (self)
-                           514 STORE_ATTR              11 (_Ping__ping_worker)
-               
-               135         524 LOAD_FAST                9 (live_mode)
-                           526 POP_JUMP_FORWARD_IF_NONE    28 (to 584)
-               
-               136         528 LOAD_CONST               8 (True)
-                           530 LOAD_FAST                0 (self)
-                           532 STORE_ATTR              13 (live_mode)
-               
-               137         542 LOAD_GLOBAL             29 (NULL + PingMonitor)
-                           554 LOAD_FAST                0 (self)
-                           556 PRECALL                  1
-                           560 CALL                     1
-                           570 LOAD_FAST                0 (self)
-                           572 STORE_ATTR              15 (ping_monitor)
-                           582 JUMP_FORWARD            15 (to 614)
-               
-               140     >>  584 LOAD_CONST               9 (False)
-                           586 LOAD_FAST                0 (self)
-                           588 STORE_ATTR              13 (live_mode)
-                           598 JUMP_FORWARD             7 (to 614)
-               
-               143     >>  600 LOAD_CONST               7 (None)
-                           602 LOAD_FAST                0 (self)
-                           604 STORE_ATTR              11 (_Ping__ping_worker)
-               
-               145     >>  614 LOAD_FAST                0 (self)
-                           616 LOAD_ATTR                5 (auto_run)
-                           626 POP_JUMP_FORWARD_IF_FALSE    22 (to 672)
-               
-               146         628 LOAD_FAST                0 (self)
-                           630 LOAD_METHOD             16 (start)
-                           652 PRECALL                  0
-                           656 CALL                     0
-                           666 POP_TOP
-                           668 LOAD_CONST               7 (None)
-                           670 RETURN_VALUE
+               166         460 LOAD_CONST               7 (None)
+                           462 LOAD_FAST                0 (self)
+                           464 STORE_ATTR              12 (_Ping__queue)
+               
+               168         474 LOAD_FAST                0 (self)
+                           476 LOAD_ATTR                7 (_Ping__continuous_ping)
+                           486 POP_JUMP_FORWARD_IF_FALSE    87 (to 662)
+               
+               169         488 LOAD_GLOBAL             27 (NULL + queue)
+                           500 LOAD_ATTR               14 (Queue)
+                           510 PRECALL                  0
+                           514 CALL                     0
+                           524 LOAD_FAST                0 (self)
+                           526 STORE_ATTR              12 (_Ping__queue)
+               
+               170         536 LOAD_FAST                0 (self)
+                           538 LOAD_METHOD             15 (create_worker)
+                           560 PRECALL                  0
+                           564 CALL                     0
+                           574 LOAD_FAST                0 (self)
+                           576 STORE_ATTR              11 (_Ping__ping_worker)
+               
+               171         586 LOAD_FAST                9 (live_mode)
+                           588 POP_JUMP_FORWARD_IF_NONE    28 (to 646)
+               
+               172         590 LOAD_CONST               8 (True)
+                           592 LOAD_FAST                0 (self)
+                           594 STORE_ATTR              16 (live_mode)
+               
+               173         604 LOAD_GLOBAL             35 (NULL + PingMonitor)
+                           616 LOAD_FAST                0 (self)
+                           618 PRECALL                  1
+                           622 CALL                     1
+                           632 LOAD_FAST                0 (self)
+                           634 STORE_ATTR              18 (ping_monitor)
+                           644 JUMP_FORWARD            15 (to 676)
+               
+               176     >>  646 LOAD_CONST               9 (False)
+                           648 LOAD_FAST                0 (self)
+                           650 STORE_ATTR              16 (live_mode)
+                           660 JUMP_FORWARD             7 (to 676)
+               
+               179     >>  662 LOAD_CONST               7 (None)
+                           664 LOAD_FAST                0 (self)
+                           666 STORE_ATTR              11 (_Ping__ping_worker)
+               
+               181     >>  676 LOAD_FAST                0 (self)
+                           678 LOAD_ATTR                5 (auto_run)
+                           688 POP_JUMP_FORWARD_IF_FALSE    22 (to 734)
+               
+               182         690 LOAD_FAST                0 (self)
+                           692 LOAD_METHOD             19 (start)
+                           714 PRECALL                  0
+                           718 CALL                     0
+                           728 POP_TOP
+                           730 LOAD_CONST               7 (None)
+                           732 RETURN_VALUE
                
-               145     >>  672 LOAD_CONST               7 (None)
-                           674 RETURN_VALUE
+               181     >>  734 LOAD_CONST               7 (None)
+                           736 RETURN_VALUE
                consts
                   '\n        Initializes the Ping object.\n\n        Args:\n            target (str):\n                The IP address or hostname to ping.\n            auto_run (bool):\n                Whether to automatically ping the ping operation upon initialization.\n            timeout (float):\n                The time in seconds to wait for a response before timing out.\n            runs (int):\n                The number of times to send a ping request to the target.\n\n        Raises:\n            TypeError:\n                If any argument is of the wrong type.\n        '
                   'PingPing.Ping.init'
                   'Ping target: '
                   'Auto-run: '
                   'Timeout: '
                   'Monitor mode active: '
                   'Ping interval: '
                   None
                   True
                   False
-               names      ('log_device', 'add_child', 'runs', 'target', 'debug', 'auto_run', 'timeout', '_Ping__continuous_ping', 'continuous_ping', 'interval', '_Ping__debug_mode', '_Ping__ping_worker', 'create_worker', 'live_mode', 'PingMonitor', 'ping_monitor', 'start')
-               varnames   ('self', 'target', 'log_device', 'auto_run', 'continuous_ping', 'timeout', 'runs', 'interval', 'packet_size', 'live_mode', 'debug_mode', 'log')
+               names      ('log_device', 'add_child', 'runs', 'target', 'debug', 'auto_run', 'timeout', '_Ping__continuous_ping', 'continuous_ping', 'interval', '_Ping__debug_mode', '_Ping__ping_worker', '_Ping__queue', 'queue', 'Queue', 'create_worker', 'live_mode', 'PingMonitor', 'ping_monitor', 'start')
+               varnames   ('self', 'target', 'log_device', 'auto_run', 'continuous_ping', 'timeout', 'runs', 'interval', 'packet_size', 'live_mode', 'debug_mode', 'gui_mode', 'log')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       '__init__'
-               firstlineno 78
+               firstlineno 110
                lnotab
-                  0x021f0e012a020e020e013a020e013a020e013a020e013a020e013a020e
-                  020e020e01320104010e012a0310030e020e012cff
+                  0x02200e012a020e020e013a020e013a020e013a020e013a020e013a020e
+                  020e020e020e013001320104010e012a0310030e020e012cff
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               151           0 RESUME                   0
+               187           0 RESUME                   0
                
-               157           2 LOAD_FAST                0 (self)
+               193           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__auto_run)
                             14 RETURN_VALUE
                consts
                   '\n        bool:\n            Whether to automatically ping the ping operation upon initialization.\n        '
                names      ('_Ping__auto_run',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'auto_run'
-               firstlineno 151
+               firstlineno 187
                lnotab 0x0206
             'new'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab020000000000000000730f7405000000000000000000006401a6
                   010000ab01000000000000000082017c017c005f03000000000000000064
                   025300
-               159           0 RESUME                   0
+               195           0 RESUME                   0
                
-               172           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               208           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (new)
                             16 LOAD_GLOBAL              2 (bool)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_TRUE    15 (to 74)
                
-               173          44 LOAD_GLOBAL              5 (NULL + TypeError)
+               209          44 LOAD_GLOBAL              5 (NULL + TypeError)
                             56 LOAD_CONST               1 ('"auto_run" must be of type "bool".')
                             58 PRECALL                  1
                             62 CALL                     1
                             72 RAISE_VARARGS            1
                
-               175     >>   74 LOAD_FAST                1 (new)
+               211     >>   74 LOAD_FAST                1 (new)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (_Ping__auto_run)
                             88 LOAD_CONST               2 (None)
                             90 RETURN_VALUE
                consts
                   '\n        Sets the auto_run attribute.\n\n        Args:\n            new (bool):\n                Whether to automatically ping the ping operation upon initialization.\n\n        Raises:\n            TypeError:\n                If new is not a boolean.\n        '
                   '"auto_run" must be of type "bool".'
                   None
                names      ('isinstance', 'bool', 'TypeError', '_Ping__auto_run')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'auto_run'
-               firstlineno 159
+               firstlineno 195
                lnotab 0x020d2a011e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               177           0 RESUME                   0
+               213           0 RESUME                   0
                
-               179           2 LOAD_FAST                0 (self)
+               215           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__continuous_ping)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_Ping__continuous_ping',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'continuous_ping'
-               firstlineno 177
+               firstlineno 213
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               181           0 RESUME                   0
+               217           0 RESUME                   0
                
-               183           2 LOAD_FAST                0 (self)
+               219           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__interval)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_Ping__interval',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'interval'
-               firstlineno 181
+               firstlineno 217
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab020000000000000000730f7405000000000000000000006401a6
                   010000ab01000000000000000082017c017c005f03000000000000000064
                   005300
-               185           0 RESUME                   0
+               221           0 RESUME                   0
                
-               187           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               223           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (new)
                             16 LOAD_GLOBAL              2 (int)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_TRUE    15 (to 74)
                
-               188          44 LOAD_GLOBAL              5 (NULL + TypeError)
+               224          44 LOAD_GLOBAL              5 (NULL + TypeError)
                             56 LOAD_CONST               1 ('"interval" must be of type "int".')
                             58 PRECALL                  1
                             62 CALL                     1
                             72 RAISE_VARARGS            1
                
-               190     >>   74 LOAD_FAST                1 (new)
+               226     >>   74 LOAD_FAST                1 (new)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (_Ping__interval)
                             88 LOAD_CONST               0 (None)
                             90 RETURN_VALUE
                consts
                   None
                   '"interval" must be of type "int".'
                names      ('isinstance', 'int', 'TypeError', '_Ping__interval')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'interval'
-               firstlineno 185
+               firstlineno 221
                lnotab 0x02022a011e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               192           0 RESUME                   0
+               228           0 RESUME                   0
                
-               194           2 LOAD_FAST                0 (self)
+               230           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (_Ping__gui_mode)
+                            14 RETURN_VALUE
+               consts
+                  None
+               names      ('_Ping__gui_mode',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
+               name       'gui_mode'
+               firstlineno 228
+               lnotab 0x0202
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 4
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c01740200000000000000000000a6
+                  020000ab020000000000000000730f7405000000000000000000006401a6
+                  010000ab01000000000000000082017c017c005f03000000000000000064
+                  005300
+               232           0 RESUME                   0
+               
+               234           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                            14 LOAD_FAST                1 (new)
+                            16 LOAD_GLOBAL              2 (bool)
+                            28 PRECALL                  2
+                            32 CALL                     2
+                            42 POP_JUMP_FORWARD_IF_TRUE    15 (to 74)
+               
+               235          44 LOAD_GLOBAL              5 (NULL + TypeError)
+                            56 LOAD_CONST               1 ('"gui_mode" must be of type "bool".')
+                            58 PRECALL                  1
+                            62 CALL                     1
+                            72 RAISE_VARARGS            1
+               
+               236     >>   74 LOAD_FAST                1 (new)
+                            76 LOAD_FAST                0 (self)
+                            78 STORE_ATTR               3 (_Ping__gui_mode)
+                            88 LOAD_CONST               0 (None)
+                            90 RETURN_VALUE
+               consts
+                  None
+                  '"gui_mode" must be of type "bool".'
+               names      ('isinstance', 'bool', 'TypeError', '_Ping__gui_mode')
+               varnames   ('self', 'new')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
+               name       'gui_mode'
+               firstlineno 232
+               lnotab 0x02022a011e01
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 1
+               flags     : 3
+               code 0x97007c006a0000000000000000005300
+               238           0 RESUME                   0
+               
+               240           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__size)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_Ping__size',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'packet_size'
-               firstlineno 192
+               firstlineno 238
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab020000000000000000730f7405000000000000000000006401a6
                   010000ab01000000000000000082017c0164026b0100000000720f740700
                   0000000000000000006403a6010000ab01000000000000000082017c017c
                   005f04000000000000000064005300
-               196           0 RESUME                   0
+               242           0 RESUME                   0
                
-               199           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               245           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (new)
                             16 LOAD_GLOBAL              2 (int)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_TRUE    15 (to 74)
                
-               200          44 LOAD_GLOBAL              5 (NULL + TypeError)
+               246          44 LOAD_GLOBAL              5 (NULL + TypeError)
                             56 LOAD_CONST               1 ('packet_size must be an integer!')
                             58 PRECALL                  1
                             62 CALL                     1
                             72 RAISE_VARARGS            1
                
-               202     >>   74 LOAD_FAST                1 (new)
+               248     >>   74 LOAD_FAST                1 (new)
                             76 LOAD_CONST               2 (0)
                             78 COMPARE_OP               1 (<=)
                             84 POP_JUMP_FORWARD_IF_FALSE    15 (to 116)
                
-               203          86 LOAD_GLOBAL              7 (NULL + ValueError)
+               249          86 LOAD_GLOBAL              7 (NULL + ValueError)
                             98 LOAD_CONST               3 ('packet_size must be a positive integer')
                            100 PRECALL                  1
                            104 CALL                     1
                            114 RAISE_VARARGS            1
                
-               205     >>  116 LOAD_FAST                1 (new)
+               251     >>  116 LOAD_FAST                1 (new)
                            118 LOAD_FAST                0 (self)
                            120 STORE_ATTR               4 (_Ping__size)
                            130 LOAD_CONST               0 (None)
                            132 RETURN_VALUE
                consts
                   None
                   'packet_size must be an integer!'
                   0
                   'packet_size must be a positive integer'
                names      ('isinstance', 'int', 'TypeError', 'ValueError', '_Ping__size')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'packet_size'
-               firstlineno 196
+               firstlineno 242
                lnotab 0x02032a011e020c011e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               207           0 RESUME                   0
+               253           0 RESUME                   0
                
-               209           2 LOAD_FAST                0 (self)
+               255           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__ping_worker)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_Ping__ping_worker',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'ping_worker'
-               firstlineno 207
+               firstlineno 253
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               211           0 RESUME                   0
+               257           0 RESUME                   0
                
-               217           2 LOAD_FAST                0 (self)
+               263           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__target)
                             14 RETURN_VALUE
                consts
                   '\n        str:\n            The IP address or hostname to ping.\n        '
                names      ('_Ping__target',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'target'
-               firstlineno 211
+               firstlineno 257
                lnotab 0x0206
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab020000000000000000730f7405000000000000000000006401a6
                   010000ab01000000000000000082017c01730f7407000000000000000000
                   006402a6010000ab01000000000000000082017c017c005f040000000000
                   00000064035300
-               219           0 RESUME                   0
+               265           0 RESUME                   0
                
-               234           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               280           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (new)
                             16 LOAD_GLOBAL              2 (str)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_TRUE    15 (to 74)
                
-               235          44 LOAD_GLOBAL              5 (NULL + TypeError)
+               281          44 LOAD_GLOBAL              5 (NULL + TypeError)
                             56 LOAD_CONST               1 ('"target" must be a string')
                             58 PRECALL                  1
                             62 CALL                     1
                             72 RAISE_VARARGS            1
                
-               237     >>   74 LOAD_FAST                1 (new)
+               283     >>   74 LOAD_FAST                1 (new)
                             76 POP_JUMP_FORWARD_IF_TRUE    15 (to 108)
                
-               238          78 LOAD_GLOBAL              7 (NULL + ValueError)
+               284          78 LOAD_GLOBAL              7 (NULL + ValueError)
                             90 LOAD_CONST               2 ('"target" cannot be an empty string')
                             92 PRECALL                  1
                             96 CALL                     1
                            106 RAISE_VARARGS            1
                
-               240     >>  108 LOAD_FAST                1 (new)
+               286     >>  108 LOAD_FAST                1 (new)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               4 (_Ping__target)
                            122 LOAD_CONST               3 (None)
                            124 RETURN_VALUE
                consts
                   '\n        Sets the target attribute.\n\n        Args:\n            new (str):\n                The IP address or hostname to ping.\n\n        Raises:\n            TypeError:\n                If new is not a string.\n            ValueError:\n                If new is an empty string.\n        '
                   '"target" must be a string'
                   '"target" cannot be an empty string'
                   None
                names      ('isinstance', 'str', 'TypeError', 'ValueError', '_Ping__target')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'target'
-               firstlineno 219
+               firstlineno 265
                lnotab 0x020f2a011e0204011e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               242           0 RESUME                   0
+               288           0 RESUME                   0
                
-               244           2 LOAD_FAST                0 (self)
+               290           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__continuous_ping)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_Ping__continuous_ping',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'continuous_ping'
-               firstlineno 242
+               firstlineno 288
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab020000000000000000730f7405000000000000000000006401a6
                   010000ab01000000000000000082017c017c005f03000000000000000064
                   005300
-               246           0 RESUME                   0
+               292           0 RESUME                   0
                
-               248           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               294           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (new)
                             16 LOAD_GLOBAL              2 (bool)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_TRUE    15 (to 74)
                
-               249          44 LOAD_GLOBAL              5 (NULL + TypeError)
+               295          44 LOAD_GLOBAL              5 (NULL + TypeError)
                             56 LOAD_CONST               1 ('"new" must be of type bool!')
                             58 PRECALL                  1
                             62 CALL                     1
                             72 RAISE_VARARGS            1
                
-               251     >>   74 LOAD_FAST                1 (new)
+               297     >>   74 LOAD_FAST                1 (new)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (_Ping__continuous_ping)
                             88 LOAD_CONST               0 (None)
                             90 RETURN_VALUE
                consts
                   None
                   '"new" must be of type bool!'
                names      ('isinstance', 'bool', 'TypeError', '_Ping__continuous_ping')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'continuous_ping'
-               firstlineno 246
+               firstlineno 292
                lnotab 0x02022a011e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               253           0 RESUME                   0
+               299           0 RESUME                   0
                
-               255           2 LOAD_FAST                0 (self)
+               301           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__monitoring)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_Ping__monitoring',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'monitoring'
-               firstlineno 253
+               firstlineno 299
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab020000000000000000730f7405000000000000000000006401a6
                   010000ab01000000000000000082017c017c005f03000000000000000064
                   005300
-               257           0 RESUME                   0
+               303           0 RESUME                   0
                
-               259           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               305           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (new)
                             16 LOAD_GLOBAL              2 (bool)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_TRUE    15 (to 74)
                
-               260          44 LOAD_GLOBAL              5 (NULL + TypeError)
+               306          44 LOAD_GLOBAL              5 (NULL + TypeError)
                             56 LOAD_CONST               1 ('"monitoring" must be of type bool"')
                             58 PRECALL                  1
                             62 CALL                     1
                             72 RAISE_VARARGS            1
                
-               262     >>   74 LOAD_FAST                1 (new)
+               308     >>   74 LOAD_FAST                1 (new)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (_Ping__monitoring)
                             88 LOAD_CONST               0 (None)
                             90 RETURN_VALUE
                consts
                   None
                   '"monitoring" must be of type bool"'
                names      ('isinstance', 'bool', 'TypeError', '_Ping__monitoring')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'monitoring'
-               firstlineno 257
+               firstlineno 303
                lnotab 0x02022a011e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               264           0 RESUME                   0
+               310           0 RESUME                   0
                
-               266           2 LOAD_FAST                0 (self)
+               312           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__history)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_Ping__history',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'history'
-               firstlineno 264
+               firstlineno 310
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab020000000000000000730f7405000000000000000000006401a6
                   010000ab010000000000000000820164005300
-               268           0 RESUME                   0
+               314           0 RESUME                   0
                
-               270           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               316           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (new)
                             16 LOAD_GLOBAL              2 (list)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_TRUE    15 (to 74)
                
-               271          44 LOAD_GLOBAL              5 (NULL + TypeError)
+               317          44 LOAD_GLOBAL              5 (NULL + TypeError)
                             56 LOAD_CONST               1 ('"new" must be of type list!')
                             58 PRECALL                  1
                             62 CALL                     1
                             72 RAISE_VARARGS            1
                
-               270     >>   74 LOAD_CONST               0 (None)
+               316     >>   74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
                   '"new" must be of type list!'
                names      ('isinstance', 'list', 'TypeError')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'history'
-               firstlineno 268
+               firstlineno 314
                lnotab 0x02022a011eff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970009007c006a00000000000000000064011900000000000000000064
                   011900000000000000000053002300740200000000000000000000240072
                   0a01007c006a0000000000000000006302590053007700780359007701
-               273           0 RESUME                   0
+               319           0 RESUME                   0
                
-               275           2 NOP
+               321           2 NOP
                
-               276           4 LOAD_FAST                0 (self)
+               322           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (history)
                             16 LOAD_CONST               1 (-1)
                             18 BINARY_SUBSCR
                             28 LOAD_CONST               1 (-1)
                             30 BINARY_SUBSCR
                             40 RETURN_VALUE
                        >>   42 PUSH_EXC_INFO
                
-               277          44 LOAD_GLOBAL              2 (TypeError)
+               323          44 LOAD_GLOBAL              2 (TypeError)
                             56 CHECK_EXC_MATCH
                             58 POP_JUMP_FORWARD_IF_FALSE    10 (to 80)
                             60 POP_TOP
                
-               278          62 LOAD_FAST                0 (self)
+               324          62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                0 (history)
                             74 SWAP                     2
                             76 POP_EXCEPT
                             78 RETURN_VALUE
                
-               277     >>   80 RERAISE                  0
+               323     >>   80 RERAISE                  0
                        >>   82 COPY                     3
                             84 POP_EXCEPT
                             86 RERAISE                  1
                ExceptionTable:
                  4 to 38 -> 42 [0]
                  42 to 74 -> 82 [1] lasti
                  80 to 80 -> 82 [1] lasti
                consts
                   None
                   -1
                names      ('history', 'TypeError')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'latest'
-               firstlineno 273
+               firstlineno 319
                lnotab 0x020202012801120112ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               280           0 RESUME                   0
+               326           0 RESUME                   0
                
-               286           2 LOAD_FAST                0 (self)
+               332           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__timeout)
                             14 RETURN_VALUE
                consts
                   '\n        float:\n            The time in seconds to wait for a response before timing out.\n        '
                names      ('_Ping__timeout',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'timeout'
-               firstlineno 280
+               firstlineno 326
                lnotab 0x0206
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000007c0174020000000000000000000074
                   04000000000000000000006602a6020000ab020000000000000000730f74
                   07000000000000000000006401a6010000ab01000000000000000082017c
                   0164026b0100000000720f7409000000000000000000006403a6010000ab
                   01000000000000000082017403000000000000000000007c01a6010000ab
                   0100000000000000007c005f05000000000000000064045300
-               288           0 RESUME                   0
+               334           0 RESUME                   0
                
-               303           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               349           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (new)
                             16 LOAD_GLOBAL              2 (int)
                             28 LOAD_GLOBAL              4 (float)
                             40 BUILD_TUPLE              2
                             42 PRECALL                  2
                             46 CALL                     2
                             56 POP_JUMP_FORWARD_IF_TRUE    15 (to 88)
                
-               304          58 LOAD_GLOBAL              7 (NULL + TypeError)
+               350          58 LOAD_GLOBAL              7 (NULL + TypeError)
                             70 LOAD_CONST               1 ('"timeout" must be a float or an integer')
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RAISE_VARARGS            1
                
-               306     >>   88 LOAD_FAST                1 (new)
+               352     >>   88 LOAD_FAST                1 (new)
                             90 LOAD_CONST               2 (0)
                             92 COMPARE_OP               1 (<=)
                             98 POP_JUMP_FORWARD_IF_FALSE    15 (to 130)
                
-               307         100 LOAD_GLOBAL              9 (NULL + ValueError)
+               353         100 LOAD_GLOBAL              9 (NULL + ValueError)
                            112 LOAD_CONST               3 ('"timeout" must be positive')
                            114 PRECALL                  1
                            118 CALL                     1
                            128 RAISE_VARARGS            1
                
-               309     >>  130 LOAD_GLOBAL              3 (NULL + int)
+               355     >>  130 LOAD_GLOBAL              3 (NULL + int)
                            142 LOAD_FAST                1 (new)
                            144 PRECALL                  1
                            148 CALL                     1
                            158 LOAD_FAST                0 (self)
                            160 STORE_ATTR               5 (_Ping__timeout)
                            170 LOAD_CONST               4 (None)
                            172 RETURN_VALUE
@@ -1369,59 +1501,106 @@
                   0
                   '"timeout" must be positive'
                   None
                names      ('isinstance', 'int', 'float', 'TypeError', 'ValueError', '_Ping__timeout')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'timeout'
-               firstlineno 288
+               firstlineno 334
                lnotab 0x020f38011e020c011e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               311           0 RESUME                   0
+               357           0 RESUME                   0
+               
+               359           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (_Ping__queue)
+                            14 RETURN_VALUE
+               consts
+                  None
+               names      ('_Ping__queue',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
+               name       'queue'
+               firstlineno 357
+               lnotab 0x0202
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 2
+               flags     : 3
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  00000000000000a6000000ab0000000000000000005300
+               361           0 RESUME                   0
+               
+               363           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (_Ping__queue)
+                            14 LOAD_METHOD              1 (empty)
+                            36 PRECALL                  0
+                            40 CALL                     0
+                            50 RETURN_VALUE
+               consts
+                  None
+               names      ('_Ping__queue', 'empty')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
+               name       'queue'
+               firstlineno 361
+               lnotab 0x0202
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 1
+               flags     : 3
+               code 0x97007c006a0000000000000000005300
+               365           0 RESUME                   0
                
-               313           2 LOAD_FAST                0 (self)
+               367           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__results)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_Ping__results',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'results'
-               firstlineno 311
+               firstlineno 365
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               315           0 RESUME                   0
+               369           0 RESUME                   0
                
-               321           2 LOAD_FAST                0 (self)
+               375           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__runs)
                             14 RETURN_VALUE
                consts
                   '\n       int:\n           The number of times to send a ping request to the target.\n       '
                names      ('_Ping__runs',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'runs'
-               firstlineno 315
+               firstlineno 369
                lnotab 0x0206
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
@@ -1433,70 +1612,70 @@
                   000000000000006403a6010000ab01000000000000000082017c02a00200
                   000000000000000000000000000000000000006404a6010000ab01000000
                   000000000001007c0164056b0100000000720f740d000000000000000000
                   006406a6010000ab01000000000000000082017c017c005f070000000000
                   0000007c02a002000000000000000000000000000000000000000064077c
                   006a0700000000000000009b009d02a6010000ab01000000000000000001
                   0064085300
-               323           0 RESUME                   0
+               377           0 RESUME                   0
                
-               338           2 LOAD_FAST                0 (self)
+               392           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (log_device)
                             14 LOAD_METHOD              1 (add_child)
                             36 LOAD_CONST               1 ('PingPing.Ping.PropSet:run')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               2 (log)
                
-               340          54 LOAD_FAST                2 (log)
+               394          54 LOAD_FAST                2 (log)
                             56 LOAD_METHOD              2 (debug)
                             78 LOAD_CONST               2 ('Received new value of ')
                             80 LOAD_FAST                1 (new)
                             82 FORMAT_VALUE             0
                             84 BUILD_STRING             2
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_TOP
                
-               342         102 LOAD_GLOBAL              7 (NULL + isinstance)
+               396         102 LOAD_GLOBAL              7 (NULL + isinstance)
                            114 LOAD_FAST                1 (new)
                            116 LOAD_GLOBAL              8 (int)
                            128 PRECALL                  2
                            132 CALL                     2
                            142 POP_JUMP_FORWARD_IF_TRUE    15 (to 174)
                
-               343         144 LOAD_GLOBAL             11 (NULL + TypeError)
+               397         144 LOAD_GLOBAL             11 (NULL + TypeError)
                            156 LOAD_CONST               3 ("'runs' must be an integer!")
                            158 PRECALL                  1
                            162 CALL                     1
                            172 RAISE_VARARGS            1
                
-               345     >>  174 LOAD_FAST                2 (log)
+               399     >>  174 LOAD_FAST                2 (log)
                            176 LOAD_METHOD              2 (debug)
                            198 LOAD_CONST               4 ('New value seems valid, setting...')
                            200 PRECALL                  1
                            204 CALL                     1
                            214 POP_TOP
                
-               347         216 LOAD_FAST                1 (new)
+               401         216 LOAD_FAST                1 (new)
                            218 LOAD_CONST               5 (0)
                            220 COMPARE_OP               1 (<=)
                            226 POP_JUMP_FORWARD_IF_FALSE    15 (to 258)
                
-               348         228 LOAD_GLOBAL             13 (NULL + ValueError)
+               402         228 LOAD_GLOBAL             13 (NULL + ValueError)
                            240 LOAD_CONST               6 ("'runs' must be positive")
                            242 PRECALL                  1
                            246 CALL                     1
                            256 RAISE_VARARGS            1
                
-               350     >>  258 LOAD_FAST                1 (new)
+               404     >>  258 LOAD_FAST                1 (new)
                            260 LOAD_FAST                0 (self)
                            262 STORE_ATTR               7 (_Ping__runs)
                
-               352         272 LOAD_FAST                2 (log)
+               406         272 LOAD_FAST                2 (log)
                            274 LOAD_METHOD              2 (debug)
                            296 LOAD_CONST               7 ('Value of Ping().runs: ')
                            298 LOAD_FAST                0 (self)
                            300 LOAD_ATTR                7 (_Ping__runs)
                            310 FORMAT_VALUE             0
                            312 BUILD_STRING             2
                            314 PRECALL                  1
@@ -1514,158 +1693,158 @@
                   "'runs' must be positive"
                   'Value of Ping().runs: '
                   None
                names      ('log_device', 'add_child', 'debug', 'isinstance', 'int', 'TypeError', 'ValueError', '_Ping__runs')
                varnames   ('self', 'new', 'log')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'runs'
-               firstlineno 323
+               firstlineno 377
                lnotab 0x020f340230022a011e022a020c011e020e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064025300
-               354           0 RESUME                   0
+               408           0 RESUME                   0
                
-               359           2 LOAD_CONST               1 (3)
+               413           2 LOAD_CONST               1 (3)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (_Ping__runs)
                             16 LOAD_CONST               2 (None)
                             18 RETURN_VALUE
                consts
                   '\n        Resets the runs attribute to its default value.\n        '
                   3
                   None
                names      ('_Ping__runs',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'runs'
-               firstlineno 354
+               firstlineno 408
                lnotab 0x0205
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a0000000000000000007201090064017c006a010000000000
                   00000064027c006a0200000000000000006a030000000000000000a00400
                   00000000000000000000000000000000000000a6000000ab000000000000
                   000000720264036e016404690164059c0269017d0164005300
-               361           0 RESUME                   0
+               415           0 RESUME                   0
                
-               363           2 LOAD_FAST                0 (self)
+               417           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Ping__debug_mode)
                             14 POP_JUMP_FORWARD_IF_FALSE     1 (to 18)
                
-               364          16 NOP
+               418          16 NOP
                
-               366     >>   18 LOAD_CONST               1 ('continuous_mode')
+               420     >>   18 LOAD_CONST               1 ('continuous_mode')
                
-               367          20 LOAD_FAST                0 (self)
+               421          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                1 (continuous_ping)
                
-               370          32 LOAD_CONST               2 ('alive')
+               424          32 LOAD_CONST               2 ('alive')
                             34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                2 (ping_worker)
                             46 LOAD_ATTR                3 (thread)
                             56 LOAD_METHOD              4 (is_alive)
                             78 PRECALL                  0
                             82 CALL                     0
                             92 POP_JUMP_FORWARD_IF_FALSE     2 (to 98)
                             94 LOAD_CONST               3 (True)
                             96 JUMP_FORWARD             1 (to 100)
                        >>   98 LOAD_CONST               4 (False)
                
-               369     >>  100 BUILD_MAP                1
+               423     >>  100 BUILD_MAP                1
                
-               366         102 LOAD_CONST               5 (('enabled', 'state'))
+               420         102 LOAD_CONST               5 (('enabled', 'state'))
                            104 BUILD_CONST_KEY_MAP      2
                
-               365         106 BUILD_MAP                1
+               419         106 BUILD_MAP                1
                            108 STORE_FAST               1 (status)
                            110 LOAD_CONST               0 (None)
                            112 RETURN_VALUE
                consts
                   None
                   'continuous_mode'
                   'alive'
                   True
                   False
                   ('enabled', 'state')
                names      ('_Ping__debug_mode', 'continuous_ping', 'ping_worker', 'thread', 'is_alive')
                varnames   ('self', 'status')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'status'
-               firstlineno 361
+               firstlineno 415
                lnotab 0x02020e01020202010c0344ff02fd04ff
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x9700640164026c006d017d0201007c006a02000000000000000081127c
                   01731074070000000000000000000064036404a6020000ab020000000000
                   000000820102007c027c00a6010000ab0100000000000000007c005f0400
                   000000000000007c006a0200000000000000005300
-               376           0 RESUME                   0
+               430           0 RESUME                   0
                
-               377           2 LOAD_CONST               1 (0)
+               431           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('PingWorker',))
-                             6 IMPORT_NAME              0 (ping_ping.utils.workers)
+                             6 IMPORT_NAME              0 (ping_stat.utils.workers)
                              8 IMPORT_FROM              1 (PingWorker)
                             10 STORE_FAST               2 (PingWorker)
                             12 POP_TOP
                
-               378          14 LOAD_FAST                0 (self)
+               432          14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                2 (ping_worker)
                             26 POP_JUMP_FORWARD_IF_NONE    18 (to 64)
                             28 LOAD_FAST                1 (reset)
                             30 POP_JUMP_FORWARD_IF_TRUE    16 (to 64)
                
-               379          32 LOAD_GLOBAL              7 (NULL + RedundantWorkOrderError)
+               433          32 LOAD_GLOBAL              7 (NULL + RedundantWorkOrderError)
                             44 LOAD_CONST               3 ('ping_worker')
                             46 LOAD_CONST               4 ('Try resetting the ping worker.')
                             48 PRECALL                  2
                             52 CALL                     2
                             62 RAISE_VARARGS            1
                
-               381     >>   64 PUSH_NULL
+               435     >>   64 PUSH_NULL
                             66 LOAD_FAST                2 (PingWorker)
                             68 LOAD_FAST                0 (self)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 LOAD_FAST                0 (self)
                             86 STORE_ATTR               4 (_Ping__ping_worker)
                
-               383          96 LOAD_FAST                0 (self)
+               437          96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                2 (ping_worker)
                            108 RETURN_VALUE
                consts
                   None
                   0
                   ('PingWorker',)
                   'ping_worker'
                   'Try resetting the ping worker.'
-               names      ('ping_ping.utils.workers', 'PingWorker', 'ping_worker', 'RedundantWorkOrderError', '_Ping__ping_worker')
+               names      ('ping_stat.utils.workers', 'PingWorker', 'ping_worker', 'RedundantWorkOrderError', '_Ping__ping_worker')
                varnames   ('self', 'reset', 'PingWorker')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'create_worker'
-               firstlineno 376
+               firstlineno 430
                lnotab 0x02010c01120120022002
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 10
                flags     : 3
                code
@@ -1680,125 +1859,125 @@
                   007c006a0600000000000000007415000000000000000000007c006a0700
                   00000000000000a6010000ab010000000000000000ac05a6030000ab0300
                   00000000000000a6010000ab010000000000000000010074170000000000
                   00000000007c006a0c0000000000000000a6010000ab0100000000000000
                   0001008c9f741b000000000000000000007c01a6010000ab010000000000
                   00000064066b020000000072087c016407190000000000000000007d017c
                   017c005f0e00000000000000007c015300
-               386           0 RESUME                   0
+               440           0 RESUME                   0
                
-               407           2 BUILD_LIST               0
+               461           2 BUILD_LIST               0
                              4 STORE_FAST               1 (pings)
                
-               409           6 LOAD_GLOBAL              1 (NULL + range)
+               463           6 LOAD_GLOBAL              1 (NULL + range)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (runs)
                             30 PRECALL                  1
                             34 CALL                     1
                             44 GET_ITER
                        >>   46 FOR_ITER               158 (to 364)
                             48 STORE_FAST               2 (_)
                
-               410          50 LOAD_FAST                0 (self)
+               464          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                2 (log_device)
                             62 LOAD_METHOD              3 (add_child)
                             84 LOAD_CONST               1 ('PingPing.Ping.ping')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 STORE_FAST               3 (log)
                
-               411         102 LOAD_FAST                3 (log)
+               465         102 LOAD_FAST                3 (log)
                            104 LOAD_METHOD              4 (debug)
                            126 LOAD_CONST               2 ('Pinging ')
                            128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                5 (target)
                            140 FORMAT_VALUE             0
                            142 LOAD_CONST               3 (' with a payload of ')
                            144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                6 (packet_size)
                            156 FORMAT_VALUE             0
                            158 LOAD_CONST               4 (' bytes and a titmeout of ')
                
-               412         160 LOAD_FAST                0 (self)
+               466         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                7 (timeout)
                
-               411         172 FORMAT_VALUE             0
+               465         172 FORMAT_VALUE             0
                            174 BUILD_STRING             6
                            176 PRECALL                  1
                            180 CALL                     1
                            190 POP_TOP
                
-               417         192 LOAD_FAST                1 (pings)
+               471         192 LOAD_FAST                1 (pings)
                            194 LOAD_METHOD              8 (append)
                
-               418         216 LOAD_GLOBAL             19 (NULL + _ping)
+               472         216 LOAD_GLOBAL             19 (NULL + _ping)
                
-               419         228 LOAD_FAST                0 (self)
+               473         228 LOAD_FAST                0 (self)
                            230 LOAD_ATTR                5 (target)
                
-               420         240 LOAD_FAST                0 (self)
+               474         240 LOAD_FAST                0 (self)
                            242 LOAD_ATTR                6 (packet_size)
                
-               421         252 LOAD_GLOBAL             21 (NULL + int)
+               475         252 LOAD_GLOBAL             21 (NULL + int)
                            264 LOAD_FAST                0 (self)
                            266 LOAD_ATTR                7 (timeout)
                            276 PRECALL                  1
                            280 CALL                     1
                
-               418         290 KW_NAMES                 5
+               472         290 KW_NAMES                 5
                            292 PRECALL                  3
                            296 CALL                     3
                
-               417         306 PRECALL                  1
+               471         306 PRECALL                  1
                            310 CALL                     1
                            320 POP_TOP
                
-               425         322 LOAD_GLOBAL             23 (NULL + sleep)
+               479         322 LOAD_GLOBAL             23 (NULL + sleep)
                            334 LOAD_FAST                0 (self)
                            336 LOAD_ATTR               12 (interval)
                            346 PRECALL                  1
                            350 CALL                     1
                            360 POP_TOP
                            362 JUMP_BACKWARD          159 (to 46)
                
-               427     >>  364 LOAD_GLOBAL             27 (NULL + len)
+               481     >>  364 LOAD_GLOBAL             27 (NULL + len)
                            376 LOAD_FAST                1 (pings)
                            378 PRECALL                  1
                            382 CALL                     1
                            392 LOAD_CONST               6 (1)
                            394 COMPARE_OP               2 (==)
                            400 POP_JUMP_FORWARD_IF_FALSE     8 (to 418)
                
-               428         402 LOAD_FAST                1 (pings)
+               482         402 LOAD_FAST                1 (pings)
                            404 LOAD_CONST               7 (0)
                            406 BINARY_SUBSCR
                            416 STORE_FAST               1 (pings)
                
-               430     >>  418 LOAD_FAST                1 (pings)
+               484     >>  418 LOAD_FAST                1 (pings)
                            420 LOAD_FAST                0 (self)
                            422 STORE_ATTR              14 (_Ping__results)
                
-               432         432 LOAD_FAST                1 (pings)
+               486         432 LOAD_FAST                1 (pings)
                            434 RETURN_VALUE
                consts
                   "\n        Runs the ping operation and returns a list of ping times (in milliseconds).\n\n        Returns:\n            list or float:\n\n                - If the 'runs' attribute is greater than 1, returns a list of ping times (in milliseconds).\n\n                - If the 'runs' attribute is 1, returns a single ping time (in milliseconds).\n\n        Raises:\n            PingError:\n                If the ping operation failed.\n\n        "
                   'PingPing.Ping.ping'
                   'Pinging '
                   ' with a payload of '
                   ' bytes and a titmeout of '
                   ('size', 'timeout')
                   1
                   0
                names      ('range', 'runs', 'log_device', 'add_child', 'debug', 'target', 'packet_size', 'timeout', 'append', '_ping', 'int', 'sleep', 'interval', 'len', '_Ping__results')
                varnames   ('self', 'pings', '_', 'log')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'ping'
-               firstlineno 386
+               firstlineno 440
                lnotab
                   0x021504022c0134013a010cff140618010c010c010c0126fd10ff10082a
                   02260110020e02
             code
                argcount  : 1
                nlocals   : 8
                stacksize : 8
@@ -1809,90 +1988,90 @@
                   00ab0100000000000000007d037403000000000000000000007c02a60100
                   00ab0100000000000000007d047405000000000000000000007c01a60100
                   00ab0100000000000000007d057407000000000000000000007c01a60100
                   00ab0100000000000000007d067409000000000000000000007c01a60100
                   00ab0100000000000000007d077c037c047c077c067c05740b0000000000
                   00000000007c01a6010000ab01000000000000000064039c0464049c0353
                   00
-               435           0 RESUME                   0
+               489           0 RESUME                   0
                
-               436           2 LOAD_GLOBAL              1 (NULL + gather_times)
+               490           2 LOAD_GLOBAL              1 (NULL + gather_times)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_CONST               1 (True)
                             18 KW_NAMES                 2
                             20 PRECALL                  2
                             24 CALL                     2
                             34 UNPACK_SEQUENCE          2
                             38 STORE_FAST               1 (successful)
                             40 STORE_FAST               2 (failed)
                
-               437          42 LOAD_GLOBAL              3 (NULL + len)
+               491          42 LOAD_GLOBAL              3 (NULL + len)
                             54 LOAD_FAST                1 (successful)
                             56 PRECALL                  1
                             60 CALL                     1
                             70 STORE_FAST               3 (num_successful)
                
-               438          72 LOAD_GLOBAL              3 (NULL + len)
+               492          72 LOAD_GLOBAL              3 (NULL + len)
                             84 LOAD_FAST                2 (failed)
                             86 PRECALL                  1
                             90 CALL                     1
                            100 STORE_FAST               4 (num_failed)
                
-               439         102 LOAD_GLOBAL              5 (NULL + mean)
+               493         102 LOAD_GLOBAL              5 (NULL + mean)
                            114 LOAD_FAST                1 (successful)
                            116 PRECALL                  1
                            120 CALL                     1
                            130 STORE_FAST               5 (ping_mean)
                
-               440         132 LOAD_GLOBAL              7 (NULL + max)
+               494         132 LOAD_GLOBAL              7 (NULL + max)
                            144 LOAD_FAST                1 (successful)
                            146 PRECALL                  1
                            150 CALL                     1
                            160 STORE_FAST               6 (max_time)
                
-               441         162 LOAD_GLOBAL              9 (NULL + min)
+               495         162 LOAD_GLOBAL              9 (NULL + min)
                            174 LOAD_FAST                1 (successful)
                            176 PRECALL                  1
                            180 CALL                     1
                            190 STORE_FAST               7 (min_time)
                
-               444         192 LOAD_FAST                3 (num_successful)
+               498         192 LOAD_FAST                3 (num_successful)
                
-               445         194 LOAD_FAST                4 (num_failed)
+               499         194 LOAD_FAST                4 (num_failed)
                
-               447         196 LOAD_FAST                7 (min_time)
+               501         196 LOAD_FAST                7 (min_time)
                
-               448         198 LOAD_FAST                6 (max_time)
+               502         198 LOAD_FAST                6 (max_time)
                
-               449         200 LOAD_FAST                5 (ping_mean)
+               503         200 LOAD_FAST                5 (ping_mean)
                
-               450         202 LOAD_GLOBAL             11 (NULL + sum)
+               504         202 LOAD_GLOBAL             11 (NULL + sum)
                            214 LOAD_FAST                1 (successful)
                            216 PRECALL                  1
                            220 CALL                     1
                
-               446         230 LOAD_CONST               3 (('min', 'max', 'mean', 'average'))
+               500         230 LOAD_CONST               3 (('min', 'max', 'mean', 'average'))
                            232 BUILD_CONST_KEY_MAP      4
                
-               443         234 LOAD_CONST               4 (('pings_returned', 'pings_failed', 'wait_time'))
+               497         234 LOAD_CONST               4 (('pings_returned', 'pings_failed', 'wait_time'))
                            236 BUILD_CONST_KEY_MAP      3
                            238 RETURN_VALUE
                consts
                   None
                   True
                   ('count_timeout_time_for_fails',)
                   ('min', 'max', 'mean', 'average')
                   ('pings_returned', 'pings_failed', 'wait_time')
                names      ('gather_times', 'len', 'mean', 'max', 'min', 'sum')
                varnames   ('self', 'successful', 'failed', 'num_successful', 'num_failed', 'ping_mean', 'max_time', 'min_time')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'generate_report'
-               firstlineno 435
+               firstlineno 489
                lnotab 0x020128011e011e011e011e011e03020102020201020102011cfc04fd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
@@ -1901,180 +2080,189 @@
                   00000000007c006a0100000000000000006a0400000000000000006a0500
                   00000000000000a6010000ab01000000000000000082017c006a01000000
                   0000000000a0060000000000000000000000000000000000000000a60000
                   00ab00000000000000000001007c006a070000000000000000722464027c
                   005f0800000000000000007c006a090000000000000000a0060000000000
                   000000000000000000000000000000a6000000ab00000000000000000001
                   00640053006400530064005300
-               454           0 RESUME                   0
+               508           0 RESUME                   0
                
-               457           2 LOAD_FAST                0 (self)
+               511           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (continuous_ping)
                             14 POP_JUMP_FORWARD_IF_FALSE   114 (to 244)
                
-               458          16 LOAD_FAST                0 (self)
+               512          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (ping_worker)
                             28 LOAD_ATTR                2 (status)
                             38 LOAD_CONST               1 ('started')
                             40 BINARY_SUBSCR
                             50 POP_JUMP_FORWARD_IF_FALSE    30 (to 112)
                
-               459          52 LOAD_GLOBAL              7 (NULL + WorkerAlreadyStartedError)
+               513          52 LOAD_GLOBAL              7 (NULL + WorkerAlreadyStartedError)
                             64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                1 (ping_worker)
                             76 LOAD_ATTR                4 (thread)
                             86 LOAD_ATTR                5 (name)
                             96 PRECALL                  1
                            100 CALL                     1
                            110 RAISE_VARARGS            1
                
-               461     >>  112 LOAD_FAST                0 (self)
+               515     >>  112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                1 (ping_worker)
                            124 LOAD_METHOD              6 (start)
                            146 PRECALL                  0
                            150 CALL                     0
                            160 POP_TOP
                
-               463         162 LOAD_FAST                0 (self)
+               517         162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                7 (live_mode)
                            174 POP_JUMP_FORWARD_IF_FALSE    36 (to 248)
                
-               464         176 LOAD_CONST               2 (True)
+               518         176 LOAD_CONST               2 (True)
                            178 LOAD_FAST                0 (self)
                            180 STORE_ATTR               8 (monitoring)
                
-               465         190 LOAD_FAST                0 (self)
+               519         190 LOAD_FAST                0 (self)
                            192 LOAD_ATTR                9 (ping_monitor)
                            202 LOAD_METHOD              6 (start)
                            224 PRECALL                  0
                            228 CALL                     0
                            238 POP_TOP
                            240 LOAD_CONST               0 (None)
                            242 RETURN_VALUE
                
-               457     >>  244 LOAD_CONST               0 (None)
+               511     >>  244 LOAD_CONST               0 (None)
                            246 RETURN_VALUE
                
-               463     >>  248 LOAD_CONST               0 (None)
+               517     >>  248 LOAD_CONST               0 (None)
                            250 RETURN_VALUE
                consts
                   None
                   'started'
                   True
                names      ('continuous_ping', 'ping_worker', 'status', 'WorkerAlreadyStartedError', 'thread', 'name', 'start', 'live_mode', 'monitoring', 'ping_monitor')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'start'
-               firstlineno 454
+               firstlineno 508
                lnotab 0x02030e0124013c0232020e010e0136f80406
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
-                  0x9700640161007c006a0100000000000000006a020000000000000000a0
-                  030000000000000000000000000000000000000000a6000000ab00000000
-                  0000000000010064005300
-               468           0 RESUME                   0
+                  0x9700640161007c006a010000000000000000a002000000000000000000
+                  0000000000000000000000a6000000ab00000000000000000001007c006a
+                  0100000000000000006a030000000000000000a004000000000000000000
+                  0000000000000000000000a6000000ab0000000000000000000100640053
+                  00
+               522           0 RESUME                   0
                
-               470           2 LOAD_CONST               1 (False)
+               524           2 LOAD_CONST               1 (False)
                              4 STORE_GLOBAL             0 (monitoring)
                
-               471           6 LOAD_FAST                0 (self)
+               525           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                1 (ping_monitor)
-                            18 LOAD_ATTR                2 (thread)
-                            28 LOAD_METHOD              3 (join)
-                            50 PRECALL                  0
-                            54 CALL                     0
-                            64 POP_TOP
-                            66 LOAD_CONST               0 (None)
-                            68 RETURN_VALUE
+                            18 LOAD_METHOD              2 (stop)
+                            40 PRECALL                  0
+                            44 CALL                     0
+                            54 POP_TOP
+               
+               526          56 LOAD_FAST                0 (self)
+                            58 LOAD_ATTR                1 (ping_monitor)
+                            68 LOAD_ATTR                3 (thread)
+                            78 LOAD_METHOD              4 (join)
+                           100 PRECALL                  0
+                           104 CALL                     0
+                           114 POP_TOP
+                           116 LOAD_CONST               0 (None)
+                           118 RETURN_VALUE
                consts
                   None
                   False
-               names      ('monitoring', 'ping_monitor', 'thread', 'join')
+               names      ('monitoring', 'ping_monitor', 'stop', 'thread', 'join')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'stop_monitoring'
-               firstlineno 468
-               lnotab 0x02020401
+               firstlineno 522
+               lnotab 0x020204013201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a00000000000000000072147c00a001000000000000000000
                   0000000000000000000000a6000000ab000000000000000000010064017c
                   005f0200000000000000007c006a030000000000000000a0040000000000
                   000000000000000000000000000000a6000000ab00000000000000000001
                   0064005300
-               473           0 RESUME                   0
+               528           0 RESUME                   0
                
-               474           2 LOAD_FAST                0 (self)
+               529           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (live_mode)
                             14 POP_JUMP_FORWARD_IF_FALSE    20 (to 56)
                
-               475          16 LOAD_FAST                0 (self)
+               530          16 LOAD_FAST                0 (self)
                             18 LOAD_METHOD              1 (stop_monitoring)
                             40 PRECALL                  0
                             44 CALL                     0
                             54 POP_TOP
                
-               477     >>   56 LOAD_CONST               1 (False)
+               532     >>   56 LOAD_CONST               1 (False)
                             58 LOAD_FAST                0 (self)
                             60 STORE_ATTR               2 (monitoring)
                
-               478          70 LOAD_FAST                0 (self)
+               533          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                3 (ping_worker)
                             82 LOAD_METHOD              4 (join)
                            104 PRECALL                  0
                            108 CALL                     0
                            118 POP_TOP
                            120 LOAD_CONST               0 (None)
                            122 RETURN_VALUE
                consts
                   None
                   False
                names      ('live_mode', 'stop_monitoring', 'monitoring', 'ping_worker', 'join')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
                name       'stop'
-               firstlineno 473
+               firstlineno 528
                lnotab 0x02010e0128020e01
             (False,)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ping_ping.logging', 'add_child', '_Ping__cls_log', '_Ping__auto_run', '_Ping__target', '_Ping__timeout', '_Ping__runs', '_Ping__results', '_Ping__interval', '_Ping__size', '_Ping__history', '_Ping__monitoring', '_Ping__continuous_ping', 'Null', 'str', '__init__', 'property', 'bool', 'auto_run', 'setter', 'continuous_ping', 'int', 'interval', 'packet_size', 'ping_worker', 'target', 'monitoring', 'history', 'latest', 'float', 'timeout', 'results', 'runs', 'deleter', 'status', 'create_worker', 'ping', 'generate_report', 'start', 'stop_monitoring', 'stop')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ping_stat.logging', 'add_child', '_Ping__cls_log', '_Ping__auto_run', '_Ping__target', '_Ping__timeout', '_Ping__runs', '_Ping__results', '_Ping__interval', '_Ping__size', '_Ping__history', '_Ping__monitoring', '_Ping__continuous_ping', 'Null', 'str', '__init__', 'property', 'bool', 'auto_run', 'setter', 'continuous_ping', 'int', 'interval', 'gui_mode', 'packet_size', 'ping_worker', 'target', 'monitoring', 'history', 'latest', 'float', 'timeout', 'queue', 'deleter', 'results', 'runs', 'status', 'create_worker', 'ping', 'generate_report', 'start', 'stop_monitoring', 'stop')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
          name       'Ping'
-         firstlineno 26
+         firstlineno 58
          lnotab
             0x0a0104240c021602040104010401040104010401040104010401040512
-            01020102010201020102010201020102f5040202fe084902010aff0e0102
-            070c010aff0e010211020104ff0e01020302010aff0e0102030c0104ff0e
-            010206020104ff0e0102030c0104ff0e01020a020104ff0e010203020104
-            ff0e0102070c0104ff0e010216020104ff0e0102030c0104ff0e01020602
-            0104ff0e0102030c0104ff0e010206020104ff0e0102030c0104ff0e0102
-            04020104ff0e01020602010aff0e0102070c0104ff0e010216020104ff0e
-            010203020104ff0e0102070c0104ff0e01021e0c0104ff0e010206020104
-            ff0e01020e080a06310613060e0605
+            010201020102010201020102010201020102f4040202fe084d02010aff0e
+            0102070c010aff0e010211020104ff0e01020302010aff0e0102030c0104
+            ff0e01020602010aff0e0102030c0104ff0e010205020104ff0e0102030c
+            0104ff0e01020a020104ff0e010203020104ff0e0102070c0104ff0e0102
+            16020104ff0e0102030c0104ff0e010206020104ff0e0102030c0104ff0e
+            010206020104ff0e0102030c0104ff0e010204020104ff0e01020602010a
+            ff0e0102070c0104ff0e010216020104ff0e0102030c0104ff0e01020302
+            0104ff0e010203020104ff0e0102070c0104ff0e01021e0c0104ff0e0102
+            06020104ff0e01020e080a06310613060e0606
       'Ping'
-      None
-   names      ('__doc__', 'time', 'sleep', 'ping_ping.errors', 'RedundantWorkOrderError', 'WorkerAlreadyStartedError', 'ping_ping.utils', 'gather_times', 'ping_ping.utils.workers', 'PingMonitor', 'PingWorker', 'statistics', 'mean', 'median', 'ping3', 'ping', '_ping', 'pypattyrn.behavioral.null', 'Null', 'threading', 'Thread', 'rich.console', 'Console', 'console', 'track_mean', 'Ping')
+   names      ('__doc__', 'ping3', 'ping', '_ping', 'ping_stat.errors', 'RedundantWorkOrderError', 'WorkerAlreadyStartedError', 'ping_stat.utils', 'gather_times', 'ping_stat.utils.workers', 'PingMonitor', 'PingWorker', 'pypattyrn.behavioral.null', 'Null', 'queue', 'rich.console', 'Console', 'statistics', 'mean', 'median', 'threading', 'Thread', 'time', 'sleep', 'console', 'track_mean', 'Ping')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\network.py'
+   filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\network.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010407100110020c01100110010c010c010c010c03140304031a
-      7f007f007f004b
+      0x00ff020104260c0110020c0110010c0108010c0110010c011003140304
+      031a7f007f007f0062
```

### Comparing `ping_stat-0.1.0/ping_stat/utils/decorators.py` & `ping_stat-1.0/ping_stat/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/helpers.py` & `ping_stat-1.0/ping_stat/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/network.py` & `ping_stat-1.0/ping_stat/utils/network.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,26 +32,25 @@
 Disclaimer:
 Please use this tool only with the express permission of the target system's network administrator and
 exercise due care and responsibility in doing so. The author of this tool assumes no liability for any damage,
 legal or otherwise, caused by its use. Pinging a target is not a passive operation and may be detected by
 intrusion detection systems or firewall logs. Irresponsible use of this tool could potentially cause a
 denial of service to the target system's network services, or your own.
 """
-
-
-from time import sleep, time
+from ping3 import ping as _ping
 from ping_stat.errors import RedundantWorkOrderError, WorkerAlreadyStartedError
 
 from ping_stat.utils import gather_times
 from ping_stat.utils.workers import PingMonitor, PingWorker
-from statistics import mean, median
-from ping3 import ping as _ping
 from pypattyrn.behavioral.null import Null
-from threading import Thread
+import queue
 from rich.console import Console
+from statistics import mean, median
+from threading import Thread
+from time import sleep, time
 
 
 console = Console()
 
 
 track_mean = False
 
@@ -160,15 +159,18 @@
         self.interval = interval
         log.debug(f'Ping interval: {self.interval}')
 
         self.__debug_mode = debug_mode
 
         self.__ping_worker = None
 
+        self.__queue = None
+
         if self.__continuous_ping:
+            self.__queue = queue.Queue()
             self.__ping_worker = self.create_worker()
             if live_mode is not None:
                 self.live_mode = True
                 self.ping_monitor = PingMonitor(self)
 
             else:
                 self.live_mode = False
@@ -349,14 +351,22 @@
 
         if new <= 0:
             raise ValueError('"timeout" must be positive')
 
         self.__timeout = int(new)
 
     @property
+    def queue(self):
+        return self.__queue
+
+    @queue.deleter
+    def queue(self):
+        return self.__queue.empty()
+
+    @property
     def results(self):
         return self.__results
 
     @property
     def runs(self):
         """
        int:
```

### Comparing `ping_stat-0.1.0/ping_stat/utils/workers/__init__.py` & `ping_stat-1.0/ping_stat/utils/workers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 if self.latest is None:
                     console.print('')
 
                 cur_style = 'green' if last_ping > mean(self.latest) else 'red'
                 avg_style = 'green' if current_avg < self.last_avg else 'red'
                 console.print(
                     f'[bold]Last ping time: [/][{cur_style}]{self.ping_object.latest[-1]}[/]'
-                    f'[bold] | Average ping time:[/][{avg_style}]{current_avg}[/]'
+                    f'[bold] | Average ping time: [/][{avg_style}]{current_avg}[/]'
                 )
                 self.last_avg = current_avg
 
     @property
     def history(self):
         return self.ping_object.history
```

### Comparing `ping_stat-0.1.0/ping_stat/utils/workers/__pycache__/__init__.cpython-310.pyc` & `ping_stat-1.0/ping_stat/utils/workers/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ping_stat-0.1.0/ping_stat/utils/workers/__pycache__/__init__.cpython-311.pyc` & `ping_stat-1.0/ping_stat/utils/workers/__pycache__/__init__.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf3847864 (Thu Jun  1 11:45:55 2023 UTC)
-files sz: 8215
+moddate:  0xed9f9464 (Thu Jun 22 19:24:29 2023 UTC)
+files sz: 8249
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x970064005a00640164026c015a01640164026c025a02640164026c035a
@@ -13,15 +13,15 @@
       0e5a0e6d0f5a0f0100640164076c106d115a116d125a120100640164086c
       136d145a14010002006506a6000000ab0000000000000000005a15020065
       0b6409a6010000ab0100000000000000005a1602004700640a8400640ba6
       020000ab0200000000000000005a1702004700640c8400640da6020000ab
       0200000000000000005a1864025300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.tech\nCreated: 5/9/2023 @ 4:05 PM\nFile:\n  Name: __init__.py\n  Filepath: ping_ping/utils/workers\n')
+     1           2 LOAD_CONST               0 ('\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.tech\nCreated: 5/9/2023 @ 4:05 PM\nFile:\n  Name: __init__.py\n  Filepath: ping_stat/utils/workers\n')
                  4 STORE_NAME               0 (__doc__)
    
      9           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
                 10 IMPORT_NAME              1 (datetime)
                 12 STORE_NAME               1 (datetime)
    
@@ -60,15 +60,15 @@
                 70 STORE_NAME              10 (Type)
                 72 IMPORT_FROM             11 (TypeVar)
                 74 STORE_NAME              11 (TypeVar)
                 76 POP_TOP
    
     15          78 LOAD_CONST               1 (0)
                 80 LOAD_CONST               6 (('RedundantWorkOrderError', 'WorkerAlreadyStartedError', 'WorkerNotStartedError'))
-                82 IMPORT_NAME             12 (ping_ping.errors)
+                82 IMPORT_NAME             12 (ping_stat.errors)
                 84 IMPORT_FROM             13 (RedundantWorkOrderError)
                 86 STORE_NAME              13 (RedundantWorkOrderError)
                 88 IMPORT_FROM             14 (WorkerAlreadyStartedError)
                 90 STORE_NAME              14 (WorkerAlreadyStartedError)
                 92 IMPORT_FROM             15 (WorkerNotStartedError)
                 94 STORE_NAME              15 (WorkerNotStartedError)
                 96 POP_TOP
@@ -80,15 +80,15 @@
                106 STORE_NAME              17 (mean)
                108 IMPORT_FROM             18 (median)
                110 STORE_NAME              18 (median)
                112 POP_TOP
    
     20         114 LOAD_CONST               1 (0)
                116 LOAD_CONST               8 (('get_ping_mean',))
-               118 IMPORT_NAME             19 (ping_ping.utils)
+               118 IMPORT_NAME             19 (ping_stat.utils)
                120 IMPORT_FROM             20 (get_ping_mean)
                122 STORE_NAME              20 (get_ping_mean)
                124 POP_TOP
    
     22         126 PUSH_NULL
                128 LOAD_NAME                6 (Console)
                130 PRECALL                  0
@@ -100,34 +100,34 @@
                150 LOAD_CONST               9 ('PING')
                152 PRECALL                  1
                156 CALL                     1
                166 STORE_NAME              22 (PING)
    
     26         168 PUSH_NULL
                170 LOAD_BUILD_CLASS
-               172 LOAD_CONST              10 (<code object PingMonitor, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 26>)
+               172 LOAD_CONST              10 (<code object PingMonitor, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 26>)
                174 MAKE_FUNCTION            0
                176 LOAD_CONST              11 ('PingMonitor')
                178 PRECALL                  2
                182 CALL                     2
                192 STORE_NAME              23 (PingMonitor)
    
    103         194 PUSH_NULL
                196 LOAD_BUILD_CLASS
-               198 LOAD_CONST              12 (<code object PingWorker, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 103>)
+               198 LOAD_CONST              12 (<code object PingWorker, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 103>)
                200 MAKE_FUNCTION            0
                202 LOAD_CONST              13 ('PingWorker')
                204 PRECALL                  2
                208 CALL                     2
                218 STORE_NAME              24 (PingWorker)
    
-   246         220 LOAD_CONST               2 (None)
+   248         220 LOAD_CONST               2 (None)
                222 RETURN_VALUE
    consts
-      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.tech\nCreated: 5/9/2023 @ 4:05 PM\nFile:\n  Name: __init__.py\n  Filepath: ping_ping/utils/workers\n'
+      '\nProject: PingPing\nAuthor: Inspyre Softworks - https://inspyre.tech\nCreated: 5/9/2023 @ 4:05 PM\nFile:\n  Name: __init__.py\n  Filepath: ping_stat/utils/workers\n'
       0
       None
       ('sleep',)
       ('Console',)
       ('Optional', 'Union', 'Type', 'TypeVar')
       ('RedundantWorkOrderError', 'WorkerAlreadyStartedError', 'WorkerNotStartedError')
       ('mean', 'median')
@@ -146,71 +146,71 @@
             005a0b640984005a0c640a5300
           26           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PingMonitor')
                        8 STORE_NAME               2 (__qualname__)
          
-          27          10 LOAD_CONST               1 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 27>)
+          27          10 LOAD_CONST               1 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 27>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
           36          16 LOAD_NAME                4 (property)
          
-          37          18 LOAD_CONST               2 (<code object thread, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 36>)
+          37          18 LOAD_CONST               2 (<code object thread, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 36>)
                       20 MAKE_FUNCTION            0
          
           36          22 PRECALL                  0
                       26 CALL                     0
          
           37          36 STORE_NAME               5 (thread)
          
-          41          38 LOAD_CONST               3 (<code object start, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 41>)
+          41          38 LOAD_CONST               3 (<code object start, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 41>)
                       40 MAKE_FUNCTION            0
                       42 STORE_NAME               6 (start)
          
-          49          44 LOAD_CONST               4 (<code object stop, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 49>)
+          49          44 LOAD_CONST               4 (<code object stop, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 49>)
                       46 MAKE_FUNCTION            0
                       48 STORE_NAME               7 (stop)
          
-          52          50 LOAD_CONST               5 (<code object _monitor, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 52>)
+          52          50 LOAD_CONST               5 (<code object _monitor, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 52>)
                       52 MAKE_FUNCTION            0
                       54 STORE_NAME               8 (_monitor)
          
           76          56 LOAD_NAME                4 (property)
          
-          77          58 LOAD_CONST               6 (<code object history, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 76>)
+          77          58 LOAD_CONST               6 (<code object history, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 76>)
                       60 MAKE_FUNCTION            0
          
           76          62 PRECALL                  0
                       66 CALL                     0
          
           77          76 STORE_NAME               9 (history)
          
           80          78 LOAD_NAME                4 (property)
          
-          81          80 LOAD_CONST               7 (<code object latest, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 80>)
+          81          80 LOAD_CONST               7 (<code object latest, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 80>)
                       82 MAKE_FUNCTION            0
          
           80          84 PRECALL                  0
                       88 CALL                     0
          
           81          98 STORE_NAME              10 (latest)
          
           84         100 LOAD_NAME                4 (property)
          
-          85         102 LOAD_CONST               8 (<code object status, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 84>)
+          85         102 LOAD_CONST               8 (<code object status, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 84>)
                      104 MAKE_FUNCTION            0
          
           84         106 PRECALL                  0
                      110 CALL                     0
          
           85         120 STORE_NAME              11 (status)
          
-          92         122 LOAD_CONST               9 (<code object __repr__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 92>)
+          92         122 LOAD_CONST               9 (<code object __repr__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 92>)
                      124 MAKE_FUNCTION            0
                      126 STORE_NAME              12 (__repr__)
                      128 LOAD_CONST              10 (None)
                      130 RETURN_VALUE
          consts
             'PingMonitor'
             code
@@ -249,15 +249,15 @@
                   None
                   0
                   False
                names      ('ping_object', 'hist_len', 'last_avg', 'monitoring', '_PingMonitor__thread')
                varnames   ('self', 'ping_object')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       '__init__'
                firstlineno 27
                lnotab 0x02010e010e010e010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -270,15 +270,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_PingMonitor__thread',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'thread'
                firstlineno 36
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
@@ -327,15 +327,15 @@
                   None
                   True
                   ('target', 'daemon')
                names      ('monitoring', 'threading', 'Thread', '_monitor', '_PingMonitor__thread', 'start')
                varnames   ('self', 'thread')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'start'
                firstlineno 41
                lnotab 0x02010e0104010e0136010e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
@@ -351,15 +351,15 @@
                consts
                   None
                   False
                names      ('monitoring',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'stop'
                firstlineno 49
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 6
                stacksize : 11
@@ -494,15 +494,15 @@
                            456 LOAD_CONST               9 (']')
                            458 LOAD_FAST                0 (self)
                            460 LOAD_ATTR                4 (ping_object)
                            470 LOAD_ATTR                9 (latest)
                            480 LOAD_CONST               3 (-1)
                            482 BINARY_SUBSCR
                            492 FORMAT_VALUE             0
-                           494 LOAD_CONST              10 ('[/][bold] | Average ping time:[/][')
+                           494 LOAD_CONST              10 ('[/][bold] | Average ping time: [/][')
                
                 72         496 LOAD_FAST                5 (avg_style)
                
                 71         498 FORMAT_VALUE             0
                            500 LOAD_CONST               9 (']')
                
                 72         502 LOAD_FAST                2 (current_avg)
@@ -538,21 +538,21 @@
                   -1
                   0
                   ''
                   'green'
                   'red'
                   '[bold]Last ping time: [/]['
                   ']'
-                  '[/][bold] | Average ping time:[/]['
+                  '[/][bold] | Average ping time: [/]['
                   '[/]'
                names      ('monitoring', 'time', 'sleep', 'len', 'ping_object', 'history', 'hist_len', 'get_ping_mean', 'IndexError', 'latest', 'console', 'print', 'mean', 'last_avg')
                varnames   ('self', 'h_len', 'current_avg', 'last_ping', 'cur_style', 'avg_style')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       '_monitor'
                firstlineno 52
                lnotab
                   0x020110012801320116010e021e0102013601120108ff08030e01340238
                   011e0122012e0102ff040102ff06ff10040eeb
             code
                argcount  : 1
@@ -568,15 +568,15 @@
                             24 RETURN_VALUE
                consts
                   None
                names      ('ping_object', 'history')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'history'
                firstlineno 76
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -590,15 +590,15 @@
                             24 RETURN_VALUE
                consts
                   None
                names      ('ping_object', 'latest')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'latest'
                firstlineno 80
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
@@ -623,15 +623,15 @@
                consts
                   None
                   ('monitoring', 'last_avg', 'hist_len')
                names      ('monitoring', 'last_avg', 'hist_len')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'status'
                firstlineno 84
                lnotab 0x02030c010c010cfd
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
@@ -676,24 +676,24 @@
                   'hist_len'
                   '>'
                   '<PingMonitor: not monitoring>'
                names      ('status',)
                varnames   ('self', 'status')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       '__repr__'
                firstlineno 92
                lnotab 0x02010e0110012a02
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'property', 'thread', 'start', 'stop', '_monitor', 'history', 'latest', 'status', '__repr__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
          name       'PingMonitor'
          firstlineno 26
          lnotab
             0x0a010609020104ff0e010204060806030618020104ff0e010203020104
             ff0e010203020104ff0e010207
       'PingMonitor'
       code
@@ -725,65 +725,65 @@
                        6 LOAD_CONST               0 ('PingWorker')
                        8 STORE_NAME               2 (__qualname__)
          
          104          10 LOAD_CONST              24 ((True,))
                       12 LOAD_CONST               2 ('ping_object')
                       14 LOAD_NAME                3 (PING)
                       16 BUILD_TUPLE              2
-                      18 LOAD_CONST               3 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 104>)
+                      18 LOAD_CONST               3 (<code object __init__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 104>)
                       20 MAKE_FUNCTION            5 (defaults, annotations)
                       22 STORE_NAME               4 (__init__)
          
          115          24 LOAD_NAME                5 (property)
          
-         116          26 LOAD_CONST               4 (<code object history, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 115>)
+         116          26 LOAD_CONST               4 (<code object history, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 115>)
                       28 MAKE_FUNCTION            0
          
          115          30 PRECALL                  0
                       34 CALL                     0
          
          116          44 STORE_NAME               6 (history)
          
          119          46 LOAD_NAME                5 (property)
          
-         120          48 LOAD_CONST               5 (<code object interval, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 119>)
+         120          48 LOAD_CONST               5 (<code object interval, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 119>)
                       50 MAKE_FUNCTION            0
          
          119          52 PRECALL                  0
                       56 CALL                     0
          
          120          66 STORE_NAME               7 (interval)
          
          123          68 LOAD_NAME                5 (property)
          
-         124          70 LOAD_CONST               6 (<code object monitoring, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 123>)
+         124          70 LOAD_CONST               6 (<code object monitoring, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 123>)
                       72 MAKE_FUNCTION            0
          
          123          74 PRECALL                  0
                       78 CALL                     0
          
          124          88 STORE_NAME               8 (monitoring)
          
          127          90 LOAD_NAME                8 (monitoring)
                       92 LOAD_ATTR                9 (setter)
          
-         128         102 LOAD_CONST               7 (<code object monitoring, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 127>)
+         128         102 LOAD_CONST               7 (<code object monitoring, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 127>)
                      104 MAKE_FUNCTION            0
          
          127         106 PRECALL                  0
                      110 CALL                     0
          
          128         120 STORE_NAME               8 (monitoring)
          
          131         122 LOAD_NAME                5 (property)
          
          132         124 LOAD_CONST               8 ('return')
                      126 LOAD_NAME                3 (PING)
                      128 BUILD_TUPLE              2
-                     130 LOAD_CONST               9 (<code object ping_object, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 131>)
+                     130 LOAD_CONST               9 (<code object ping_object, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 131>)
                      132 MAKE_FUNCTION            4 (annotations)
          
          131         134 PRECALL                  0
                      138 CALL                     0
          
          132         148 STORE_NAME              10 (ping_object)
          
@@ -793,50 +793,50 @@
          136         162 LOAD_CONST              10 ('new')
                      164 LOAD_NAME               11 (Type)
                      166 LOAD_NAME                3 (PING)
                      168 BINARY_SUBSCR
                      178 LOAD_CONST               8 ('return')
                      180 LOAD_CONST              11 (None)
                      182 BUILD_TUPLE              4
-                     184 LOAD_CONST              12 (<code object ping_object, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 135>)
+                     184 LOAD_CONST              12 (<code object ping_object, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 135>)
                      186 MAKE_FUNCTION            4 (annotations)
          
          135         188 PRECALL                  0
                      192 CALL                     0
          
          136         202 STORE_NAME              10 (ping_object)
          
          139         204 LOAD_NAME                5 (property)
          
          140         206 LOAD_CONST               8 ('return')
                      208 LOAD_NAME               12 (threading)
                      210 LOAD_ATTR               13 (Thread)
                      220 BUILD_TUPLE              2
-                     222 LOAD_CONST              13 (<code object thread, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 139>)
+                     222 LOAD_CONST              13 (<code object thread, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 139>)
                      224 MAKE_FUNCTION            4 (annotations)
          
          139         226 PRECALL                  0
                      230 CALL                     0
          
          140         240 STORE_NAME              14 (thread)
          
          143         242 LOAD_NAME               14 (thread)
                      244 LOAD_ATTR                9 (setter)
          
-         144         254 LOAD_CONST              14 (<code object thread, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 143>)
+         144         254 LOAD_CONST              14 (<code object thread, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 143>)
                      256 MAKE_FUNCTION            0
          
          143         258 PRECALL                  0
                      262 CALL                     0
          
          144         272 STORE_NAME              14 (thread)
          
          149         274 LOAD_NAME                5 (property)
          
-         150         276 LOAD_CONST              15 (<code object target, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 149>)
+         150         276 LOAD_CONST              15 (<code object target, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 149>)
                      278 MAKE_FUNCTION            0
          
          149         280 PRECALL                  0
                      284 CALL                     0
          
          150         294 STORE_NAME              15 (target)
          
@@ -848,15 +848,15 @@
                      304 LOAD_CONST              11 (None)
                      306 LOAD_NAME               18 (datetime)
                      308 LOAD_ATTR               18 (datetime)
                      318 BUILD_TUPLE              2
                      320 BINARY_SUBSCR
                      330 BINARY_SUBSCR
                      340 BUILD_TUPLE              2
-                     342 LOAD_CONST              16 (<code object started, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 153>)
+                     342 LOAD_CONST              16 (<code object started, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 153>)
                      344 MAKE_FUNCTION            4 (annotations)
          
          153         346 PRECALL                  0
                      350 CALL                     0
          
          154         360 STORE_NAME              19 (started)
          
@@ -871,49 +871,49 @@
                      384 LOAD_ATTR               18 (datetime)
                      394 BUILD_TUPLE              2
                      396 BINARY_SUBSCR
                      406 BINARY_SUBSCR
                      416 LOAD_CONST               8 ('return')
                      418 LOAD_CONST              11 (None)
                      420 BUILD_TUPLE              4
-                     422 LOAD_CONST              17 (<code object started, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 157>)
+                     422 LOAD_CONST              17 (<code object started, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 157>)
                      424 MAKE_FUNCTION            4 (annotations)
          
          157         426 PRECALL                  0
                      430 CALL                     0
          
          158         440 STORE_NAME              19 (started)
          
          163         442 LOAD_NAME                5 (property)
          
-         164         444 LOAD_CONST              18 (<code object status, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 163>)
+         164         444 LOAD_CONST              18 (<code object status, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 163>)
                      446 MAKE_FUNCTION            0
          
          163         448 PRECALL                  0
                      452 CALL                     0
          
          164         462 STORE_NAME              20 (status)
          
-         175         464 LOAD_CONST              19 (<code object create, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 175>)
+         175         464 LOAD_CONST              19 (<code object create, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 175>)
                      466 MAKE_FUNCTION            0
                      468 STORE_NAME              21 (create)
          
-         191         470 LOAD_CONST              20 (<code object start, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 191>)
+         191         470 LOAD_CONST              20 (<code object start, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 191>)
                      472 MAKE_FUNCTION            0
                      474 STORE_NAME              22 (start)
          
-         204         476 LOAD_CONST              21 (<code object stop, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 204>)
+         204         476 LOAD_CONST              21 (<code object stop, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 204>)
                      478 MAKE_FUNCTION            0
                      480 STORE_NAME              23 (stop)
          
-         210         482 LOAD_CONST              22 (<code object worker, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 210>)
+         212         482 LOAD_CONST              22 (<code object worker, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 212>)
                      484 MAKE_FUNCTION            0
                      486 STORE_NAME              24 (worker)
          
-         232         488 LOAD_CONST              23 (<code object __repr__, file "C:\Users\tayja\PycharmProjects\PingPing\ping_ping\utils\workers\__init__.py", line 232>)
+         234         488 LOAD_CONST              23 (<code object __repr__, file "C:\Users\tayja\PycharmProjects\PingStat\ping_stat\utils\workers\__init__.py", line 234>)
                      490 MAKE_FUNCTION            0
                      492 STORE_NAME              25 (__repr__)
                      494 LOAD_CONST              11 (None)
                      496 RETURN_VALUE
          consts
             'PingWorker'
             True
@@ -970,15 +970,15 @@
                            152 RETURN_VALUE
                consts
                   None
                names      ('_PingWorker__started', '_PingWorker__thread', '_PingWorker__ping_object', 'ping_object', 'ping', 'create')
                varnames   ('self', 'ping_object', 'auto_create')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       '__init__'
                firstlineno 104
                lnotab 0x02010e010e020e010e012202040136ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -992,15 +992,15 @@
                             24 RETURN_VALUE
                consts
                   None
                names      ('ping_object', 'history')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'history'
                firstlineno 115
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1014,15 +1014,15 @@
                             24 RETURN_VALUE
                consts
                   None
                names      ('ping_object', 'interval')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'interval'
                firstlineno 119
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1036,15 +1036,15 @@
                             24 RETURN_VALUE
                consts
                   None
                names      ('ping_object', 'monitoring')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'monitoring'
                firstlineno 123
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
@@ -1062,15 +1062,15 @@
                             28 RETURN_VALUE
                consts
                   None
                names      ('ping_object', 'monitoring')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'monitoring'
                firstlineno 127
                lnotab 0x0202
             'return'
             code
                argcount  : 1
                nlocals   : 1
@@ -1084,15 +1084,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_PingWorker__ping_object',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'ping_object'
                firstlineno 131
                lnotab 0x0202
             'new'
             None
             code
                argcount  : 2
@@ -1109,15 +1109,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('_PingWorker__ping_object',)
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'ping_object'
                firstlineno 135
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1130,15 +1130,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_PingWorker__thread',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'thread'
                firstlineno 139
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -1172,15 +1172,15 @@
                consts
                   None
                   '"thread" must be of type "threading.Thread"'
                names      ('isinstance', 'threading', 'Thread', 'TypeError', '_PingWorker__thread')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'thread'
                firstlineno 143
                lnotab 0x020234011e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1194,15 +1194,15 @@
                             24 RETURN_VALUE
                consts
                   None
                names      ('ping_object', 'target')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'target'
                firstlineno 149
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1215,15 +1215,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_PingWorker__started',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'started'
                firstlineno 153
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -1257,15 +1257,15 @@
                consts
                   None
                   '"started" must be a datetime object'
                names      ('isinstance', 'datetime', 'TypeError', '_PingWorker__started')
                varnames   ('self', 'new')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'started'
                firstlineno 157
                lnotab 0x020234011e01
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
@@ -1371,15 +1371,15 @@
                   True
                   ('running', 'started', 'runtime')
                   ('running', 'started', 'stopped_at', 'runtime')
                names      ('thread', 'started', 'is_alive', 'datetime', 'now', 'join')
                varnames   ('self', 'stopped_at', 'runtime')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'status'
                firstlineno 163
                lnotab 0x02020e01180132014c010cff0a034e017601
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
@@ -1422,15 +1422,15 @@
                   '\n        Create a new thread for the worker.\n\n        Raises:\n            RedundantWorkOrderError: If the worker already has a thread.\n\n        Returns:\n            threading.Thread: The new thread.\n        '
                   True
                   ('target', 'daemon')
                names      ('thread', 'RedundantWorkOrderError', '__class__', '__name__', 'threading', 'Thread', 'worker')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'create'
                firstlineno 175
                lnotab 0x020a0e0132024001
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
@@ -1486,29 +1486,30 @@
                   "\n        Start the worker's thread.\n\n        Raises:\n            WorkerAlreadyStartedError: If the worker's thread is already running.\n        "
                   True
                   None
                names      ('started', 'WorkerAlreadyStartedError', 'thread', 'name', 'str', 'monitoring', 'start', 'datetime', 'now')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'start'
                firstlineno 191
                lnotab 0x02070e014e010e013201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a00000000000000000073277403000000000000000000007c
                   006a0200000000000000006a030000000000000000740900000000000000
                   0000007c00a6010000ab010000000000000000a6020000ab020000000000
-                  00000082017c006a020000000000000000a0050000000000000000000000
-                  000000000000000000a6000000ab000000000000000000010064005300
+                  000000820164017c005f0500000000000000007c006a0200000000000000
+                  00a0060000000000000000000000000000000000000000a6000000ab0000
+                  00000000000000010064005300
                204           0 RESUME                   0
                
                205           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (started)
                             14 POP_JUMP_FORWARD_IF_TRUE    39 (to 94)
                
                206          16 LOAD_GLOBAL              3 (NULL + WorkerNotStartedError)
@@ -1519,32 +1520,37 @@
                             62 LOAD_FAST                0 (self)
                             64 PRECALL                  1
                             68 CALL                     1
                             78 PRECALL                  2
                             82 CALL                     2
                             92 RAISE_VARARGS            1
                
-               208     >>   94 LOAD_FAST                0 (self)
-                            96 LOAD_ATTR                2 (thread)
-                           106 LOAD_METHOD              5 (join)
-                           128 PRECALL                  0
-                           132 CALL                     0
-                           142 POP_TOP
-                           144 LOAD_CONST               0 (None)
-                           146 RETURN_VALUE
+               208     >>   94 LOAD_CONST               1 (False)
+                            96 LOAD_FAST                0 (self)
+                            98 STORE_ATTR               5 (monitoring)
+               
+               210         108 LOAD_FAST                0 (self)
+                           110 LOAD_ATTR                2 (thread)
+                           120 LOAD_METHOD              6 (join)
+                           142 PRECALL                  0
+                           146 CALL                     0
+                           156 POP_TOP
+                           158 LOAD_CONST               0 (None)
+                           160 RETURN_VALUE
                consts
                   None
-               names      ('started', 'WorkerNotStartedError', 'thread', 'name', 'str', 'join')
+                  False
+               names      ('started', 'WorkerNotStartedError', 'thread', 'name', 'str', 'monitoring', 'join')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'stop'
                firstlineno 204
-               lnotab 0x02010e014e02
+               lnotab 0x02010e014e020e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 8
                flags     : 3
                code
                   0x970064017c006a0000000000000000005f0100000000000000007c006a
@@ -1556,37 +1562,37 @@
                   0000006a090000000000000000a6000000ab000000000000000000a60100
                   00ab010000000000000000a00a0000000000000000000000000000000000
                   000000a6000000ab000000000000000000a6010000ab0100000000000000
                   007c006a0b00000000000000007c00a00c00000000000000000000000000
                   00000000000000a6000000ab0000000000000000006603a6010000ab0100
                   0000000000000001007c006a010000000000000000b09c64025300640253
                   00
-               210           0 RESUME                   0
+               212           0 RESUME                   0
                
-               221           2 LOAD_CONST               1 (True)
+               223           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (ping_object)
                             16 STORE_ATTR               1 (monitoring)
                
-               222          26 LOAD_FAST                0 (self)
+               224          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (monitoring)
                             38 POP_JUMP_FORWARD_IF_FALSE   158 (to 356)
                
-               223     >>   40 LOAD_GLOBAL              5 (NULL + sleep)
+               225     >>   40 LOAD_GLOBAL              5 (NULL + sleep)
                             52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (interval)
                             64 PRECALL                  1
                             68 CALL                     1
                             78 POP_TOP
                
-               224          80 LOAD_FAST                0 (self)
+               226          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (history)
                             92 LOAD_METHOD              5 (append)
                
-               226         114 LOAD_GLOBAL             13 (NULL + str)
+               228         114 LOAD_GLOBAL             13 (NULL + str)
                            126 LOAD_GLOBAL             14 (datetime)
                            138 LOAD_ATTR                7 (datetime)
                            148 LOAD_METHOD              8 (fromtimestamp)
                            170 LOAD_GLOBAL             19 (NULL + time)
                            182 LOAD_ATTR                9 (time)
                            192 PRECALL                  0
                            196 CALL                     0
@@ -1594,46 +1600,46 @@
                            210 CALL                     1
                            220 LOAD_METHOD             10 (isoformat)
                            242 PRECALL                  0
                            246 CALL                     0
                            256 PRECALL                  1
                            260 CALL                     1
                
-               227         270 LOAD_FAST                0 (self)
+               229         270 LOAD_FAST                0 (self)
                            272 LOAD_ATTR               11 (target)
                
-               228         282 LOAD_FAST                0 (self)
+               230         282 LOAD_FAST                0 (self)
                            284 LOAD_METHOD             12 (ping)
                            306 PRECALL                  0
                            310 CALL                     0
                
-               225         320 BUILD_TUPLE              3
+               227         320 BUILD_TUPLE              3
                
-               224         322 PRECALL                  1
+               226         322 PRECALL                  1
                            326 CALL                     1
                            336 POP_TOP
                
-               222         338 LOAD_FAST                0 (self)
+               224         338 LOAD_FAST                0 (self)
                            340 LOAD_ATTR                1 (monitoring)
                            350 POP_JUMP_BACKWARD_IF_TRUE   156 (to 40)
                            352 LOAD_CONST               2 (None)
                            354 RETURN_VALUE
                        >>  356 LOAD_CONST               2 (None)
                            358 RETURN_VALUE
                consts
                   "\n        The worker's main loop.\n\n        This method runs in the worker's thread and repeatedly pings the target at the specified interval, adding the\n        ping results to the worker's history.\n\n        Note:\n            This method should not be called directly; instead, it should be run in a separate thread using the `start` method.\n\n        "
                   True
                   None
                names      ('ping_object', 'monitoring', 'sleep', 'interval', 'history', 'append', 'str', 'datetime', 'fromtimestamp', 'time', 'isoformat', 'target', 'ping')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       'worker'
-               firstlineno 210
+               firstlineno 212
                lnotab 0x020b18010e01280122029c010c0126fd02ff10fe
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
                flags     : 3
                code
@@ -1641,40 +1647,40 @@
                   00720c64027c016403190000000000000000009b0064049d0353007c0164
                   0519000000000000000000724464067c01640519000000000000000000a0
                   0100000000000000000000000000000000000000006407a6010000ab0100
                   000000000000009b0064087c01640919000000000000000000a001000000
                   00000000000000000000000000000000006407a6010000ab010000000000
                   0000009b00640a7c016403190000000000000000009b0064049d07530064
                   0b5300
-               232           0 RESUME                   0
+               234           0 RESUME                   0
                
-               233           2 LOAD_FAST                0 (self)
+               235           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (status)
                             14 STORE_FAST               1 (status)
                
-               234          16 LOAD_FAST                1 (status)
+               236          16 LOAD_FAST                1 (status)
                             18 LOAD_CONST               1 ('running')
                             20 BINARY_SUBSCR
                             30 POP_JUMP_FORWARD_IF_FALSE    12 (to 56)
                
-               235          32 LOAD_CONST               2 ('<PingWorker: running for ')
+               237          32 LOAD_CONST               2 ('<PingWorker: running for ')
                             34 LOAD_FAST                1 (status)
                             36 LOAD_CONST               3 ('runtime')
                             38 BINARY_SUBSCR
                             48 FORMAT_VALUE             0
                             50 LOAD_CONST               4 ('>')
                             52 BUILD_STRING             3
                             54 RETURN_VALUE
                
-               236     >>   56 LOAD_FAST                1 (status)
+               238     >>   56 LOAD_FAST                1 (status)
                             58 LOAD_CONST               5 ('started')
                             60 BINARY_SUBSCR
                             70 POP_JUMP_FORWARD_IF_FALSE    68 (to 208)
                
-               237          72 LOAD_CONST               6 ('<PingWorker: started at ')
+               239          72 LOAD_CONST               6 ('<PingWorker: started at ')
                             74 LOAD_FAST                1 (status)
                             76 LOAD_CONST               5 ('started')
                             78 BINARY_SUBSCR
                             88 LOAD_METHOD              1 (strftime)
                            110 LOAD_CONST               7 ('%Y-%m-%d %H:%M:%S')
                            112 PRECALL                  1
                            116 CALL                     1
@@ -1693,15 +1699,15 @@
                            188 LOAD_CONST               3 ('runtime')
                            190 BINARY_SUBSCR
                            200 FORMAT_VALUE             0
                            202 LOAD_CONST               4 ('>')
                            204 BUILD_STRING             7
                            206 RETURN_VALUE
                
-               239     >>  208 LOAD_CONST              11 ('<PingWorker: not started>')
+               241     >>  208 LOAD_CONST              11 ('<PingWorker: not started>')
                            210 RETURN_VALUE
                consts
                   None
                   'running'
                   '<PingWorker: running for '
                   'runtime'
                   '>'
@@ -1712,35 +1718,35 @@
                   'stopped_at'
                   ', ran for '
                   '<PingWorker: not started>'
                names      ('status', 'strftime')
                varnames   ('self', 'status')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+               filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
                name       '__repr__'
-               firstlineno 232
+               firstlineno 234
                lnotab 0x02010e011001180110018802
             (True,)
          names      ('__name__', '__module__', '__qualname__', 'PING', '__init__', 'property', 'history', 'interval', 'monitoring', 'setter', 'ping_object', 'Type', 'threading', 'Thread', 'thread', 'target', 'Optional', 'Union', 'datetime', 'started', 'status', 'create', 'start', 'stop', 'worker', '__repr__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+         filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
          name       'PingWorker'
          firstlineno 103
          lnotab
             0x0a010e0b020104ff0e010203020104ff0e010203020104ff0e0102030c
             0104ff0e01020302010aff0e0102030c011aff0e010203020114ff0e0102
             030c0104ff0e010205020104ff0e010203020130ff0e0102030c0134ff0e
-            010205020104ff0e01020b0610060d06060616
+            010205020104ff0e01020b0610060d06080616
       'PingWorker'
-   names      ('__doc__', 'datetime', 'threading', 'time', 'sleep', 'rich.console', 'Console', 'typing', 'Optional', 'Union', 'Type', 'TypeVar', 'ping_ping.errors', 'RedundantWorkOrderError', 'WorkerAlreadyStartedError', 'WorkerNotStartedError', 'statistics', 'mean', 'median', 'ping_ping.utils', 'get_ping_mean', 'console', 'PING', 'PingMonitor', 'PingWorker')
+   names      ('__doc__', 'datetime', 'threading', 'time', 'sleep', 'rich.console', 'Console', 'typing', 'Optional', 'Union', 'Type', 'TypeVar', 'ping_stat.errors', 'RedundantWorkOrderError', 'WorkerAlreadyStartedError', 'WorkerNotStartedError', 'statistics', 'mean', 'median', 'ping_stat.utils', 'get_ping_mean', 'console', 'PING', 'PingMonitor', 'PingWorker')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\tayja\\PycharmProjects\\PingPing\\ping_ping\\utils\\workers\\__init__.py'
+   filename   'C:\\Users\\tayja\\PycharmProjects\\PingStat\\ping_stat\\utils\\workers\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020104080801080108010c010c011801140410010c02140116031a
-      4d1a7f0010
+      4d1a7f0012
```

### Comparing `ping_stat-0.1.0/ping_stat/utils/workers/gui.py` & `ping_stat-1.0/ping_stat/utils/workers/gui.py`

 * *Files identical despite different names*

