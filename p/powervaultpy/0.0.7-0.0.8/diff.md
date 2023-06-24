# Comparing `tmp/powervaultpy-0.0.7.tar.gz` & `tmp/powervaultpy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powervaultpy-0.0.7.tar", last modified: Wed Jun 21 23:05:04 2023, max compression
+gzip compressed data, was "powervaultpy-0.0.8.tar", last modified: Sat Jun 24 17:02:45 2023, max compression
```

## Comparing `powervaultpy-0.0.7.tar` & `powervaultpy-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 23:05:04.324443 powervaultpy-0.0.7/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-06-21 23:05:04.324443 powervaultpy-0.0.7/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1478 2023-06-21 23:04:45.000000 powervaultpy-0.0.7/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-21 23:05:04.324443 powervaultpy-0.0.7/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 23:05:04.323443 powervaultpy-0.0.7/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 23:05:04.323443 powervaultpy-0.0.7/src/powervaultpy/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       63 2023-06-21 22:09:08.000000 powervaultpy-0.0.7/src/powervaultpy/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9040 2023-06-21 23:03:12.000000 powervaultpy-0.0.7/src/powervaultpy/powervault.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 23:05:04.324443 powervaultpy-0.0.7/src/powervaultpy.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-06-21 23:05:04.000000 powervaultpy-0.0.7/src/powervaultpy.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      273 2023-06-21 23:05:04.000000 powervaultpy-0.0.7/src/powervaultpy.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-21 23:05:04.000000 powervaultpy-0.0.7/src/powervaultpy.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       99 2023-06-21 23:05:04.000000 powervaultpy-0.0.7/src/powervaultpy.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       13 2023-06-21 23:05:04.000000 powervaultpy-0.0.7/src/powervaultpy.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-24 17:02:45.902410 powervaultpy-0.0.8/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-06-24 17:02:45.902410 powervaultpy-0.0.8/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1478 2023-06-24 17:02:39.000000 powervaultpy-0.0.8/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-24 17:02:45.902410 powervaultpy-0.0.8/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-24 17:02:45.901410 powervaultpy-0.0.8/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-24 17:02:45.901410 powervaultpy-0.0.8/src/powervaultpy/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       63 2023-06-21 22:09:08.000000 powervaultpy-0.0.8/src/powervaultpy/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9918 2023-06-24 16:47:49.000000 powervaultpy-0.0.8/src/powervaultpy/powervault.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-24 17:02:45.902410 powervaultpy-0.0.8/src/powervaultpy.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-06-24 17:02:45.000000 powervaultpy-0.0.8/src/powervaultpy.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      273 2023-06-24 17:02:45.000000 powervaultpy-0.0.8/src/powervaultpy.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-24 17:02:45.000000 powervaultpy-0.0.8/src/powervaultpy.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       99 2023-06-24 17:02:45.000000 powervaultpy-0.0.8/src/powervaultpy.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       13 2023-06-24 17:02:45.000000 powervaultpy-0.0.8/src/powervaultpy.egg-info/top_level.txt
```

### Comparing `powervaultpy-0.0.7/PKG-INFO` & `powervaultpy-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powervaultpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: An integration to control the Powervault battery
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/powervaultpy
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/powervaultpy/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/powervaultpy/blob/main/CHANGELOG.md
 Keywords: powervault,home,automation
```

### Comparing `powervaultpy-0.0.7/pyproject.toml` & `powervaultpy-0.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "powervaultpy"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Adam McDonagh", email="adam@elitemonkey.net" },
 ]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `powervaultpy-0.0.7/src/powervaultpy/powervault.py` & `powervaultpy-0.0.8/src/powervaultpy/powervault.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,14 +140,38 @@
         _LOGGER.debug("Data: %s", data_response)
 
         if (data_response is not None) and ("data" in data_response):
             return data_response["data"]
 
         _LOGGER.error("Failed to retrieve data")
 
+    def get_kwh(self, data: dict) -> dict:
+        # List of attributes to retrieve from data dict
+        attributes = [
+            "batteryInputFromGrid",
+            "batteryInputFromSolar",
+            "batteryOutputConsumedByHome",
+            "batteryOutputExported",
+            "homeConsumed",
+            "gridConsumedByHome",
+            "solarConsumedByHome",
+            "solarExported",
+            "solarGenerated",
+        ]
+        # For each attribute, loop through the data dict and conver the W reading to kWh over the 5 minute period
+        totals = {}
+        for row in data:
+            for attribute in attributes:
+                if attribute in row:
+                    if attribute not in totals:
+                        totals[attribute] = 0
+                    totals[attribute] += round(row[attribute] / 1000 * (5/60), 2)
+
+        return totals
+
     def set_battery_state(self, unit_id: str, battery_state) -> bool:
         """Override the current battery status with the provided one."""
         url = f"{self._base_url}/unit/{unit_id}/stateOverride"
 
         start_time = datetime.now(pytz.timezone('UTC')).strftime("%Y-%m-%d %H:%M:%S")
         end_time = (datetime.now(pytz.timezone('UTC')) + timedelta(hours=24)).strftime("%Y-%m-%d %H:%M:%S")
```

### Comparing `powervaultpy-0.0.7/src/powervaultpy.egg-info/PKG-INFO` & `powervaultpy-0.0.8/src/powervaultpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powervaultpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: An integration to control the Powervault battery
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/powervaultpy
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/powervaultpy/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/powervaultpy/blob/main/CHANGELOG.md
 Keywords: powervault,home,automation
```

