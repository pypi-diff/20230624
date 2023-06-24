# Comparing `tmp/describr-0.0.6.tar.gz` & `tmp/describr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "describr-0.0.6.tar", last modified: Sat Jun 24 05:40:11 2023, max compression
+gzip compressed data, was "describr-0.0.7.tar", last modified: Sat Jun 24 13:02:56 2023, max compression
```

## Comparing `describr-0.0.6.tar` & `describr-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 05:40:11.461003 describr-0.0.6/
--rw-rw-rw-   0        0        0     1099 2023-06-20 15:03:20.000000 describr-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5002 2023-06-24 05:40:11.461003 describr-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3794 2023-06-24 05:38:46.000000 describr-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 05:40:11.437997 describr-0.0.6/describr/
--rw-rw-rw-   0        0        0      129 2023-06-24 05:33:59.000000 describr-0.0.6/describr/__init__.py
--rw-rw-rw-   0        0        0    16777 2023-06-24 05:33:43.000000 describr-0.0.6/describr/describr.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:40:11.459000 describr-0.0.6/describr.egg-info/
--rw-rw-rw-   0        0        0     5002 2023-06-24 05:40:11.000000 describr-0.0.6/describr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-24 05:40:11.000000 describr-0.0.6/describr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 05:40:11.000000 describr-0.0.6/describr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-24 05:40:11.000000 describr-0.0.6/describr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 05:40:11.000000 describr-0.0.6/describr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 05:40:11.461003 describr-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1613 2023-06-24 05:34:28.000000 describr-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:02:56.236786 describr-0.0.7/
+-rw-rw-rw-   0        0        0     1099 2023-06-20 15:03:20.000000 describr-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5002 2023-06-24 13:02:56.235786 describr-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3905 2023-06-24 13:01:11.000000 describr-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 13:02:56.206786 describr-0.0.7/describr/
+-rw-rw-rw-   0        0        0      129 2023-06-24 13:01:37.000000 describr-0.0.7/describr/__init__.py
+-rw-rw-rw-   0        0        0    16776 2023-06-24 12:57:52.000000 describr-0.0.7/describr/describr.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:02:56.234787 describr-0.0.7/describr.egg-info/
+-rw-rw-rw-   0        0        0     5002 2023-06-24 13:02:56.000000 describr-0.0.7/describr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-24 13:02:56.000000 describr-0.0.7/describr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:02:56.000000 describr-0.0.7/describr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-24 13:02:56.000000 describr-0.0.7/describr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 13:02:56.000000 describr-0.0.7/describr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:02:56.236786 describr-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1613 2023-06-24 13:01:22.000000 describr-0.0.7/setup.py
```

### Comparing `describr-0.0.6/LICENSE` & `describr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `describr-0.0.6/PKG-INFO` & `describr-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.
 Home-page: https://github.com/famutimine/describr
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: descriptive statistics
 Platform: UNKNOWN
```

### Comparing `describr-0.0.6/README.md` & `describr-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,30 +45,33 @@
 df = pd.DataFrame(data)
 ```
 #### Parameters
 **df**: name of dataframe
 
 **id_col**: Primary key of the dataframe; accepts string or integer or float.
 
-**group_col**: A Column to group by, It must be a binary column. 
+**group_col**: A Column to group by, It must be a dichotomous variable with only two uniques responses. Only Strings response values are acceptable, e.g. 'Yes and 'No', 'Case' and 'Control', 'Intervention' and 'Non_Intervention_Group' e.t.c. 
 
-**positive_class**: This is the response value for the primary outcome of interest. Only Strings response values are acceptable, e.g. 'Yes and 'No', 'Case' and 'Control', 'Intervention' and 'Non_Intervention_Group' e.t.c. In this example, positive_class would be 'Yes' or 'Case' or 'Intervention' respectively.
+**positive_class**: This is the response value for the primary outcome of interest. Following on prior example, positive_class would be 'Yes' or 'Case' or 'Intervention' respectively.
 
 **continuous_var_summary**: Users specifies measures of central tendency, only mean and median are acceptable. This parameter is case insensitive.
 
 
 #### Example usage of FindOutliers Class
 
 This returns a dataframe (outliers_flag_df) with outlier_flag column (outlier_flag =1: record contains one or more ouliers). Tukey's IQR method is used to detect outliers in the data
 
 ```python
 outliers_flag=FindOutliers(df=df, id_col='MCID', group_col='TREATMENT')
 outliers_flag_df=outliers_flag.flag_outliers()
 ```
 #### This example counts number of rows with outliers stratified by a defined grouping variable
+
+If you have a large dataframe, this can take some time.
+
 ```python
 outliers_flag.count_outliers()
 ```
 #### This example removes all outliers
 ```python
 df2=outliers_flag.remove_outliers()
 df2.shape
```

### Comparing `describr-0.0.6/describr/describr.py` & `describr-0.0.7/describr/describr.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         sample_size = row[column_name.replace('_Proportion', '_n')]
         fraction = row[column_name]
         return '{:.0f} ({:.1%})'.format(sample_size, fraction)
     
     def format_continuous_column(self, row, column_name):
         mean = row[column_name.replace('_mean', '_std')]
         std = row[column_name]
-        return '{:.2f} ({:.2f})'.format(mean, std)
+        return '{:.2f} ({:.2f})'.format(std,mean)
     
     def format_continuous_median_column(self, row, column_name):
         median = row[column_name]
         q1 = row[column_name.replace('_median', '_Q1')]
         q3 = row[column_name.replace('_median', '_Q3')]
         return '{:.2f} ({:.2f} - {:.2f})'.format(median, q1, q3)
```

### Comparing `describr-0.0.6/describr.egg-info/PKG-INFO` & `describr-0.0.7/describr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.
 Home-page: https://github.com/famutimine/describr
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: descriptive statistics
 Platform: UNKNOWN
```

### Comparing `describr-0.0.6/setup.py` & `describr-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from urllib.request import urlopen
 
 with urlopen("https://raw.githubusercontent.com/famutimine/describr/main/README.md") as fh:
     long_description = fh.read().decode()
 
 setuptools.setup(
     name='describr',
-    version='0.0.6',
+    version='0.0.7',
     description='Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/famutimine/describr',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

