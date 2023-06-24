# Comparing `tmp/presslink-0.0.1.tar.gz` & `tmp/presslink-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "presslink-0.0.1.tar", last modified: Sun Apr 16 13:10:40 2023, max compression
+gzip compressed data, was "presslink-0.0.2.tar", last modified: Sat Jun 24 02:13:11 2023, max compression
```

## Comparing `presslink-0.0.1.tar` & `presslink-0.0.2.tar`

### file list

```diff
@@ -1,46 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 13:10:40.061516 presslink-0.0.1/
--rw-rw-rw-   0        0        0      623 2023-04-16 13:10:40.061516 presslink-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-16 12:43:08.000000 presslink-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 13:10:40.030266 presslink-0.0.1/presslink/
--rw-rw-rw-   0        0        0        0 2022-08-06 09:05:24.000000 presslink-0.0.1/presslink/__init__.py
--rw-rw-rw-   0        0        0      683 2023-04-16 05:42:25.000000 presslink-0.0.1/presslink/diff_list.py
--rw-rw-rw-   0        0        0     1612 2023-04-12 21:55:56.000000 presslink-0.0.1/presslink/diff_peak_remover.py
--rw-rw-rw-   0        0        0     1759 2023-04-16 06:45:22.000000 presslink-0.0.1/presslink/drag_link_bc_interference_check.py
--rw-rw-rw-   0        0        0    12896 2023-04-16 06:56:23.000000 presslink-0.0.1/presslink/drag_link_excel_writer.py
--rw-rw-rw-   0        0        0     5755 2023-04-14 17:15:26.000000 presslink-0.0.1/presslink/drag_link_graph_plot.py
--rw-rw-rw-   0        0        0    12999 2023-04-16 06:22:43.000000 presslink-0.0.1/presslink/drag_link_modular.py
--rw-rw-rw-   0        0        0     1902 2023-04-14 18:49:44.000000 presslink-0.0.1/presslink/drag_link_rocker_force.py
--rw-rw-rw-   0        0        0    16096 2023-04-16 02:28:03.000000 presslink-0.0.1/presslink/drag_link_sizer.py
--rw-rw-rw-   0        0        0     9555 2023-04-16 06:56:29.000000 presslink-0.0.1/presslink/drag_link_user_calculation.py
--rw-rw-rw-   0        0        0      821 2023-04-14 20:17:40.000000 presslink-0.0.1/presslink/kj_conrod_force.py
--rw-rw-rw-   0        0        0    10266 2023-04-14 17:19:50.000000 presslink-0.0.1/presslink/kj_excel_writer.py
--rw-rw-rw-   0        0        0    16905 2023-04-16 06:22:13.000000 presslink-0.0.1/presslink/kj_modular.py
--rw-rw-rw-   0        0        0      865 2023-04-16 06:06:53.000000 presslink-0.0.1/presslink/kj_rkr_th_finder.py
--rw-rw-rw-   0        0        0     5249 2023-04-16 05:37:02.000000 presslink-0.0.1/presslink/kj_sizer.py
--rw-rw-rw-   0        0        0     8139 2023-04-16 06:54:08.000000 presslink-0.0.1/presslink/kj_user_calculation.py
--rw-rw-rw-   0        0        0    12734 2023-04-14 17:21:50.000000 presslink-0.0.1/presslink/ld_excel_writer.py
--rw-rw-rw-   0        0        0     5828 2023-04-14 17:18:40.000000 presslink-0.0.1/presslink/ld_graph_plot.py
--rw-rw-rw-   0        0        0    17438 2023-04-16 06:28:24.000000 presslink-0.0.1/presslink/ld_modular.py
--rw-rw-rw-   0        0        0     3532 2023-04-14 21:29:50.000000 presslink-0.0.1/presslink/ld_rocker_force.py
--rw-rw-rw-   0        0        0     8919 2023-04-16 05:11:07.000000 presslink-0.0.1/presslink/ld_sizer.py
--rw-rw-rw-   0        0        0     8753 2023-04-16 06:54:16.000000 presslink-0.0.1/presslink/ld_user_calculation.py
--rw-rw-rw-   0        0        0     6742 2023-04-16 05:59:04.000000 presslink-0.0.1/presslink/link4_rj4.py
--rw-rw-rw-   0        0        0     3962 2023-04-16 05:59:16.000000 presslink-0.0.1/presslink/link5_rj4_sj1.py
--rw-rw-rw-   0        0        0    12218 2023-04-14 17:22:34.000000 presslink-0.0.1/presslink/ml_excel_writer.py
--rw-rw-rw-   0        0        0     5721 2023-04-14 17:19:08.000000 presslink-0.0.1/presslink/ml_graph_plot.py
--rw-rw-rw-   0        0        0    17047 2023-04-16 06:25:41.000000 presslink-0.0.1/presslink/ml_modular.py
--rw-rw-rw-   0        0        0     5467 2023-04-16 05:28:55.000000 presslink-0.0.1/presslink/ml_sizer.py
--rw-rw-rw-   0        0        0     6997 2023-04-14 22:17:12.000000 presslink-0.0.1/presslink/ml_ternary_link_force.py
--rw-rw-rw-   0        0        0     9095 2023-04-16 06:55:47.000000 presslink-0.0.1/presslink/ml_user_calculation.py
--rw-rw-rw-   0        0        0    16666 2023-04-16 05:58:39.000000 presslink-0.0.1/presslink/pretty_graph_datagen.py
--rw-rw-rw-   0        0        0      484 2023-04-16 05:45:24.000000 presslink-0.0.1/presslink/remove_trailing_zeros.py
--rw-rw-rw-   0        0        0     1983 2023-04-16 05:43:38.000000 presslink-0.0.1/presslink/shaft.py
--rw-rw-rw-   0        0        0      672 2023-04-16 05:41:51.000000 presslink-0.0.1/presslink/vector_difference.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:10:40.061516 presslink-0.0.1/presslink.egg-info/
--rw-rw-rw-   0        0        0      623 2023-04-16 13:10:39.000000 presslink-0.0.1/presslink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1180 2023-04-16 13:10:39.000000 presslink-0.0.1/presslink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 13:10:39.000000 presslink-0.0.1/presslink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-16 13:10:39.000000 presslink-0.0.1/presslink.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 13:10:39.000000 presslink-0.0.1/presslink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 13:10:40.061516 presslink-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      780 2023-04-16 13:10:12.000000 presslink-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:13:11.662171 presslink-0.0.2/
+-rw-rw-rw-   0        0        0      623 2023-06-24 02:13:11.662171 presslink-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-04-16 12:43:08.000000 presslink-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 02:13:11.662171 presslink-0.0.2/presslink.egg-info/
+-rw-rw-rw-   0        0        0      623 2023-06-24 02:13:11.000000 presslink-0.0.2/presslink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-06-24 02:13:11.000000 presslink-0.0.2/presslink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 02:13:11.000000 presslink-0.0.2/presslink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-24 02:13:11.000000 presslink-0.0.2/presslink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 02:13:11.000000 presslink-0.0.2/presslink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 02:13:11.662171 presslink-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-06-24 02:11:19.000000 presslink-0.0.2/setup.py
```

### Comparing `presslink-0.0.1/PKG-INFO` & `presslink-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: presslink
-Version: 0.0.1
+Version: 0.0.2
 Summary: link mechanisms of mechanical press
 Home-page: UNKNOWN
 Author: Sanchit
 Author-email: sanchitsharma84@gmail.com
 License: MIT
 Description: This package contains set of modules for various link mechanisms used in mechanical presses
 Keywords: mechanical press link mechanism
```

### Comparing `presslink-0.0.1/presslink.egg-info/PKG-INFO` & `presslink-0.0.2/presslink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: presslink
-Version: 0.0.1
+Version: 0.0.2
 Summary: link mechanisms of mechanical press
 Home-page: UNKNOWN
 Author: Sanchit
 Author-email: sanchitsharma84@gmail.com
 License: MIT
 Description: This package contains set of modules for various link mechanisms used in mechanical presses
 Keywords: mechanical press link mechanism
```

### Comparing `presslink-0.0.1/setup.py` & `presslink-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
   'Programming Language :: Python :: 3'
 ]
 
 
  
 setup(
   name='presslink',
-  version='0.0.1',
+  version='0.0.2',
   description='link mechanisms of mechanical press',
   long_description="This package contains set of modules for various link mechanisms used in mechanical presses",
   url='',  
   author='Sanchit',
   author_email='sanchitsharma84@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='mechanical press link mechanism', 
   packages=find_packages(),
-  install_requires=["numpy", "xlsxwriter", "matplotlib"],
+  install_requires=["numpy", "xlsxwriter", "matplotlib", "mechpress"],
 )
```

