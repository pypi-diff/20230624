# Comparing `tmp/describr-0.0.4.tar.gz` & `tmp/describr-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "describr-0.0.4.tar", last modified: Tue Jun 20 18:12:16 2023, max compression
+gzip compressed data, was "describr-0.0.5.tar", last modified: Fri Jun 23 23:45:21 2023, max compression
```

## Comparing `describr-0.0.4.tar` & `describr-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 18:12:16.265346 describr-0.0.4/
--rw-rw-rw-   0        0        0     1099 2023-06-20 15:03:20.000000 describr-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4995 2023-06-20 18:12:16.265346 describr-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3740 2023-06-20 15:28:09.000000 describr-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 18:12:16.245315 describr-0.0.4/describr/
--rw-rw-rw-   0        0        0      129 2023-06-20 18:10:20.000000 describr-0.0.4/describr/__init__.py
--rw-rw-rw-   0        0        0    16784 2023-06-20 18:10:00.000000 describr-0.0.4/describr/describr.py
-drwxrwxrwx   0        0        0        0 2023-06-20 18:12:16.264339 describr-0.0.4/describr.egg-info/
--rw-rw-rw-   0        0        0     4995 2023-06-20 18:12:16.000000 describr-0.0.4/describr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-20 18:12:16.000000 describr-0.0.4/describr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 18:12:16.000000 describr-0.0.4/describr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-20 18:12:16.000000 describr-0.0.4/describr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 18:12:16.000000 describr-0.0.4/describr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 18:12:16.265346 describr-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1613 2023-06-20 18:10:29.000000 describr-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 23:45:21.618896 describr-0.0.5/
+-rw-rw-rw-   0        0        0     1099 2023-06-20 15:03:20.000000 describr-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5002 2023-06-23 23:45:21.617896 describr-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3740 2023-06-20 15:28:09.000000 describr-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 23:45:21.594651 describr-0.0.5/describr/
+-rw-rw-rw-   0        0        0      129 2023-06-23 23:41:10.000000 describr-0.0.5/describr/__init__.py
+-rw-rw-rw-   0        0        0    16799 2023-06-23 23:40:36.000000 describr-0.0.5/describr/describr.py
+drwxrwxrwx   0        0        0        0 2023-06-23 23:45:21.616895 describr-0.0.5/describr.egg-info/
+-rw-rw-rw-   0        0        0     5002 2023-06-23 23:45:21.000000 describr-0.0.5/describr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-23 23:45:21.000000 describr-0.0.5/describr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 23:45:21.000000 describr-0.0.5/describr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-23 23:45:21.000000 describr-0.0.5/describr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 23:45:21.000000 describr-0.0.5/describr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 23:45:21.618896 describr-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1613 2023-06-23 23:41:44.000000 describr-0.0.5/setup.py
```

### Comparing `describr-0.0.4/LICENSE` & `describr-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `describr-0.0.4/PKG-INFO` & `describr-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describr
-Version: 0.0.4
+Version: 0.0.5
 Summary: Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.
 Home-page: https://github.com/famutimine/describr
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: descriptive statistics
 Platform: UNKNOWN
@@ -100,29 +100,30 @@
 df2.shape
 ```
 
 #### Example usage of DescriptiveStats Class
 ```python 
 descriptive_stats = DescriptiveStats(df=df, id_col='MCID', group_col='TREATMENT', positive_class='Yes', continuous_var_summary='median')
 ```
-#### Get statistics for binary and categorical variables and returns a dataframe.
+#### Gets statistics for binary and categorical variables and returns a dataframe.
 ```python
 binary_stats_df = descriptive_stats.get_binary_stats()
 ```
 
-#### Get mean and standard deviation for continuous variables and returns a dataframe.
+#### Gets mean and standard deviation for continuous variables and returns a dataframe.
 
 ```python
 continuous_stats_mean_df = descriptive_stats.get_continuous_mean_stats()
 ```
 
-#### Get median and interquartile range for continuous variables and returns a dataframe.
+#### Gets median and interquartile range for continuous variables and returns a dataframe.
 ```python
 continuous_stats_median_df = descriptive_stats.get_continuous_median_stats()
 ```
 
-#### Compute summary statistics for binary and continuous variables based on defined measure of central tendency. Method returns a dataframe.
+#### Computes summary statistics for binary and continuous variables based on defined measure of central tendency. Method returns a dataframe.
 ````python
 descriptive_stats.compute_descriptive_stats()
 summary_stats = descriptive_stats.summary_stats()
-````
+````
+
```

### Comparing `describr-0.0.4/README.md` & `describr-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `describr-0.0.4/describr/describr.py` & `describr-0.0.5/describr/describr.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         binary_stats_df_sample_mean.drop('stats', axis=1, inplace=True)
         
         binary_p_values_df.reset_index(inplace=True)
         binary_p_values_df.rename(columns={'index': 'variable'}, inplace=True)
 
         df_binary = binary_stats_df_sample_mean.merge(binary_p_values_df, on='variable')
         
-        positive_class_columns = [col for col in df_binary.columns if self.positive_class in col]
+        positive_class_columns = [col for col in df_binary.columns if str(self.positive_class) in col]
         column_order = [col for col in df_binary.columns if col not in positive_class_columns]
         column_order.insert(1, positive_class_columns[0])
         column_order.insert(2, positive_class_columns[1])
         df_binary = df_binary[column_order]
 
         return df_binary
 
@@ -162,15 +162,15 @@
 
         mean_df.drop('stats', axis=1, inplace=True)
 
         continuous_p_values_df.reset_index(inplace=True)
         continuous_p_values_df.rename(columns={'index': 'variable'}, inplace=True)
 
         df_continuous = mean_df.merge(continuous_p_values_df, on='variable')
-        positive_class_columns = [col for col in df_continuous.columns if self.positive_class in col]
+        positive_class_columns = [col for col in df_continuous.columns if str(self.positive_class) in col]
         column_order = [col for col in df_continuous.columns if col not in positive_class_columns]
         column_order.insert(1, positive_class_columns[0])
         column_order.insert(2, positive_class_columns[1])
         df_continuous = df_continuous[column_order]
 
         return df_continuous
 
@@ -212,15 +212,15 @@
 
         continuous_p_values_median_df = pd.DataFrame.from_dict(continuous_p_values_median, orient='index', columns=['p-value'])
 
         continuous_p_values_median_df.reset_index(inplace=True)
         continuous_p_values_median_df.rename(columns={'index': 'variable'}, inplace=True)
 
         df_continuous_median = continuous_stats_median_df.merge(continuous_p_values_median_df, on='variable')
-        positive_class_columns = [col for col in df_continuous_median.columns if self.positive_class in col]
+        positive_class_columns = [col for col in df_continuous_median.columns if str(self.positive_class) in col]
         
         if len(positive_class_columns) > 1:
             column_order = [col for col in df_continuous_median.columns if col not in positive_class_columns]
             column_order.insert(1, positive_class_columns[0])
             column_order.insert(2, positive_class_columns[1])
             column_order.insert(3, positive_class_columns[2])
             df_continuous_median = df_continuous_median[column_order]
```

### Comparing `describr-0.0.4/describr.egg-info/PKG-INFO` & `describr-0.0.5/describr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describr
-Version: 0.0.4
+Version: 0.0.5
 Summary: Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.
 Home-page: https://github.com/famutimine/describr
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: descriptive statistics
 Platform: UNKNOWN
@@ -100,29 +100,30 @@
 df2.shape
 ```
 
 #### Example usage of DescriptiveStats Class
 ```python 
 descriptive_stats = DescriptiveStats(df=df, id_col='MCID', group_col='TREATMENT', positive_class='Yes', continuous_var_summary='median')
 ```
-#### Get statistics for binary and categorical variables and returns a dataframe.
+#### Gets statistics for binary and categorical variables and returns a dataframe.
 ```python
 binary_stats_df = descriptive_stats.get_binary_stats()
 ```
 
-#### Get mean and standard deviation for continuous variables and returns a dataframe.
+#### Gets mean and standard deviation for continuous variables and returns a dataframe.
 
 ```python
 continuous_stats_mean_df = descriptive_stats.get_continuous_mean_stats()
 ```
 
-#### Get median and interquartile range for continuous variables and returns a dataframe.
+#### Gets median and interquartile range for continuous variables and returns a dataframe.
 ```python
 continuous_stats_median_df = descriptive_stats.get_continuous_median_stats()
 ```
 
-#### Compute summary statistics for binary and continuous variables based on defined measure of central tendency. Method returns a dataframe.
+#### Computes summary statistics for binary and continuous variables based on defined measure of central tendency. Method returns a dataframe.
 ````python
 descriptive_stats.compute_descriptive_stats()
 summary_stats = descriptive_stats.summary_stats()
-````
+````
+
```

### Comparing `describr-0.0.4/setup.py` & `describr-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from urllib.request import urlopen
 
 with urlopen("https://raw.githubusercontent.com/famutimine/describr/main/README.md") as fh:
     long_description = fh.read().decode()
 
 setuptools.setup(
     name='describr',
-    version='0.0.4',
+    version='0.0.5',
     description='Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/famutimine/describr',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

