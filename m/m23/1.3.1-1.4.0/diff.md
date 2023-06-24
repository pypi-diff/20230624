# Comparing `tmp/m23-1.3.1.tar.gz` & `tmp/m23-1.4.0.tar.gz`

## Comparing `m23-1.3.1.tar` & `m23-1.4.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.3.1/.flake8
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 m23-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.3.1/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.3.1/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.3.1/nights_csv.toml
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.3.1/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.3.1/renormalize.toml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.3.1/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.3.1/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 m23-1.3.1/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/matrix/utils.py
--rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/__init__.py
--rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    22109 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725377 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/reference/README.md
--rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/reference/ref_revised_71.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.3.1/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.3.1/.gitignore
--rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 m23-1.3.1/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 m23-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.4.0/.flake8
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 m23-1.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.4.0/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.4.0/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.4.0/nights_csv.toml
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.4.0/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.4.0/renormalize.toml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.4.0/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.4.0/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 m23-1.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    22194 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725377 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/reference/README.md
+-rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/reference/ref_revised_71.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.4.0/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.4.0/.gitignore
+-rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 m23-1.4.0/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 m23-1.4.0/PKG-INFO
```

### Comparing `m23-1.3.1/CHANGELOG.md` & `m23-1.4.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.4.0 (2023-06-24)
+
+### Feature
+
+* Add cols for first/last logfile used in sky bg file ([`7093c10`](https://github.com/LutherAstrophysics/m23/commit/7093c10bbcc3caa679c7c8e2f7e0448691027f5f))
+* Account for surrounding boxes in sky adu calc ([`bef88e6`](https://github.com/LutherAstrophysics/m23/commit/bef88e69c78fe56ac16c6ca1f40a59e286171149))
+
 ## v1.3.1 (2023-06-24)
 
 ### Fix
 
 * Use correct datatype when saving aligned images ([`386cf38`](https://github.com/LutherAstrophysics/m23/commit/386cf3854771c600dd785dfaf5c39962b4ae69c8))
 * Use IDL like round during extraction ([`2fc9c35`](https://github.com/LutherAstrophysics/m23/commit/2fc9c3546ad852e6e191a84e7a6589ebe4dc9530))
 * Allow sky bg to be 0 ([`6b98aa2`](https://github.com/LutherAstrophysics/m23/commit/6b98aa20acb2ba86831dd5b1f900b3a8f3f632bf))
```

### Comparing `m23-1.3.1/brown.toml` & `m23-1.4.0/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/mf.toml` & `m23-1.4.0/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/nights_csv.toml` & `m23-1.4.0/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/rainbow.toml` & `m23-1.4.0/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/requirements.txt` & `m23-1.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/.github/workflows/python-publish.yml` & `m23-1.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/.vscode/settings.json` & `m23-1.4.0/.vscode/settings.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984615384615385%*

 * *Differences: {"'cSpell.words'": "{insert: [(59, 'xweight'), (64, 'yweight')]}"}*

```diff
@@ -61,18 +61,20 @@
         "starttime",
         "tuti",
         "venv",
         "writeto",
         "XFWHM",
         "xlabel",
         "xlim",
+        "xweight",
         "yaspin",
         "YFWHM",
         "ylabel",
-        "ylim"
+        "ylim",
+        "yweight"
     ],
     "editor.formatOnSave": true,
     "files.associations": {
         "**/**/*.toml": "plaintext"
     },
     "isort.args": [
         "--profile",
```

### Comparing `m23-1.3.1/src/m23/__main__.py` & `m23-1.4.0/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/constants.py` & `m23-1.4.0/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/align/__init__.py` & `m23-1.4.0/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/calibrate/calibration.py` & `m23-1.4.0/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/calibrate/master_calibrate.py` & `m23-1.4.0/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/charts/__init__.py` & `m23-1.4.0/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/combine/__init__.py` & `m23-1.4.0/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/extract/__init__.py` & `m23-1.4.0/src/m23/extract/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 from functools import cache
-from typing import Tuple
+from typing import Dict, Iterable, Tuple
 
 import numpy as np
 import numpy.typing as npt
 
 from m23.constants import SKY_BG_BOX_REGION_SIZE
 from m23.file.aligned_combined_file import AlignedCombinedFile
 from m23.file.log_file_combined_file import LogFileCombinedFile
@@ -176,17 +176,19 @@
 
         # IDL like round
         x, y = position
         x, y = half_round_up_to_int(x), half_round_up_to_int(y)
 
         starBox = image_data[x - radius : x + radius + 1, y - radius : y + radius + 1]
         starBox = np.multiply(starBox, circleMatrix(radius))
-        backgroundAverageInStarRegion = sky_backgrounds[
-            (x_exact // regionSize, y_exact // regionSize)
-        ]
+
+        backgroundAverageInStarRegion = calculate_star_sky_adu(
+            ref.get_star_xy(star_no), sky_backgrounds, box_width=regionSize
+        )
+
         subtractedStarFlux = np.sum(starBox) - backgroundAverageInStarRegion * pixelsPerStar
 
         # Convert to zero, in case there's any nan.
         # This ensures that two log files correspond to same star number as they are
         # or after reading with something like getLinesWithNumbersFromFile
         # This step makes our normalization code faster than the reslife code written in IDL!
         return (
@@ -229,7 +231,69 @@
         ) * ((half_round_up_to_int(yweight) + axis) - yweight) ** 2
     col_sum = col_sum - (aduPerPixel * 11)
     row_sum = row_sum - (aduPerPixel * 11)
     xFWHM = 2.355 * np.sqrt(weighted_col_sum / (col_sum - 1))
     yFWHM = 2.355 * np.sqrt(weighted_row_sum / (row_sum - 1))
     average_FWHM = np.mean([xFWHM, yFWHM])
     return xFWHM, yFWHM, average_FWHM
+
+
+def get_star_background_boxes(
+    position_in_ref: Tuple[float, float], box_width: float
+) -> Iterable[Tuple[int, int]]:
+    """
+    Returns the sky background boxes that influence the star's brightness.
+    @param position_in_ref:
+        tuple of x, y position in the reference file. Important to provide position
+        in reference and not weighted as these boxes have to be the same for all nights
+    @param: width of the sky background box
+    returns list of box positions
+    """
+    threshold = 20
+    x, y = position_in_ref
+
+    # Use surrounding boxes for sky background calculation
+    b1 = x - threshold, y
+    b2 = x + threshold, y
+    b3 = x, y + threshold
+    b4 = x, y - threshold
+
+    # In order to use just the box that the star falls under for
+    # sky background, uncomment the followings:
+    # b1 = x, y
+    # b2 = x, y
+    # b3 = x, y
+    # b4 = x, y
+
+    boxes = []
+    for box in [b1, b2, b3, b4]:
+        bx, by = box
+        if bx < 0:
+            bx = 0
+        if bx >= 1024:
+            bx = 1023
+        if by < 0:
+            by = 0
+        if by >= 1024:
+            by = 1023
+        # Cols are assumed as X, rows Y by IDL convention
+        row = by // box_width
+        col = bx // box_width
+        boxes.append((row, col))
+    return boxes
+
+
+def calculate_star_sky_adu(
+    star_position_in_ref: Tuple[float, float],
+    sky_backgrounds: Dict[Tuple[int, int], float],
+    box_width: int,
+) -> float:
+    """
+    @param star_position_in_ref: x, y position of the star in ref
+    @sky_background: Average sky background per pixel in all different sky
+    background boxes
+
+    Return the average star background per pixel for the star
+    """
+    boxes = get_star_background_boxes(star_position_in_ref, box_width)
+    sky_bg_in_boxes = list(map(sky_backgrounds.get, boxes))
+    return np.mean(sky_bg_in_boxes)
```

### Comparing `m23-1.3.1/src/m23/file/__init__.py` & `m23-1.4.0/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/aligned_combined_file.py` & `m23-1.4.0/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/alignment_stats_file.py` & `m23-1.4.0/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/color_normalized_file.py` & `m23-1.4.0/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/flux_log_combined_file.py` & `m23-1.4.0/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/log_file_combined_file.py` & `m23-1.4.0/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/masterflat_file.py` & `m23-1.4.0/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/normfactor_file.py` & `m23-1.4.0/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/raw_image_file.py` & `m23-1.4.0/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/reference_log_file.py` & `m23-1.4.0/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/ri_color_file.py` & `m23-1.4.0/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/file/sky_bg_file.py` & `m23-1.4.0/src/m23/file/sky_bg_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     def create_file(
         self,
         sky_bg_data: SkyBGDataType,
         color_normfactors_title: Iterable[str],
         color_normfactors_values: Iterable[float],
         brightness_normfactors_title: Iterable[str],
         brightness_normfactors_values: Iterable[float],
+        first_img_number: int,
+        last_img_number: int,
     ):
         """
         Creates/Updates sky background file based on the `sky_bg_data`
         """
         if len(sky_bg_data) == 0:
             # Nothing to do
             with open(self.path(), "w") as fd:
@@ -79,14 +81,16 @@
         bg_sections = map(lambda x: "_".join(map(str, x)), sky_bg_data[0][1].keys())
         bg_sections_str = "".join(map("{:<10s}".format, bg_sections))
 
         with open(self.path(), "w") as fd:
             fd.write(
                 f"{'Date':<26s}"
                 f"{'Image_number':<15s}"
+                f"{'First_img':<15s}"  # Img number of the first logfile combined used
+                f"{'Last_img':<15s}"  # Img number of the last logfile combined used
                 f"{'Moon_Phase':<16s}"
                 f"{'Moon_Phase_Name':<20s}"
                 f"{'Cluster_Angle_Round':<20s}"
                 f"{'Cluster_Angle':<20s}"
                 f"{'Cluster_Angle_Uncertainty':<30s}"
                 f"{'Moon_Distance':<20s}"
                 f"{'Mean':<10s}{'Median':<10s}"
@@ -115,14 +119,16 @@
                 cluster_angle, cluster_angle_uncertainty = angle_of_elevation(
                     date_time_of_observation
                 )  # noqa
                 moon_dist_degrees = moon_distance(date_time_of_observation)
                 fd.write(
                     f"{night_datetime:<26s}"
                     f"{img_number:<15d}"
+                    f"{first_img_number:<15d}"
+                    f"{last_img_number:<15d}"
                     f"{moon_phase:<16.5f}"
                     f"{moon_phase_name:<20s}"
                     f"{np.round(cluster_angle):<20.0f}"
                     f"{cluster_angle:<20.1f}"
                     f"{cluster_angle_uncertainty:<30.1f}"
                     f"{moon_dist_degrees:<20.2f}"
                     f"{mean:<10.2f}{median:<10.2f}"
```

### Comparing `m23-1.3.1/src/m23/internight_normalize/__init__.py` & `m23-1.4.0/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/matrix/fill.py` & `m23-1.4.0/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/norm/__init__.py` & `m23-1.4.0/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/norm/get_line.py` & `m23-1.4.0/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/processor/config_loader.py` & `m23-1.4.0/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/processor/generate_masterflat.py` & `m23-1.4.0/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.4.0/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/processor/nights_csv.py` & `m23-1.4.0/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/processor/nights_csv_config_loader.py` & `m23-1.4.0/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/processor/process_nights.py` & `m23-1.4.0/src/m23/processor/process_nights.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,16 @@
 
     sky_bg_file.create_file(
         bg_data_of_all_images,
         color_normfactors_title,
         color_normfactors_values,
         brightness_normfactors_title,
         brightness_normfactors_values,
+        log_files_to_use[0].img_number(),
+        log_files_to_use[-1].img_number(),
     )
     logger.info("Completed generating sky background file")
 
 
 def get_datetime_to_use(
     aligned_combined: AlignedCombinedFile,
     night_config: ConfigInputNight,
```

### Comparing `m23-1.3.1/src/m23/processor/renormalize.py` & `m23-1.4.0/src/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/processor/renormalize_config_loader.py` & `m23-1.4.0/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.4.0/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/reference/MeanRI100.txt` & `m23-1.4.0/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/reference/README.md` & `m23-1.4.0/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/reference/ref_revised_71.txt` & `m23-1.4.0/src/m23/reference/ref_revised_71.txt`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/sky/__init__.py` & `m23-1.4.0/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/sky/moon/__init__.py` & `m23-1.4.0/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/utils/__init__.py` & `m23-1.4.0/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/utils/date.py` & `m23-1.4.0/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/src/m23/utils/rename.py` & `m23-1.4.0/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/.gitignore` & `m23-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/README.md` & `m23-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.3.1/pyproject.toml` & `m23-1.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.3.1"
+version = "1.4.0"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.3.1/PKG-INFO` & `m23-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.3.1
+Version: 1.4.0
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: numpy==1.24.2
 Requires-Dist: opencv-python==4.7.0.68
```

