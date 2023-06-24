# Comparing `tmp/pmcyg-3.2.0.tar.gz` & `tmp/pmcyg-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmcyg-3.2.0.tar", last modified: Mon May 29 12:17:02 2023, max compression
+gzip compressed data, was "pmcyg-3.2.2.tar", last modified: Sat Jun 24 07:36:04 2023, max compression
```

## Comparing `pmcyg-3.2.0.tar` & `pmcyg-3.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-05-29 12:17:02.773532 pmcyg-3.2.0/
--rw-r-----   0 richard   (1000) richard   (1000)      487 2023-05-29 07:50:12.000000 pmcyg-3.2.0/Authors.txt
--rw-r-----   0 richard   (1000) richard   (1000)     9812 2023-05-29 07:37:12.000000 pmcyg-3.2.0/ChangeLog.txt
--rw-r-----   0 richard   (1000) richard   (1000)    35068 2009-04-21 20:11:53.000000 pmcyg-3.2.0/LICENSE.txt
--rw-r-----   0 richard   (1000) richard   (1000)      118 2020-08-08 10:13:30.000000 pmcyg-3.2.0/MANIFEST.in
--rw-r-----   0 richard   (1000) richard   (1000)      930 2023-05-28 18:11:57.000000 pmcyg-3.2.0/Makefile
--rw-r-----   0 richard   (1000) richard   (1000)      812 2023-05-29 12:17:02.773532 pmcyg-3.2.0/PKG-INFO
--rw-r-----   0 richard   (1000) richard   (1000)     8820 2023-05-29 07:55:20.000000 pmcyg-3.2.0/README.md
--rw-r-----   0 richard   (1000) richard   (1000)     3650 2023-05-29 07:42:13.000000 pmcyg-3.2.0/example.pkgs
-drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-05-29 12:17:02.773532 pmcyg-3.2.0/pmcyg/
--rw-r-----   0 richard   (1000) richard   (1000)      907 2021-10-03 15:31:33.000000 pmcyg-3.2.0/pmcyg/__init__.py
--rw-r-----   0 richard   (1000) richard   (1000)      987 2021-10-09 09:35:05.000000 pmcyg-3.2.0/pmcyg/apptools.py
--rw-r-----   0 richard   (1000) richard   (1000)     5645 2021-10-03 15:38:59.000000 pmcyg-3.2.0/pmcyg/command_line.py
--rw-r-----   0 richard   (1000) richard   (1000)    60432 2023-05-29 07:29:06.000000 pmcyg-3.2.0/pmcyg/core.py
--rw-r-----   0 richard   (1000) richard   (1000)    25575 2023-05-28 18:24:22.000000 pmcyg-3.2.0/pmcyg/gui.py
--rw-r-----   0 richard   (1000) richard   (1000)    10180 2020-08-08 10:13:30.000000 pmcyg-3.2.0/pmcyg/gui_imgs.py
--rw-r-----   0 richard   (1000) richard   (1000)       97 2023-05-29 04:48:48.000000 pmcyg-3.2.0/pmcyg/version.py
-drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-05-29 12:17:02.773532 pmcyg-3.2.0/pmcyg.egg-info/
--rw-r-----   0 richard   (1000) richard   (1000)      812 2023-05-29 12:17:02.000000 pmcyg-3.2.0/pmcyg.egg-info/PKG-INFO
--rw-r-----   0 richard   (1000) richard   (1000)      400 2023-05-29 12:17:02.000000 pmcyg-3.2.0/pmcyg.egg-info/SOURCES.txt
--rw-r-----   0 richard   (1000) richard   (1000)        1 2023-05-29 12:17:02.000000 pmcyg-3.2.0/pmcyg.egg-info/dependency_links.txt
--rw-r-----   0 richard   (1000) richard   (1000)       51 2023-05-29 12:17:02.000000 pmcyg-3.2.0/pmcyg.egg-info/entry_points.txt
--rw-r-----   0 richard   (1000) richard   (1000)        6 2023-05-29 12:17:02.000000 pmcyg-3.2.0/pmcyg.egg-info/top_level.txt
--rwxr-x--x   0 richard   (1000) richard   (1000)      854 2023-05-28 16:17:49.000000 pmcyg-3.2.0/pmcyg.py
--rw-r-----   0 richard   (1000) richard   (1000)       90 2021-10-03 14:52:29.000000 pmcyg-3.2.0/pyproject.toml
--rw-r-----   0 richard   (1000) richard   (1000)       38 2023-05-29 12:17:02.773532 pmcyg-3.2.0/setup.cfg
--rw-r-----   0 richard   (1000) richard   (1000)     1392 2021-10-03 15:19:53.000000 pmcyg-3.2.0/setup.py
-drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-05-29 12:17:02.773532 pmcyg-3.2.0/test/
--rw-r-----   0 richard   (1000) richard   (1000)    25827 2023-05-29 04:45:42.000000 pmcyg-3.2.0/test/testPMCyg.py
+drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-06-24 07:36:04.368392 pmcyg-3.2.2/
+-rw-r-----   0 richard   (1000) richard   (1000)      613 2023-06-24 07:20:19.000000 pmcyg-3.2.2/Authors.txt
+-rw-r-----   0 richard   (1000) richard   (1000)     9933 2023-06-24 07:22:05.000000 pmcyg-3.2.2/ChangeLog.txt
+-rw-r-----   0 richard   (1000) richard   (1000)    35068 2009-04-21 20:11:53.000000 pmcyg-3.2.2/LICENSE.txt
+-rw-r-----   0 richard   (1000) richard   (1000)      118 2020-08-08 10:13:30.000000 pmcyg-3.2.2/MANIFEST.in
+-rw-r-----   0 richard   (1000) richard   (1000)      930 2023-05-28 18:11:57.000000 pmcyg-3.2.2/Makefile
+-rw-r-----   0 richard   (1000) richard   (1000)      812 2023-06-24 07:36:04.368392 pmcyg-3.2.2/PKG-INFO
+-rw-r-----   0 richard   (1000) richard   (1000)     8820 2023-05-29 07:55:20.000000 pmcyg-3.2.2/README.md
+-rw-r-----   0 richard   (1000) richard   (1000)     3650 2023-05-29 07:42:13.000000 pmcyg-3.2.2/example.pkgs
+drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-06-24 07:36:04.368392 pmcyg-3.2.2/pmcyg/
+-rw-r-----   0 richard   (1000) richard   (1000)      907 2021-10-03 15:31:33.000000 pmcyg-3.2.2/pmcyg/__init__.py
+-rw-r-----   0 richard   (1000) richard   (1000)      987 2021-10-09 09:35:05.000000 pmcyg-3.2.2/pmcyg/apptools.py
+-rw-r-----   0 richard   (1000) richard   (1000)     5685 2023-06-24 07:08:16.000000 pmcyg-3.2.2/pmcyg/command_line.py
+-rw-r-----   0 richard   (1000) richard   (1000)    60451 2023-06-24 07:10:36.000000 pmcyg-3.2.2/pmcyg/core.py
+-rw-r-----   0 richard   (1000) richard   (1000)    25575 2023-05-28 18:24:22.000000 pmcyg-3.2.2/pmcyg/gui.py
+-rw-r-----   0 richard   (1000) richard   (1000)    10180 2020-08-08 10:13:30.000000 pmcyg-3.2.2/pmcyg/gui_imgs.py
+-rw-r-----   0 richard   (1000) richard   (1000)       97 2023-06-24 06:59:46.000000 pmcyg-3.2.2/pmcyg/version.py
+drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-06-24 07:36:04.368392 pmcyg-3.2.2/pmcyg.egg-info/
+-rw-r-----   0 richard   (1000) richard   (1000)      812 2023-06-24 07:36:04.000000 pmcyg-3.2.2/pmcyg.egg-info/PKG-INFO
+-rw-r-----   0 richard   (1000) richard   (1000)      400 2023-06-24 07:36:04.000000 pmcyg-3.2.2/pmcyg.egg-info/SOURCES.txt
+-rw-r-----   0 richard   (1000) richard   (1000)        1 2023-06-24 07:36:04.000000 pmcyg-3.2.2/pmcyg.egg-info/dependency_links.txt
+-rw-r-----   0 richard   (1000) richard   (1000)       51 2023-06-24 07:36:04.000000 pmcyg-3.2.2/pmcyg.egg-info/entry_points.txt
+-rw-r-----   0 richard   (1000) richard   (1000)        6 2023-06-24 07:36:04.000000 pmcyg-3.2.2/pmcyg.egg-info/top_level.txt
+-rwxr-x--x   0 richard   (1000) richard   (1000)      854 2023-05-28 16:17:49.000000 pmcyg-3.2.2/pmcyg.py
+-rw-r-----   0 richard   (1000) richard   (1000)       90 2021-10-03 14:52:29.000000 pmcyg-3.2.2/pyproject.toml
+-rw-r-----   0 richard   (1000) richard   (1000)       38 2023-06-24 07:36:04.368392 pmcyg-3.2.2/setup.cfg
+-rw-r-----   0 richard   (1000) richard   (1000)     1465 2023-06-13 16:43:51.000000 pmcyg-3.2.2/setup.py
+drwxr-x--x   0 richard   (1000) richard   (1000)        0 2023-06-24 07:36:04.368392 pmcyg-3.2.2/test/
+-rw-r-----   0 richard   (1000) richard   (1000)    25827 2023-05-29 04:45:42.000000 pmcyg-3.2.2/test/testPMCyg.py
```

### Comparing `pmcyg-3.2.0/ChangeLog.txt` & `pmcyg-3.2.2/ChangeLog.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ## ChangeLog for 'pmcyg' - a tool for partial mirroring of Cygwin(TM) archives
 ## https://github.com/rwpenney/pmcyg
 ## (C)Copyright 2009-2023, RW Penney
 
+24Jun23
+    Fixed missing import for --generate-replica option
+
+13Jun23
+    Fixed local-import issue affecting pip-23.1
+
 29May23 **** pmcyg-3.2 released ****
 
 29May23
     Fixed missing line-ending on output setup.ini
     Added explicit text encodings on textfile read/write operations
 
 28May23
```

### Comparing `pmcyg-3.2.0/LICENSE.txt` & `pmcyg-3.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pmcyg-3.2.0/Makefile` & `pmcyg-3.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `pmcyg-3.2.0/PKG-INFO` & `pmcyg-3.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: pmcyg
-Version: 3.2.0
+Version: 3.2.2
 Summary: Utility for creating offline Cygwin installers
 Home-page: https://github.com/rwpenney/pmcyg
 Author: RW Penney
 Author-email: rwpenney@users.sourceforge.net
 License: GPL v3
-Download-URL: https://github.com/rwpenney/pmcyg/archive/pmcyg-3.2.0.tar.gz
+Download-URL: https://github.com/rwpenney/pmcyg/archive/pmcyg-3.2.2.tar.gz
 Description: pmcyg is a tool for creating an offline Cygwin installer containing customized collections of packages. This avoids having to download the entirety of a Cygwin release, which might occupy many GB, instead allowing installers that can be as small as 40MB. pmcyg enables Cygwin installation from a self-contained CD/DVD image or USB-flash for use on systems without internet access.
 Keywords: Cygwin
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `pmcyg-3.2.0/README.md` & `pmcyg-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pmcyg-3.2.0/example.pkgs` & `pmcyg-3.2.2/example.pkgs`

 * *Files identical despite different names*

### Comparing `pmcyg-3.2.0/pmcyg/__init__.py` & `pmcyg-3.2.2/pmcyg/__init__.py`

 * *Files identical despite different names*

### Comparing `pmcyg-3.2.0/pmcyg/apptools.py` & `pmcyg-3.2.2/pmcyg/apptools.py`

 * *Files identical despite different names*

### Comparing `pmcyg-3.2.0/pmcyg/command_line.py` & `pmcyg-3.2.2/pmcyg/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Application entry-point for "pmcyg" tool
 """
 
 import argparse, sys
 from . import apptools, core, gui, version
-from .core import PMbuilder
+from .core import HOST_IS_CYGWIN, PMbuilder
 from .version import PMCYG_VERSION
 
 
 def ProcessPackageFiles(builder: PMbuilder, pkgfiles: list) -> None:
     """Subsidiary program entry-point if used as command-line application"""
     try:
         apptools.ProcessPackageFiles(builder, pkgfiles)
@@ -18,14 +18,17 @@
         #import traceback; traceback.print_exc()
 
 
 def TemplateMain(builder: PMbuilder, outfile: str,
                  pkgfiles: list, cygwinReplica: bool=False) -> None:
     """Subsidiary program entry-point for command-line list generation"""
 
+    if cygwinReplica and not HOST_IS_CYGWIN:
+        print('WARNING: pmcyg attempting to create replica of non-Cygwin host',
+              file=sys.stderr)
     builder.TemplateFromLists(outfile, pkgfiles, cygwinReplica)
 
 
 def GUImain(builder: PMbuilder, pkgfiles: list) -> None:
     """Subsidiary program entry-point if used as GUI application"""
 
     pgui = gui.TKgui(builder, pkgfiles=pkgfiles)
@@ -112,16 +115,14 @@
     builder.SetOption('IncludeSources', args.with_sources)
     builder.SetOption('RemoveOutdated', args.remove_outdated)
     builder.SetOption('ISOfilename', args.iso_filename)
 
     if args.pkg_file:
         TemplateMain(builder, args.pkg_file, args.package_files)
     elif args.cyg_list:
-        if not HOST_IS_CYGWIN:
-            print('WARNING: pmcyg attempting to create replica of non-Cygwin host', file=sys.stderr)
         TemplateMain(builder, args.cyg_list,
                      args.package_files, cygwinReplica=True)
     elif gui.HASGUI and not args.nogui:
         GUImain(builder, args.package_files)
     else:
         ProcessPackageFiles(builder, args.package_files)
```

### Comparing `pmcyg-3.2.0/pmcyg/core.py` & `pmcyg-3.2.2/pmcyg/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,15 +515,15 @@
         as a fall-back in case the live listing of mirrors cannot
         be downloaded."""
         return io.BytesIO(b'''
 http://ucmirror.canterbury.ac.nz/cygwin/;ucmirror.canterbury.ac.nz;Australasia;New Zealand
 https://mirror.csclub.uwaterloo.ca/cygwin/;mirror.csclub.uwaterloo.ca;North America;Canada
 https://ftp.fsn.hu/pub/cygwin/;ftp.fsn.hu;Europe;Hungary
 https://ftp.iij.ad.jp/pub/cygwin/;ftp.iij.ad.jp;Asia;Japan
-https://cygwin.osuosl.org/;cygwin.osuosl.org;North America;United States
+https://mirror.csclub.uwaterloo.ca/cygwin/;mirror.csclub.uwaterloo.ca;North America;Canada
 https://mirrors.dotsrc.org/cygwin/;mirrors.dotsrc.org;Europe;Denmark
 https://www.mirrorservice.org/sites/sourceware.org/pub/cygwin/;www.mirrorservice.org;Europe;UK
                 ''')
 
     def _resolveDependencies(self, usrpkgs=None):
         """Constuct list of packages, including all their dependencies"""
 
@@ -1046,15 +1046,15 @@
         catgroups = self._masterList.GetCategories()
         catlist = [ c for c in catgroups.keys() if c != 'All' ]
         catlist.sort()
 
         if pkgset:
             userpkgs = set(pkgset.extract())
         else:
-            userpkgs = None
+            userpkgs = set()
 
         lines = [ \
             '# Package listing for pmcyg (Cygwin(TM) Partial Mirror)',
             '# Autogenerated on ' + time.asctime(),
             '# from: ' + self._masterList.GetSourceURL(),
             '',
             '# This file contains listings of cygwin package names,' \
```

### Comparing `pmcyg-3.2.0/pmcyg/gui.py` & `pmcyg-3.2.2/pmcyg/gui.py`

 * *Files identical despite different names*

### Comparing `pmcyg-3.2.0/pmcyg/gui_imgs.py` & `pmcyg-3.2.2/pmcyg/gui_imgs.py`

 * *Files identical despite different names*

### Comparing `pmcyg-3.2.0/pmcyg.egg-info/PKG-INFO` & `pmcyg-3.2.2/pmcyg.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: pmcyg
-Version: 3.2.0
+Version: 3.2.2
 Summary: Utility for creating offline Cygwin installers
 Home-page: https://github.com/rwpenney/pmcyg
 Author: RW Penney
 Author-email: rwpenney@users.sourceforge.net
 License: GPL v3
-Download-URL: https://github.com/rwpenney/pmcyg/archive/pmcyg-3.2.0.tar.gz
+Download-URL: https://github.com/rwpenney/pmcyg/archive/pmcyg-3.2.2.tar.gz
 Description: pmcyg is a tool for creating an offline Cygwin installer containing customized collections of packages. This avoids having to download the entirety of a Cygwin release, which might occupy many GB, instead allowing installers that can be as small as 40MB. pmcyg enables Cygwin installation from a self-contained CD/DVD image or USB-flash for use on systems without internet access.
 Keywords: Cygwin
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `pmcyg-3.2.0/pmcyg.py` & `pmcyg-3.2.2/pmcyg.py`

 * *Files identical despite different names*

### Comparing `pmcyg-3.2.0/setup.py` & `pmcyg-3.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/python3
 # Installation/setup script for Simple Python Fixed-Point Module
 # RW Penney, July 2010
 
 from setuptools import setup
-import os, re, shutil
+import os, re, sys, shutil
+base_path = os.path.dirname(__file__)
+sys.path.insert(0, base_path)
 from pmcyg.version import PMCYG_VERSION
 
 
 setup(
     author = 'RW Penney',
     author_email = 'rwpenney@users.sourceforge.net',
     description = 'Utility for creating offline Cygwin installers',
```

### Comparing `pmcyg-3.2.0/test/testPMCyg.py` & `pmcyg-3.2.2/test/testPMCyg.py`

 * *Files identical despite different names*

