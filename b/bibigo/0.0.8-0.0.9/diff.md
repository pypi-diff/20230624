# Comparing `tmp/bibigo-0.0.8.tar.gz` & `tmp/bibigo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibigo-0.0.8.tar", last modified: Sun May 28 11:30:01 2023, max compression
+gzip compressed data, was "bibigo-0.0.9.tar", last modified: Sat Jun 24 05:10:42 2023, max compression
```

## Comparing `bibigo-0.0.8.tar` & `bibigo-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.8/LICENSE
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 11:30:01.851439 bibigo-0.0.8/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.8/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.8/pyproject.toml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      564 2023-05-28 11:30:01.851439 bibigo-0.0.8/setup.cfg
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.847439 bibigo-0.0.8/src/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.847439 bibigo-0.0.8/src/bibigo/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.8/src/bibigo/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/src/bibigo/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.8/src/bibigo/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1528 2023-05-28 11:11:35.000000 bibigo-0.0.8/src/bibigo/__pycache__/scripts.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.8/src/bibigo/__pycache__/test.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1009 2023-05-28 10:15:03.000000 bibigo-0.0.8/src/bibigo/__pycache__/utils.cpython-39.pyc
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/src/bibigo/init/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.8/src/bibigo/init/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/src/bibigo/init/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.8/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2527 2023-05-28 10:15:03.000000 bibigo-0.0.8/src/bibigo/init/__pycache__/package.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.8/src/bibigo/init/__pycache__/settings.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2616 2023-05-28 11:26:47.000000 bibigo-0.0.8/src/bibigo/init/docker_compose.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3476 2023-05-28 11:16:01.000000 bibigo-0.0.8/src/bibigo/init/package.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.8/src/bibigo/init/settings.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1116 2023-05-28 11:11:31.000000 bibigo-0.0.8/src/bibigo/scripts.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/src/bibigo/static/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1293 2023-05-28 05:03:37.000000 bibigo-0.0.8/src/bibigo/static/.dockerignore.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1798 2023-05-28 05:23:42.000000 bibigo-0.0.8/src/bibigo/static/.gitignore.default
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/src/bibigo/static/.vscode/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:01:16.000000 bibigo-0.0.8/src/bibigo/static/.vscode/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      455 2023-05-28 07:19:46.000000 bibigo-0.0.8/src/bibigo/static/.vscode/settings.json.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      244 2023-05-28 10:12:41.000000 bibigo-0.0.8/src/bibigo/static/Dockerfile.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.8/src/bibigo/static/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1318 2023-05-28 11:29:11.000000 bibigo-0.0.8/src/bibigo/static/docker-compose.yml.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.8/src/bibigo/static/pyproject.toml.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      616 2023-05-28 08:20:22.000000 bibigo-0.0.8/src/bibigo/static/setup.cfg.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      736 2023-05-28 10:14:42.000000 bibigo-0.0.8/src/bibigo/utils.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.847439 bibigo-0.0.8/src/bibigo.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1117 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.9/LICENSE
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-06-24 05:10:42.216777 bibigo-0.0.9/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.9/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.9/pyproject.toml
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      540 2023-06-24 05:10:42.216777 bibigo-0.0.9/setup.cfg
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.212777 bibigo-0.0.9/src/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.9/src/bibigo/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/__pycache__/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.9/src/bibigo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1528 2023-06-24 05:06:55.000000 bibigo-0.0.9/src/bibigo/__pycache__/scripts.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.9/src/bibigo/__pycache__/test.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1009 2023-05-28 10:15:03.000000 bibigo-0.0.9/src/bibigo/__pycache__/utils.cpython-39.pyc
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/init/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.9/src/bibigo/init/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/init/__pycache__/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.9/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2515 2023-06-24 05:07:50.000000 bibigo-0.0.9/src/bibigo/init/__pycache__/package.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.9/src/bibigo/init/__pycache__/settings.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2771 2023-06-24 05:09:07.000000 bibigo-0.0.9/src/bibigo/init/docker_compose.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3476 2023-06-24 05:07:30.000000 bibigo-0.0.9/src/bibigo/init/package.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.9/src/bibigo/init/settings.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1109 2023-06-24 05:06:23.000000 bibigo-0.0.9/src/bibigo/scripts.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/static/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1293 2023-05-28 05:03:37.000000 bibigo-0.0.9/src/bibigo/static/.dockerignore.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1798 2023-05-28 05:23:42.000000 bibigo-0.0.9/src/bibigo/static/.gitignore.default
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo/static/.vscode/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:01:16.000000 bibigo-0.0.9/src/bibigo/static/.vscode/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      455 2023-05-28 07:19:46.000000 bibigo-0.0.9/src/bibigo/static/.vscode/settings.json.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      244 2023-05-28 10:12:41.000000 bibigo-0.0.9/src/bibigo/static/Dockerfile.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.9/src/bibigo/static/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1318 2023-05-28 11:29:11.000000 bibigo-0.0.9/src/bibigo/static/docker-compose.yml.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.9/src/bibigo/static/pyproject.toml.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      616 2023-05-28 08:20:22.000000 bibigo-0.0.9/src/bibigo/static/setup.cfg.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      736 2023-05-28 10:14:42.000000 bibigo-0.0.9/src/bibigo/utils.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-06-24 05:10:42.216777 bibigo-0.0.9/src/bibigo.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1117 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       28 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-06-24 05:10:42.000000 bibigo-0.0.9/src/bibigo.egg-info/top_level.txt
```

### Comparing `bibigo-0.0.8/LICENSE` & `bibigo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.8/README.md` & `bibigo-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.8/setup.cfg` & `bibigo-0.0.9/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 packages = find:
 package_dir = 
 	= src
 install_requires = 
 	rich
 	click
 	boto3
-	prompt_toolkit==1.0.14
-	PyInquirer
+	InquirerPy
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 bibigo =
```

### Comparing `bibigo-0.0.8/src/bibigo/__pycache__/scripts.cpython-39.pyc` & `bibigo-0.0.9/src/bibigo/__pycache__/scripts.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 28 11:11:31 2023 UTC, .py size: 1116 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 e336 7364 5c04 0000  a........6sd\...
+00000000: 610d 0d0a 0000 0000 cf79 9664 5504 0000  a........y.dU...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6503 a004 a100 6403 6404  d.l.Z.e.....d.d.
 00000050: 8400 8301 5a05 6505 a004 a100 6405 6406  ....Z.e.....d.d.
 00000060: 8400 8301 5a06 6506 a007 a100 6503 a008  ....Z.e.....e...
 00000070: 6407 a101 6408 6409 8400 8301 8301 5a09  d...d.d.......Z.
@@ -16,15 +16,15 @@
 000000f0: 2916 e900 0000 0029 02da 0e70 7269 6e74  )......)...print
 00000100: 5f66 756e 6374 696f 6eda 1075 6e69 636f  _function..unico
 00000110: 6465 5f6c 6974 6572 616c 734e 6300 0000  de_literalsNc...
 00000120: 0000 0000 0000 0000 0000 0000 0001 0000  ................
 00000130: 0043 0000 0073 0400 0000 6400 5300 a901  .C...s....d.S...
 00000140: 4ea9 0072 0500 0000 7205 0000 0072 0500  N..r....r....r..
 00000150: 0000 fa32 2f68 6f6d 652f 6575 6765 6e65  ...2/home/eugene
-00000160: 2f70 726f 6a65 6374 732f 6269 6269 676f  /projects/bibigo
+00000160: 2f70 6163 6b61 6765 732f 6269 6269 676f  /packages/bibigo
 00000170: 2f73 7263 2f62 6962 6967 6f2f 7363 7269  /src/bibigo/scri
 00000180: 7074 732e 7079 da06 6269 6269 676f 0900  pts.py..bibigo..
 00000190: 0000 7302 0000 0000 0272 0700 0000 6300  ..s......r....c.
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 000001b0: 0000 0043 0000 0073 0400 0000 6400 5300  ...C...s....d.S.
 000001c0: 7204 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
 000001d0: 0500 0000 7205 0000 0072 0600 0000 da04  ....r....r......
@@ -57,40 +57,40 @@
 00000380: 4300 0000 7318 0000 0064 0164 026c 006d  C...s....d.d.l.m
 00000390: 017d 0101 007c 017c 0083 0101 0064 0053  .}...|.|.....d.S
 000003a0: 0029 034e 720a 0000 0029 01da 0a69 6e69  .).Nr....)...ini
 000003b0: 745f 7374 6163 6b29 025a 1369 6e69 742e  t_stack).Z.init.
 000003c0: 646f 636b 6572 5f63 6f6d 706f 7365 7212  docker_composer.
 000003d0: 0000 0029 0272 0900 0000 7212 0000 0072  ...).r....r....r
 000003e0: 0500 0000 7205 0000 0072 0600 0000 da0e  ....r....r......
-000003f0: 646f 636b 6572 5f63 6f6d 706f 7365 2700  docker_compose'.
+000003f0: 646f 636b 6572 5f63 6f6d 706f 7365 2800  docker_compose(.
 00000400: 0000 7304 0000 0000 030c 0272 1300 0000  ..s........r....
 00000410: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000420: 0001 0000 0043 0000 0073 0400 0000 6400  .....C...s....d.
 00000430: 5300 7204 0000 0072 0500 0000 7205 0000  S.r....r....r...
 00000440: 0072 0500 0000 7205 0000 0072 0600 0000  .r....r....r....
-00000450: da05 6465 6275 6732 0000 0073 0200 0000  ..debug2...s....
+00000450: da05 6465 6275 6733 0000 0073 0200 0000  ..debug3...s....
 00000460: 0002 7214 0000 00da 0866 696c 656e 616d  ..r......filenam
 00000470: 657a 092d 2d76 6572 7369 6f6e da07 6465  ez.--version..de
 00000480: 6661 756c 7429 0172 1600 0000 6302 0000  fault).r....c...
 00000490: 0000 0000 0000 0000 0004 0000 0004 0000  ................
 000004a0: 0043 0000 0073 2400 0000 6401 6402 6c00  .C...s$...d.d.l.
 000004b0: 6d01 7d02 0100 7c02 7c00 7c01 6403 8d02  m.}...|.|.|.d...
 000004c0: 7d03 7402 7c03 8301 0100 6400 5300 2904  }.t.|.....d.S.).
 000004d0: 4e72 0a00 0000 2901 da04 7265 6164 2902  Nr....)...read).
 000004e0: da02 666e da07 7665 7273 696f 6e29 035a  ..fn..version).Z
 000004f0: 0575 7469 6c73 7217 0000 00da 0570 7269  .utilsr......pri
 00000500: 6e74 2904 7215 0000 0072 1900 0000 7217  nt).r....r....r.
 00000510: 0000 005a 0763 6f6e 7465 6e74 7205 0000  ...Z.contentr...
 00000520: 0072 0500 0000 7206 0000 00da 0466 696c  .r....r......fil
-00000530: 6537 0000 0073 0600 0000 0004 0c02 0c01  e7...s..........
+00000530: 6538 0000 0073 0600 0000 0004 0c02 0c01  e8...s..........
 00000540: 721b 0000 0029 0f5a 0a5f 5f66 7574 7572  r....).Z.__futur
 00000550: 655f 5f72 0200 0000 7203 0000 005a 0563  e__r....r....Z.c
 00000560: 6c69 636b da05 6772 6f75 7072 0700 0000  lick..groupr....
 00000570: 7208 0000 005a 0763 6f6d 6d61 6e64 5a08  r....Z.commandZ.
 00000580: 6172 6775 6d65 6e74 720f 0000 0072 1100  argumentr....r..
 00000590: 0000 7213 0000 0072 1400 0000 5a06 6f70  ..r....r....Z.op
 000005a0: 7469 6f6e 721b 0000 0072 0500 0000 7205  tionr....r....r.
 000005b0: 0000 0072 0500 0000 7206 0000 00da 083c  ...r....r......<
 000005c0: 6d6f 6475 6c65 3e01 0000 0073 2800 0000  module>....s(...
 000005d0: 1002 0806 0601 0a07 0601 0a04 0601 0801  ................
-000005e0: 0c06 0601 0801 0c07 0601 0801 0c09 0601  ................
+000005e0: 0c06 0601 0801 0c08 0601 0801 0c09 0601  ................
 000005f0: 0a04 0601 0801 0c01                      ........
```

### Comparing `bibigo-0.0.8/src/bibigo/__pycache__/utils.cpython-39.pyc` & `bibigo-0.0.9/src/bibigo/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.8/src/bibigo/init/__pycache__/package.cpython-39.pyc` & `bibigo-0.0.9/src/bibigo/init/__pycache__/package.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 28 10:14:42 2023 UTC, .py size: 3488 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 9229 7364 a00d 0000  a........)sd....
+00000000: 610d 0d0a 0000 0000 127a 9664 940d 0000  a........z.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6405 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6504  m.Z.m.Z.m.Z...e.
 00000070: 6407 6408 8d01 5a0b 6409 640a 8400 5a0c  d.d...Z.d.d...Z.
@@ -77,16 +77,16 @@
 000004c0: 0073 1400 0000 6401 6402 8400 7c00 a000  .s....d.d...|...
 000004d0: 6403 a101 4400 8301 5300 2904 4e63 0100  d...D...S.).Nc..
 000004e0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
 000004f0: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
 00000500: 0c7d 017c 01a0 00a1 0091 0271 0453 00a9  .}.|.......q.S..
 00000510: 0029 01da 0573 7472 6970 2902 da02 2e30  .)...strip)....0
 00000520: da01 5f72 1600 0000 7216 0000 00fa 372f  .._r....r.....7/
-00000530: 686f 6d65 2f65 7567 656e 652f 7072 6f6a  home/eugene/proj
-00000540: 6563 7473 2f62 6962 6967 6f2f 7372 632f  ects/bibigo/src/
+00000530: 686f 6d65 2f65 7567 656e 652f 7061 636b  home/eugene/pack
+00000540: 6167 6573 2f62 6962 6967 6f2f 7372 632f  ages/bibigo/src/
 00000550: 6269 6269 676f 2f69 6e69 742f 7061 636b  bibigo/init/pack
 00000560: 6167 652e 7079 da0a 3c6c 6973 7463 6f6d  age.py..<listcom
 00000570: 703e 2700 0000 f300 0000 007a 3269 6e69  p>'........z2ini
 00000580: 745f 7061 636b 6167 652e 3c6c 6f63 616c  t_package.<local
 00000590: 733e 2e3c 6c61 6d62 6461 3e2e 3c6c 6f63  s>.<lambda>.<loc
 000005a0: 616c 733e 2e3c 6c69 7374 636f 6d70 3efa  als>.<listcomp>.
 000005b0: 012c 2901 da05 7370 6c69 7429 01da 0178  .,)...split)...x
@@ -94,65 +94,65 @@
 000005d0: 083c 6c61 6d62 6461 3e27 0000 0072 1c00  .<lambda>'...r..
 000005e0: 0000 7a1e 696e 6974 5f70 6163 6b61 6765  ..z.init_package
 000005f0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
 00000600: 613e 2904 720f 0000 0072 1000 0000 7212  a>).r....r....r.
 00000610: 0000 00da 0666 696c 7465 725a 1064 6570  .....filterZ.dep
 00000620: 656e 6465 6e63 795f 6c69 6e6b 737a 1159  endency_linksz.Y
 00000630: 6f75 7220 5072 6976 6174 6520 5079 5049  our Private PyPI
-00000640: da07 636f 6e66 6972 6d7a 1343 6f6e 6669  ..confirmz.Confi
-00000650: 726d 2049 6e69 7469 616c 697a 6572 7a18  rm Initializerz.
-00000660: 5b45 5849 545d 204e 6f74 6869 6e67 2048  [EXIT] Nothing H
-00000670: 6170 7065 6e65 6421 7a04 2020 2020 da01  appened!z.    ..
-00000680: 0a7a 0e70 7970 726f 6a65 6374 2e74 6f6d  .z.pyproject.tom
-00000690: 6c29 025a 0664 7374 5f66 70da 0763 6f6e  l).Z.dst_fp..con
-000006a0: 7465 6e74 7a09 7365 7475 702e 6366 675a  tentz.setup.cfgZ
-000006b0: 0a44 6f63 6b65 7266 696c 65da 0373 7263  .Dockerfile..src
-000006c0: 5429 01da 0865 7869 7374 5f6f 6b7a 0b5f  T)...exist_okz._
-000006d0: 5f69 6e69 745f 5f2e 7079 7a16 5b62 6f6c  _init__.pyz.[bol
-000006e0: 645d 5079 7468 6f6e 2070 726f 6a65 6374  d]Python project
-000006f0: 2027 7a12 2720 6973 2072 6561 6479 2e5b   'z.' is ready.[
-00000700: 2f62 6f6c 645d 7a48 202d 2042 7569 6c64  /bold]zH - Build
-00000710: 2050 6163 6b61 6765 3a20 2770 7974 686f   Package: 'pytho
-00000720: 6e20 2d6d 2062 7569 6c64 272c 2070 7974  n -m build', pyt
-00000730: 686f 6e20 7061 636b 6167 6520 2762 7569  hon package 'bui
-00000740: 6c64 2720 6973 2072 6571 7569 7265 642e  ld' is required.
-00000750: 7a4c 202d 2055 706c 6f61 6420 746f 2050  zL - Upload to P
-00000760: 7950 493a 2027 7477 696e 6520 7570 6c6f  yPI: 'twine uplo
-00000770: 6164 2064 6973 742f 2a27 2c20 7079 7468  ad dist/*', pyth
-00000780: 6f6e 2070 6163 6b61 6765 2027 7477 696e  on package 'twin
-00000790: 6520 6973 2072 6571 7569 7265 642e 2913  e is required.).
-000007a0: 5a0a 5079 496e 7175 6972 6572 720b 0000  Z.PyInquirerr...
-000007b0: 0072 0200 0000 5a08 6162 736f 6c75 7465  .r....Z.absolute
-000007c0: 7210 0000 00da 026f 73da 0667 6574 656e  r......os..geten
-000007d0: 76da 0370 6f70 da05 7072 696e 74da 046a  v..pop..print..j
-000007e0: 6f69 6e72 0700 0000 7206 0000 00da 0666  oinr....r......f
-000007f0: 6f72 6d61 74da 056d 6b64 6972 da06 6578  ormat..mkdir..ex
-00000800: 6973 7473 5a05 746f 7563 6872 0800 0000  istsZ.touchr....
-00000810: da07 636f 6e73 6f6c 6572 0400 0000 290e  ..consoler....).
-00000820: da04 726f 6f74 720b 0000 00da 0266 7072  ..rootr......fpr
-00000830: 0e00 0000 5a0c 7072 6976 6174 655f 7079  ....Z.private_py
-00000840: 7069 5a0a 7365 7475 705f 636f 6e66 5a04  piZ.setup_confZ.
-00000850: 636f 6e66 7222 0000 005a 0354 4142 5a13  confr"...Z.TABZ.
-00000860: 5059 5052 4f4a 4543 545f 544f 4d4c 5f46  PYPROJECT_TOML_F
-00000870: 494c 455a 0e53 4554 5550 5f43 4647 5f46  ILEZ.SETUP_CFG_F
-00000880: 494c 455a 0f44 4f43 4b45 5246 494c 455f  ILEZ.DOCKERFILE_
-00000890: 4649 4c45 5a05 5f69 6e69 745a 0773 756d  FILEZ._initZ.sum
-000008a0: 6d61 7279 7216 0000 0072 1600 0000 721a  maryr....r....r.
-000008b0: 0000 00da 0c69 6e69 745f 7061 636b 6167  .....init_packag
-000008c0: 650f 0000 0073 8400 0000 0001 0c03 0801  e....s..........
-000008d0: 0a03 0e04 0c01 0a01 0a01 0a01 0c01 0a01  ................
-000008e0: 0c01 0c02 0201 0201 0201 06fc 0407 0201  ................
-000008f0: 0201 0201 02fc 0406 0aeb 0419 0801 0a01  ................
-00000900: 0401 0801 0403 0e01 0c01 1201 0401 1804  ................
-00000910: 0401 0201 0601 06fe 0606 0401 0201 0601  ................
-00000920: 12fe 0606 0401 0201 0601 06fe 0606 1001  ................
-00000930: 1801 1401 0a01 0801 1c01 1801 0a01 0803  ................
-00000940: 0402 0a01 0201 02fd 02ff 0407 0601 7232  ..............r2
-00000950: 0000 0029 0d72 2700 0000 da07 7061 7468  ...).r'.....path
-00000960: 6c69 6272 0200 0000 5a0c 7269 6368 2e63  libr....Z.rich.c
-00000970: 6f6e 736f 6c65 7203 0000 005a 0a72 6963  onsoler....Z.ric
-00000980: 682e 7061 6e65 6c72 0400 0000 da05 7574  h.panelr......ut
-00000990: 696c 7372 0600 0000 7207 0000 0072 0800  ilsr....r....r..
-000009a0: 0000 722f 0000 0072 3200 0000 7216 0000  ..r/...r2...r...
-000009b0: 0072 1600 0000 7216 0000 0072 1a00 0000  .r....r....r....
-000009c0: da08 3c6d 6f64 756c 653e 0100 0000 730c  ..<module>....s.
-000009d0: 0000 0008 010c 020c 010c 0214 020a 06    ...............
+00000640: da07 636f 6e66 6972 6d5a 0743 6f6e 6669  ..confirmZ.Confi
+00000650: 726d 7a18 5b45 5849 545d 204e 6f74 6869  rmz.[EXIT] Nothi
+00000660: 6e67 2048 6170 7065 6e65 6421 7a04 2020  ng Happened!z.  
+00000670: 2020 da01 0a7a 0e70 7970 726f 6a65 6374    ...z.pyproject
+00000680: 2e74 6f6d 6c29 025a 0664 7374 5f66 70da  .toml).Z.dst_fp.
+00000690: 0763 6f6e 7465 6e74 7a09 7365 7475 702e  .contentz.setup.
+000006a0: 6366 675a 0a44 6f63 6b65 7266 696c 65da  cfgZ.Dockerfile.
+000006b0: 0373 7263 5429 01da 0865 7869 7374 5f6f  .srcT)...exist_o
+000006c0: 6b7a 0b5f 5f69 6e69 745f 5f2e 7079 7a16  kz.__init__.pyz.
+000006d0: 5b62 6f6c 645d 5079 7468 6f6e 2070 726f  [bold]Python pro
+000006e0: 6a65 6374 2027 7a12 2720 6973 2072 6561  ject 'z.' is rea
+000006f0: 6479 2e5b 2f62 6f6c 645d 7a48 202d 2042  dy.[/bold]zH - B
+00000700: 7569 6c64 2050 6163 6b61 6765 3a20 2770  uild Package: 'p
+00000710: 7974 686f 6e20 2d6d 2062 7569 6c64 272c  ython -m build',
+00000720: 2070 7974 686f 6e20 7061 636b 6167 6520   python package 
+00000730: 2762 7569 6c64 2720 6973 2072 6571 7569  'build' is requi
+00000740: 7265 642e 7a4c 202d 2055 706c 6f61 6420  red.zL - Upload 
+00000750: 746f 2050 7950 493a 2027 7477 696e 6520  to PyPI: 'twine 
+00000760: 7570 6c6f 6164 2064 6973 742f 2a27 2c20  upload dist/*', 
+00000770: 7079 7468 6f6e 2070 6163 6b61 6765 2027  python package '
+00000780: 7477 696e 6520 6973 2072 6571 7569 7265  twine is require
+00000790: 642e 2913 5a0a 496e 7175 6972 6572 5079  d.).Z.InquirerPy
+000007a0: 720b 0000 0072 0200 0000 5a08 6162 736f  r....r....Z.abso
+000007b0: 6c75 7465 7210 0000 00da 026f 73da 0667  luter......os..g
+000007c0: 6574 656e 76da 0370 6f70 da05 7072 696e  etenv..pop..prin
+000007d0: 74da 046a 6f69 6e72 0700 0000 7206 0000  t..joinr....r...
+000007e0: 00da 0666 6f72 6d61 74da 056d 6b64 6972  ...format..mkdir
+000007f0: da06 6578 6973 7473 5a05 746f 7563 6872  ..existsZ.touchr
+00000800: 0800 0000 da07 636f 6e73 6f6c 6572 0400  ......consoler..
+00000810: 0000 290e da04 726f 6f74 720b 0000 00da  ..)...rootr.....
+00000820: 0266 7072 0e00 0000 5a0c 7072 6976 6174  .fpr....Z.privat
+00000830: 655f 7079 7069 5a0a 7365 7475 705f 636f  e_pypiZ.setup_co
+00000840: 6e66 5a04 636f 6e66 7222 0000 005a 0354  nfZ.confr"...Z.T
+00000850: 4142 5a13 5059 5052 4f4a 4543 545f 544f  ABZ.PYPROJECT_TO
+00000860: 4d4c 5f46 494c 455a 0e53 4554 5550 5f43  ML_FILEZ.SETUP_C
+00000870: 4647 5f46 494c 455a 0f44 4f43 4b45 5246  FG_FILEZ.DOCKERF
+00000880: 494c 455f 4649 4c45 5a05 5f69 6e69 745a  ILE_FILEZ._initZ
+00000890: 0773 756d 6d61 7279 7216 0000 0072 1600  .summaryr....r..
+000008a0: 0000 721a 0000 00da 0c69 6e69 745f 7061  ..r......init_pa
+000008b0: 636b 6167 650f 0000 0073 8400 0000 0001  ckage....s......
+000008c0: 0c03 0801 0a03 0e04 0c01 0a01 0a01 0a01  ................
+000008d0: 0c01 0a01 0c01 0c02 0201 0201 0201 06fc  ................
+000008e0: 0407 0201 0201 0201 02fc 0406 0aeb 0419  ................
+000008f0: 0801 0a01 0401 0801 0403 0e01 0c01 1201  ................
+00000900: 0401 1804 0401 0201 0601 06fe 0606 0401  ................
+00000910: 0201 0601 12fe 0606 0401 0201 0601 06fe  ................
+00000920: 0606 1001 1801 1401 0a01 0801 1c01 1801  ................
+00000930: 0a01 0803 0402 0a01 0201 02fd 02ff 0407  ................
+00000940: 0601 7232 0000 0029 0d72 2700 0000 da07  ..r2...).r'.....
+00000950: 7061 7468 6c69 6272 0200 0000 5a0c 7269  pathlibr....Z.ri
+00000960: 6368 2e63 6f6e 736f 6c65 7203 0000 005a  ch.consoler....Z
+00000970: 0a72 6963 682e 7061 6e65 6c72 0400 0000  .rich.panelr....
+00000980: da05 7574 696c 7372 0600 0000 7207 0000  ..utilsr....r...
+00000990: 0072 0800 0000 722f 0000 0072 3200 0000  .r....r/...r2...
+000009a0: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+000009b0: 1a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000009c0: 0000 730c 0000 0008 010c 020c 010c 0214  ..s.............
+000009d0: 020a 06                                  ...
```

### Comparing `bibigo-0.0.8/src/bibigo/init/__pycache__/settings.cpython-39.pyc` & `bibigo-0.0.9/src/bibigo/init/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.8/src/bibigo/init/docker_compose.py` & `bibigo-0.0.9/src/bibigo/init/docker_compose.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,34 +9,49 @@
 console = Console(width=88)
 
 
 ################################################################
 # init package
 ################################################################
 def init_stack(root):
-    from PyInquirer import prompt
+    from InquirerPy import prompt
 
     # get service name from input
     fp = Path(root)
     service = fp.absolute().name
 
     # get private pypi url
     domain = os.getenv("DOMAIN") or "example.com"
 
     # set setup configuration
     deploy_conf = [
         {"type": "input", "name": "service", "default": service, "message": "Service Name"},
         {"type": "input", "name": "image", "default": "hello-world:latest", "message": "Image"},
         {"type": "input", "name": "command", "default": "/hello", "message": "Container Command"},
-        {"type": "input", "name": "mode", "default": "replicated", "message": "Deploy Mode ('replicated' or 'global')"},
+        {
+            "type": "input",
+            "name": "mode",
+            "default": "replicated",
+            "message": "Deploy Mode ('replicated' or 'global')",
+        },
         {"type": "input", "name": "role", "default": "worker", "message": "Deploy Placement ('manager' or 'worker')"},
         {"type": "input", "name": "replicas", "default": "1", "message": "Replicas (No. of Containers)"},
         {"type": "input", "name": "http-entrypoint", "default": "web", "message": "Traefik Entrypoint for HTTP"},
-        {"type": "input", "name": "https-entrypoint", "default": "websecure", "message": "Traefik Entrypoint for HTTPS"},
-        {"type": "input", "name": "http-redirect", "default": "http-redirect", "message": "Traefik Middlware for HTTP Redirect"},
+        {
+            "type": "input",
+            "name": "https-entrypoint",
+            "default": "websecure",
+            "message": "Traefik Entrypoint for HTTPS",
+        },
+        {
+            "type": "input",
+            "name": "http-redirect",
+            "default": "http-redirect",
+            "message": "Traefik Middlware for HTTP Redirect",
+        },
         {"type": "input", "name": "certresolver", "default": "lego", "message": "Certificate Resolver"},
         {"type": "input", "name": "traefik-network", "default": "traefik", "message": "Docker Network for Traefik"},
         {"type": "input", "name": "domain", "default": f"{service}.{domain}", "message": "Domain for Your Service"},
         {"type": "input", "name": "port", "default": "3000", "message": "Service Port"},
         {"type": "confirm", "name": "confirm", "message": "Confirm"},
     ]
 
@@ -45,18 +60,15 @@
     confirm = conf.pop("confirm")
     if not confirm:
         print("[EXIT] Nothing Happened!")
         return
 
     # [WRITE FILES]
     DOCKER_COMPOSE_FILE = "docker-compose.yml"
-    write(
-        dst_fp=fp / DOCKER_COMPOSE_FILE,
-        content=read(DOCKER_COMPOSE_FILE).format(**conf)
-    )
+    write(dst_fp=fp / DOCKER_COMPOSE_FILE, content=read(DOCKER_COMPOSE_FILE).format(**conf))
 
     # [LOGGING]
     summary = "\n".join(
         [
             f"[bold]docker-compose.yml for '{service}' is ready.[/bold]",
         ]
     )
```

### Comparing `bibigo-0.0.8/src/bibigo/init/package.py` & `bibigo-0.0.9/src/bibigo/init/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 console = Console(width=88)
 
 
 ################################################################
 # init package
 ################################################################
 def init_package(root):
-    from PyInquirer import prompt
+    from InquirerPy import prompt
 
     # get project name from input
     fp = Path(root)
     project = fp.absolute().name
 
     # get private pypi url
     private_pypi = os.getenv("PIP_INDEX_URL") or ""
```

### Comparing `bibigo-0.0.8/src/bibigo/init/settings.py` & `bibigo-0.0.9/src/bibigo/init/settings.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.8/src/bibigo/scripts.py` & `bibigo-0.0.9/src/bibigo/scripts.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,20 +31,21 @@
 @click.argument("root")
 def package(root):
     from .init.package import init_package
     from .init.settings import init_settings
 
     init_settings(root)
     init_package(root)
-    
+
+
 @init.command()
 @click.argument("root")
 def docker_compose(root):
     from .init.docker_compose import init_stack
-    
+
     init_stack(root)
 
 
 ################
 # debug
 ################
 @bibigo.group()
```

### Comparing `bibigo-0.0.8/src/bibigo/static/.dockerignore.default` & `bibigo-0.0.9/src/bibigo/static/.dockerignore.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.8/src/bibigo/static/.gitignore.default` & `bibigo-0.0.9/src/bibigo/static/.gitignore.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.8/src/bibigo/static/docker-compose.yml.default` & `bibigo-0.0.9/src/bibigo/static/docker-compose.yml.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.8/src/bibigo/static/setup.cfg.default` & `bibigo-0.0.9/src/bibigo/static/setup.cfg.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.8/src/bibigo/utils.py` & `bibigo-0.0.9/src/bibigo/utils.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.8/src/bibigo.egg-info/SOURCES.txt` & `bibigo-0.0.9/src/bibigo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

