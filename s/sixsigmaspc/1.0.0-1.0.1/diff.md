# Comparing `tmp/sixsigmaspc-1.0.0.tar.gz` & `tmp/sixsigmaspc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixsigmaspc-1.0.0.tar", last modified: Sun May 28 13:20:09 2023, max compression
+gzip compressed data, was "sixsigmaspc-1.0.1.tar", last modified: Sat Jun 24 06:36:34 2023, max compression
```

## Comparing `sixsigmaspc-1.0.0.tar` & `sixsigmaspc-1.0.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 velzm     (1000) users      (100)        0 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/
--rw-rw-r--   0 velzm     (1000) users      (100)      958 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/PKG-INFO
--rw-r--r--   0 velzm     (1000) users      (100)      167 2023-05-27 10:29:02.000000 sixsigmaspc-1.0.0/README.md
-drwxrwxr-x   0 velzm     (1000) users      (100)        0 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/SPC/
--rw-r--r--   0 velzm     (1000) users      (100)     6928 2023-05-28 13:08:04.000000 sixsigmaspc-1.0.0/SPC/CControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     4416 2023-05-28 12:07:32.000000 sixsigmaspc-1.0.0/SPC/ControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)      349 2023-05-19 05:20:44.000000 sixsigmaspc-1.0.0/SPC/ControlChartConstants.py
--rw-r--r--   0 velzm     (1000) users      (100)    14337 2023-05-28 11:23:34.000000 sixsigmaspc-1.0.0/SPC/ImRControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     1164 2023-05-27 08:27:38.000000 sixsigmaspc-1.0.0/SPC/MultiVariChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     7748 2023-05-28 13:12:46.000000 sixsigmaspc-1.0.0/SPC/NPControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     7698 2023-05-28 13:07:58.000000 sixsigmaspc-1.0.0/SPC/PControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     2219 2023-05-27 08:25:16.000000 sixsigmaspc-1.0.0/SPC/ProcessCapabilityChart.py
--rw-r--r--   0 velzm     (1000) users      (100)      283 2022-07-09 10:06:18.000000 sixsigmaspc-1.0.0/SPC/Rule.py
--rw-r--r--   0 velzm     (1000) users      (100)      851 2023-05-27 08:11:04.000000 sixsigmaspc-1.0.0/SPC/Rule01.py
--rw-r--r--   0 velzm     (1000) users      (100)     1295 2023-05-27 08:12:22.000000 sixsigmaspc-1.0.0/SPC/Rule02.py
--rw-r--r--   0 velzm     (1000) users      (100)     2410 2023-05-27 08:12:22.000000 sixsigmaspc-1.0.0/SPC/Rule03.py
--rw-r--r--   0 velzm     (1000) users      (100)     1512 2023-05-27 08:12:22.000000 sixsigmaspc-1.0.0/SPC/Rule04.py
--rw-r--r--   0 velzm     (1000) users      (100)     1407 2023-05-27 08:12:22.000000 sixsigmaspc-1.0.0/SPC/Rule05.py
--rw-r--r--   0 velzm     (1000) users      (100)     1365 2023-05-27 08:12:22.000000 sixsigmaspc-1.0.0/SPC/Rule06.py
--rw-r--r--   0 velzm     (1000) users      (100)     3212 2023-05-27 08:12:22.000000 sixsigmaspc-1.0.0/SPC/Rule07.py
--rw-r--r--   0 velzm     (1000) users      (100)     2154 2023-05-27 08:12:22.000000 sixsigmaspc-1.0.0/SPC/Rule08.py
--rw-r--r--   0 velzm     (1000) users      (100)     7467 2023-05-28 13:06:54.000000 sixsigmaspc-1.0.0/SPC/UControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)    14336 2023-05-28 10:52:38.000000 sixsigmaspc-1.0.0/SPC/XbarRControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     1430 2023-05-27 08:12:22.000000 sixsigmaspc-1.0.0/SPC/XbarRControlChartConstants.py
--rw-r--r--   0 velzm     (1000) users      (100)    14374 2023-05-28 10:52:38.000000 sixsigmaspc-1.0.0/SPC/XbarSControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     1441 2023-05-28 06:07:40.000000 sixsigmaspc-1.0.0/SPC/XbarSControlChartConstants.py
--rw-r--r--   0 velzm     (1000) users      (100)    14059 2023-05-28 11:19:48.000000 sixsigmaspc-1.0.0/SPC/XmRControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     1053 2023-05-28 13:12:28.000000 sixsigmaspc-1.0.0/SPC/__init__.py
--rw-rw-r--   0 velzm     (1000) users      (100)       38 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/setup.cfg
--rw-r--r--   0 velzm     (1000) users      (100)     1444 2023-05-28 13:20:04.000000 sixsigmaspc-1.0.0/setup.py
-drwxrwxr-x   0 velzm     (1000) users      (100)        0 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/sixsigmaspc.egg-info/
--rw-r--r--   0 velzm     (1000) users      (100)      958 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/sixsigmaspc.egg-info/PKG-INFO
--rw-r--r--   0 velzm     (1000) users      (100)      965 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/sixsigmaspc.egg-info/SOURCES.txt
--rw-r--r--   0 velzm     (1000) users      (100)        1 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/sixsigmaspc.egg-info/dependency_links.txt
--rw-r--r--   0 velzm     (1000) users      (100)       76 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/sixsigmaspc.egg-info/requires.txt
--rw-r--r--   0 velzm     (1000) users      (100)       10 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/sixsigmaspc.egg-info/top_level.txt
-drwxrwxr-x   0 velzm     (1000) users      (100)        0 2023-05-28 13:20:09.000000 sixsigmaspc-1.0.0/tests/
--rw-r--r--   0 velzm     (1000) users      (100)     2174 2023-05-28 12:35:26.000000 sixsigmaspc-1.0.0/tests/CControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     2892 2023-05-28 11:24:08.000000 sixsigmaspc-1.0.0/tests/ImRControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     1006 2023-05-27 08:27:54.000000 sixsigmaspc-1.0.0/tests/MultiVariChartTest.py
--rw-r--r--   0 velzm     (1000) users      (100)     2056 2023-05-28 13:13:08.000000 sixsigmaspc-1.0.0/tests/NPControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     2075 2023-05-28 12:51:00.000000 sixsigmaspc-1.0.0/tests/PControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     1842 2023-05-27 08:26:26.000000 sixsigmaspc-1.0.0/tests/ProcessCapabilityChartTest.py
--rw-r--r--   0 velzm     (1000) users      (100)     2082 2023-05-28 12:19:32.000000 sixsigmaspc-1.0.0/tests/UControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     3292 2023-05-28 08:16:52.000000 sixsigmaspc-1.0.0/tests/XbarRControlChartTest.py
--rw-r--r--   0 velzm     (1000) users      (100)     2819 2023-05-28 08:04:04.000000 sixsigmaspc-1.0.0/tests/XbarSControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)     2470 2023-05-28 11:20:24.000000 sixsigmaspc-1.0.0/tests/XmRControlChart.py
--rw-r--r--   0 velzm     (1000) users      (100)        0 2023-05-27 09:46:58.000000 sixsigmaspc-1.0.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:36:34.843572 sixsigmaspc-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1001 2023-06-24 06:36:34.841833 sixsigmaspc-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 06:36:34.779471 sixsigmaspc-1.0.1/SPC/
+-rw-rw-rw-   0        0        0     7007 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/SPC/CControlChart.py
+-rw-rw-rw-   0        0        0     4606 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/SPC/ControlChart.py
+-rw-rw-rw-   0        0        0      349 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/ControlChartConstants.py
+-rw-rw-rw-   0        0        0    14848 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/SPC/ImRControlChart.py
+-rw-rw-rw-   0        0        0     2520 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/SPC/MultiVariChart.py
+-rw-rw-rw-   0        0        0     7827 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/SPC/NPControlChart.py
+-rw-rw-rw-   0        0        0     7777 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/SPC/PControlChart.py
+-rw-rw-rw-   0        0        0     2219 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/ProcessCapabilityChart.py
+-rw-rw-rw-   0        0        0      283 2023-06-22 13:01:22.000000 sixsigmaspc-1.0.1/SPC/Rule.py
+-rw-rw-rw-   0        0        0      851 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/Rule01.py
+-rw-rw-rw-   0        0        0     1295 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/Rule02.py
+-rw-rw-rw-   0        0        0     2410 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/Rule03.py
+-rw-rw-rw-   0        0        0     1512 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/Rule04.py
+-rw-rw-rw-   0        0        0     1407 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/Rule05.py
+-rw-rw-rw-   0        0        0     1365 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/Rule06.py
+-rw-rw-rw-   0        0        0     3212 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/Rule07.py
+-rw-rw-rw-   0        0        0     2154 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/Rule08.py
+-rw-rw-rw-   0        0        0     7546 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/SPC/UControlChart.py
+-rw-rw-rw-   0        0        0    14844 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/SPC/XbarRControlChart.py
+-rw-rw-rw-   0        0        0     1430 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/XbarRControlChartConstants.py
+-rw-rw-rw-   0        0        0    14882 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/SPC/XbarSControlChart.py
+-rw-rw-rw-   0        0        0     1441 2023-06-22 11:52:39.000000 sixsigmaspc-1.0.1/SPC/XbarSControlChartConstants.py
+-rw-rw-rw-   0        0        0    14583 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/SPC/XmRControlChart.py
+-rw-rw-rw-   0        0        0     1053 2023-06-23 10:21:56.000000 sixsigmaspc-1.0.1/SPC/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-24 06:36:34.843992 sixsigmaspc-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1444 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:36:34.819950 sixsigmaspc-1.0.1/sixsigmaspc.egg-info/
+-rw-rw-rw-   0        0        0     1001 2023-06-24 06:36:34.000000 sixsigmaspc-1.0.1/sixsigmaspc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-06-24 06:36:34.000000 sixsigmaspc-1.0.1/sixsigmaspc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 06:36:34.000000 sixsigmaspc-1.0.1/sixsigmaspc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-06-24 06:36:34.000000 sixsigmaspc-1.0.1/sixsigmaspc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-24 06:36:34.000000 sixsigmaspc-1.0.1/sixsigmaspc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 06:36:34.835394 sixsigmaspc-1.0.1/tests/
+-rw-rw-rw-   0        0        0     1501 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/tests/CControlChart.py
+-rw-rw-rw-   0        0        0     2278 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/tests/ImRControlChart.py
+-rw-rw-rw-   0        0        0     4102 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/tests/MultiVariChartTest.py
+-rw-rw-rw-   0        0        0     1383 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/tests/NPControlChart.py
+-rw-rw-rw-   0        0        0     1402 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/tests/PControlChart.py
+-rw-rw-rw-   0        0        0     1842 2023-06-22 11:52:40.000000 sixsigmaspc-1.0.1/tests/ProcessCapabilityChartTest.py
+-rw-rw-rw-   0        0        0     1409 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/tests/UControlChart.py
+-rw-rw-rw-   0        0        0     2660 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/tests/XbarRControlChartTest.py
+-rw-rw-rw-   0        0        0     2203 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/tests/XbarSControlChart.py
+-rw-rw-rw-   0        0        0     1768 2023-06-24 06:29:38.000000 sixsigmaspc-1.0.1/tests/XmRControlChart.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 11:52:40.000000 sixsigmaspc-1.0.1/tests/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sixsigmaspc-1.0.0/SPC/CControlChart.py` & `sixsigmaspc-1.0.1/SPC/CControlChart.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,29 @@
 import matplotlib.dates as mdates
 import numpy as np
 import pandas as pd
 from datetime import datetime
 from SPC import ControlChart
 
 class CControlChart(ControlChart):
-    def __init__(self, c:list, n:list):
+    def __init__(self, c:list, n:list, xlabel:str="", ylabel:str=""):
         """ Initialization.
 
             :param c: number of defects in the samples.
             :param n: sample sizes.
+            :param xlabel: x-as label.
+            :param ylabel: y-as label.
         """
         # Initialization of the base class.
         super().__init__(1) # C chart.
 
-        # The number of defects.
+        # Remember the parameters.
         self.number_of_defects = len(c)
+        self._xlabel = xlabel
+        self._ylabel = ylabel
 
         # Remember the number of defects.
         self.c = c
 
         # Remember the sample sizes.
         self.n = n
 
@@ -50,24 +54,25 @@
         self.one_sigma_plus[:] = self.c.mean() + 3 * np.sqrt(self.c.mean()) * 1/3
         self.one_sigma_min[:] = self.c.mean() - 3 * np.sqrt(self.c.mean()) * 1/3
         self.two_sigma_min[:] = self.c.mean() - 3 * np.sqrt(self.c.mean()) * 2/3
 
     def plot(self):
         """ Create the plot.
         """
+        plt.figure(figsize=(15,5))
+
         # The x-axis can be numeric or datetime.
         if (len(super().dates) == 0):
             x_values_C = list(range(0, self.number_of_defects))
         else:
             format=super().dateformat
             x_values_C = [datetime.strptime(d, format).date() for d in super().dates]
             plt.gca().xaxis.set_major_formatter(mdates.DateFormatter(super().dateformat))
 
         # C chart.
-        plt.figure(figsize=(15,5))
         plt.plot(x_values_C, self.c, marker="o",color="k",label="c")
         plt.plot(x_values_C, self.ucl_c,color="r",label="UCL")
 
         # Retrieve the data.
         df = self.data(0)
 
         # Plot the signals.
@@ -85,23 +90,23 @@
         if super().limits:
             plt.plot(x_values_C, self.one_sigma_min, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_C, self.two_sigma_min, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_C, self.lcl_c,color="r",label="LCL")
         plt.title("C Control Chart")
 
-        # Check numerical or datetime for the x-axis.
-        if (len(super().dates) == 0):
-            plt.xticks(np.arange(self.number_of_defects))
-        else:
-            plt.xticks(rotation=45, ha='right')
-        
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the x-label.
+        plt.xlabel( self._xlabel)
+
+        # Set the y-label.
+        plt.ylabel( self._ylabel)
+
         plt.show()
 
     def split(self, stages:list):
         """ Split the chart.
 
             :param stages: The stages.
         """
```

### Comparing `sixsigmaspc-1.0.0/SPC/ControlChart.py` & `sixsigmaspc-1.0.1/SPC/ControlChart.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,22 @@
         """ Append a rule.
 
             :param rule: The rule.
         """
         # Append the rule.
         self._rules.append(rule)
 
+    def append_rules(self, rules : list[Rule]):
+        """ Append the rules.
+
+            :param rules: The rules.
+        """
+        # Set the rules.
+        self._rules = rules
+
     def execute_rules(self, df: pd.DataFrame):
         """ Rules execution.
 
             :param df: The dataframe.
         """
         # Create the signal column.
         df["SIGNAL"] = False
```

### Comparing `sixsigmaspc-1.0.0/SPC/ImRControlChart.py` & `sixsigmaspc-1.0.1/SPC/ImRControlChart.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,24 +23,30 @@
 
 class ImRControlChart(ControlChart):
     _E2 : float # The Control Chart E2 constant.
     _d2 : float # The Control Chart d2 constant.
     _D3 : float # The Control Chart D3 constant.
     _D4 : float # The Control Chart D4 constant.
 
-    def __init__(self, data:list):
+    def __init__(self, data:list, xlabel:str="", ylabel_top:str="", ylabel_bottom:str=""):
         """ Initialization.
 
             :param data: values.
+            :param xlabel: x-as label.
+            :param ylabel_top: top y-as label.
+            :param ylabel_bottom: bottom y-as label.
         """
         # Initialization of the base class.
         super().__init__(2) # X chart and mR chart.
 
-        # Remember the data.
+        # Remember the parameters.
         self._data = data
+        self._xlabel = xlabel
+        self._ylabel_top = ylabel_top
+        self._ylabel_bottom = ylabel_bottom
 
         # Remember the Control chart constants size=2 (comparing the current state with previous state).
         self._E2 = 2.66
         self._d2 = 1.128
         self._D3 = 0
         self._D4 = 3.267
 
@@ -101,15 +107,15 @@
         plt.figure(figsize=(15,10))
 
         # The 1st vertical plot.
         plt.subplot(2,1,1)
 
         # The x-axis can be numeric or datetime.
         if (len(super().dates) == 0):
-            x_values_I = list(range(1, len(self.value_I)+1))
+            x_values_I = list(range(0, len(self.value_I)))
         else:
             format=super().dateformat
             x_values_I = [datetime.strptime(d, format).date() for d in super().dates]
             plt.gca().xaxis.set_major_formatter(mdates.DateFormatter(super().dateformat))
 
         # I chart.
         plt.plot(x_values_I, self.value_I, marker="o", color="k", label="I")
@@ -133,28 +139,30 @@
         if super().limits:
             plt.plot(x_values_I, self.one_sigma_min_I, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_I, self.two_sigma_min_I, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_I, self.lcl_I, color="r", label="LCL")
         plt.title("I Chart")
 
-        # Check numerical or datetime for the x-axis.
-        if (len(super().dates) == 0):
-            plt.xticks(np.arange(len(self.value_I)))
-        else:
-            plt.xticks(rotation=45, ha='right')
-
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the y-label.
+        plt.ylabel( self._ylabel_top)
+
         # The 2nd vertical plot.
         plt.subplot(2,1,2)
 
-        # The x-axis is numeric.
-        x_values_mR = list(range(1, len(self.value_I)))
+        # The x-axis can be numeric or datetime.
+        if (len(super().dates) == 0):
+            x_values_mR = list(range(1, len(self.value_I)))
+        else:
+            format=super().dateformat
+            x_values_mR = [datetime.strptime(d, format).date() for d in super().dates][1:]
+            plt.gca().xaxis.set_major_formatter(mdates.DateFormatter(super().dateformat))
 
         # mR chart.
         plt.plot(x_values_mR, self.value_mR, marker="o", color="k", label="R")
         plt.plot(x_values_mR, self.ucl_mR, color="r", label="UCL")
 
         # Retrieve the data.
         df = self.data(1)
@@ -174,20 +182,23 @@
         if super().limits:
             plt.plot(x_values_mR, self.one_sigma_min_mR, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_mR, self.two_sigma_min_mR, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_mR, self.lcl_mR, color="r", label="LCL")
         plt.title("mR Chart")
 
-        # Set numerical for the x-axis.
-        plt.xticks(np.arange(len(self.value_I)))
-
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the y-label.
+        plt.ylabel(self._ylabel_bottom)
+
+        # Set the x-label.
+        plt.xlabel( self._xlabel)
+
         # Show the plot.
         plt.show()
 
     def split(self, stages:list):
         """ Split the chart.
 
             :param stages: The stages.
```

### Comparing `sixsigmaspc-1.0.0/SPC/NPControlChart.py` & `sixsigmaspc-1.0.1/SPC/NPControlChart.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,29 @@
 import matplotlib.dates as mdates
 import numpy as np
 import pandas as pd
 from datetime import datetime
 from SPC import ControlChart
 
 class NPControlChart(ControlChart):
-    def __init__(self, c:list, n:list):
+    def __init__(self, c:list, n:list, xlabel:str="", ylabel:str=""):
         """ Initialization.
 
             :param c: number of defects in the samples.
             :param n: sample sizes.
+            :param xlabel: x-as label.
+            :param ylabel: y-as label.
         """
         # Initialization of the base class.
         super().__init__(1) # NP chart.
 
-        # The number of defects.
+        # Remember the parameters.
         self.number_of_defects = len(c)
+        self._xlabel = xlabel
+        self._ylabel = ylabel
 
         # Remember the number of defective in the sample.
         self.c = c
 
         # Remember the sample sizes.
         self.n = n
 
@@ -54,24 +58,25 @@
         self.one_sigma_plus[:] = self.value_p.mean() + 3 * np.sqrt(self.value_p.mean() * (1 - self.c.sum() / self.n.sum())) * 1/3
         self.one_sigma_min[:] = max(self.value_p.mean() - 3 * np.sqrt(self.value_p.mean() * (1 - self.c.sum() / self.n.sum())) * 1/3, 0.0)
         self.two_sigma_min[:] = max(self.value_p.mean() - 3 * np.sqrt(self.value_p.mean() * (1 - self.c.sum() / self.n.sum())) * 2/3, 0.0)
 
     def plot(self):
         """ Create the P chart.
         """
+        plt.figure(figsize=(15,5))
+
         # The x-axis can be numeric or datetime.
         if (len(super().dates) == 0):
             x_values_p = list(range(0, self.number_of_defects))
         else:
             format=super().dateformat
             x_values_p = [datetime.strptime(d, format).date() for d in super().dates]
             plt.gca().xaxis.set_major_formatter(mdates.DateFormatter(super().dateformat))
 
         # NP chart.
-        plt.figure(figsize=(15,5))
         plt.plot(x_values_p, self.value_p, marker="o",color="k",label="p")
         plt.plot(x_values_p, self.ucl_p,color="r",label="UCL")
 
         # The limits indicator for +2s, +1s.
         if super().limits:
             plt.plot(x_values_p, self.two_sigma_plus, color="r", linestyle='dashed', label="+2s")
             plt.plot(x_values_p, self.one_sigma_plus, color="r", linestyle='dashed', label="+1s")
@@ -82,23 +87,23 @@
         if super().limits:
             plt.plot(x_values_p, self.one_sigma_min, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_p, self.two_sigma_min, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_p, self.lcl_p,color="r",label="LCL")
         plt.title("P Control Chart")
 
-        # Check numerical or datetime for the x-axis.
-        if (len(super().dates) == 0):
-            plt.xticks(np.arange(self.number_of_defects))
-        else:
-            plt.xticks(rotation=45, ha='right')
-        
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the x-label.
+        plt.xlabel( self._xlabel)
+
+        # Set the y-label.
+        plt.ylabel( self._ylabel)
+
         plt.show()
 
     def split(self, stages:list):
         """ Split the chart.
 
             :param stages: The stages.
         """
```

### Comparing `sixsigmaspc-1.0.0/SPC/PControlChart.py` & `sixsigmaspc-1.0.1/SPC/PControlChart.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,29 @@
 import matplotlib.dates as mdates
 import numpy as np
 import pandas as pd
 from datetime import datetime
 from SPC import ControlChart
 
 class PControlChart(ControlChart):
-    def __init__(self, c:list, n:list):
+    def __init__(self, c:list, n:list, xlabel:str="", ylabel:str=""):
         """ Initialization.
 
             :param c: number of defects in the samples.
             :param n: sample sizes.
+            :param xlabel: x-as label.
+            :param ylabel: y-as label.
         """
         # Initialization of the base class.
         super().__init__(1) # P chart.
 
-        # The number of defects.
+        # Remember the parameters.
         self.number_of_defects = len(c)
+        self._xlabel = xlabel
+        self._ylabel = ylabel
 
         # Remember the number of defective in the sample.
         self.c = c
 
         # Remember the sample sizes.
         self.n = n
 
@@ -56,24 +60,25 @@
             self.one_sigma_plus[i] = self.value_p.mean() + 3 * np.sqrt((self.value_p.mean() * (1 - self.value_p.mean()))/n[i]) * 1/3
             self.one_sigma_min[i] = self.value_p.mean() - 3 * np.sqrt((self.value_p.mean() * (1 - self.value_p.mean()))/n[i]) * 1/3
             self.two_sigma_min[i] = self.value_p.mean() - 3 * np.sqrt((self.value_p.mean() * (1 - self.value_p.mean()))/n[i]) * 2/3
 
     def plot(self):
         """ Create the P chart.
         """
+        plt.figure(figsize=(15,5))
+
         # The x-axis can be numeric or datetime.
         if (len(super().dates) == 0):
             x_values_p = list(range(0, self.number_of_defects))
         else:
             format=super().dateformat
             x_values_p = [datetime.strptime(d, format).date() for d in super().dates]
             plt.gca().xaxis.set_major_formatter(mdates.DateFormatter(super().dateformat))
 
         # P chart.
-        plt.figure(figsize=(15,5))
         plt.plot(x_values_p, self.value_p, marker="o",color="k",label="p")
         plt.plot(x_values_p, self.ucl_p,color="r",label="UCL")
 
         # The limits indicator for +2s, +1s.
         if super().limits:
             plt.plot(x_values_p, self.two_sigma_plus, color="r", linestyle='dashed', label="+2s")
             plt.plot(x_values_p, self.one_sigma_plus, color="r", linestyle='dashed', label="+1s")
@@ -84,23 +89,23 @@
         if super().limits:
             plt.plot(x_values_p, self.one_sigma_min, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_p, self.two_sigma_min, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_p, self.lcl_p,color="r",label="LCL")
         plt.title("P Control Chart")
 
-        # Check numerical or datetime for the x-axis.
-        if (len(super().dates) == 0):
-            plt.xticks(np.arange(self.number_of_defects))
-        else:
-            plt.xticks(rotation=45, ha='right')
-        
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the x-label.
+        plt.xlabel( self._xlabel)
+
+        # Set the y-label.
+        plt.ylabel( self._ylabel)
+
         plt.show()
 
     def split(self, stages:list):
         """ Split the chart.
 
             :param stages: The stages.
         """
```

### Comparing `sixsigmaspc-1.0.0/SPC/ProcessCapabilityChart.py` & `sixsigmaspc-1.0.1/SPC/ProcessCapabilityChart.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/Rule01.py` & `sixsigmaspc-1.0.1/SPC/Rule01.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/Rule02.py` & `sixsigmaspc-1.0.1/SPC/Rule02.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/Rule03.py` & `sixsigmaspc-1.0.1/SPC/Rule03.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/Rule04.py` & `sixsigmaspc-1.0.1/SPC/Rule04.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/Rule05.py` & `sixsigmaspc-1.0.1/SPC/Rule05.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/Rule06.py` & `sixsigmaspc-1.0.1/SPC/Rule06.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/Rule07.py` & `sixsigmaspc-1.0.1/SPC/Rule07.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/Rule08.py` & `sixsigmaspc-1.0.1/SPC/Rule08.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/UControlChart.py` & `sixsigmaspc-1.0.1/SPC/UControlChart.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,29 @@
 import matplotlib.dates as mdates
 import numpy as np
 import pandas as pd
 from datetime import datetime
 from SPC import ControlChart
 
 class UControlChart(ControlChart):
-    def __init__(self, c:list, n:list):
+    def __init__(self, c:list, n:list, xlabel:str="", ylabel:str=""):
         """ Initialization.
 
             :param c: number of defects in the samples.
             :param n: sample sizes.
+            :param xlabel: x-as label.
+            :param ylabel: y-as label.
         """
         # Initialization of the base class.
         super().__init__(1) # U chart.
 
-        # The number of defects.
+        # Remember the parameters.
         self.number_of_defects = len(c)
+        self._xlabel = xlabel
+        self._ylabel = ylabel
 
         # Remember the number of defects.
         self.c = c
 
         # Remember the sample sizes.
         self.n = n
 
@@ -54,24 +58,25 @@
         self.one_sigma_plus[:] = self.value_u.mean() + 3 * np.sqrt(self.value_u.mean()/n.mean()) * 1/3
         self.one_sigma_min[:] = self.value_u.mean() - 3 * np.sqrt(self.value_u.mean()/n.mean()) * 1/3
         self.two_sigma_min[:] = self.value_u.mean() - 3 * np.sqrt(self.value_u.mean()/n.mean()) * 2/3
 
     def plot(self):
         """ Create the plot.
         """
+        plt.figure(figsize=(15,5))
+
         # The x-axis can be numeric or datetime.
         if (len(super().dates) == 0):
             x_values_U = list(range(0, self.number_of_defects))
         else:
             format=super().dateformat
             x_values_U = [datetime.strptime(d, format).date() for d in super().dates]
             plt.gca().xaxis.set_major_formatter(mdates.DateFormatter(super().dateformat))
 
         # U chart.
-        plt.figure(figsize=(15,5))
         plt.plot(x_values_U, self.value_u, marker="o",color="k",label="u")
         plt.plot(x_values_U, self.ucl_u,color="r",label="UCL")
 
         # Retrieve the data.
         df = self.data(0)
 
         # Plot the signals.
@@ -89,23 +94,23 @@
         if super().limits:
             plt.plot(x_values_U, self.one_sigma_min, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_U, self.two_sigma_min, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_U, self.lcl_u,color="r",label="LCL")
         plt.title("U Control Chart")
 
-        # Check numerical or datetime for the x-axis.
-        if (len(super().dates) == 0):
-            plt.xticks(np.arange(self.number_of_defects))
-        else:
-            plt.xticks(rotation=45, ha='right')
-        
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the x-label.
+        plt.xlabel( self._xlabel)
+
+        # Set the y-label.
+        plt.ylabel( self._ylabel)
+
         plt.show()
 
     def split(self, stages:list):
         """ Split the chart.
 
             :param stages: The stages.
         """
```

### Comparing `sixsigmaspc-1.0.0/SPC/XbarRControlChart.py` & `sixsigmaspc-1.0.1/SPC/XbarRControlChart.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,24 +21,30 @@
 
 class XbarRControlChart(ControlChart):
     _A2 : float # The Control Chart A2 constant.
     _d2 : float # The Control Chart d2 constant.
     _D3 : float # The Control Chart D3 constant.
     _D4 : float # The Control Chart D4 constant.
 
-    def __init__(self, data:list):
+    def __init__(self, data:list, xlabel:str="", ylabel_top:str="", ylabel_bottom:str=""):
         """ Initialization.
 
             :param data: values.
+            :param xlabel: x-as label.
+            :param ylabel_top: top y-as label.
+            :param ylabel_bottom: bottom y-as label.
         """
         # Initialization of the base class.
         super().__init__(2) # X bar chart and R chart.
 
-        # Remember the data.
+        # Remember the parameters.
         self._data = data
+        self._xlabel = xlabel
+        self._ylabel_top = ylabel_top
+        self._ylabel_bottom = ylabel_bottom
 
         # Initialization of the constants.
         constants = XbarRControlChartConstants()
 
         # Determine the subgroup size.
         n = len(data[0])
 
@@ -136,28 +142,30 @@
         if super().limits:
             plt.plot(x_values_X, self.one_sigma_min_X, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_X, self.two_sigma_min_X, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_X, self.lcl_Xbar, color="r", label="LCL")
         plt.title("X bar Chart")
 
-        # Check numerical or datetime for the x-axis.
-        if (len(super().dates) == 0):
-            plt.xticks(np.arange(len(self.value_X)))
-        else:
-            plt.xticks(rotation=45, ha='right')
-
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the y-label.
+        plt.ylabel( self._ylabel_top)
+
         # The 2nd vertical plot.
         plt.subplot(2,1,2)
 
-        # The x-axis is numeric.
-        x_values_R = list(range(0, len(self.value_R)))
+        # The x-axis can be numeric or datetime.
+        if (len(super().dates) == 0):
+            x_values_R = list(range(0, len(self.value_R)))
+        else:
+            format=super().dateformat
+            x_values_R = [datetime.strptime(d, format).date() for d in super().dates]
+            plt.gca().xaxis.set_major_formatter(mdates.DateFormatter(super().dateformat))
 
         # R chart.
         plt.plot(x_values_R, self.value_R, marker="o", color="k", label="R")
         plt.plot(x_values_R, self.ucl_R, color="r", label="UCL")
 
         # Retrieve the data.
         df = self.data(1)
@@ -177,20 +185,23 @@
         if super().limits:
             plt.plot(x_values_R, self.one_sigma_min_R, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_R, self.two_sigma_min_R, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_R, self.lcl_R, color="r", label="LCL")
         plt.title("R Chart")
 
-        # Set numerical for the x-axis.
-        plt.xticks(np.arange(len(self.value_X)))
-
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the y-label.
+        plt.ylabel(self._ylabel_bottom)
+
+        # Set the x-label.
+        plt.xlabel( self._xlabel)
+
         # Show the plot.
         plt.show()
 
     def split(self, stages:list):
         """ Split the chart.
 
             :param stages: The stages.
```

### Comparing `sixsigmaspc-1.0.0/SPC/XbarRControlChartConstants.py` & `sixsigmaspc-1.0.1/SPC/XbarRControlChartConstants.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/XbarSControlChart.py` & `sixsigmaspc-1.0.1/SPC/XbarSControlChart.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,24 +20,30 @@
 
 class XbarSControlChart(ControlChart):
     _A3 : float # The Control Chart A3 constant.
     _c4 : float # The Control Chart c4 constant.
     _B3 : float # The Control Chart B3 constant.
     _B4 : float # The Control Chart B4 constant.
 
-    def __init__(self, data:list):
+    def __init__(self, data:list, xlabel:str="", ylabel_top:str="", ylabel_bottom:str=""):
         """ Initialization.
 
             :param data: values.
+            :param xlabel: x-as label.
+            :param ylabel_top: top y-as label.
+            :param ylabel_bottom: bottom y-as label.
         """
         # Initialization of the base class.
         super().__init__(2) # X bar chart and S chart.
 
-        # Remember the data.
+        # Remember the parameters.
         self._data = data
+        self._xlabel = xlabel
+        self._ylabel_top = ylabel_top
+        self._ylabel_bottom = ylabel_bottom
 
         # Initialization of the constants.
         constants = XbarSControlChartConstants()
 
         # Determine the subgroup size.
         n = len(data[0])
 
@@ -135,28 +141,30 @@
         if super().limits:
             plt.plot(x_values_X, self.one_sigma_min_X, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_X, self.two_sigma_min_X, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_X, self.lcl_Xbar, color="r", label="LCL")
         plt.title("X bar Chart")
 
-        # Check numerical or datetime for the x-axis.
-        if (len(super().dates) == 0):
-            plt.xticks(np.arange(len(self.value_X)))
-        else:
-            plt.xticks(rotation=45, ha='right')
-
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the y-label.
+        plt.ylabel( self._ylabel_top)
+
         # The 2nd vertical plot.
         plt.subplot(2,1,2)
 
-        # The x-axis is numeric.
-        x_values_S = list(range(0, len(self.value_S)))
+        # The x-axis can be numeric or datetime.
+        if (len(super().dates) == 0):
+            x_values_S = list(range(0, len(self.value_S)))
+        else:
+            format=super().dateformat
+            x_values_S = [datetime.strptime(d, format).date() for d in super().dates]
+            plt.gca().xaxis.set_major_formatter(mdates.DateFormatter(super().dateformat))
 
         # S chart.
         plt.plot(x_values_S, self.value_S, marker="o", color="k", label="S")
         plt.plot(x_values_S, self.ucl_S, color="r", label="UCL")
 
         # Retrieve the data.
         df = self.data(1)
@@ -176,20 +184,23 @@
         if super().limits:
             plt.plot(x_values_S, self.one_sigma_min_S, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_S, self.two_sigma_min_S, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_S, self.lcl_S, color="r", label="LCL")
         plt.title("S Chart")
 
-        # Set numerical for the x-axis.
-        plt.xticks(np.arange(len(self.value_X)))
-
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the y-label.
+        plt.ylabel(self._ylabel_bottom)
+
+        # Set the x-label.
+        plt.xlabel( self._xlabel)
+
         # Show the plot.
         plt.show()
 
     def split(self, stages:list):
         """ Split the chart.
 
             :param stages: The stages.
```

### Comparing `sixsigmaspc-1.0.0/SPC/XbarSControlChartConstants.py` & `sixsigmaspc-1.0.1/SPC/XbarSControlChartConstants.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/SPC/XmRControlChart.py` & `sixsigmaspc-1.0.1/SPC/XmRControlChart.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,33 +7,39 @@
 https://sixsigmastudyguide.com/xmr-charts/
 """
 
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 import numpy as np
 import pandas as pd
-from datetime import datetime
+from datetime import datetime, timedelta
 from SPC import ControlChart
 
 class XmRControlChart(ControlChart):
     _A2 : float # The Control Chart A2 constant.
     _d2 : float # The Control Chart d2 constant.
     _D3 : float # The Control Chart D3 constant.
     _D4 : float # The Control Chart D4 constant.
 
-    def __init__(self, data:list):
+    def __init__(self, data:list, xlabel:str="", ylabel_top:str="", ylabel_bottom:str=""):
         """ Initialization.
 
             :param data: values.
+            :param xlabel: x-as label.
+            :param ylabel_top: top y-as label.
+            :param ylabel_bottom: bottom y-as label.
         """
         # Initialization of the base class.
         super().__init__(2) # X chart and mR chart.
 
-        # Remember the data.
+        # Remember the parameters.
         self._data = data
+        self._xlabel = xlabel
+        self._ylabel_top = ylabel_top
+        self._ylabel_bottom = ylabel_bottom
 
         # Remember the Control chart constants size=2 (comparing the current state with previous state).
         self._A2 = 0
         self._d2 = 1.128
         self._D3 = 0
         self._D4 = 3.267
 
@@ -126,28 +132,30 @@
         if super().limits:
             plt.plot(x_values_X, self.one_sigma_min_X, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_X, self.two_sigma_min_X, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_X, self.lcl_X, color="r", label="LCL")
         plt.title("X Chart")
 
-        # Check numerical or datetime for the x-axis.
-        if (len(super().dates) == 0):
-            plt.xticks(np.arange(len(self.value_X)))
-        else:
-            plt.xticks(rotation=45, ha='right')
-
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the y-label.
+        plt.ylabel( self._ylabel_top)
+
         # The 2nd vertical plot.
         plt.subplot(2,1,2)
 
-        # The x-axis is numeric.
-        x_values_mR = list(range(1, len(self.value_X)))
+        # The x-axis can be numeric or datetime.
+        if (len(super().dates) == 0):
+            x_values_mR = list(range(1, len(self.value_X)))
+        else:
+            format=super().dateformat
+            x_values_mR = [datetime.strptime(d, format).date() for d in super().dates][1:]
+            plt.gca().xaxis.set_major_formatter(mdates.DateFormatter(super().dateformat))
 
         # mR chart.
         plt.plot(x_values_mR, self.value_mR, marker="o", color="k", label="R")
         plt.plot(x_values_mR, self.ucl_mR, color="r", label="UCL")
 
         # Retrieve the data.
         df = self.data(1)
@@ -167,20 +175,23 @@
         if super().limits:
             plt.plot(x_values_mR, self.one_sigma_min_mR, color="r", linestyle='dashed', label="-1s")
             plt.plot(x_values_mR, self.two_sigma_min_mR, color="r", linestyle='dashed', label="-2s")
 
         plt.plot(x_values_mR, self.lcl_mR, color="r", label="LCL")
         plt.title("mR Chart")
 
-        # Set numerical for the x-axis.
-        plt.xticks(np.arange(len(self.value_X)))
-
         # Add a legend.
         plt.legend(loc='upper right')
 
+        # Set the y-label.
+        plt.ylabel(self._ylabel_bottom)
+
+        # Set the x-label.
+        plt.xlabel( self._xlabel)
+
         # Show the plot.
         plt.show()
 
     def split(self, stages:list):
         """ Split the chart.
 
             :param stages: The stages.
```

### Comparing `sixsigmaspc-1.0.0/SPC/__init__.py` & `sixsigmaspc-1.0.1/SPC/__init__.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/setup.py` & `sixsigmaspc-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="sixsigmaspc",
-    version="1.0.0",
+    version="1.0.1",
     description="Statistical Process Control library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sixsigmaspc.readthedocs.io/",
     author="Junior Marte Garcia, Marcel van Velzen",
     author_email="",
     license="MIT",
```

### Comparing `sixsigmaspc-1.0.0/sixsigmaspc.egg-info/SOURCES.txt` & `sixsigmaspc-1.0.1/sixsigmaspc.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 SPC/CControlChart.py
 SPC/ControlChart.py
 SPC/ControlChartConstants.py
 SPC/ImRControlChart.py
 SPC/MultiVariChart.py
```

### Comparing `sixsigmaspc-1.0.0/tests/ImRControlChart.py` & `sixsigmaspc-1.0.1/tests/ImRControlChart.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,33 +23,26 @@
 from SPC import Rule06
 from SPC import Rule07
 from SPC import Rule08
 from SPC import ImRControlChart
 
 if __name__ == '__main__':
     data = np.array([82, 84, 75, 79, 84, 81, 81, 82, 80, 78, 74])
-    #dates = ['21-12-2021', '22-12-2021', '23-12-2021', '24-12-2021', '25-12-2021', '26-12-2021', '27-12-2021', '28-12-2021', '29-12-2021','30-12-2021', '31-12-2021']
-    chart = ImRControlChart(data=data)
+    dates = ['21-12-21', '22-12-21', '23-12-21', '24-12-21', '25-12-21', '26-12-21', '27-12-21', '28-12-21', '29-12-21','30-12-21', '31-12-21']
+    chart = ImRControlChart(data=data, xlabel="x-label", ylabel_top="y-label-top", ylabel_bottom="y-label-bottom")
     normally_distributed=chart.normally_distributed(data=chart.value_I, significance_level=0.05)
     print("normally_distributed={0}".format(normally_distributed))
-    #chart.dates = dates
-    #chart.dateformat = "%d-%m-%Y"
+    chart.dates = dates
+    chart.dateformat = "%d-%m-%y"
     #stages=chart.stages(data=chart.value_I, max_stages=2)
     #if stages is not None:
     #    chart.split(stages)
     #chart.split([4, 7])
     #chart.limits=True
-    chart.append_rule(Rule01()) # Beyond limits: one or more points are beyond the control limits.
-    chart.append_rule(Rule02()) # Zone A: 2 out of 3 consecutive points in Zone A or beyond.
-    chart.append_rule(Rule03()) # Zone B: 4 out of 5 consecutive points in Zone B or beyond.
-    chart.append_rule(Rule04()) # Zone C: 7 or more consecutive points on one side of the average (in Zone C or beyond).
-    chart.append_rule(Rule05()) # Trend: 7 consecutive points trending up or trending down.
-    chart.append_rule(Rule06()) # Mixture: 8 consecutive points with no points in Zone C.
-    chart.append_rule(Rule07()) # Stratification: 15 consecutive points in Zone C.
-    chart.append_rule(Rule08()) # Over-control: 14 consecutive points alternating up and down.
+    chart.append_rules([Rule01(), Rule02(), Rule03(), Rule04(), Rule05(), Rule06(), Rule07(), Rule08()])
     chart.plot()
 
     df1 = chart.data(0)
-    print(df1[["CL", "UCL", "LCL"]])
+    #print(df1[["CL", "UCL", "LCL"]])
     df2 = chart.data(1)
-    print(df2[["CL", "UCL", "LCL"]])
-    print("stable={0}".format(chart.stable()))
+    #print(df2[["CL", "UCL", "LCL"]])
+    #print("stable={0}".format(chart.stable()))
```

### Comparing `sixsigmaspc-1.0.0/tests/ProcessCapabilityChartTest.py` & `sixsigmaspc-1.0.1/tests/ProcessCapabilityChartTest.py`

 * *Files identical despite different names*

### Comparing `sixsigmaspc-1.0.0/tests/XmRControlChart.py` & `sixsigmaspc-1.0.1/tests/XmRControlChart.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,33 +16,26 @@
 from SPC import Rule06
 from SPC import Rule07
 from SPC import Rule08
 from SPC import XmRControlChart
 
 if __name__ == '__main__':
     data = np.array([2.92, 2.96, 2.86, 3.04, 3.07, 2.85, 3.00, 2.92, 2.97, 2.97, 3.09, 3.07, 2.99, 3.06, 3.05, 3.02, 3.07, 2.91, 3.07, 3.20])
-    #dates = ['21-12-2021', '22-12-2021', '23-12-2021', '24-12-2021', '25-12-2021', '26-12-2021', '27-12-2021', '28-12-2021', '29-12-2021','30-12-2021', '31-12-2021', '01-01-2022', '02-01-2022', '03-01-2022', '05-01-2022', '06-01-2022', '07-01-2022', '08-01-2022', '09-01-2022', '10-01-2022']
-    chart = XmRControlChart(data=data)
+    dates = ['21-12-21', '22-12-21', '23-12-21', '24-12-21', '25-12-21', '26-12-21', '27-12-21', '28-12-21', '29-12-21','30-12-21', '31-12-21', '01-01-22', '02-01-22', '03-01-22', '05-01-22', '06-01-22', '07-01-22', '08-01-22', '09-01-22', '10-01-22']
+    chart = XmRControlChart(data=data, xlabel="x-label", ylabel_top="y-label-top", ylabel_bottom="y-label-bottom")
     normally_distributed=chart.normally_distributed(data=chart.value_X, significance_level=0.05)
     print("normally_distributed={0}".format(normally_distributed))
-    #chart.dates = dates
-    #chart.dateformat = "%d-%m-%Y"
+    chart.dates = dates
+    chart.dateformat = "%d-%m-%y"
     #stages=chart.stages(data=chart.value_X, max_stages=4)
     #if stages is not None:
     #    chart.split(stages)
     #chart.split([4, 7])
     #chart.limits=True
-    chart.append_rule(Rule01()) # Beyond limits: one or more points are beyond the control limits.
-    chart.append_rule(Rule02()) # Zone A: 2 out of 3 consecutive points in Zone A or beyond.
-    chart.append_rule(Rule03()) # Zone B: 4 out of 5 consecutive points in Zone B or beyond.
-    chart.append_rule(Rule04()) # Zone C: 7 or more consecutive points on one side of the average (in Zone C or beyond).
-    chart.append_rule(Rule05()) # Trend: 7 consecutive points trending up or trending down.
-    chart.append_rule(Rule06()) # Mixture: 8 consecutive points with no points in Zone C.
-    chart.append_rule(Rule07()) # Stratification: 15 consecutive points in Zone C.
-    chart.append_rule(Rule08()) # Over-control: 14 consecutive points alternating up and down.
+    chart.append_rules([Rule01()])
     chart.plot()
 
     df1 = chart.data(0)
-    print(df1[["CL", "UCL", "LCL"]])
+    #print(df1[["CL", "UCL", "LCL"]])
     df2 = chart.data(1)
-    print(df2[["CL", "UCL", "LCL"]])
-    print("stable={0}".format(chart.stable()))
+    #print(df2[["CL", "UCL", "LCL"]])
+    #print("stable={0}".format(chart.stable()))
```

