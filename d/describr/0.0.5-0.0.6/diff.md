# Comparing `tmp/describr-0.0.5.tar.gz` & `tmp/describr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "describr-0.0.5.tar", last modified: Fri Jun 23 23:45:21 2023, max compression
+gzip compressed data, was "describr-0.0.6.tar", last modified: Sat Jun 24 05:40:11 2023, max compression
```

## Comparing `describr-0.0.5.tar` & `describr-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 23:45:21.618896 describr-0.0.5/
--rw-rw-rw-   0        0        0     1099 2023-06-20 15:03:20.000000 describr-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5002 2023-06-23 23:45:21.617896 describr-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3740 2023-06-20 15:28:09.000000 describr-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 23:45:21.594651 describr-0.0.5/describr/
--rw-rw-rw-   0        0        0      129 2023-06-23 23:41:10.000000 describr-0.0.5/describr/__init__.py
--rw-rw-rw-   0        0        0    16799 2023-06-23 23:40:36.000000 describr-0.0.5/describr/describr.py
-drwxrwxrwx   0        0        0        0 2023-06-23 23:45:21.616895 describr-0.0.5/describr.egg-info/
--rw-rw-rw-   0        0        0     5002 2023-06-23 23:45:21.000000 describr-0.0.5/describr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-23 23:45:21.000000 describr-0.0.5/describr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 23:45:21.000000 describr-0.0.5/describr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-23 23:45:21.000000 describr-0.0.5/describr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 23:45:21.000000 describr-0.0.5/describr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 23:45:21.618896 describr-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1613 2023-06-23 23:41:44.000000 describr-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:40:11.461003 describr-0.0.6/
+-rw-rw-rw-   0        0        0     1099 2023-06-20 15:03:20.000000 describr-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5002 2023-06-24 05:40:11.461003 describr-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3794 2023-06-24 05:38:46.000000 describr-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 05:40:11.437997 describr-0.0.6/describr/
+-rw-rw-rw-   0        0        0      129 2023-06-24 05:33:59.000000 describr-0.0.6/describr/__init__.py
+-rw-rw-rw-   0        0        0    16777 2023-06-24 05:33:43.000000 describr-0.0.6/describr/describr.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:40:11.459000 describr-0.0.6/describr.egg-info/
+-rw-rw-rw-   0        0        0     5002 2023-06-24 05:40:11.000000 describr-0.0.6/describr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-24 05:40:11.000000 describr-0.0.6/describr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 05:40:11.000000 describr-0.0.6/describr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-24 05:40:11.000000 describr-0.0.6/describr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 05:40:11.000000 describr-0.0.6/describr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 05:40:11.461003 describr-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1613 2023-06-24 05:34:28.000000 describr-0.0.6/setup.py
```

### Comparing `describr-0.0.5/LICENSE` & `describr-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `describr-0.0.5/PKG-INFO` & `describr-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.
 Home-page: https://github.com/famutimine/describr
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: descriptive statistics
 Platform: UNKNOWN
```

### Comparing `describr-0.0.5/README.md` & `describr-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 df = pd.DataFrame(data)
 ```
 #### Parameters
 **df**: name of dataframe
 
 **id_col**: Primary key of the dataframe; accepts string or integer or float.
 
-**group_col**: A Column to group by, It must be a binary column. Strings or integers are acceptable. 
+**group_col**: A Column to group by, It must be a binary column. 
 
-**positive_class**: This is the response value for the primary outcome of interest. For instance, positive value for a Treatment cohort is 'Yes' or 1 otherwise 'No' or 0, respectively. Strings or integers are acceptable.
+**positive_class**: This is the response value for the primary outcome of interest. Only Strings response values are acceptable, e.g. 'Yes and 'No', 'Case' and 'Control', 'Intervention' and 'Non_Intervention_Group' e.t.c. In this example, positive_class would be 'Yes' or 'Case' or 'Intervention' respectively.
 
 **continuous_var_summary**: Users specifies measures of central tendency, only mean and median are acceptable. This parameter is case insensitive.
 
 
 #### Example usage of FindOutliers Class
 
 This returns a dataframe (outliers_flag_df) with outlier_flag column (outlier_flag =1: record contains one or more ouliers). Tukey's IQR method is used to detect outliers in the data
```

### Comparing `describr-0.0.5/describr/describr.py` & `describr-0.0.6/describr/describr.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,19 +216,20 @@
         continuous_p_values_median_df.rename(columns={'index': 'variable'}, inplace=True)
 
         df_continuous_median = continuous_stats_median_df.merge(continuous_p_values_median_df, on='variable')
         positive_class_columns = [col for col in df_continuous_median.columns if str(self.positive_class) in col]
         
         if len(positive_class_columns) > 1:
             column_order = [col for col in df_continuous_median.columns if col not in positive_class_columns]
-            column_order.insert(1, positive_class_columns[0])
-            column_order.insert(2, positive_class_columns[1])
-            column_order.insert(3, positive_class_columns[2])
+            n=len(column_order)-2
+            x=0
+            while x<n:
+                column_order.insert(x+1, positive_class_columns[x])
+                x += 1
             df_continuous_median = df_continuous_median[column_order]
-
         return df_continuous_median
 
 
 
     def compute_descriptive_stats(self):
         binary_vars, continuous_vars = self._identify_binary_continuous_vars()
```

### Comparing `describr-0.0.5/describr.egg-info/PKG-INFO` & `describr-0.0.6/describr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.
 Home-page: https://github.com/famutimine/describr
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: descriptive statistics
 Platform: UNKNOWN
```

### Comparing `describr-0.0.5/setup.py` & `describr-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from urllib.request import urlopen
 
 with urlopen("https://raw.githubusercontent.com/famutimine/describr/main/README.md") as fh:
     long_description = fh.read().decode()
 
 setuptools.setup(
     name='describr',
-    version='0.0.5',
+    version='0.0.6',
     description='Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/famutimine/describr',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

