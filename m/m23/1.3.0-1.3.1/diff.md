# Comparing `tmp/m23-1.3.0.tar.gz` & `tmp/m23-1.3.1.tar.gz`

## Comparing `m23-1.3.0.tar` & `m23-1.3.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.3.0/.flake8
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 m23-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.3.0/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.3.0/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.3.0/nights_csv.toml
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.3.0/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.3.0/renormalize.toml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.3.0/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.3.0/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 m23-1.3.0/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/matrix/utils.py
--rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/processor/__init__.py
--rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    22296 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725365 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/reference/README.md
--rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/reference/ref_revised_71.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.3.0/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.3.0/.gitignore
--rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 m23-1.3.0/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 m23-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.3.1/.flake8
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 m23-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.3.1/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.3.1/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.3.1/nights_csv.toml
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.3.1/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.3.1/renormalize.toml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.3.1/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.3.1/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 m23-1.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    22109 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725377 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/reference/README.md
+-rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/reference/ref_revised_71.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.3.1/.gitignore
+-rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 m23-1.3.1/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 m23-1.3.1/PKG-INFO
```

### Comparing `m23-1.3.0/CHANGELOG.md` & `m23-1.3.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.1 (2023-06-24)
+
+### Fix
+
+* Use correct datatype when saving aligned images ([`386cf38`](https://github.com/LutherAstrophysics/m23/commit/386cf3854771c600dd785dfaf5c39962b4ae69c8))
+* Use IDL like round during extraction ([`2fc9c35`](https://github.com/LutherAstrophysics/m23/commit/2fc9c3546ad852e6e191a84e7a6589ebe4dc9530))
+* Allow sky bg to be 0 ([`6b98aa2`](https://github.com/LutherAstrophysics/m23/commit/6b98aa20acb2ba86831dd5b1f900b3a8f3f632bf))
+
+### Documentation
+
+* Extraction ([`be3e805`](https://github.com/LutherAstrophysics/m23/commit/be3e805b4a515ee2fea0b7561ea09974b4acdf01))
+
 ## v1.3.0 (2023-06-22)
 
 ### Feature
 
 * Enhance aligned combined file format to matcher alternate harmless patterns ([`38b0375`](https://github.com/LutherAstrophysics/m23/commit/38b03750b3450577cd3cfefe5d653396a544f767))
 
 ### Documentation
```

### Comparing `m23-1.3.0/brown.toml` & `m23-1.3.1/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/mf.toml` & `m23-1.3.1/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/nights_csv.toml` & `m23-1.3.1/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/rainbow.toml` & `m23-1.3.1/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/requirements.txt` & `m23-1.3.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/.github/workflows/python-publish.yml` & `m23-1.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/.vscode/settings.json` & `m23-1.3.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/__main__.py` & `m23-1.3.1/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/constants.py` & `m23-1.3.1/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/align/__init__.py` & `m23-1.3.1/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/calibrate/calibration.py` & `m23-1.3.1/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/calibrate/master_calibrate.py` & `m23-1.3.1/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/charts/__init__.py` & `m23-1.3.1/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/combine/__init__.py` & `m23-1.3.1/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/extract/__init__.py` & `m23-1.3.1/src/m23/extract/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,15 +40,22 @@
             non_zero_indices = np.nonzero(sorted_data)
             # Ignore the zeros
             sorted_data = sorted_data[non_zero_indices]
 
             centered_array = sorted_data[
                 int(0.45 * len(sorted_data)) : int(0.55 * len(sorted_data)) + 1
             ]
-            bg_data[(i, j)] = np.mean(centered_array)
+
+            # If the data just contains zeros than this will mean that after the
+            # zero removal step, our array will be empty and the mean of empty
+            # array is nan, we would rather want to write it as 0
+            if len(centered_array) == 0:
+                bg_data[(i, j)] = 0
+            else:
+                bg_data[(i, j)] = np.mean(centered_array)
 
     return bg_data
 
 
 def extract_stars(
     image_data: npt.NDArray,
     reference_log_file: ReferenceLogFile,
@@ -144,24 +151,37 @@
     function i.e extract_stars
     """
     regionSize = 64
     pixelsPerStar = np.count_nonzero(circleMatrix(radius))
 
     def fluxSumForStar(position, radius, star_no) -> Tuple[int]:
         """
-        This function returns the flux of of a star at specified `position` using
-        `radius` as radius of extraction. Note that this tuple a three-tuple where
-        the first, second, and third element correspond to total star flux, background flux
-        and star flux after background subtraction respectively
+        This function returns the flux of of a star at specified `position`
+        using `radius` as radius of extraction. Note that this returns a
+        three-tuple where the first, second, and third element correspond to
+        total star flux, background flux and star flux after background
+        subtraction respectively
         """
-        # x_exact, y_exact = position
+        # Since we always want a star to fall to the same sky background box, we
+        # calculate which star box it falls into by taking the position from the
+        # reference file not its weighted X, weighted Y that might change.
+
+        # A better method would be to take the average of surrounding boxes
+        # instead because if the sky background noise gets improved because of
+        # equipment change, we'll see a step in new data because of how
+        # difference of much background we were subtracting previously vs now.
+
+        # Note that the reason y, x are reversed is because our x, y in image
+        # data matrix and in the reference file are flipped.
         y_exact, x_exact = ref.get_star_xy(star_no)
 
-        # Mimic IDL floor
-        x, y = np.round(position).astype("int")
+        # IDL like round
+        x, y = position
+        x, y = half_round_up_to_int(x), half_round_up_to_int(y)
+
         starBox = image_data[x - radius : x + radius + 1, y - radius : y + radius + 1]
         starBox = np.multiply(starBox, circleMatrix(radius))
         backgroundAverageInStarRegion = sky_backgrounds[
             (x_exact // regionSize, y_exact // regionSize)
         ]
         subtractedStarFlux = np.sum(starBox) - backgroundAverageInStarRegion * pixelsPerStar
```

### Comparing `m23-1.3.0/src/m23/file/__init__.py` & `m23-1.3.1/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/aligned_combined_file.py` & `m23-1.3.1/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/alignment_stats_file.py` & `m23-1.3.1/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/color_normalized_file.py` & `m23-1.3.1/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/flux_log_combined_file.py` & `m23-1.3.1/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/log_file_combined_file.py` & `m23-1.3.1/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/masterflat_file.py` & `m23-1.3.1/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/normfactor_file.py` & `m23-1.3.1/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/raw_image_file.py` & `m23-1.3.1/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/reference_log_file.py` & `m23-1.3.1/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/ri_color_file.py` & `m23-1.3.1/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/file/sky_bg_file.py` & `m23-1.3.1/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/internight_normalize/__init__.py` & `m23-1.3.1/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/matrix/fill.py` & `m23-1.3.1/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/norm/__init__.py` & `m23-1.3.1/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/norm/get_line.py` & `m23-1.3.1/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/processor/config_loader.py` & `m23-1.3.1/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/processor/generate_masterflat.py` & `m23-1.3.1/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.3.1/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/processor/nights_csv.py` & `m23-1.3.1/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/processor/nights_csv_config_loader.py` & `m23-1.3.1/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/processor/process_nights.py` & `m23-1.3.1/src/m23/processor/process_nights.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,26 +411,26 @@
                 aligned_images_data.append(aligned_data)
                 # We add the transformation statistics to the alignment stats
                 # file Information of the file that can't be aligned isn't
                 # written only in the logfile. This is intended so that we can
                 # easily process the alignment stats file if we keep it in a TSV
                 # like format
 
-                # Note that we're down-scaling the matrix dtype from float to int16 for
+                # Note that we're down-scaling the matrix dtype from float to int32 for
                 # support in the image viewing softwares. For the combination step though
                 # we are using the more precise float data. This means that if you read
                 # the data of the aligned images from the fit file and combined them yourself
                 # that is going to be off by a small amount that the data in the aligned
                 # combined image.
                 aligned_image = RawImageFile(
                     JUST_ALIGNED_NOT_COMBINED_OUTPUT_FOLDER / raw_image_to_align_name
                 )
 
                 if save_aligned_images:
-                    aligned_image.create_file(aligned_data.astype("int16"), raw_image_to_align)
+                    aligned_image.create_file(aligned_data.astype("int32"), raw_image_to_align)
 
                 alignment_stats_file.add_record(raw_image_to_align_name, statistics)
                 logger.info(f"Aligned {raw_image_to_align_name}")
             except CouldNotAlignException:
                 logger.error(f"Could not align image {raw_image_to_align}")
                 logger.error(f"Skipping combination {from_index}-{to_index}")
                 break
@@ -456,18 +456,15 @@
         )
         aligned_combined_file = AlignedCombinedFile(
             ALIGNED_COMBINED_OUTPUT_FOLDER / aligned_combined_file_name
         )
         # Image viewing softwares like Astromagic and Fits Liberator don't work
         # if the image data type is float, for some reason that we don't know.
         # So we're setting the datatype to int32 which has enough precision for
-        # us. Note int16 is problematic as our combined images ADU are bigger
-        # than 2^16
-        # Note that for extraction though, we use the same, more precise format
-        # that we have
+        # us.
         aligned_combined_file.create_file(
             combined_images_data.astype("int32"), sample_raw_image_file
         )
         logger.info(f"Combined images {from_index}-{to_index}")
 
         # Extraction
         log_file_combined_file_name = LogFileCombinedFile.generate_file_name(
```

### Comparing `m23-1.3.0/src/m23/processor/renormalize.py` & `m23-1.3.1/src/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/processor/renormalize_config_loader.py` & `m23-1.3.1/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/reference/MeanRI100.txt` & `m23-1.3.1/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/reference/README.md` & `m23-1.3.1/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/reference/ref_revised_71.txt` & `m23-1.3.1/src/m23/reference/ref_revised_71.txt`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/sky/__init__.py` & `m23-1.3.1/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/sky/moon/__init__.py` & `m23-1.3.1/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/utils/__init__.py` & `m23-1.3.1/src/m23/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,40 +170,37 @@
     if len(arr) % 2 == 0:
         newArray = np.append(arr, [np.multiply(np.ones(arr[0].shape), np.max(arr))], axis=0)
         return np.median(newArray, *args, **kwargs)
     else:
         return np.median(arr, *args, **kwargs)
 
 
-def sorted_by_number(lst : Iterable[Union[str, Path]]) -> Iterable[Union[str, Path]]:
+def sorted_by_number(lst: Iterable[Union[str, Path]]) -> Iterable[Union[str, Path]]:
     """
     Returns sorted list of `lst` where sorting is done in ascending order by the
     the first number present in the string. If no string is present, falls back
-    to alphabetic sorting 
+    to alphabetic sorting
     """
     # Note that this step is important if the `lst` passed is a generator
     # This is because, after we've read it once, it would be empty
     lst = list(lst)
     if not all([isinstance(x, str) or isinstance(x, Path) for x in lst]):
         raise ValueError("items of list must be either str or Path instance")
     # Get filename if path objects are given
     lst_path_normalized = [x if isinstance(x, str) else x.name for x in lst]
     # Sort by alphabet (secondary)
     alphabet_sorted = sorted(enumerate(lst_path_normalized), key=lambda x: x[1])
-    # Sort by first number present in the 
-    MATCHER = re.compile(r'\D*(\d*).*')
-    foo = zip(*list(sorted(alphabet_sorted, 
-           key= lambda x: int(MATCHER.match(x[1])[1] or 0)
-           )))
+    # Sort by first number present in the
+    MATCHER = re.compile(r"\D*(\d*).*")
+    foo = zip(*list(sorted(alphabet_sorted, key=lambda x: int(MATCHER.match(x[1])[1] or 0))))
     indices, _ = foo
     return [lst[i] for i in indices]
 
 
-
 __all__ = [
     "customMedian",
     "fitFilesInFolder",
     "rename",
     "get_closet_date",
     "raw_data_name_format",
-    "sorted_by_number"
+    "sorted_by_number",
 ]
```

### Comparing `m23-1.3.0/src/m23/utils/date.py` & `m23-1.3.1/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/src/m23/utils/rename.py` & `m23-1.3.1/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/.gitignore` & `m23-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/README.md` & `m23-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.3.0/pyproject.toml` & `m23-1.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.3.0"
+version = "1.3.1"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.3.0/PKG-INFO` & `m23-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.3.0
+Version: 1.3.1
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: numpy==1.24.2
 Requires-Dist: opencv-python==4.7.0.68
```

