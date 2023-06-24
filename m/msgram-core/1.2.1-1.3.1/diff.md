# Comparing `tmp/msgram_core-1.2.1.tar.gz` & `tmp/msgram_core-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram_core-1.2.1.tar", last modified: Tue Jun 13 23:39:57 2023, max compression
+gzip compressed data, was "msgram_core-1.3.1.tar", last modified: Sat Jun 24 19:59:32 2023, max compression
```

## Comparing `msgram_core-1.2.1.tar` & `msgram_core-1.3.1.tar`

### file list

```diff
@@ -1,41 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.525076 msgram_core-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-06-13 23:39:33.000000 msgram_core-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-06-13 23:39:57.525076 msgram_core-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-13 23:39:33.000000 msgram_core-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-13 23:39:33.000000 msgram_core-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:39:57.525076 msgram_core-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.517076 msgram_core-1.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.521076 msgram_core-1.2.1/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/agregation.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/interpretation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/measures_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/core/weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.521076 msgram_core-1.2.1/src/msgram_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-06-13 23:39:57.000000 msgram_core-1.2.1/src/msgram_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-13 23:39:57.000000 msgram_core-1.2.1/src/msgram_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:39:57.000000 msgram_core-1.2.1/src/msgram_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 23:39:57.000000 msgram_core-1.2.1/src/msgram_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 23:39:57.000000 msgram_core-1.2.1/src/msgram_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.521076 msgram_core-1.2.1/src/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/parsers/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.521076 msgram_core-1.2.1/src/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/resources/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.521076 msgram_core-1.2.1/src/staticfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/staticfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/staticfiles/default_pre_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/staticfiles/sonarqube_available_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/staticfiles/sonarqube_supported_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.525076 msgram_core-1.2.1/src/util/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/util/check_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 23:39:33.000000 msgram_core-1.2.1/src/util/get_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:39:57.525076 msgram_core-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-13 23:39:33.000000 msgram_core-1.2.1/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.770504 msgram_core-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-06-24 19:59:13.000000 msgram_core-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-06-24 19:59:32.770504 msgram_core-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-24 19:59:13.000000 msgram_core-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-24 19:59:13.000000 msgram_core-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:59:32.770504 msgram_core-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.766504 msgram_core-1.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.766504 msgram_core-1.3.1/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/core/aggregated_normalized_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/core/measures_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/core/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.766504 msgram_core-1.3.1/src/msgram_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-06-24 19:59:32.000000 msgram_core-1.3.1/src/msgram_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-24 19:59:32.000000 msgram_core-1.3.1/src/msgram_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:59:32.000000 msgram_core-1.3.1/src/msgram_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 19:59:32.000000 msgram_core-1.3.1/src/msgram_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 19:59:32.000000 msgram_core-1.3.1/src/msgram_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.766504 msgram_core-1.3.1/src/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/parsers/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.770504 msgram_core-1.3.1/src/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/resources/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.770504 msgram_core-1.3.1/src/staticfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/staticfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/staticfiles/default_pre_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/staticfiles/sonarqube_available_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/staticfiles/sonarqube_supported_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.770504 msgram_core-1.3.1/src/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/util/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/util/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.770504 msgram_core-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-24 19:59:13.000000 msgram_core-1.3.1/tests/test_helpers.py
```

### Comparing `msgram_core-1.2.1/LICENSE` & `msgram_core-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.1/PKG-INFO` & `msgram_core-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram_core
-Version: 1.2.1
+Version: 1.3.1
 Summary: The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram_core-1.2.1/README.md` & `msgram_core-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.1/src/core/schemas.py` & `msgram_core-1.3.1/src/core/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,39 +106,39 @@
         ]
     }
     """
 
     characteristics = fields.List(fields.Nested(CharacteristicSchema), required=True)
 
 
-class SQCSchema(Schema):
+class TSQMISchema(Schema):
     key = fields.Str(required=True)
     characteristics = fields.List(
         fields.Nested(CalculatedSubEntitySchema), required=True
     )
 
 
-class CalculateSQCSchema(Schema):
+class CalculateTSQMISchema(Schema):
     """
     {
-        "sqc": {
-            "key": "sqc",
+        "tsqmi": {
+            "key": "tsqmi",
             "characteristics": [
                 {
                     "key": "reliability",
                     "value": 1.0,
                     "weight": 50,
                 },
                 ...
             ]
         }
     }
     """
 
-    sqc = fields.Nested(SQCSchema, required=True)
+    tsqmi = fields.Nested(TSQMISchema, required=True)
 
 
 class NonComplexFileDensitySchema(Schema):
     """
     "key": "non_complex_file_density",
     "function": calculate_em1
     """
```

### Comparing `msgram_core-1.2.1/src/msgram_core.egg-info/PKG-INFO` & `msgram_core-1.3.1/src/msgram_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-core
-Version: 1.2.1
+Version: 1.3.1
 Summary: The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram_core-1.2.1/src/msgram_core.egg-info/SOURCES.txt` & `msgram_core-1.3.1/src/msgram_core.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
 src/__init__.py
 src/core/__init__.py
-src/core/agregation.py
-src/core/dataframe.py
-src/core/interpretation_functions.py
+src/core/aggregated_normalized_measures.py
 src/core/measures_functions.py
 src/core/schemas.py
-src/core/weighting.py
+src/core/transformations.py
 src/msgram_core.egg-info/PKG-INFO
 src/msgram_core.egg-info/SOURCES.txt
 src/msgram_core.egg-info/dependency_links.txt
 src/msgram_core.egg-info/requires.txt
 src/msgram_core.egg-info/top_level.txt
 src/parsers/__init__.py
 src/parsers/sonarqube.py
 src/resources/__init__.py
 src/resources/analysis.py
 src/staticfiles/__init__.py
 src/staticfiles/default_pre_config.py
 src/staticfiles/sonarqube_available_metrics.py
 src/staticfiles/sonarqube_supported_metrics.py
 src/util/__init__.py
-src/util/check_functions.py
+src/util/check.py
 src/util/constants.py
 src/util/exceptions.py
-src/util/get_functions.py
 tests/test_helpers.py
```

### Comparing `msgram_core-1.2.1/src/parsers/sonarqube.py` & `msgram_core-1.3.1/src/parsers/sonarqube.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,15 @@
-import os
-
-import requests
-
 from staticfiles import SONARQUBE_AVAILABLE_METRICS, SONARQUBE_SUPPORTED_MEASURES
 
 
 class Sonarqube:
-    def __init__(self):
-        self.endpoint = os.getenv(
-            "SONAR_URL", "https://sonarcloud.io/api/metrics/search"
-        )
-
-    def extract_supported_metrics(self, metrics, first_request=False):
+    def extract_supported_metrics(self, metrics):
         data = SONARQUBE_AVAILABLE_METRICS
 
-        if not first_request:
-            return self.__extract_sonarqube_supported_metrics(metrics, data)
-
-        try:
-            request = requests.get(self.endpoint)
-            data = request.json() if request.ok else SONARQUBE_AVAILABLE_METRICS
-
-        except Exception:
-            data = SONARQUBE_AVAILABLE_METRICS
-
-        finally:
-            return self.__extract_sonarqube_supported_metrics(metrics, data)
+        return self.__extract_sonarqube_supported_metrics(metrics, data)
 
     def __extract_sonarqube_supported_metrics(self, metrics, sonar_metrics):
         collected_metrics = {}
         supported_metrics = []
 
         # NOTE: list comprehension que preenche o supported_metrics apenas
         #       com os valores das "metrics" do dicionário de SUPPORTEDs
```

### Comparing `msgram_core-1.2.1/src/resources/analysis.py` & `msgram_core-1.3.1/src/resources/analysis.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,186 +1,195 @@
-import requests
+import numpy as np
 from marshmallow.exceptions import ValidationError
 
 from core.schemas import (
+    CalculateCharacteristicSchema,
     CalculateMeasureSchema,
     CalculateSubCharacteristicSchema,
-    CalculateCharacteristicSchema,
-    CalculateSQCSchema,
+    CalculateTSQMISchema,
 )
-from core.agregation import aggregation_operation
-from core.weighting import weighting_operation
-from util.constants import MEASURES_INTERPRETATION_MAPPING
-
-
-def calculate_aggregated_value(values_list, weights_list):
-    weighted_items = weighting_operation(values_list, weights_list)
-    return aggregation_operation(weighted_items, weights_list)
+from core.transformations import calculate_aggregated_weighted_value
+from util.constants import AGGREGATED_NORMALIZED_MEASURES_MAPPING
+from util.exceptions import MeasureKeyNotSupported
 
 
 def calculate_measures(
-    extracted_measures,
+    extracted_measures: CalculateMeasureSchema,
     config: dict = {
         "characteristics": [{"subcharacteristics": [{"measures": [{"key": ""}]}]}]
     },
 ):
     # Validate if outter keys is valid
     try:
         data = CalculateMeasureSchema().load(extracted_measures)
     except ValidationError as error:
-        return {
-            "error": "Failed to validate request",
-            "schema_errors": error.messages,
-            "code": requests.codes.unprocessable_entity,
-        }
+        raise ValidationError(
+            f"error: Failed to validate input.\nschema_errors: {error.messages}"
+        )
 
     # Objeto retornado em caso de sucesso
-    response_data = {"measures": []}
+    result_data = {"measures": []}
 
-    valid_measures = MEASURES_INTERPRETATION_MAPPING.keys()
+    valid_measures = AGGREGATED_NORMALIZED_MEASURES_MAPPING.keys()
 
     for measure in data["measures"]:
         measure_key: str = measure["key"]
 
         if measure_key not in valid_measures:
-            return {
-                "error": f"Measure {measure_key} is not supported",
-                "code": requests.codes.unprocessable_entity,
-            }
+            raise MeasureKeyNotSupported(f"Measure {measure_key} is not supported")
 
         measure_params = measure["parameters"]
-        schema = MEASURES_INTERPRETATION_MAPPING[measure_key]["schema"]
+        schema = AGGREGATED_NORMALIZED_MEASURES_MAPPING[measure_key]["schema"]
 
         try:
             validated_params = schema().load(measure_params)
         except ValidationError as exc:
-            return {
-                "error": f"Metric parameters {measure_key} are not valid",
-                "schema_errors": exc.messages,
-                "code": requests.codes.unprocessable_entity,
-            }
-
-        interpretation_function = MEASURES_INTERPRETATION_MAPPING[measure_key][
-            "interpretation_function"
-        ]
+            raise ValidationError(
+                f"error: Metric parameters {measure_key} are not valid.\nschema_errors: {exc.messages}"
+            )
+
+        aggregated_normalized_measure = AGGREGATED_NORMALIZED_MEASURES_MAPPING[
+            measure_key
+        ]["aggregated_normalized_measure"]
 
         measures = [
             measure
             for characteristic in config["characteristics"]
             for subcharacteristic in characteristic["subcharacteristics"]
             for measure in subcharacteristic["measures"]
         ]
 
         threshold_config = {
             key: value
             for measure in measures
             for key, value in measure.items()
             if measure["key"] == measure_key
-            and key in MEASURES_INTERPRETATION_MAPPING[measure_key]["thresholds"]
+            and key in AGGREGATED_NORMALIZED_MEASURES_MAPPING[measure_key]["thresholds"]
         }
 
-        result = interpretation_function(validated_params, **threshold_config)
+        result = aggregated_normalized_measure(validated_params, **threshold_config)
 
-        response_data["measures"].append(
+        result_data["measures"].append(
             {
                 "key": measure_key,
                 "value": result,
             }
         )
 
-    return response_data
+    return result_data
 
 
 def calculate_subcharacteristics(extracted_subcharacteristics):
     try:
         data = CalculateSubCharacteristicSchema().load(extracted_subcharacteristics)
     except ValidationError as error:
-        return {
-            "error": "Failed to validate request",
-            "schema_errors": error.messages,
-            "code": requests.codes.unprocessable_entity,
-        }
+        raise ValidationError(
+            f"error: Failed to validate input.\nschema_errors: {error.messages}"
+        )
 
-    response_data = {"subcharacteristics": []}
+    result_data = {"subcharacteristics": []}
 
     for subcharacteristic in data["subcharacteristics"]:
         subcharacteristic_key: str = subcharacteristic["key"]
 
-        values_list, weights_list = [], []
-        for measure in subcharacteristic["measures"]:
-            values_list.append(measure["value"])
-            weights_list.append(measure["weight"])
+        vector_aggregated_normalized_measure = np.array([])
+        vector_weight_aggregated_normalized_measure = np.array([])
 
-        aggregated_value = calculate_aggregated_value(values_list, weights_list)
+        for measure in subcharacteristic["measures"]:
+            vector_aggregated_normalized_measure = np.append(
+                vector_aggregated_normalized_measure, measure["value"]
+            )
+            vector_weight_aggregated_normalized_measure = np.append(
+                vector_weight_aggregated_normalized_measure, measure["weight"]
+            )
+        aggregated_value = calculate_aggregated_weighted_value(
+            vector_aggregated_normalized_measure,
+            vector_weight_aggregated_normalized_measure,
+        )
 
-        response_data["subcharacteristics"].append(
+        result_data["subcharacteristics"].append(
             {
                 "key": subcharacteristic_key,
                 "value": aggregated_value,
             }
         )
 
-    return response_data
+    return result_data
 
 
 def calculate_characteristics(extracted_characteristics):
     try:
         data = CalculateCharacteristicSchema().load(extracted_characteristics)
     except ValidationError as error:
-        return {
-            "error": "Failed to validate request",
-            "schema_errors": error.messages,
-            "code": requests.codes.unprocessable_entity,
-        }
+        raise ValidationError(
+            f"error: Failed to validate input.\nschema_errors: {error.messages}"
+        )
 
-    response_data = {"characteristics": []}
+    result_data = {"characteristics": []}
 
     for characteristic in data["characteristics"]:
         characteristic_key: str = characteristic["key"]
 
-        values_list, weights_list = [], []
-        for measure in characteristic["subcharacteristics"]:
-            values_list.append(measure["value"])
-            weights_list.append(measure["weight"])
-
-        aggregated_value = calculate_aggregated_value(values_list, weights_list)
+        vector_aggregated_normalized_subcharacteristics = np.array([])
+        vector_weight_aggregated_normalized_subcharacteristics = np.array([])
+        for subcharacteristics in characteristic["subcharacteristics"]:
+            vector_aggregated_normalized_subcharacteristics = np.append(
+                vector_aggregated_normalized_subcharacteristics,
+                subcharacteristics["value"],
+            )
+            vector_weight_aggregated_normalized_subcharacteristics = np.append(
+                vector_weight_aggregated_normalized_subcharacteristics,
+                subcharacteristics["weight"],
+            )
+
+        aggregated_value = calculate_aggregated_weighted_value(
+            vector_aggregated_normalized_subcharacteristics,
+            vector_weight_aggregated_normalized_subcharacteristics,
+        )
 
-        response_data["characteristics"].append(
+        result_data["characteristics"].append(
             {
                 "key": characteristic_key,
                 "value": aggregated_value,
             }
         )
 
-    return response_data
+    return result_data
 
 
-def calculate_sqc(extracted_sqc):
+def calculate_tsqmi(extracted_tsqmi):
     try:
-        data = CalculateSQCSchema().load(extracted_sqc)
+        data = CalculateTSQMISchema().load(extracted_tsqmi)
     except ValidationError as error:
-        return {
-            "error": "Failed to validate request",
-            "schema_errors": error.messages,
-            "code": requests.codes.unprocessable_entity,
-        }
+        raise ValidationError(
+            f"error: Failed to validate input.\nschema_errors: {error.messages}"
+        )
 
-    response_data = {"sqc": []}
+    result_data = {"tsqmi": []}
 
-    sqc = data["sqc"]
-    sqc_key: str = sqc["key"]
+    tsqmi = data["tsqmi"]
+    tsqmi_key: str = tsqmi["key"]
 
-    values_list, weights_list = [], []
-    for characteristic in sqc["characteristics"]:
-        values_list.append(characteristic["value"])
-        weights_list.append(characteristic["weight"])
+    vector_aggregated_normalized_characteristics = np.array([])
+    vector_weight_aggregated_normalized_characteristics = np.array([])
+    for characteristic in tsqmi["characteristics"]:
+        vector_aggregated_normalized_characteristics = np.append(
+            vector_aggregated_normalized_characteristics, characteristic["value"]
+        )
+        vector_weight_aggregated_normalized_characteristics = np.append(
+            vector_weight_aggregated_normalized_characteristics,
+            characteristic["weight"],
+        )
 
-    aggregated_value = calculate_aggregated_value(values_list, weights_list)
+    aggregated_value = calculate_aggregated_weighted_value(
+        vector_aggregated_normalized_characteristics,
+        vector_weight_aggregated_normalized_characteristics,
+    )
 
-    response_data["sqc"].append(
+    result_data["tsqmi"].append(
         {
-            "key": sqc_key,
+            "key": tsqmi_key,
             "value": aggregated_value,
         }
     )
 
-    return response_data
+    return result_data
```

### Comparing `msgram_core-1.2.1/src/staticfiles/default_pre_config.py` & `msgram_core-1.3.1/src/staticfiles/default_pre_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                             "min_fast_test_time": 0,
                             "max_fast_test_time": 300000,
                         },
                         {
                             "key": "test_coverage",
                             "weight": 34,
                             "min_coverage": 60,
-                            "max_coverage": 90,
+                            "max_coverage": 100,
                         },
                     ],
                 }
             ],
         },
         {
             "key": "maintainability",
```

### Comparing `msgram_core-1.2.1/src/staticfiles/sonarqube_available_metrics.py` & `msgram_core-1.3.1/src/staticfiles/sonarqube_available_metrics.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.1/src/staticfiles/sonarqube_supported_metrics.py` & `msgram_core-1.3.1/src/staticfiles/sonarqube_supported_metrics.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.2.1/src/util/constants.py` & `msgram_core-1.3.1/src/util/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import core.measures_functions as ems_functions
 from core import schemas
-from core.interpretation_functions import (
+from core.aggregated_normalized_measures import (
     absence_of_duplications,
     commented_files_density,
     fast_test_builds,
     non_complex_files_density,
     passed_tests,
     test_coverage,
 )
@@ -94,52 +93,44 @@
                 "number_of_resolved_issues_with_US_label_in_the_last_x_days",
                 "total_number_of_issues_with_US_label_in_the_last_x_days",
             ],
         },
     },
 }
 
-
-MEASURES_INTERPRETATION_MAPPING = {
+AGGREGATED_NORMALIZED_MEASURES_MAPPING = {
     "non_complex_file_density": {
-        "interpretation_function": non_complex_files_density,
-        "calculation_function": ems_functions.calculate_em1,
+        "aggregated_normalized_measure": non_complex_files_density,
         "schema": schemas.NonComplexFileDensitySchema,
         "thresholds": ["min_complex_files_density", "max_complex_files_density"],
     },
     "commented_file_density": {
-        "interpretation_function": commented_files_density,
-        "calculation_function": ems_functions.calculate_em2,
+        "aggregated_normalized_measure": commented_files_density,
         "schema": schemas.CommentedFileDensitySchema,
         "thresholds": ["min_comment_density", "max_comment_density"],
     },
     "duplication_absense": {
-        "interpretation_function": absence_of_duplications,
-        "calculation_function": ems_functions.calculate_em3,
+        "aggregated_normalized_measure": absence_of_duplications,
         "schema": schemas.DuplicationAbsenceSchema,
         "thresholds": ["min_duplicated_lines", "max_duplicated_lines"],
     },
     "passed_tests": {
-        "interpretation_function": passed_tests,
-        "calculation_function": ems_functions.calculate_em4,
+        "aggregated_normalized_measure": passed_tests,
         "schema": schemas.PassedTestsSchema,
         "thresholds": ["min_passed_tests", "max_passed_tests"],
     },
     "test_builds": {
-        "interpretation_function": fast_test_builds,
-        "calculation_function": ems_functions.calculate_em5,
+        "aggregated_normalized_measure": fast_test_builds,
         "schema": schemas.TestBuildsSchema,
         "thresholds": ["min_fast_test_time", "max_fast_test_time"],
     },
     "test_coverage": {
-        "interpretation_function": test_coverage,
-        "calculation_function": ems_functions.calculate_em6,
+        "aggregated_normalized_measure": test_coverage,
         "schema": schemas.TestCoverageSchema,
         "thresholds": ["min_coverage", "max_coverage"],
     },
     "team_throughput": {
-        "interpretation_function": ...,
-        "calculation_function": ems_functions.calculate_em7,
+        "aggregated_normalized_measure": ...,
         "schema": schemas.TeamThroughputSchema,
         "thresholds": [],
     },
 }
```

### Comparing `msgram_core-1.2.1/src/util/exceptions.py` & `msgram_core-1.3.1/src/util/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -31,7 +31,31 @@
     pass
 
 
 class InvalidThresholdValue(MeasureSoftGramCoreException):
     """Raised when a invalid threshold value is provided to the interpretation function"""
 
     pass
+
+
+class InvalidGainInterpretationValue(MeasureSoftGramCoreException):
+    """Raised when a invalid gain interpretation value is provided to the interpretation function"""
+
+    pass
+
+
+class InvalidCheckThreshold(MeasureSoftGramCoreException):
+    """Raised when a invalid check threshold function is called"""
+
+    pass
+
+
+class MeasureKeyNotSupported(MeasureSoftGramCoreException):
+    """Raised when a measure key is not supported"""
+
+    pass
+
+
+class ReleasePlannedAndDevelopedOfDifferentSizes(MeasureSoftGramCoreException):
+    """Raised when the sizes of the planned and developed release vectors are different"""
+
+    pass
```

### Comparing `msgram_core-1.2.1/tests/test_helpers.py` & `msgram_core-1.3.1/tests/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,59 +15,53 @@
     "test_failures",
     "test_execution_time",
     "security_rating",
 ]
 
 
 def read_json(json_path):
-
     with open(json_path) as json_file:
         json_obj = json.load(json_file)
 
     return json_obj
 
 
 def create_base_component_df(json_list):
-
     df = pd.DataFrame()
 
     for i in json_list:
-
         base_component = read_json(i)
 
         base_component_data = base_component["baseComponent"]["measures"]
 
         base_component_df = pd.DataFrame(base_component_data)
 
         base_component_df["filename"] = os.path.basename(i)
 
         df = pd.concat([df, base_component_df], ignore_index=True)
 
     return df
 
 
 def metric_per_file(json):
-
     file_json = []
 
     for component in json["components"]:
         file_json.append(component)
 
     return file_json
 
 
 def check_component_is_valid(component, language_extension):
-
     return (
         component["qualifier"] == "DIR" or component["language"] == language_extension
     )
 
 
 def generate_file_dataframe_per_release(metric_list, json, language_extension):
-
     df_columns = metric_list + ["qualifier"]
     df = pd.DataFrame(columns=df_columns)
 
     for file in json:
         if check_component_is_valid(file, language_extension):
             df.at[file["path"], "qualifier"] = file["qualifier"]
             for measure in file["measures"]:
@@ -76,19 +70,17 @@
     df.reset_index(inplace=True)
     df = df.rename({"index": "path"}, axis=1).drop(["files"], axis=1)
 
     return df
 
 
 def create_file_df(json_list, language_extension="js"):
-
     df = pd.DataFrame()
 
     for json_file in json_list:
-
         file_component = read_json(json_file)
 
         file_component_data = metric_per_file(file_component)
 
         file_component_df = generate_file_dataframe_per_release(
             METRICS_LIST, file_component_data, language_extension=language_extension
         )
```

