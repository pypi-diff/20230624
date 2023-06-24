# Comparing `tmp/loanpy-3.0.1.tar.gz` & `tmp/loanpy-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loanpy-3.0.1.tar", last modified: Wed May 17 22:08:27 2023, max compression
+gzip compressed data, was "loanpy-3.0.2.tar", last modified: Sat Jun 24 14:24:56 2023, max compression
```

## Comparing `loanpy-3.0.1.tar` & `loanpy-3.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-17 22:08:27.587864 loanpy-3.0.1/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2023-04-16 19:03:02.000000 loanpy-3.0.1/LICENSE
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       20 2023-04-26 13:54:21.000000 loanpy-3.0.1/MANIFEST.in
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     4890 2023-05-17 22:08:27.587864 loanpy-3.0.1/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     3222 2023-05-04 19:19:00.000000 loanpy-3.0.1/README.rst
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-17 22:08:27.587864 loanpy-3.0.1/loanpy/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-04-24 21:01:57.000000 loanpy-3.0.1/loanpy/__init__.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     8355 2023-05-17 21:41:29.000000 loanpy-3.0.1/loanpy/eval_sca.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)   435389 2023-04-25 21:27:41.000000 loanpy-3.0.1/loanpy/ipa_all.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     6845 2023-05-17 21:37:27.000000 loanpy-3.0.1/loanpy/loanfinder.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    37335 2023-05-03 17:44:27.000000 loanpy-3.0.1/loanpy/scapplier.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     9260 2023-04-27 23:29:00.000000 loanpy-3.0.1/loanpy/scminer.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    23190 2023-04-27 23:28:10.000000 loanpy-3.0.1/loanpy/utils.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-17 22:08:27.587864 loanpy-3.0.1/loanpy.egg-info/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     4890 2023-05-17 22:08:27.000000 loanpy-3.0.1/loanpy.egg-info/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      643 2023-05-17 22:08:27.000000 loanpy-3.0.1/loanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2023-05-17 22:08:27.000000 loanpy-3.0.1/loanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       64 2023-05-17 22:08:27.000000 loanpy-3.0.1/loanpy.egg-info/requires.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        7 2023-05-17 22:08:27.000000 loanpy-3.0.1/loanpy.egg-info/top_level.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      210 2023-05-17 22:08:27.587864 loanpy-3.0.1/setup.cfg
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1956 2023-05-17 22:07:15.000000 loanpy-3.0.1/setup.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-17 22:08:27.587864 loanpy-3.0.1/tests/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     5427 2023-04-25 17:53:13.000000 loanpy-3.0.1/tests/test_eval_sca_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     5117 2023-05-17 21:53:28.000000 loanpy-3.0.1/tests/test_eval_sca_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      660 2023-04-23 22:13:44.000000 loanpy-3.0.1/tests/test_loanfinder_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1680 2023-04-23 22:13:26.000000 loanpy-3.0.1/tests/test_loanfinder_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    12621 2023-04-25 23:59:22.000000 loanpy-3.0.1/tests/test_scapplier_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    27616 2023-04-25 23:59:22.000000 loanpy-3.0.1/tests/test_scapplier_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1727 2023-04-16 19:03:02.000000 loanpy-3.0.1/tests/test_scminer_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     6820 2023-04-25 23:59:23.000000 loanpy-3.0.1/tests/test_scminer_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     3482 2023-04-25 21:48:43.000000 loanpy-3.0.1/tests/test_utils_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    11626 2023-04-25 22:18:49.000000 loanpy-3.0.1/tests/test_utils_unit.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-06-24 14:24:56.719296 loanpy-3.0.2/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2023-04-16 19:03:02.000000 loanpy-3.0.2/LICENSE
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       20 2023-04-26 13:54:21.000000 loanpy-3.0.2/MANIFEST.in
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     4890 2023-06-24 14:24:56.719296 loanpy-3.0.2/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3222 2023-05-04 19:19:00.000000 loanpy-3.0.2/README.rst
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-06-24 14:24:56.719296 loanpy-3.0.2/loanpy/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-04-24 21:01:57.000000 loanpy-3.0.2/loanpy/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     8355 2023-05-17 21:41:29.000000 loanpy-3.0.2/loanpy/eval_sca.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)   435389 2023-04-25 21:27:41.000000 loanpy-3.0.2/loanpy/ipa_all.csv
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     6845 2023-05-17 21:37:27.000000 loanpy-3.0.2/loanpy/loanfinder.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    37330 2023-06-23 15:12:21.000000 loanpy-3.0.2/loanpy/scapplier.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     9389 2023-06-24 14:21:30.000000 loanpy-3.0.2/loanpy/scminer.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    23190 2023-04-27 23:28:10.000000 loanpy-3.0.2/loanpy/utils.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-06-24 14:24:56.719296 loanpy-3.0.2/loanpy.egg-info/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     4890 2023-06-24 14:24:56.000000 loanpy-3.0.2/loanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      643 2023-06-24 14:24:56.000000 loanpy-3.0.2/loanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2023-06-24 14:24:56.000000 loanpy-3.0.2/loanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       64 2023-06-24 14:24:56.000000 loanpy-3.0.2/loanpy.egg-info/requires.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        7 2023-06-24 14:24:56.000000 loanpy-3.0.2/loanpy.egg-info/top_level.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      210 2023-06-24 14:24:56.719296 loanpy-3.0.2/setup.cfg
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1956 2023-06-24 14:23:26.000000 loanpy-3.0.2/setup.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-06-24 14:24:56.719296 loanpy-3.0.2/tests/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     5427 2023-04-25 17:53:13.000000 loanpy-3.0.2/tests/test_eval_sca_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     5117 2023-05-17 21:53:28.000000 loanpy-3.0.2/tests/test_eval_sca_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      660 2023-04-23 22:13:44.000000 loanpy-3.0.2/tests/test_loanfinder_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1680 2023-04-23 22:13:26.000000 loanpy-3.0.2/tests/test_loanfinder_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    12621 2023-04-25 23:59:22.000000 loanpy-3.0.2/tests/test_scapplier_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    27616 2023-04-25 23:59:22.000000 loanpy-3.0.2/tests/test_scapplier_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1727 2023-04-16 19:03:02.000000 loanpy-3.0.2/tests/test_scminer_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     6820 2023-04-25 23:59:23.000000 loanpy-3.0.2/tests/test_scminer_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3482 2023-04-25 21:48:43.000000 loanpy-3.0.2/tests/test_utils_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    11626 2023-04-25 22:18:49.000000 loanpy-3.0.2/tests/test_utils_unit.py
```

### Comparing `loanpy-3.0.1/LICENSE` & `loanpy-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/PKG-INFO` & `loanpy-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loanpy
-Version: 3.0.1
+Version: 3.0.2
 Summary: a linguistic toolkit for detecting old loanwords by predicting,evaluating and applying changes in horizontal and vertical lexical transfers
 Home-page: https://github.com/martino-vic/loanpy
 Download-URL: https://github.com/LoanpyDataHub/loanpy/archive/3.0.0.tar.gz
 Author: Viktor Martinović
 Author-email: viktor_martinovic@eva.mpg.de
 License: MIT
 Project-URL: documentation, https://loanpy.readthedocs.io/en/latest/home.html
```

### Comparing `loanpy-3.0.1/README.rst` & `loanpy-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/loanpy/eval_sca.py` & `loanpy-3.0.2/loanpy/eval_sca.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/loanpy/ipa_all.csv` & `loanpy-3.0.2/loanpy/ipa_all.csv`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/loanpy/loanfinder.py` & `loanpy-3.0.2/loanpy/loanfinder.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/loanpy/scapplier.py` & `loanpy-3.0.2/loanpy/scapplier.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 
             >>> from loanpy.scapplier import Adrc
             >>> adrc = Adrc("examples/sc2.json", "examples/inv.json")
             >>> adrc.repair_phonotactics(["d", "a", "d", "a"], "CVCV")
             ['d', 'a', 'd']
         """
 
-        # check if there is data available data for this structure
+        # check if there is available data for this structure
         try:
             predicted_phonotactics = self.sc[3][prosody][0]
         except KeyError:
             predicted_phonotactics = self.get_closest_phonotactics(prosody)
         #print("predicted phonotactics: ", predicted_phonotactics)
         # Get edit operations between structures, apply them 2 input IPA string
         matrix = get_mtx(prosody, predicted_phonotactics)
```

### Comparing `loanpy-3.0.1/loanpy/scminer.py` & `loanpy-3.0.2/loanpy/scminer.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,18 @@
         phoneme_inventory = json.load(f)["by_language"][tgtlg]["segments"]
 
     # sort phoneme_inventory phonemes by euclidean distance to every ipa sound
     heur = {}
     for row in ipa_all[1:]:
         distances = []
         for phoneme in phoneme_inventory:
-            v1, v2 = vectors[phoneme], vectors[row[0]]
+            try:  # Bugfix for Bislama diphthong "ae": not in ipa_all!
+                v1, v2 = vectors[phoneme], vectors[row[0]]
+            except KeyError:
+                continue
             # measure euclidean distance between feature vectors
             distances.append(
             math.sqrt(sum((v1[i] - v2[i]) ** 2 for i in range(len(v1))))
             )
         dist_and_phon = sorted(zip(distances, phoneme_inventory))
         heur[row[0]] = [i[1] for i in dist_and_phon]
```

### Comparing `loanpy-3.0.1/loanpy/utils.py` & `loanpy-3.0.2/loanpy/utils.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/loanpy.egg-info/PKG-INFO` & `loanpy-3.0.2/loanpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loanpy
-Version: 3.0.1
+Version: 3.0.2
 Summary: a linguistic toolkit for detecting old loanwords by predicting,evaluating and applying changes in horizontal and vertical lexical transfers
 Home-page: https://github.com/martino-vic/loanpy
 Download-URL: https://github.com/LoanpyDataHub/loanpy/archive/3.0.0.tar.gz
 Author: Viktor Martinović
 Author-email: viktor_martinovic@eva.mpg.de
 License: MIT
 Project-URL: documentation, https://loanpy.readthedocs.io/en/latest/home.html
```

### Comparing `loanpy-3.0.1/loanpy.egg-info/SOURCES.txt` & `loanpy-3.0.2/loanpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/setup.py` & `loanpy-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup(
   name='loanpy',
   description='a linguistic toolkit for detecting old loanwords by predicting,\
 evaluating and applying changes in horizontal and vertical lexical transfers',
   long_description=open("README.rst").read(),
   author='Viktor Martinović',
   author_email='viktor_martinovic@eva.mpg.de',
-  version='3.0.1',
+  version='3.0.2',
   packages=find_packages(),
   data_files=[("loanpy", ["loanpy/ipa_all.csv"])],
   include_package_data=True,
   extras_require={
   "test": ["pytest>=7.1.2", "coverage>=7.2.2"],
   "dev": ["wheel", "twine", "sphinx"]
   },
```

### Comparing `loanpy-3.0.1/tests/test_eval_sca_integration.py` & `loanpy-3.0.2/tests/test_eval_sca_integration.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/tests/test_eval_sca_unit.py` & `loanpy-3.0.2/tests/test_eval_sca_unit.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/tests/test_loanfinder_integration.py` & `loanpy-3.0.2/tests/test_loanfinder_integration.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/tests/test_loanfinder_unit.py` & `loanpy-3.0.2/tests/test_loanfinder_unit.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/tests/test_scapplier_integration.py` & `loanpy-3.0.2/tests/test_scapplier_integration.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/tests/test_scapplier_unit.py` & `loanpy-3.0.2/tests/test_scapplier_unit.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/tests/test_scminer_integration.py` & `loanpy-3.0.2/tests/test_scminer_integration.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/tests/test_scminer_unit.py` & `loanpy-3.0.2/tests/test_scminer_unit.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/tests/test_utils_integration.py` & `loanpy-3.0.2/tests/test_utils_integration.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.1/tests/test_utils_unit.py` & `loanpy-3.0.2/tests/test_utils_unit.py`

 * *Files identical despite different names*

