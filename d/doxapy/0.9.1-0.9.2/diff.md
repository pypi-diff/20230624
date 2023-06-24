# Comparing `tmp/doxapy-0.9.1.tar.gz` & `tmp/doxapy-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doxapy-0.9.1.tar", last modified: Sun Oct 10 04:58:19 2021, max compression
+gzip compressed data, was "doxapy-0.9.2.tar", last modified: Sat Jun 24 18:09:21 2023, max compression
```

## Comparing `doxapy-0.9.1.tar` & `doxapy-0.9.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-10 04:58:19.607852 doxapy-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-10 04:58:19.607852 doxapy-0.9.1/Doxa/
--rw-r--r--   0 runner    (1001) docker     (121)     4186 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Algorithm.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    12884 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Bataineh.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Bernsen.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/BinarizationFactory.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3717 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/ChanMeanCalc.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4724 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/ChanMeanVarianceCalc.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4351 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/ClassifiedPerformance.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/ContrastImage.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4328 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Convolution.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4756 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/DRDM.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/EdgeDetector.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     5032 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Gatos.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7795 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Grayscale.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     5471 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/ISauvola.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3569 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Image.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     8290 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/IntegralImageMeanVarianceCalc.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/LocalWindow.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    10685 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Morphology.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      975 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Niblack.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Nick.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Otsu.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    11839 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/PNM.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Palette.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2587 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Parameters.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Region.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      998 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Sauvola.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Su.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/TRSingh.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      560 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Types.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Wan.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/WienerFilter.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2021-10-10 04:58:14.000000 doxapy-0.9.1/Doxa/Wolf.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3933 2021-10-10 04:58:14.000000 doxapy-0.9.1/DoxaPy.cpp
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-10-10 04:58:14.000000 doxapy-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2021-10-10 04:58:19.607852 doxapy-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4050 2021-10-10 04:58:14.000000 doxapy-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-10 04:58:19.607852 doxapy-0.9.1/doxapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2021-10-10 04:58:19.000000 doxapy-0.9.1/doxapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      790 2021-10-10 04:58:19.000000 doxapy-0.9.1/doxapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-10 04:58:19.000000 doxapy-0.9.1/doxapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-10 04:58:19.000000 doxapy-0.9.1/doxapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      113 2021-10-10 04:58:14.000000 doxapy-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-10 04:58:19.607852 doxapy-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      982 2021-10-10 04:58:14.000000 doxapy-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:09:21.671142 doxapy-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:09:21.667142 doxapy-0.9.2/Doxa/
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Algorithm.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Bataineh.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Bernsen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/BinarizationFactory.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/ChanMeanCalc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/ChanMeanVarianceCalc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/ClassifiedPerformance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/ContrastImage.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Convolution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/DRDM.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/EdgeDetector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Gatos.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Grayscale.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/ISauvola.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Image.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/IntegralImageMeanVarianceCalc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/LocalWindow.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Morphology.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Niblack.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Nick.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Otsu.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/PNM.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Palette.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Parameters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Region.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Sauvola.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Su.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/TRSingh.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-24 18:09:15.000000 doxapy-0.9.2/Doxa/Types.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-24 18:09:16.000000 doxapy-0.9.2/Doxa/Wan.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-24 18:09:16.000000 doxapy-0.9.2/Doxa/WienerFilter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-24 18:09:16.000000 doxapy-0.9.2/Doxa/Wolf.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-24 18:09:15.000000 doxapy-0.9.2/DoxaPy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 18:09:15.000000 doxapy-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-24 18:09:21.671142 doxapy-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-24 18:09:15.000000 doxapy-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:09:21.671142 doxapy-0.9.2/doxapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-24 18:09:21.000000 doxapy-0.9.2/doxapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-24 18:09:21.000000 doxapy-0.9.2/doxapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 18:09:21.000000 doxapy-0.9.2/doxapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 18:09:21.000000 doxapy-0.9.2/doxapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-24 18:09:15.000000 doxapy-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 18:09:21.671142 doxapy-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-24 18:09:15.000000 doxapy-0.9.2/setup.py
```

### Comparing `doxapy-0.9.1/Doxa/Algorithm.hpp` & `doxapy-0.9.2/Doxa/Algorithm.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Bataineh.hpp` & `doxapy-0.9.2/Doxa/Bataineh.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Bernsen.hpp` & `doxapy-0.9.2/Doxa/Bernsen.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/BinarizationFactory.hpp` & `doxapy-0.9.2/Doxa/BinarizationFactory.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/ChanMeanCalc.hpp` & `doxapy-0.9.2/Doxa/ChanMeanCalc.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/ChanMeanVarianceCalc.hpp` & `doxapy-0.9.2/Doxa/ChanMeanVarianceCalc.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/ClassifiedPerformance.hpp` & `doxapy-0.9.2/Doxa/ClassifiedPerformance.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/ContrastImage.hpp` & `doxapy-0.9.2/Doxa/ContrastImage.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Convolution.hpp` & `doxapy-0.9.2/Doxa/Convolution.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/DRDM.hpp` & `doxapy-0.9.2/Doxa/DRDM.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/EdgeDetector.hpp` & `doxapy-0.9.2/Doxa/EdgeDetector.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Gatos.hpp` & `doxapy-0.9.2/Doxa/Gatos.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Grayscale.hpp` & `doxapy-0.9.2/Doxa/Grayscale.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/ISauvola.hpp` & `doxapy-0.9.2/Doxa/ISauvola.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Image.hpp` & `doxapy-0.9.2/Doxa/Image.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/IntegralImageMeanVarianceCalc.hpp` & `doxapy-0.9.2/Doxa/IntegralImageMeanVarianceCalc.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/LocalWindow.hpp` & `doxapy-0.9.2/Doxa/LocalWindow.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Morphology.hpp` & `doxapy-0.9.2/Doxa/Morphology.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Niblack.hpp` & `doxapy-0.9.2/Doxa/Niblack.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Nick.hpp` & `doxapy-0.9.2/Doxa/Nick.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Otsu.hpp` & `doxapy-0.9.2/Doxa/Otsu.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/PNM.hpp` & `doxapy-0.9.2/Doxa/PNM.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Palette.hpp` & `doxapy-0.9.2/Doxa/Palette.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Parameters.hpp` & `doxapy-0.9.2/Doxa/Parameters.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Region.hpp` & `doxapy-0.9.2/Doxa/Region.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Sauvola.hpp` & `doxapy-0.9.2/Doxa/Sauvola.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Su.hpp` & `doxapy-0.9.2/Doxa/Su.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/TRSingh.hpp` & `doxapy-0.9.2/Doxa/TRSingh.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Types.hpp` & `doxapy-0.9.2/Doxa/Types.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Wan.hpp` & `doxapy-0.9.2/Doxa/Wan.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/WienerFilter.hpp` & `doxapy-0.9.2/Doxa/WienerFilter.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/Doxa/Wolf.hpp` & `doxapy-0.9.2/Doxa/Wolf.hpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/DoxaPy.cpp` & `doxapy-0.9.2/DoxaPy.cpp`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/PKG-INFO` & `doxapy-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: doxapy
-Version: 0.9.1
+Version: 0.9.2
 Summary: An image binarization library focussing on local adaptive thresholding
 Home-page: https://github.com/brandonmpetty/doxa
 Author: Brandon M. Petty
 Author-email: brandonpetty1981@gmail.com
 License: CC0-1.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # DoxaPy
 
 ## Introduction
 DoxaPy is an image binarization library focussing on local adaptive thresholding algorithms. In English, this means that it has the ability to turn a color or gray scale image into a black and white image.
 
@@ -98,8 +97,7 @@
 CC0 - Brandon M. Petty, 2021
 
 To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to this software to the public domain worldwide. This software is distributed without any warranty.
 
 [View Online](https://creativecommons.org/publicdomain/zero/1.0/legalcode)
 
 "*Freely you have received; freely give.*" - Matt 10:8
-
```

### Comparing `doxapy-0.9.1/README.md` & `doxapy-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/doxapy.egg-info/PKG-INFO` & `doxapy-0.9.2/doxapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: doxapy
-Version: 0.9.1
+Version: 0.9.2
 Summary: An image binarization library focussing on local adaptive thresholding
 Home-page: https://github.com/brandonmpetty/doxa
 Author: Brandon M. Petty
 Author-email: brandonpetty1981@gmail.com
 License: CC0-1.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # DoxaPy
 
 ## Introduction
 DoxaPy is an image binarization library focussing on local adaptive thresholding algorithms. In English, this means that it has the ability to turn a color or gray scale image into a black and white image.
 
@@ -98,8 +97,7 @@
 CC0 - Brandon M. Petty, 2021
 
 To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to this software to the public domain worldwide. This software is distributed without any warranty.
 
 [View Online](https://creativecommons.org/publicdomain/zero/1.0/legalcode)
 
 "*Freely you have received; freely give.*" - Matt 10:8
-
```

### Comparing `doxapy-0.9.1/doxapy.egg-info/SOURCES.txt` & `doxapy-0.9.2/doxapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doxapy-0.9.1/setup.py` & `doxapy-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,12 +24,12 @@
     setup(
         author="Brandon M. Petty",
         author_email="brandonpetty1981@gmail.com",
         name="doxapy",
         description="An image binarization library focussing on local adaptive thresholding",
         long_description=long_description,
         long_description_content_type="text/markdown",
-        version="0.9.1",
+        version="0.9.2",
         url="https://github.com/brandonmpetty/doxa",
         license="CC0-1.0",
         ext_modules=ext_modules
     )
```

