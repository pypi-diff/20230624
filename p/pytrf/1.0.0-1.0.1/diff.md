# Comparing `tmp/pytrf-1.0.0.tar.gz` & `tmp/pytrf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrf-1.0.0.tar", last modified: Mon Jun  5 12:53:22 2023, max compression
+gzip compressed data, was "pytrf-1.0.1.tar", last modified: Sat Jun 24 14:32:27 2023, max compression
```

## Comparing `pytrf-1.0.0.tar` & `pytrf-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:53:22.818163 pytrf-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-05 12:53:20.000000 pytrf-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 12:53:20.000000 pytrf-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-05 12:53:22.818163 pytrf-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-05 12:53:20.000000 pytrf-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:53:22.818163 pytrf-1.0.0/pytrf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-05 12:53:22.000000 pytrf-1.0.0/pytrf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-05 12:53:22.000000 pytrf-1.0.0/pytrf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:53:22.000000 pytrf-1.0.0/pytrf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 12:53:22.000000 pytrf-1.0.0/pytrf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 12:53:22.000000 pytrf-1.0.0/pytrf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-06-05 12:53:20.000000 pytrf-1.0.0/pytrfcli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:53:22.818163 pytrf-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-05 12:53:20.000000 pytrf-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:53:22.818163 pytrf-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/atr.c
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/atr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/etr.c
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/etr.h
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/gtr.c
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/gtr.h
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/itr.c
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/itr.h
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/pytrf.c
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/str.c
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/str.h
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/util.h
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 12:53:20.000000 pytrf-1.0.0/src/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:53:22.818163 pytrf-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 12:53:20.000000 pytrf-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-05 12:53:20.000000 pytrf-1.0.0/tests/test_stripy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:32:27.528494 pytrf-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-24 14:32:24.000000 pytrf-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-24 14:32:24.000000 pytrf-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-24 14:32:27.524494 pytrf-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-24 14:32:24.000000 pytrf-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:32:27.524494 pytrf-1.0.1/pytrf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-24 14:32:27.000000 pytrf-1.0.1/pytrf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-24 14:32:27.000000 pytrf-1.0.1/pytrf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:32:27.000000 pytrf-1.0.1/pytrf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-24 14:32:27.000000 pytrf-1.0.1/pytrf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-24 14:32:27.000000 pytrf-1.0.1/pytrf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-06-24 14:32:24.000000 pytrf-1.0.1/pytrfcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:32:27.528494 pytrf-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-24 14:32:24.000000 pytrf-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:32:27.524494 pytrf-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/atr.c
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/atr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/etr.c
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/etr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/gtr.c
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/gtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/itr.c
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/itr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/pytrf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/str.c
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/str.h
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/util.h
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-24 14:32:24.000000 pytrf-1.0.1/src/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:32:27.524494 pytrf-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 14:32:24.000000 pytrf-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-24 14:32:24.000000 pytrf-1.0.1/tests/test_stripy.py
```

### Comparing `pytrf-1.0.0/LICENSE` & `pytrf-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/PKG-INFO` & `pytrf-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrf
-Version: 1.0.0
+Version: 1.0.1
 Summary: pytrf is a python package for finding tandem repeats from genomic sequences
 Home-page: https://github.com/lmdu/pytrf
 Author: Lianming Du
 Author-email: adullb@qq.com
 License: MIT
 Keywords: bioinformatics microsatellite tandem repeats
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytrf-1.0.0/README.rst` & `pytrf-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/pytrf.egg-info/PKG-INFO` & `pytrf-1.0.1/pytrf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrf
-Version: 1.0.0
+Version: 1.0.1
 Summary: pytrf is a python package for finding tandem repeats from genomic sequences
 Home-page: https://github.com/lmdu/pytrf
 Author: Lianming Du
 Author-email: adullb@qq.com
 License: MIT
 Keywords: bioinformatics microsatellite tandem repeats
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytrf-1.0.0/pytrfcli.py` & `pytrf-1.0.1/pytrfcli.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 			left, right = fa.flank(chrom, start, end, args.flank_length, True)
 			seq = fa.fetch(chrom, (start, end))
 
 			row.append(seq)
 			row.append(left)
 			row.append(right)
 			writer.writerow(row)
-	
-if __name__ == '__main__':
+
+def main():
 	parser = argparse.ArgumentParser(
 		prog = 'pytrf',
 		usage = 'pytrf command [options] fastx',
 		description = "a python package for finding tandem repeats from genomic sequences"
 	)
 
 	parser.add_argument('-v', '--version',
```

### Comparing `pytrf-1.0.0/setup.py` & `pytrf-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/atr.c` & `pytrf-1.0.1/src/atr.c`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/atr.h` & `pytrf-1.0.1/src/atr.h`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/etr.c` & `pytrf-1.0.1/src/etr.c`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/etr.h` & `pytrf-1.0.1/src/etr.h`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/gtr.c` & `pytrf-1.0.1/src/gtr.c`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/gtr.h` & `pytrf-1.0.1/src/gtr.h`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/itr.c` & `pytrf-1.0.1/src/itr.c`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/itr.h` & `pytrf-1.0.1/src/itr.h`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/pytrf.c` & `pytrf-1.0.1/src/pytrf.c`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/str.c` & `pytrf-1.0.1/src/str.c`

 * *Files identical despite different names*

### Comparing `pytrf-1.0.0/src/str.h` & `pytrf-1.0.1/src/str.h`

 * *Files identical despite different names*

