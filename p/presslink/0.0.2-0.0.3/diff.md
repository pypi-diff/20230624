# Comparing `tmp/presslink-0.0.2.tar.gz` & `tmp/presslink-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "presslink-0.0.2.tar", last modified: Sat Jun 24 02:13:11 2023, max compression
+gzip compressed data, was "presslink-0.0.3.tar", last modified: Sat Jun 24 16:19:33 2023, max compression
```

## Comparing `presslink-0.0.2.tar` & `presslink-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 02:13:11.662171 presslink-0.0.2/
--rw-rw-rw-   0        0        0      623 2023-06-24 02:13:11.662171 presslink-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-16 12:43:08.000000 presslink-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 02:13:11.662171 presslink-0.0.2/presslink.egg-info/
--rw-rw-rw-   0        0        0      623 2023-06-24 02:13:11.000000 presslink-0.0.2/presslink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-06-24 02:13:11.000000 presslink-0.0.2/presslink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 02:13:11.000000 presslink-0.0.2/presslink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-24 02:13:11.000000 presslink-0.0.2/presslink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 02:13:11.000000 presslink-0.0.2/presslink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 02:13:11.662171 presslink-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-06-24 02:11:19.000000 presslink-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:19:33.606075 presslink-0.0.3/
+-rw-rw-rw-   0        0        0      623 2023-06-24 16:19:33.606075 presslink-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-04-16 12:43:08.000000 presslink-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 16:19:33.559201 presslink-0.0.3/presslink/
+-rw-rw-rw-   0        0        0        0 2022-08-06 09:05:24.000000 presslink-0.0.3/presslink/__init__.py
+-rw-rw-rw-   0        0        0      683 2023-04-15 17:12:24.000000 presslink-0.0.3/presslink/diff_list.py
+-rw-rw-rw-   0        0        0     1612 2023-04-12 09:25:56.000000 presslink-0.0.3/presslink/diff_peak_remover.py
+-rw-rw-rw-   0        0        0     1759 2023-04-15 18:15:22.000000 presslink-0.0.3/presslink/drag_link_bc_interference_check.py
+-rw-rw-rw-   0        0        0    13270 2023-06-19 20:36:08.000000 presslink-0.0.3/presslink/drag_link_excel_writer.py
+-rw-rw-rw-   0        0        0     5755 2023-04-14 04:45:26.000000 presslink-0.0.3/presslink/drag_link_graph_plot.py
+-rw-rw-rw-   0        0        0    13039 2023-04-17 16:57:26.000000 presslink-0.0.3/presslink/drag_link_modular.py
+-rw-rw-rw-   0        0        0     1902 2023-04-14 06:19:44.000000 presslink-0.0.3/presslink/drag_link_rocker_force.py
+-rw-rw-rw-   0        0        0    16467 2023-06-19 19:55:18.000000 presslink-0.0.3/presslink/drag_link_sizer.py
+-rw-rw-rw-   0        0        0     9969 2023-06-19 21:13:54.000000 presslink-0.0.3/presslink/drag_link_user_calculation.py
+-rw-rw-rw-   0        0        0      821 2023-04-14 07:47:40.000000 presslink-0.0.3/presslink/kj_conrod_force.py
+-rw-rw-rw-   0        0        0    10266 2023-04-14 04:49:50.000000 presslink-0.0.3/presslink/kj_excel_writer.py
+-rw-rw-rw-   0        0        0    16945 2023-04-17 17:01:32.000000 presslink-0.0.3/presslink/kj_modular.py
+-rw-rw-rw-   0        0        0      865 2023-04-15 17:36:52.000000 presslink-0.0.3/presslink/kj_rkr_th_finder.py
+-rw-rw-rw-   0        0        0     5274 2023-04-17 17:02:02.000000 presslink-0.0.3/presslink/kj_sizer.py
+-rw-rw-rw-   0        0        0     8234 2023-04-17 16:35:12.000000 presslink-0.0.3/presslink/kj_user_calculation.py
+-rw-rw-rw-   0        0        0    12734 2023-04-14 04:51:50.000000 presslink-0.0.3/presslink/ld_excel_writer.py
+-rw-rw-rw-   0        0        0     5828 2023-04-14 04:48:40.000000 presslink-0.0.3/presslink/ld_graph_plot.py
+-rw-rw-rw-   0        0        0    17470 2023-04-17 17:10:38.000000 presslink-0.0.3/presslink/ld_modular.py
+-rw-rw-rw-   0        0        0     3532 2023-04-14 08:59:50.000000 presslink-0.0.3/presslink/ld_rocker_force.py
+-rw-rw-rw-   0        0        0     8934 2023-04-17 17:11:00.000000 presslink-0.0.3/presslink/ld_sizer.py
+-rw-rw-rw-   0        0        0     8823 2023-04-17 16:44:24.000000 presslink-0.0.3/presslink/ld_user_calculation.py
+-rw-rw-rw-   0        0        0     6742 2023-04-15 17:29:04.000000 presslink-0.0.3/presslink/link4_rj4.py
+-rw-rw-rw-   0        0        0     3962 2023-04-15 17:29:16.000000 presslink-0.0.3/presslink/link5_rj4_sj1.py
+-rw-rw-rw-   0        0        0    12213 2023-04-17 17:36:36.000000 presslink-0.0.3/presslink/ml_excel_writer.py
+-rw-rw-rw-   0        0        0     5721 2023-04-14 04:49:08.000000 presslink-0.0.3/presslink/ml_graph_plot.py
+-rw-rw-rw-   0        0        0    17087 2023-04-17 17:27:26.000000 presslink-0.0.3/presslink/ml_modular.py
+-rw-rw-rw-   0        0        0     5492 2023-04-17 17:27:52.000000 presslink-0.0.3/presslink/ml_sizer.py
+-rw-rw-rw-   0        0        0     6997 2023-04-14 09:47:12.000000 presslink-0.0.3/presslink/ml_ternary_link_force.py
+-rw-rw-rw-   0        0        0     9180 2023-04-17 17:01:30.000000 presslink-0.0.3/presslink/ml_user_calculation.py
+-rw-rw-rw-   0        0        0    16681 2023-04-17 16:58:10.000000 presslink-0.0.3/presslink/pretty_graph_datagen.py
+-rw-rw-rw-   0        0        0      484 2023-04-15 17:15:24.000000 presslink-0.0.3/presslink/remove_trailing_zeros.py
+-rw-rw-rw-   0        0        0     1983 2023-04-15 17:13:38.000000 presslink-0.0.3/presslink/shaft.py
+-rw-rw-rw-   0        0        0      672 2023-04-15 17:11:50.000000 presslink-0.0.3/presslink/vector_difference.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:19:33.590451 presslink-0.0.3/presslink.egg-info/
+-rw-rw-rw-   0        0        0      623 2023-06-24 16:19:33.000000 presslink-0.0.3/presslink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1180 2023-06-24 16:19:33.000000 presslink-0.0.3/presslink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 16:19:33.000000 presslink-0.0.3/presslink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-24 16:19:33.000000 presslink-0.0.3/presslink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-24 16:19:33.000000 presslink-0.0.3/presslink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 16:19:33.606075 presslink-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-06-24 16:12:04.000000 presslink-0.0.3/setup.py
```

### Comparing `presslink-0.0.2/PKG-INFO` & `presslink-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: presslink
-Version: 0.0.2
+Version: 0.0.3
 Summary: link mechanisms of mechanical press
 Home-page: UNKNOWN
 Author: Sanchit
 Author-email: sanchitsharma84@gmail.com
 License: MIT
 Description: This package contains set of modules for various link mechanisms used in mechanical presses
 Keywords: mechanical press link mechanism
```

### Comparing `presslink-0.0.2/presslink.egg-info/PKG-INFO` & `presslink-0.0.3/presslink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: presslink
-Version: 0.0.2
+Version: 0.0.3
 Summary: link mechanisms of mechanical press
 Home-page: UNKNOWN
 Author: Sanchit
 Author-email: sanchitsharma84@gmail.com
 License: MIT
 Description: This package contains set of modules for various link mechanisms used in mechanical presses
 Keywords: mechanical press link mechanism
```

### Comparing `presslink-0.0.2/setup.py` & `presslink-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   'Programming Language :: Python :: 3'
 ]
 
 
  
 setup(
   name='presslink',
-  version='0.0.2',
+  version='0.0.3',
   description='link mechanisms of mechanical press',
   long_description="This package contains set of modules for various link mechanisms used in mechanical presses",
   url='',  
   author='Sanchit',
   author_email='sanchitsharma84@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

