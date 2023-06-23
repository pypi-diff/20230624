# Comparing `tmp/EclipsingBinaries-3.1.3.tar.gz` & `tmp/EclipsingBinaries-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-3.1.3.tar", last modified: Tue Jun 20 20:39:02 2023, max compression
+gzip compressed data, was "EclipsingBinaries-3.1.5.tar", last modified: Fri Jun 23 22:29:10 2023, max compression
```

## Comparing `EclipsingBinaries-3.1.3.tar` & `EclipsingBinaries-3.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:10.716999 EclipsingBinaries-3.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:10.716999 EclipsingBinaries-3.1.5/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-06-23 22:28:49.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-23 22:28:49.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20774 2023-06-23 22:28:49.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-23 22:28:49.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 22:28:49.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-06-23 22:28:49.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-23 22:28:49.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:10.716999 EclipsingBinaries-3.1.5/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:10.716999 EclipsingBinaries-3.1.5/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:10.716999 EclipsingBinaries-3.1.5/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-23 22:29:10.000000 EclipsingBinaries-3.1.5/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-23 22:29:10.000000 EclipsingBinaries-3.1.5/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:29:10.000000 EclipsingBinaries-3.1.5/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-23 22:29:10.000000 EclipsingBinaries-3.1.5/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-23 22:29:10.000000 EclipsingBinaries-3.1.5/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 22:29:10.000000 EclipsingBinaries-3.1.5/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-23 22:29:10.716999 EclipsingBinaries-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:29:10.720999 EclipsingBinaries-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-23 22:28:55.000000 EclipsingBinaries-3.1.5/setup.py
```

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/OC_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 Author: Kyle Koeller
 Created: 12/19/2022
-Last Edited: 06/13/2023
+Last Edited: 06/23/2023
 
 This calculates O-C values and produces an O-C plot.
 """
 
-from math import sqrt, floor
+from math import sqrt, floor, ceil
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.polynomial import Polynomial
 import statsmodels.formula.api as smf
 import seaborn as sns
 from numba import jit
 import time
 
 
 def main(period=None, loop=0, num=None, nights=None):
     if loop == 0:
         print("\n\nThe format of these input files should be the of the raw form given from Dr. Robert Berrginton's"
-              " 'find_minimum' C program.")
+              " 'find_minimum' C program. Please check the GitHub for an example of this.")
         print("Run TESS data by itself through the TESS option and filtered SARA/BSUO data through the BSU option.\n"
               "DO NOT combine them in any way unless you have already run them through to get the (O-C) values and"
               "are about to run the 'All Data' option.")
         print("Enter the corresponding number to what you would like to do.\n")
         try:
             num = int(input("Would you like to use BSUO data(1), TESS data(2), All Data(3), or Close Program(4): "))
         except ValueError:
@@ -191,14 +191,15 @@
 def all_data(nights, period, loop):
     """
     Merges all the data into a singular file for ease of use
 
     :param nights: number of files there are for the first time through
     :param period: period of the system
     :param loop: number of loops through the program either o or 1
+
     :return: None
     """
     count = 0
 
     minimum_list = []
     e_list = []
     o_c_list = []
@@ -249,16 +250,16 @@
     table_header += '$BJD_{\\rm TDB}$ & E & O-C \\\ \n'
     table_header += '\\hline\n' + '\\endhead\n' + '\\hline\n'
     table_header += '\\multicolumn{3}{c}{\\textit{Continued on next page}} \\\ \n'
     table_header += '\\endfoot\n' + '\\endlastfoot\n'
 
     minimum_lines = []
     for i in range(len(minimum)):
-        line = str("%.5f" % minimum[i]) + ' & ' + str(e[i]) + ' & $' + str("%.5f" % o_c[i]) + ' \pm ' + \
-               str("%.5f" % o_c_err[i]) + '$ ' + "\\\ \n"
+        line = str("%.5f" % minimum[i]) + ' & ' + str(e[i]) + ' & $' + str("%.5f" % o_c[i]) + ' \pm ' + str(
+            "%.5f" % o_c_err[i]) + '$ ' + "\\\ \n"
         minimum_lines.append(line)
 
     output = table_header
     for count, line in enumerate(minimum_lines):
         output += line
 
     output += '\\hline\n' + '\\caption{NSVS 896797 O-C. The first column is the \n' \
@@ -313,15 +314,18 @@
     """
     if T0 == 0:
         T0 = m
         T0_err = err
     # get the exact E value
     E_act = (m - T0) / p
     # estimate for the primary or secondary eclipse by rounding to the nearest 0.5
-    e = floor(E_act * 2) / 2
+    if E_act > 0:
+        e = ceil(E_act * 2) / 2
+    else:
+        e = floor(E_act * 2) / 2
     # calculate the calculated ToM and find the O-C value
     T_calc = T0 + (e * p)
     OC = "%.5f" % (m - T_calc)
 
     # determine the error of the O-C
     OC_err = "%.5f" % sqrt(T0_err ** 2 + err ** 2)
 
@@ -510,20 +514,14 @@
 
     # allows for easy change of the format of the subplots
     rows = 2
     cols = 1
     # creates the figure subplot for appending next
     fig, (ax1, ax2) = plt.subplots(rows, cols)
     # adds gridlines to both subplots
-    """
-    a[0].grid(visible=True, which='major', color='black', linewidth=1.0)
-    a[0].grid(visible=True, which='minor', color='black', linewidth=0.5)
-    a[1].grid(visible=True, which='major', color='black', linewidth=1.0)
-    a[1].grid(visible=True, which='minor', color='black', linewidth=0.5)
-    """
     ax1.grid()
     ax2.grid()
     # creates the model line fit
     sns.lineplot(x=x_label, y=y_label, data=model_dat, ax=ax1, color="red")
     # plots the original data to the same subplot as the model fit
     # edge color is removed to any sort of weird visual overlay on the plots as the normal edge color is white
     sns.scatterplot(x=x_label, y=y_label, data=raw_dat, ax=ax1, color="black", edgecolor="none")
```

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/apass.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-3.1.5/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-3.1.5/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-3.1.5/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-3.1.5/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/find_min.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/gaia.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/menu.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/multi_aperture_photometry.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Analyze images using aperture photometry within Python and not with Astro ImageJ (AIJ)
 
 Author: Kyle Koeller
 Created: 05/07/2023
-Last Updated: 06/20/2023
+Last Updated: 06/23/2023
 """
 
 # Python imports
 import numpy as np
 import pandas as pd
 from pathlib import Path
 import matplotlib.pyplot as plt
@@ -44,18 +44,18 @@
     pipeline : bool
         If True, then the program is being run from the pipeline and will not ask for user input.
     Returns
     -------
     N/A
     """
     if not pipeline:
-        path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the reduced images are or type "
-                     "the word 'Close' to leave: ")
+        # path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the reduced images are or type "
+        #              "the word 'Close' to leave: ")
 
-        # path = "D:\\BSUO data\\2022.09.29-reduced"  # For testing purposes
+        path = "D:\\BSUO data\\2022.09.29-reduced"  # For testing purposes
 
         if path.lower() == "close":
             exit()
     else:
         pass
 
     science_imagetyp = 'LIGHT'
@@ -228,63 +228,98 @@
 
         # ccd = CCDData(image_data, wcs=wcs, unit='adu')
 
         # Convert RA and DEC to pixel positions
         sky_coords = SkyCoord(ra, dec, unit=(u.h, u.deg), frame='icrs')
         pixel_coords = wcs_.world_to_pixel(sky_coords)
 
-        target_position = list(pixel_coords[0])
-        comparison_positions = list(pixel_coords[1:])
+        x_coords, y_coords = pixel_coords
+
+        # target_position = np.array(pixel_coords[0])
+        # comparison_positions = np.array(pixel_coords[1:])
+        target_position = (x_coords[0], y_coords[0])
+        comparison_positions = list(zip(x_coords[1:], y_coords[1:]))
 
         hjd.append(header['HJD-OBS'])
         bjd.append(header['BJD-OBS'])
 
         # Create the apertures and annuli
         target_aperture = CircularAperture(target_position, r=aperture_radius)
         target_annulus = CircularAnnulus(target_position, *annulus_radii)
 
-        comparison_aperture = CircularAperture(comparison_positions, r=aperture_radius)
-        comparison_annulus = CircularAnnulus(comparison_positions, *annulus_radii)
-
+        comparison_aperture = [CircularAperture(pos1, r=aperture_radius) for pos1 in comparison_positions]
+        comparison_annulus = [CircularAnnulus(pos2, *annulus_radii) for pos2 in comparison_positions]
         target_phot_table = aperture_photometry(image_data, target_aperture)
-        comparison_phot_table = aperture_photometry(image_data, comparison_aperture)
+        # comparison_phot_table = aperture_photometry(image_data, comparison_aperture)
+
+        im_plot(image_data, target_aperture, comparison_aperture, target_annulus, comparison_annulus)
+
+        comparison_phot_table = []
+
+        for comp_aperture, comp_annulus in zip(comparison_aperture, comparison_annulus):
+            # Perform aperture photometry on the star
+            aperture_phot_table = aperture_photometry(image_data, comp_aperture)
+
+            # Perform aperture photometry on the annulus (background)
+            annulus_phot_table = aperture_photometry(image_data, comp_annulus)
+
+            # Store the result in the comparison_phot_table list
+            comparison_phot_table.append((aperture_phot_table, annulus_phot_table))
 
         # Perform annulus photometry to estimate the background
         target_bkg_mean = ApertureStats(image_data, target_annulus).mean
-        comparison_bkg_mean = ApertureStats(image_data, comparison_annulus).mean
+        # comparison_bkg_mean = ApertureStats(image_data, comparison_annulus).mean
 
-        # Calculate the total background
-        if np.isnan(target_bkg_mean) or np.isinf(target_bkg_mean) \
-                or np.isnan(comparison_bkg_mean) or np.isinf(comparison_bkg_mean):
+        # Calculate the total background for the comparison stars
+        comparison_bkg_mean = []
+        for annulus in comparison_annulus:
+            stats = ApertureStats(image_data, annulus)
+            if np.isnan(stats.mean) or np.isinf(stats.mean):
+                comparison_bkg_mean.append(0)
+            else:
+                comparison_bkg_mean.append(stats.mean)
+
+        # Calculate the total background for the target star
+        if np.isnan(target_bkg_mean) or np.isinf(target_bkg_mean):
             target_bkg_mean = 0
-            comparison_bkg_mean = 0
 
         target_bkg = ApertureStats(image_data, target_aperture, local_bkg=target_bkg_mean).sum
-        comparison_bkg = ApertureStats(image_data, comparison_aperture, local_bkg=comparison_bkg_mean).sum
+        # comparison_bkg = ApertureStats(image_data, comparison_aperture, local_bkg=comparison_bkg_mean).sum
+
+        comparison_bkg = []
+        for aperture, bkg_mean in zip(comparison_aperture, comparison_bkg_mean):
+            stats = ApertureStats(image_data, aperture, local_bkg=bkg_mean)
+            comparison_bkg.append(stats.sum)
 
         # Calculate the background subtracted counts
         target_flx = target_phot_table['aperture_sum'] - target_bkg
         target_flux_err = np.sqrt(target_phot_table['aperture_sum'] + target_aperture.area * read_noise**2)
-        comparison_flx = comparison_phot_table['aperture_sum'] - comparison_bkg
-        comp_flux_err = np.sqrt(comparison_phot_table['aperture_sum'] + comparison_aperture.area * read_noise ** 2)
+        # comparison_flx = comparison_phot_table['aperture_sum'] - comparison_bkg
+        # comp_flux_err = np.sqrt(comparison_phot_table['aperture_sum'] + comparison_aperture.area * read_noise ** 2)
+        comparison_flx = [phot_table[0]['aperture_sum'] - bkg
+                          for phot_table, bkg in zip(comparison_phot_table, comparison_bkg)]
+
+        comp_flux_err = [np.sqrt(phot_table[0]['aperture_sum'] + aperture.area * read_noise ** 2)
+                         for phot_table, aperture in zip(comparison_phot_table, comparison_aperture)]
 
         # calculate the relative flux for each comparison star and the target star
         rel_flx_T1 = target_flx / sum(comparison_flx)
         count = 0
         for i in comparison_flx:
             if i == comparison_flx[count]:
                 rel_flux_comp = i / (sum(comparison_flx) - i)
             count += 1
 
         # find the number of pixels used to estimate the sky background
-        n_b_mask_comp = comparison_annulus.to_mask(method="center")
-        n_b_comp = np.sum(n_b_mask_comp)
+        n_b = (np.pi * annulus_radii[1]**2) - (np.pi * annulus_radii[0] ** 2)
+        # n_b_mask_comp = comparison_annulus.to_mask(method="center")
+        # n_b_comp = np.sum(n_b_mask_comp)
 
-        n_b_mask_tar = target_annulus.to_mask(method="center")
-        n_b_tar = np.sum(n_b_mask_tar.data)
+        # n_b_mask_tar = target_annulus.to_mask(method="center")
+        # n_b_tar = np.sum(n_b_mask_tar.data)
 
         """
         # find the number of pixels used in the aperture if the radius of the apertures is in arcseconds not pixels
         focal_length = 4114  # mm
         pixel_size = 9  # microns
         pixel_size = pixel_size * 10 ** -3  # mm
         ap_area = np.pi * aperture_radius.area**2  # area of the aperture in mm^2
@@ -295,34 +330,37 @@
 
         n_pix = np.pi * aperture_radius**2  # number of pixels in the aperture
 
         # Calculate the total noise
         sigma_f = 0.289  # quoted from Collins 2017 https://iopscience.iop.org/article/10.3847/1538-3881/153/2/77/pdf
         F_s = 0.01  # number of sky background counts per pixel in ADU
 
-        N_comp = np.sqrt(gain * comparison_flx + n_pix * (1 + (n_pix_comp / n_b_comp)) *
-                         (gain * F_s + F_dark + read_noise ** 2 + gain ** 2 + sigma_f ** 2)) / gain
-        N_tar = np.sqrt(gain * target_flx + n_pix * (1 + (n_pix_tar / n_b_tar)) *
+        # N_comp = np.sqrt(gain * comparison_flx + n_pix * (1 + (n_pix / n_b)) *
+        #                  (gain * F_s + F_dark + read_noise ** 2 + gain ** 2 + sigma_f ** 2)) / gain
+        N_comp = [np.sqrt(gain * flx + n_pix * (1 + (n_pix / n_b)) *
+                          (gain * F_s + F_dark + read_noise ** 2 + gain ** 2 + sigma_f ** 2)) / gain
+                  for flx in comparison_flx]
+        N_tar = np.sqrt(gain * target_flx + n_pix * (1 + (n_pix / n_b)) *
                         (gain * F_s + F_dark + read_noise ** 2 + gain ** 2 + sigma_f ** 2)) / gain
 
         # calculate the total comparison ensemble noise
-        N_e_comp = np.sqrt(np.sum(N_comp ** 2))
+        N_e_comp = np.sqrt(np.sum(np.array(N_comp) ** 2))
 
         rel_flux_err = (rel_flx_T1/rel_flux_comp)*np.sqrt((N_tar**2/target_flx**2) +
                                                           (N_e_comp**2/sum(comparison_flx)**2))
 
         # calculate the total target magnitude and error
         target_magnitude = -np.log(sum(2.512**(magnitudes_comp)))/np.log(2.512) - \
                            (2.5*np.log10(target_bkg/sum(comparison_bkg)))
         target_magnitude_error = 2.5*np.log10(1 + np.sqrt(target_flux_err**2/target_bkg**2) +
                                               (sum(comp_flux_err)**2/sum(comparison_bkg)**2))
 
         # Append the calculated magnitude and error to the lists
-        magnitudes.append(target_magnitude[0])
-        mag_err.append(target_magnitude_error[0])
+        magnitudes.append(target_magnitude)
+        mag_err.append(target_magnitude_error)
 
         # Clear the axis
         ax.clear()
 
         # Plot the magnitudes with error bars
         # ax.errorbar(hjd, magnitudes, yerr=mag_err, fmt='o')
         ax.scatter(hjd, magnitudes, marker='o', color='black')
@@ -336,11 +374,33 @@
 
         # Pause for a bit to allow the figure to update
         time.sleep(0.1)
         plt.pause(0.0001)
 
     # Disable interactive mode
     plt.ioff()
+    plt.show()
+
+
+def im_plot(image_data, target_aperture, comparison_apertures, target_annulus, comparison_annuli):
+    # First, plot the image
+    plt.figure(figsize=(10, 10))
+    plt.imshow(image_data, cmap='gray', origin='lower', vmin=np.percentile(image_data, 5),
+               vmax=np.percentile(image_data, 95))
+    plt.colorbar(label='Counts')
+
+    # Now plot the apertures
+    target_aperture.plot(color='blue', lw=1.5, alpha=0.5)
+    for comparison_aperture in comparison_apertures:
+        comparison_aperture.plot(color='red', lw=1.5, alpha=0.5)
+
+    # Now plot the annuli
+    target_annulus.plot(color='blue', lw=1.5, alpha=0.5, linestyle='dashed')
+    for comparison_annulus in comparison_annuli:
+        comparison_annulus.plot(color='red', lw=1.5, alpha=0.5, linestyle='dashed')
+
+    plt.pause(1000)
+    plt.show()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/pipeline.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/pipeline.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-3.1.5/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-3.1.5/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.1.3
+Version: 3.1.5
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-3.1.5/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/LICENSE` & `EclipsingBinaries-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/PKG-INFO` & `EclipsingBinaries-3.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.1.3
+Version: 3.1.5
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-3.1.3/README.md` & `EclipsingBinaries-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.3/setup.py` & `EclipsingBinaries-3.1.5/setup.py`

 * *Files identical despite different names*

