# Comparing `tmp/pyqos-0.2.2.tar.gz` & `tmp/pyqos-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyqos-0.2.2.tar", last modified: Fri Jun 23 07:50:30 2017, max compression
+gzip compressed data, was "pyqos-0.3.0.tar", last modified: Sat Jun 24 12:20:09 2023, max compression
```

## Comparing `pyqos-0.2.2.tar` & `pyqos-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,65 @@
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2017-06-23 07:50:30.000000 pyqos-0.2.2/
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2017-06-23 07:50:30.000000 pyqos-0.2.2/pyqos/
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2017-06-23 07:50:30.000000 pyqos-0.2.2/pyqos/algorithms/
--rw-r--r--   0 anthony   (1000) users      (100)     4018 2017-03-21 00:08:16.000000 pyqos-0.2.2/pyqos/algorithms/__init__.py
--rw-r--r--   0 anthony   (1000) users      (100)     2235 2017-03-21 00:08:16.000000 pyqos-0.2.2/pyqos/algorithms/classless_qdiscs.py
--rw-r--r--   0 anthony   (1000) users      (100)    12881 2017-03-21 00:08:16.000000 pyqos-0.2.2/pyqos/algorithms/htb.py
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2017-06-23 07:50:30.000000 pyqos-0.2.2/pyqos/backend/
--rw-r--r--   0 anthony   (1000) users      (100)        0 2017-03-21 00:08:16.000000 pyqos-0.2.2/pyqos/backend/__init__.py
--rw-r--r--   0 anthony   (1000) users      (100)     8737 2017-03-21 00:08:16.000000 pyqos-0.2.2/pyqos/backend/tc.py
--rw-r--r--   0 anthony   (1000) users      (100)      214 2017-03-21 00:08:16.000000 pyqos-0.2.2/pyqos/__init__.py
--rw-r--r--   0 anthony   (1000) users      (100)     5166 2017-03-21 00:08:16.000000 pyqos-0.2.2/pyqos/app.py
--rw-r--r--   0 anthony   (1000) users      (100)     4143 2017-06-23 07:36:45.000000 pyqos-0.2.2/pyqos/config.py
--rw-r--r--   0 anthony   (1000) users      (100)      800 2017-03-21 00:08:16.000000 pyqos-0.2.2/pyqos/decorators.py
--rw-r--r--   0 anthony   (1000) users      (100)      151 2017-03-21 00:08:16.000000 pyqos-0.2.2/pyqos/exceptions.py
--rw-r--r--   0 anthony   (1000) users      (100)     1265 2017-03-21 00:08:16.000000 pyqos-0.2.2/pyqos/tools.py
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2017-06-23 07:50:30.000000 pyqos-0.2.2/pyqos.egg-info/
--rw-r--r--   0 anthony   (1000) users      (100)     2216 2017-06-23 07:50:30.000000 pyqos-0.2.2/pyqos.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) users      (100)      435 2017-06-23 07:50:30.000000 pyqos-0.2.2/pyqos.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) users      (100)        1 2017-06-23 07:50:30.000000 pyqos-0.2.2/pyqos.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) users      (100)        9 2017-06-23 07:50:30.000000 pyqos-0.2.2/pyqos.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) users      (100)        6 2017-06-23 07:50:30.000000 pyqos-0.2.2/pyqos.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) users      (100)     1514 2017-03-21 00:08:16.000000 pyqos-0.2.2/LICENSE.mkd
--rw-r--r--   0 anthony   (1000) users      (100)       74 2017-03-21 00:08:17.000000 pyqos-0.2.2/MANIFEST.in
--rw-r--r--   0 anthony   (1000) users      (100)     1280 2017-03-21 00:08:16.000000 pyqos-0.2.2/README.mkd
--rw-r--r--   0 anthony   (1000) users      (100)      190 2017-06-23 07:50:30.000000 pyqos-0.2.2/setup.cfg
--rwxr-xr-x   0 anthony   (1000) users      (100)     1145 2017-06-23 07:38:19.000000 pyqos-0.2.2/setup.py
--rw-r--r--   0 anthony   (1000) users      (100)     2216 2017-06-23 07:50:30.000000 pyqos-0.2.2/PKG-INFO
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/
+-rw-r--r--   0 anthony   (1000) users      (100)      742 2022-04-12 08:46:23.000000 pyqos-0.3.0/.gitignore
+-rw-r--r--   0 anthony   (1000) users      (100)     1514 2017-03-21 00:08:16.000000 pyqos-0.3.0/LICENSE.mkd
+-rw-r--r--   0 anthony   (1000) users      (100)       74 2022-04-12 08:46:23.000000 pyqos-0.3.0/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) users      (100)     1835 2023-06-24 12:20:09.774125 pyqos-0.3.0/PKG-INFO
+-rw-r--r--   0 anthony   (1000) users      (100)     1280 2022-04-12 08:46:23.000000 pyqos-0.3.0/README.mkd
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.770792 pyqos-0.3.0/docs/
+-rw-r--r--   0 anthony   (1000) users      (100)     6770 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/Makefile
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.770792 pyqos-0.3.0/docs/_static/
+-rw-r--r--   0 anthony   (1000) users      (100)       40 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/_static/theme_override.css
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/docs/api/
+-rw-r--r--   0 anthony   (1000) users      (100)     1247 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/api/alg_classful.rst
+-rw-r--r--   0 anthony   (1000) users      (100)      700 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/api/alg_classless.rst
+-rw-r--r--   0 anthony   (1000) users      (100)      118 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/api/algorithms.rst
+-rw-r--r--   0 anthony   (1000) users      (100)      576 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/api/global.rst
+-rw-r--r--   0 anthony   (1000) users      (100)      481 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/api/index.rst
+-rw-r--r--   0 anthony   (1000) users      (100)     2616 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/conf.py
+-rw-r--r--   0 anthony   (1000) users      (100)     4063 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/configuration.rst
+-rw-r--r--   0 anthony   (1000) users      (100)      395 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/index.rst
+-rw-r--r--   0 anthony   (1000) users      (100)     6705 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/make.bat
+-rw-r--r--   0 anthony   (1000) users      (100)     6175 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/quickstart.rst
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/docs/tutorial/
+-rw-r--r--   0 anthony   (1000) users      (100)      446 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/tutorial/index.rst
+-rw-r--r--   0 anthony   (1000) users      (100)     3711 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/tutorial/tutorial_part1.rst
+-rw-r--r--   0 anthony   (1000) users      (100)      789 2022-04-12 08:46:23.000000 pyqos-0.3.0/docs/tutorial/tutorial_part2.rst
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/example/
+-rw-r--r--   0 anthony   (1000) users      (100)        0 2022-04-12 08:46:23.000000 pyqos-0.3.0/example/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)     1310 2022-04-12 08:46:23.000000 pyqos-0.3.0/example/config.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/example/rules/
+-rw-r--r--   0 anthony   (1000) users      (100)      144 2022-04-12 08:46:23.000000 pyqos-0.3.0/example/rules/__init__.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/example/rules/download/
+-rw-r--r--   0 anthony   (1000) users      (100)      463 2022-04-12 08:46:23.000000 pyqos-0.3.0/example/rules/download/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)     1704 2022-04-12 08:46:23.000000 pyqos-0.3.0/example/rules/download/download.py
+-rw-r--r--   0 anthony   (1000) users      (100)      470 2022-04-12 08:46:23.000000 pyqos-0.3.0/example/rules/qos_formulas.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/example/rules/upload/
+-rw-r--r--   0 anthony   (1000) users      (100)      474 2022-04-12 08:46:23.000000 pyqos-0.3.0/example/rules/upload/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)     1685 2022-04-12 08:46:23.000000 pyqos-0.3.0/example/rules/upload/upload.py
+-rwxr-xr-x   0 anthony   (1000) users      (100)       88 2022-04-12 08:46:23.000000 pyqos-0.3.0/example/run.py
+-rw-r--r--   0 anthony   (1000) users      (100)      146 2022-04-12 08:46:23.000000 pyqos-0.3.0/exceptions.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/pyqos/
+-rw-r--r--   0 anthony   (1000) users      (100)      214 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/__init__.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/pyqos/algorithms/
+-rw-r--r--   0 anthony   (1000) users      (100)     4039 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/algorithms/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)     7001 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/algorithms/classless_qdiscs.py
+-rw-r--r--   0 anthony   (1000) users      (100)    13050 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/algorithms/htb.py
+-rw-r--r--   0 anthony   (1000) users      (100)     5166 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/app.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/pyqos/backend/
+-rw-r--r--   0 anthony   (1000) users      (100)        0 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/backend/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)     8990 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/backend/tc.py
+-rw-r--r--   0 anthony   (1000) users      (100)     4143 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/config.py
+-rw-r--r--   0 anthony   (1000) users      (100)      800 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/decorators.py
+-rw-r--r--   0 anthony   (1000) users      (100)      151 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/exceptions.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.770792 pyqos-0.3.0/pyqos/tests/
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/pyqos/tests/backend/
+-rw-r--r--   0 anthony   (1000) users      (100)     6700 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/tests/backend/test_tc.py
+-rw-r--r--   0 anthony   (1000) users      (100)     1265 2022-04-12 08:46:23.000000 pyqos-0.3.0/pyqos/tools.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-06-24 12:20:09.774125 pyqos-0.3.0/pyqos.egg-info/
+-rw-r--r--   0 anthony   (1000) users      (100)     1835 2023-06-24 12:20:09.000000 pyqos-0.3.0/pyqos.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) users      (100)     1088 2023-06-24 12:20:09.000000 pyqos-0.3.0/pyqos.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) users      (100)        1 2023-06-24 12:20:09.000000 pyqos-0.3.0/pyqos.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) users      (100)        9 2023-06-24 12:20:09.000000 pyqos-0.3.0/pyqos.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) users      (100)        6 2023-06-24 12:20:09.000000 pyqos-0.3.0/pyqos.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) users      (100)        9 2022-04-12 08:46:23.000000 pyqos-0.3.0/requirements.txt
+-rw-r--r--   0 anthony   (1000) users      (100)      190 2023-06-24 12:20:09.774125 pyqos-0.3.0/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) users      (100)     1145 2022-04-12 08:46:23.000000 pyqos-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyqos-0.2.2/pyqos/algorithms/__init__.py` & `pyqos-0.3.0/pyqos/algorithms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,12 +120,12 @@
         if parent is not None:
             self.parent = parent
         if interface is not None:
             self.interface = interface
         if id is not None:
             self.id = id
 
-    def apply(self):
-        raise NotImplemented
+    def apply(self, dryrun=False):
+        raise NotImplementedError()
 
 
 from . import classless_qdiscs, htb
```

### Comparing `pyqos-0.2.2/pyqos/algorithms/htb.py` & `pyqos-0.3.0/pyqos/algorithms/htb.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import inspect
 
 from pyqos import tools
 from pyqos.backend import tc
 from pyqos.exceptions import BadAttributeValueException, NoParentException
 from . import _BasicQDisc
-from .classless_qdiscs import FQCodel, PFIFO, SFQ
+from .classless_qdiscs import Cake, FQCodel, PFIFO, SFQ
 
 
 class HTBQdisc(_BasicQDisc):
     """
     Implement the qdisc which will be directly set on the network interface
     """
     @property
@@ -242,15 +242,15 @@
         return self._getter_burst_cburst(self._cburst)
 
     def _set_cburst(self, obj=None, value=None):
         if obj is not None:
             self = obj
         self._cburst = value
 
-    def _add_class(self):
+    def _add_class(self, *args, **kwargs):
         pass
 
     def add_child(self, *args):
         """
         Add a class as children
         """
         for class_child in args:
@@ -408,14 +408,21 @@
         self._add_class(dryrun=dryrun)
         self.qdisc.apply(dryrun=dryrun)
         self._add_filter(dryrun=dryrun)
         for child in self.children:
             child.apply(auto_quantum=auto_quantum, dryrun=dryrun)
 
 
+class HTBFilterCake(HTBFilter):
+    """
+    Lazy wrapper to get a HTB class with a filter and a Cake qdisc already set
+    """
+    qdisc = Cake
+
+
 class HTBFilterFQCodel(HTBFilter):
     """
     Lazy wrapper to get a HTB class with a filter and a FQCodel qdisc already
     set
     """
     qdisc = FQCodel
```

### Comparing `pyqos-0.2.2/pyqos/backend/tc.py` & `pyqos-0.3.0/pyqos/backend/tc.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,58 +3,66 @@
 
 from pyqos.tools import launch_command
 from pyqos.decorators import multiple_interfaces
 
 
 @multiple_interfaces
 def qdisc(interface, action, algorithm=None, handle=None, parent=None,
-          stderr=None, dryrun=False, *args, **kwargs):
+          stderr=None, dryrun=False, opts_args=None, **kwargs):
     """
     Add/change/replace/replace qdisc
 
     **kwargs will be used for specific arguments, depending on the algorithm
     used.
 
     :param action: "add", "replace", "change" or "delete"
     :param interface: target interface
     :param algorithm: algorithm used for this leaf (htb, pfifo, sfq, ...)
     :param handle: handle parameter for tc (default: None)
     :param parent: if is None, the rule will be added as root. (default: None)
     :param stderr: indicates stderr to use during the tc commands execution
+    :param opts_args: list of options without value, to append to the command
     """
+    opts_args = opts_args or []
     command = ["tc", "qdisc", action, "dev", interface]
     if parent is None:
         command.append("root")
     else:
         command += ["parent", parent]
     if handle is not None:
         command += ["handle", str(handle)]
     if algorithm is not None:
         command.append(algorithm)
     for i, j in sorted(kwargs.items()):
         if j is not None:
             command += [str(i), str(j)]
+    command.extend(sorted(opts_args))
 
     launch_command(command, stderr, dryrun)
 
 
 @multiple_interfaces
-def qdisc_add(interface, handle, algorithm, parent=None, *args, **kwargs):
+def qdisc_add(interface, handle, algorithm, parent=None, opts_args=None,
+              **kwargs):
     """
     Add qdisc
 
     **kwargs will be used for specific arguments, depending on the algorithm
     used.
 
     :param interface: target interface
     :param algorithm: algorithm used for this leaf (htb, pfifo, sfq, ...)
     :param handle: handle parameter for tc
     :param parent: if is None, the rule will be added as root. (default: None)
+    :param opts_args: list of options without value, to append to the command
     """
-    return qdisc(interface, "add", algorithm, handle, parent, *args, **kwargs)
+    return qdisc(
+        interface, "add", algorithm, handle, parent, opts_args=opts_args,
+        **kwargs
+    )
 
 
 @multiple_interfaces
 def qdisc_del(interface, algorithm=None, handle=None, parent=None, *args,
               **kwargs):
     """
     Delete qdisc
@@ -63,16 +71,18 @@
     used.
 
     :param interface: target interface
     :param algorithm: algorithm used for this leaf (htb, pfifo, sfq, ...)
     :param handle: handle parameter for tc (default: None)
     :param parent: if is None, the rule will be added as root. (default: None)
     """
-    return qdisc(interface, "delete", algorithm, handle, parent, *args,
-                 **kwargs)
+    return qdisc(
+        interface, "delete", algorithm, handle, parent, opts_args=args,
+        **kwargs
+    )
 
 
 @multiple_interfaces
 def qdisc_show(interface=None, show_format=None, dryrun=False):
     """
     Show qdiscs
 
@@ -100,16 +110,15 @@
 def qos_class(interface, action, parent, classid=None, algorithm="htb",
               dryrun=False, *args, **kwargs):
     """
     Add/change/replace/replace class
 
     **kwargs will be used for specific arguments, depending on the algorithm
     used.
-    Parameters need to be in kbit. If the unit isn't indicated, add it
-    automagically
+    Parameters need to be in kbit or kbytes.
 
     :param action: "add", "replace", "change" or "delete"
     :param interface: target interface
     :param parent: parent class/qdisc
     :param classid: id for the current class (default: None)
     :param algorithm: algorithm used for this class (default: htb)
     """
@@ -117,21 +126,21 @@
     if classid is not None:
         command += ["classid", classid]
     command.append(algorithm)
     if algorithm == "htb":
         for key in ("rate", "ceil"):
             if key in kwargs.keys():
                 try:
-                    kwargs[key] = str(int(kwargs[key])) + "kbit"
+                    kwargs[key] = int(kwargs[key]) * 1024
                 except:
                     pass
         for key in ("burst", "cburst"):
             if key in kwargs.keys():
                 try:
-                    kwargs[key] = str(int(kwargs[key])) + "k"
+                    kwargs[key] = int(kwargs[key]) * 1024
                 except:
                     pass
     for i, j in sorted(kwargs.items()):
         if j is not None:
             command += [str(i), str(j)]
     launch_command(command, dryrun=dryrun)
```

### Comparing `pyqos-0.2.2/pyqos/app.py` & `pyqos-0.3.0/pyqos/app.py`

 * *Files identical despite different names*

### Comparing `pyqos-0.2.2/pyqos/config.py` & `pyqos-0.3.0/pyqos/config.py`

 * *Files identical despite different names*

### Comparing `pyqos-0.2.2/pyqos/decorators.py` & `pyqos-0.3.0/pyqos/decorators.py`

 * *Files identical despite different names*

### Comparing `pyqos-0.2.2/pyqos/tools.py` & `pyqos-0.3.0/pyqos/tools.py`

 * *Files identical despite different names*

### Comparing `pyqos-0.2.2/pyqos.egg-info/PKG-INFO` & `pyqos-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyqos
-Version: 0.2.2
+Version: 0.3.0
 Summary: Framework that helps setting a QoS on Linux
 Home-page: https://github.com/Anthony25/pyqos
 Author: Anthony25 <Anthony Ruhier>
 Author-email: anthony.ruhier@gmail.com
 License: Simplified BSD
-Description: QoS framework for Python and Linux
-        ==================================
-        
-        When setting a QoS with TC with a shell script, the syntax is not easy to read.
-        This framework helps you to set all your rules easily, in a hierarchical way.
-        
-        Documentation: https://pyqos.readthedocs.org/en/dev/
-        
-        Dependencies
-        ------------
-          * python 3.4 (it certainly works with prior versions, just not tested)
-        
-        
-        Example
-        -------
-        
-        There is an example about how using the framework in the `example` folder.
-        
-        
-        Contributors
-        ------------
-        
-         * [Anthony Ruhier](https://github.com/Anthony25)
-         * [Thomas Gagneret](https://github.com/tgagneret)
-        
-        
-        Special thanks
-        --------------
-         * [Flask Project:](https://github.com/mitsuhiko/flask) Some parts about the
-            application and configuration were inspired a lot from it.
-        
-        
-        Readings about tc
-        -----------------
-        
-         * http://wiki.linuxwall.info/doku.php/en:ressources:dossiers:networking:traffic_control
-           : General explanations about QoS and tc
-         * http://luxik.cdi.cz/~devik/qos/htb/manual/userg.htm : Details about htb
-         * http://joekane.eu/cisco-rate-limit-burst-explained/ : Details about burst
-           and cburst and how to define it.
-        
-        
-        License
-        -------
-        
-        Tool under the BSD license. Do not hesitate to report bugs, ask me some
-        questions or do some pull request if you want to !
-        
 Keywords: networking qos linux development
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: BSD License
+License-File: LICENSE.mkd
+
+QoS framework for Python and Linux
+==================================
+
+When setting a QoS with TC with a shell script, the syntax is not easy to read.
+This framework helps you to set all your rules easily, in a hierarchical way.
+
+Documentation: https://pyqos.readthedocs.org/en/dev/
+
+Dependencies
+------------
+  * python 3.4 (it certainly works with prior versions, just not tested)
+
+
+Example
+-------
+
+There is an example about how using the framework in the `example` folder.
+
+
+Contributors
+------------
+
+ * [Anthony Ruhier](https://github.com/Anthony25)
+ * [Thomas Gagneret](https://github.com/tgagneret)
+
+
+Special thanks
+--------------
+ * [Flask Project:](https://github.com/mitsuhiko/flask) Some parts about the
+    application and configuration were inspired a lot from it.
+
+
+Readings about tc
+-----------------
+
+ * http://wiki.linuxwall.info/doku.php/en:ressources:dossiers:networking:traffic_control
+   : General explanations about QoS and tc
+ * http://luxik.cdi.cz/~devik/qos/htb/manual/userg.htm : Details about htb
+ * http://joekane.eu/cisco-rate-limit-burst-explained/ : Details about burst
+   and cburst and how to define it.
+
+
+License
+-------
+
+Tool under the BSD license. Do not hesitate to report bugs, ask me some
+questions or do some pull request if you want to !
```

### Comparing `pyqos-0.2.2/LICENSE.mkd` & `pyqos-0.3.0/LICENSE.mkd`

 * *Files identical despite different names*

### Comparing `pyqos-0.2.2/README.mkd` & `pyqos-0.3.0/README.mkd`

 * *Files identical despite different names*

### Comparing `pyqos-0.2.2/setup.py` & `pyqos-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from os import path
 from setuptools import setup
 
 here = path.abspath(path.dirname(__file__))
 
 setup(
     name="pyqos",
-    version="0.2.2",
+    version="0.3.0",
 
     description="Framework that helps setting a QoS on Linux",
     long_description=open(
         path.join(path.dirname(__file__), "README.mkd")
     ).read(),
 
     url="https://github.com/Anthony25/pyqos",
```

### Comparing `pyqos-0.2.2/PKG-INFO` & `pyqos-0.3.0/pyqos.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyqos
-Version: 0.2.2
+Version: 0.3.0
 Summary: Framework that helps setting a QoS on Linux
 Home-page: https://github.com/Anthony25/pyqos
 Author: Anthony25 <Anthony Ruhier>
 Author-email: anthony.ruhier@gmail.com
 License: Simplified BSD
-Description: QoS framework for Python and Linux
-        ==================================
-        
-        When setting a QoS with TC with a shell script, the syntax is not easy to read.
-        This framework helps you to set all your rules easily, in a hierarchical way.
-        
-        Documentation: https://pyqos.readthedocs.org/en/dev/
-        
-        Dependencies
-        ------------
-          * python 3.4 (it certainly works with prior versions, just not tested)
-        
-        
-        Example
-        -------
-        
-        There is an example about how using the framework in the `example` folder.
-        
-        
-        Contributors
-        ------------
-        
-         * [Anthony Ruhier](https://github.com/Anthony25)
-         * [Thomas Gagneret](https://github.com/tgagneret)
-        
-        
-        Special thanks
-        --------------
-         * [Flask Project:](https://github.com/mitsuhiko/flask) Some parts about the
-            application and configuration were inspired a lot from it.
-        
-        
-        Readings about tc
-        -----------------
-        
-         * http://wiki.linuxwall.info/doku.php/en:ressources:dossiers:networking:traffic_control
-           : General explanations about QoS and tc
-         * http://luxik.cdi.cz/~devik/qos/htb/manual/userg.htm : Details about htb
-         * http://joekane.eu/cisco-rate-limit-burst-explained/ : Details about burst
-           and cburst and how to define it.
-        
-        
-        License
-        -------
-        
-        Tool under the BSD license. Do not hesitate to report bugs, ask me some
-        questions or do some pull request if you want to !
-        
 Keywords: networking qos linux development
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: BSD License
+License-File: LICENSE.mkd
+
+QoS framework for Python and Linux
+==================================
+
+When setting a QoS with TC with a shell script, the syntax is not easy to read.
+This framework helps you to set all your rules easily, in a hierarchical way.
+
+Documentation: https://pyqos.readthedocs.org/en/dev/
+
+Dependencies
+------------
+  * python 3.4 (it certainly works with prior versions, just not tested)
+
+
+Example
+-------
+
+There is an example about how using the framework in the `example` folder.
+
+
+Contributors
+------------
+
+ * [Anthony Ruhier](https://github.com/Anthony25)
+ * [Thomas Gagneret](https://github.com/tgagneret)
+
+
+Special thanks
+--------------
+ * [Flask Project:](https://github.com/mitsuhiko/flask) Some parts about the
+    application and configuration were inspired a lot from it.
+
+
+Readings about tc
+-----------------
+
+ * http://wiki.linuxwall.info/doku.php/en:ressources:dossiers:networking:traffic_control
+   : General explanations about QoS and tc
+ * http://luxik.cdi.cz/~devik/qos/htb/manual/userg.htm : Details about htb
+ * http://joekane.eu/cisco-rate-limit-burst-explained/ : Details about burst
+   and cburst and how to define it.
+
+
+License
+-------
+
+Tool under the BSD license. Do not hesitate to report bugs, ask me some
+questions or do some pull request if you want to !
```

