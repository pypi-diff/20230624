# Comparing `tmp/censoredsummarystats-0.2.5.tar.gz` & `tmp/censoredsummarystats-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredsummarystats-0.2.5.tar", max compression
+gzip compressed data, was "censoredsummarystats-0.2.6.tar", max compression
```

## Comparing `censoredsummarystats-0.2.5.tar` & `censoredsummarystats-0.2.6.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0       58 2023-06-21 09:23:06.539217 censoredsummarystats-0.2.5/censoredsummarystats/__init__.py
--rw-r--r--   0        0        0    56782 2023-06-22 20:35:27.332270 censoredsummarystats-0.2.5/censoredsummarystats/statistics.py
--rw-r--r--   0        0        0     2291 2023-06-21 07:54:57.800594 censoredsummarystats-0.2.5/censoredsummarystats/utils.py
--rw-r--r--   0        0        0    11558 2023-06-21 07:54:57.796594 censoredsummarystats-0.2.5/LICENSE
--rw-r--r--   0        0        0      558 2023-06-22 20:35:27.338269 censoredsummarystats-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     8399 2023-06-22 11:23:41.035725 censoredsummarystats-0.2.5/README.md
--rw-r--r--   0        0        0     9029 1970-01-01 00:00:00.000000 censoredsummarystats-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-06-21 09:23:06.539217 censoredsummarystats-0.2.6/censoredsummarystats/__init__.py
+-rw-r--r--   0        0        0     7686 2023-06-24 15:44:48.393790 censoredsummarystats-0.2.6/censoredsummarystats/interval_to_result.py
+-rw-r--r--   0        0        0     3347 2023-06-24 15:44:48.413793 censoredsummarystats-0.2.6/censoredsummarystats/merge_count_info.py
+-rw-r--r--   0        0        0     5009 2023-06-24 15:44:48.419795 censoredsummarystats-0.2.6/censoredsummarystats/percent_exceedance.py
+-rw-r--r--   0        0        0     2466 2023-06-24 15:44:48.428794 censoredsummarystats-0.2.6/censoredsummarystats/precision.py
+-rw-r--r--   0        0        0    15228 2023-06-24 15:44:48.435796 censoredsummarystats-0.2.6/censoredsummarystats/stat_interval_aggregation.py
+-rw-r--r--   0        0        0    14180 2023-06-24 15:44:48.444795 censoredsummarystats-0.2.6/censoredsummarystats/statistics.py
+-rw-r--r--   0        0        0     6055 2023-06-24 15:44:48.450797 censoredsummarystats-0.2.6/censoredsummarystats/validation.py
+-rw-r--r--   0        0        0    11558 2023-06-21 07:54:57.796594 censoredsummarystats-0.2.6/LICENSE
+-rw-r--r--   0        0        0      558 2023-06-24 15:44:48.458799 censoredsummarystats-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     8600 2023-06-24 15:44:48.385792 censoredsummarystats-0.2.6/README.md
+-rw-r--r--   0        0        0     9230 1970-01-01 00:00:00.000000 censoredsummarystats-0.2.6/PKG-INFO
```

### Comparing `censoredsummarystats-0.2.5/censoredsummarystats/utils.py` & `censoredsummarystats-0.2.6/censoredsummarystats/precision.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-# Import numpy
+'''
+These functions apply a specific rounding algorithm based on value. Some values
+are rounded based on specified decimal places while others are based on
+significant digits.
+
+'''
 
 import numpy as np
 
-def string_precision(value,
-                     thousands_comma=False):
+def _string_precision(value,
+                      thousands_comma=False):
     '''
     A function that applies a specified rounding method that is value
     dependent. This method is specifically designed to reflect the
     typical measurement precision for water quality results. Depending on the
     value, the rounding is either to a particular number of decimal places or
     to a particular number of significant digits.
 
@@ -46,15 +51,15 @@
     # Values below 0.1 should be rounded to 2 significant digits
     else:
         string = f'{value:.2g}'
 
     return string
 
 
-def numeric_precision(value):
+def _numeric_precision(value):
     '''
     A function that returns a float data type from a rounding function instead
     of a string data type.
 
     Parameters
     ----------
     value : float
@@ -65,9 +70,9 @@
     -------
     float
         Float value that is rounded appropriately
 
     '''
     
     # Return the same rounded result as string_precision but as a float
-    return float(string_precision(value))
+    return float(_string_precision(value))
```

### Comparing `censoredsummarystats-0.2.5/LICENSE` & `censoredsummarystats-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.5/pyproject.toml` & `censoredsummarystats-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censoredsummarystats"
-version = "0.2.5"
+version = "0.2.6"
 description = "A python package for calculating summary stats on censored data (data that contains < and > symbols)."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/CensoredSummaryStats"
 license = "Apache-2.0"
 packages = [{include = "censoredsummarystats"}]
```

### Comparing `censoredsummarystats-0.2.5/README.md` & `censoredsummarystats-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # censoredsummarystats
 A repository that contains a CensoredData class for analyzing censored data for basic stats.
 
 ## Class settings:
 
-When initiating the class, there are two required inputs, 4 default analysis settings that can be changed, and several output column names that can be customized.
+When initiating the class, there are two required inputs, 6 default analysis settings that can be changed, and several output column names that can be customized.
 
 Required inputs:
 
 - **data**: A pandas DataFrame containing data
 - **value_col**: The column name for the column of potentially censored values
 
 Default analysis settings:
 
 - **include_negative_interval**: (default False) This setting controls whether left censored results are assumed to have a lower bound of 0 or whether the result can be negative.
 - **focus_high_potential**: (default True) This setting controls whether the highest potential or lowest potential is the focus for the result. The functions in this repository consider the full range of potential values of a censored result. This can often lead to a potential range for a statistical result. This setting determines whether to focus on the high or low end of the range. The maximum and minimum statistic ignores this setting and focuses on the high and low end of possible values, respectively.
 - **precision_tolerance_to_drop_censor**: (default 0.25) This setting controls whether a range of possible results is returned as censored or non-censored. For example, if an average is known to be between 2 and 3, then 2.5 would be returned as the result since the whole range is within 20% of 2.5 (20% < 25%). If this parameter was set to 0.15 (15%), then the tolerance would not cover the range and a result of <3 or >2 would be returned depending on the value of focus_high_potential.
 - **precision_rounding**: (default True) This setting controls whether to apply a specific rounding procedure (discussed below).
+- **thousands_comma**: (default False) This setting controls whether to output values over 1000 with commas (1,000).
+- **output_interval**: (default True) This setting controls whether to output the interval was converted to the output result.
 
 Customizable output column names:
 
 - **stat_col**: (default 'Statistic') This column contains the statatistic that was analyzed (minimum, maximum, median, etc.).
 - **result_col**: (default 'Result') This column contains the result of the statistical analysis as a string value. It may contain additional information for percentile or percent exceedance results.
 - **censor_col**: (default 'CensorComponent') This column contains the censor component for statistical results.
 - **numeric_col**: (default 'NumericComponent') This column contains the numeric component for statistical results.
@@ -48,35 +50,33 @@
 
 Additional table columns can be provided as a list so that the statistical functions obtain results for specified groups.
 
 1.	**Maximum**: Calculate the maximum value for a set of values.
 
 2.	**Minimum**: Calculate the minimum value for a set of values.
 
-3.	**Mean**: Calculate the average value for a set of values.
+3.	**Mean/Average**: Calculate the average value for a set of values.
 
 4.	**Median**: Calculate the median value for a set of values.
 
 5.	**Percentile**: Calculate a percentile for a set of values. The desired percentile should be provided as a number between 0 and 100. The default percentile method is Hazen, but other methods include Weibull, Tukey, Blom, and Excel as described in https://environment.govt.nz/assets/Publications/Files/hazen-percentile-calculator-2.xls
 
 6.	**Addition**: Calculate the sum for a set of values.
 
 7.	**Percent Exceedances**: Calculate the percentage of values that exceed a specified threshold. The desired threshold should be provided as a number. The default is to not treat results equal to the threshold as exceedances, but this can be changed by setting threshold_is_exceedance to True.
 
-8.	**Results to Components**: Split results into censor component (text) and numeric component (number).
-
 
 ## Method settings:
 
 Many of the methods above have similar input parameters. Those are:
 
 - **groupby_cols**: (default None) These are the columns that should be used to define the groups. Multiple groupings can be provided for some functions. This is useful to even weight data over sites or time periods. For example, a potential input for could be [['Year','Month','Day'], ['Year','Month'], ['Year']]. This would ensure that all days are evenly weighted within the month and that all months are evenly weighted within the year for a stat such as mean or median.
 - **count_cols**: (default None) Supplying a list of strings here will cause methods to return value counts. There should be the same number of strings as there are groupings in groupby_cols. Using the same example for groupby_cols, a user could supply ['Samples', 'Days Sampled', 'Months Sampled'] to get value counts for each grouping.
-- **round_to**: (default 2) The decimal places to round to for percent exceedance method.
-- **inplace**: (default False) If true, the data attribute of the class object will be replaced with the method results.
+- **stat_name**: (default is statistic) The text to use to describe the stat ('Minimum', 'Median', etc.)
+- **filters**: (default None) A dictionary of column names with values to filter for. This allows some simple filtering without recreating CensoredData objects.
 
 ## Dependencies
 
 For the installation of `censoredsummarystats`, the following packages are required:
 - [numpy >= 1.24](https://www.numpy.org/)
 
 ## Installation
```

### Comparing `censoredsummarystats-0.2.5/PKG-INFO` & `censoredsummarystats-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censoredsummarystats
-Version: 0.2.5
+Version: 0.2.6
 Summary: A python package for calculating summary stats on censored data (data that contains < and > symbols).
 Home-page: https://github.com/kurtvanness/CensoredSummaryStats
 License: Apache-2.0
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,27 +17,29 @@
 Description-Content-Type: text/markdown
 
 # censoredsummarystats
 A repository that contains a CensoredData class for analyzing censored data for basic stats.
 
 ## Class settings:
 
-When initiating the class, there are two required inputs, 4 default analysis settings that can be changed, and several output column names that can be customized.
+When initiating the class, there are two required inputs, 6 default analysis settings that can be changed, and several output column names that can be customized.
 
 Required inputs:
 
 - **data**: A pandas DataFrame containing data
 - **value_col**: The column name for the column of potentially censored values
 
 Default analysis settings:
 
 - **include_negative_interval**: (default False) This setting controls whether left censored results are assumed to have a lower bound of 0 or whether the result can be negative.
 - **focus_high_potential**: (default True) This setting controls whether the highest potential or lowest potential is the focus for the result. The functions in this repository consider the full range of potential values of a censored result. This can often lead to a potential range for a statistical result. This setting determines whether to focus on the high or low end of the range. The maximum and minimum statistic ignores this setting and focuses on the high and low end of possible values, respectively.
 - **precision_tolerance_to_drop_censor**: (default 0.25) This setting controls whether a range of possible results is returned as censored or non-censored. For example, if an average is known to be between 2 and 3, then 2.5 would be returned as the result since the whole range is within 20% of 2.5 (20% < 25%). If this parameter was set to 0.15 (15%), then the tolerance would not cover the range and a result of <3 or >2 would be returned depending on the value of focus_high_potential.
 - **precision_rounding**: (default True) This setting controls whether to apply a specific rounding procedure (discussed below).
+- **thousands_comma**: (default False) This setting controls whether to output values over 1000 with commas (1,000).
+- **output_interval**: (default True) This setting controls whether to output the interval was converted to the output result.
 
 Customizable output column names:
 
 - **stat_col**: (default 'Statistic') This column contains the statatistic that was analyzed (minimum, maximum, median, etc.).
 - **result_col**: (default 'Result') This column contains the result of the statistical analysis as a string value. It may contain additional information for percentile or percent exceedance results.
 - **censor_col**: (default 'CensorComponent') This column contains the censor component for statistical results.
 - **numeric_col**: (default 'NumericComponent') This column contains the numeric component for statistical results.
@@ -66,35 +68,33 @@
 
 Additional table columns can be provided as a list so that the statistical functions obtain results for specified groups.
 
 1.	**Maximum**: Calculate the maximum value for a set of values.
 
 2.	**Minimum**: Calculate the minimum value for a set of values.
 
-3.	**Mean**: Calculate the average value for a set of values.
+3.	**Mean/Average**: Calculate the average value for a set of values.
 
 4.	**Median**: Calculate the median value for a set of values.
 
 5.	**Percentile**: Calculate a percentile for a set of values. The desired percentile should be provided as a number between 0 and 100. The default percentile method is Hazen, but other methods include Weibull, Tukey, Blom, and Excel as described in https://environment.govt.nz/assets/Publications/Files/hazen-percentile-calculator-2.xls
 
 6.	**Addition**: Calculate the sum for a set of values.
 
 7.	**Percent Exceedances**: Calculate the percentage of values that exceed a specified threshold. The desired threshold should be provided as a number. The default is to not treat results equal to the threshold as exceedances, but this can be changed by setting threshold_is_exceedance to True.
 
-8.	**Results to Components**: Split results into censor component (text) and numeric component (number).
-
 
 ## Method settings:
 
 Many of the methods above have similar input parameters. Those are:
 
 - **groupby_cols**: (default None) These are the columns that should be used to define the groups. Multiple groupings can be provided for some functions. This is useful to even weight data over sites or time periods. For example, a potential input for could be [['Year','Month','Day'], ['Year','Month'], ['Year']]. This would ensure that all days are evenly weighted within the month and that all months are evenly weighted within the year for a stat such as mean or median.
 - **count_cols**: (default None) Supplying a list of strings here will cause methods to return value counts. There should be the same number of strings as there are groupings in groupby_cols. Using the same example for groupby_cols, a user could supply ['Samples', 'Days Sampled', 'Months Sampled'] to get value counts for each grouping.
-- **round_to**: (default 2) The decimal places to round to for percent exceedance method.
-- **inplace**: (default False) If true, the data attribute of the class object will be replaced with the method results.
+- **stat_name**: (default is statistic) The text to use to describe the stat ('Minimum', 'Median', etc.)
+- **filters**: (default None) A dictionary of column names with values to filter for. This allows some simple filtering without recreating CensoredData objects.
 
 ## Dependencies
 
 For the installation of `censoredsummarystats`, the following packages are required:
 - [numpy >= 1.24](https://www.numpy.org/)
 
 ## Installation
```

