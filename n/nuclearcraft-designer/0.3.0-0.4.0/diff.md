# Comparing `tmp/nuclearcraft_designer-0.3.0.tar.gz` & `tmp/nuclearcraft_designer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclearcraft_designer-0.3.0.tar", last modified: Sat Jun 24 01:29:32 2023, max compression
+gzip compressed data, was "nuclearcraft_designer-0.4.0.tar", last modified: Sat Jun 24 07:45:55 2023, max compression
```

## Comparing `nuclearcraft_designer-0.3.0.tar` & `nuclearcraft_designer-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 01:29:32.382717 nuclearcraft_designer-0.3.0/
--rw-r--r--   0 GerryMa    (501) staff       (20)     1067 2023-06-19 11:30:12.000000 nuclearcraft_designer-0.3.0/LICENSE
--rw-r--r--   0 GerryMa    (501) staff       (20)     3400 2023-06-24 01:29:32.382607 nuclearcraft_designer-0.3.0/PKG-INFO
--rw-r--r--   0 GerryMa    (501) staff       (20)     2837 2023-06-23 14:40:07.000000 nuclearcraft_designer-0.3.0/README.md
--rw-r--r--   0 GerryMa    (501) staff       (20)      637 2023-06-23 14:37:48.000000 nuclearcraft_designer-0.3.0/pyproject.toml
--rw-r--r--   0 GerryMa    (501) staff       (20)       38 2023-06-24 01:29:32.382761 nuclearcraft_designer-0.3.0/setup.cfg
-drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 01:29:32.378881 nuclearcraft_designer-0.3.0/src/
-drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 01:29:32.379624 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/
--rw-r--r--   0 GerryMa    (501) staff       (20)      102 2023-06-22 02:26:11.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/__init__.py
-drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 01:29:32.380233 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/
--rw-r--r--   0 GerryMa    (501) staff       (20)      114 2023-06-23 04:01:27.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/__init__.py
-drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 01:29:32.380941 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/
--rw-r--r--   0 GerryMa    (501) staff       (20)      136 2023-06-23 13:51:37.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/__init__.py
--rw-r--r--   0 GerryMa    (501) staff       (20)     6075 2023-06-23 14:11:29.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/beta_designer.py
--rw-r--r--   0 GerryMa    (501) staff       (20)     2445 2023-06-23 09:02:46.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/data_structures.py
--rw-r--r--   0 GerryMa    (501) staff       (20)     3028 2023-06-23 13:51:37.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/designer.py
-drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 01:29:32.381501 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/
--rw-r--r--   0 GerryMa    (501) staff       (20)      136 2023-06-23 04:01:27.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/__init__.py
--rw-r--r--   0 GerryMa    (501) staff       (20)     9321 2023-06-23 12:08:34.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/beta_designer.py
--rw-r--r--   0 GerryMa    (501) staff       (20)     1078 2023-06-23 08:57:19.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/data_structures.py
--rw-r--r--   0 GerryMa    (501) staff       (20)     3666 2023-06-23 11:11:20.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/designer.py
-drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 01:29:32.382437 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/
--rw-r--r--   0 GerryMa    (501) staff       (20)      207 2023-06-23 04:01:27.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/__init__.py
--rw-r--r--   0 GerryMa    (501) staff       (20)      495 2023-06-23 05:12:28.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/component.py
--rw-r--r--   0 GerryMa    (501) staff       (20)     8496 2023-06-23 14:29:15.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/constraints.py
--rw-r--r--   0 GerryMa    (501) staff       (20)      874 2023-06-23 09:38:29.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/ndim_sequence.py
--rw-r--r--   0 GerryMa    (501) staff       (20)     5153 2023-06-22 13:40:16.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/optimizer.py
--rw-r--r--   0 GerryMa    (501) staff       (20)     8266 2023-06-23 14:29:15.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/placement_rule.py
--rw-r--r--   0 GerryMa    (501) staff       (20)     1743 2023-06-23 04:01:27.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/scaled_calculator.py
-drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 01:29:32.380097 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer.egg-info/
--rw-r--r--   0 GerryMa    (501) staff       (20)     3400 2023-06-24 01:29:32.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer.egg-info/PKG-INFO
--rw-r--r--   0 GerryMa    (501) staff       (20)     1224 2023-06-24 01:29:32.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer.egg-info/SOURCES.txt
--rw-r--r--   0 GerryMa    (501) staff       (20)        1 2023-06-24 01:29:32.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer.egg-info/dependency_links.txt
--rw-r--r--   0 GerryMa    (501) staff       (20)       22 2023-06-24 01:29:32.000000 nuclearcraft_designer-0.3.0/src/nuclearcraft_designer.egg-info/top_level.txt
+drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 07:45:55.493739 nuclearcraft_designer-0.4.0/
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     1067 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/LICENSE
+-rw-r--r--   0 GerryMa    (501) staff       (20)     3366 2023-06-24 07:45:55.493641 nuclearcraft_designer-0.4.0/PKG-INFO
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     2802 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/README.md
+-rw-rw-r--   0 GerryMa    (501) staff       (20)      638 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/pyproject.toml
+-rw-r--r--   0 GerryMa    (501) staff       (20)       38 2023-06-24 07:45:55.493773 nuclearcraft_designer-0.4.0/setup.cfg
+drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 07:45:55.490155 nuclearcraft_designer-0.4.0/src/
+drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 07:45:55.490882 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/
+-rw-rw-r--   0 GerryMa    (501) staff       (20)      102 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/__init__.py
+drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 07:45:55.491926 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/common/
+-rw-rw-r--   0 GerryMa    (501) staff       (20)      139 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/common/__init__.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)      495 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/common/component.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)    11902 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/common/constraints.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)      914 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/common/multi_sequence.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     8266 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/common/placement_rule.py
+drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 07:45:55.492056 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/
+-rw-rw-r--   0 GerryMa    (501) staff       (20)      114 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/__init__.py
+drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 07:45:55.492551 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/
+-rw-rw-r--   0 GerryMa    (501) staff       (20)      136 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/__init__.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     6579 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/beta_designer.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     2470 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/data_structures.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     3357 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/designer.py
+drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 07:45:55.493048 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/
+-rw-rw-r--   0 GerryMa    (501) staff       (20)      136 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/__init__.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     9555 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/beta_designer.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     1081 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/data_structures.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     3865 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/designer.py
+drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 07:45:55.493476 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/utils/
+-rw-rw-r--   0 GerryMa    (501) staff       (20)      100 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/utils/__init__.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     5153 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/utils/optimizer.py
+-rw-rw-r--   0 GerryMa    (501) staff       (20)     1743 2023-06-24 07:43:30.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/utils/scaled_calculator.py
+drwxr-xr-x   0 GerryMa    (501) staff       (20)        0 2023-06-24 07:45:55.491327 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer.egg-info/
+-rw-r--r--   0 GerryMa    (501) staff       (20)     3366 2023-06-24 07:45:55.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer.egg-info/PKG-INFO
+-rw-r--r--   0 GerryMa    (501) staff       (20)     1274 2023-06-24 07:45:55.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer.egg-info/SOURCES.txt
+-rw-r--r--   0 GerryMa    (501) staff       (20)        1 2023-06-24 07:45:55.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer.egg-info/dependency_links.txt
+-rw-r--r--   0 GerryMa    (501) staff       (20)       22 2023-06-24 07:45:55.000000 nuclearcraft_designer-0.4.0/src/nuclearcraft_designer.egg-info/top_level.txt
```

### Comparing `nuclearcraft_designer-0.3.0/LICENSE` & `nuclearcraft_designer-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclearcraft_designer-0.3.0/PKG-INFO` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
-Name: nuclearcraft_designer
-Version: 0.3.0
+Name: nuclearcraft-designer
+Version: 0.4.0
 Summary: Generates multiblock designs for NuclearCraft.
 Author-email: Celeste Ma <gerry.y.ma@gmail.com>
 Project-URL: Homepage, https://github.com/MtCelesteMa/nuclearcraft-designer
 Project-URL: Bug Tracker, https://github.com/MtCelesteMa/nuclearcraft-designer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NuclearCraft Designer
 Generates multiblock designs for NuclearCraft.
 
 ## Installation
 NuclearCraft Designer can be installed via pip using the following command:
 ```shell
-pip install git+https://github.com/MtCelesteMa/nuclearcraft-designer.git@v0.3.0
+pip install nuclearcraft-designer
 ```
 
 ## Usage
 Design the best rotor blade sequence of length 10 optimized for 400% expansion using a maximum of 1 SiC-SiC-CMC blade.
 ```python
 from nuclearcraft_designer.overhauled import turbine_rotor_blade
 
@@ -55,17 +55,17 @@
             "connector": 0  # Enabling connectors can lead to invalid designs.
         }
     )
     seq = []
     for seq in gen:
         pass
 
-    for y in range(seq.cols):
-        for x in range(seq.cols):
-            print(seq[x, y].name, end=" ")
+    for y in range(seq.dims[0]):
+        for x in range(seq.dims[1]):
+            print(seq[y, x].name, end=" ")
         print()
 ```
 
 ### OR-Tools Powered Designers
 Certain NuclearCraft Designer designers have OR-Tools powered alternatives. They are generally faster than the normal designers, but are less reliable and may have fewer features.
 
 OR-Tools is not a required dependency. Use the following command to install it:
@@ -77,15 +77,15 @@
 from nuclearcraft_designer.overhauled import turbine_rotor_blade
 
 if __name__ == "__main__":
     status, sequence = turbine_rotor_blade.beta_designer.RotorBladeSequenceDesigner().design(
         10,
         4.0,
         {
-            "sic_sic_cmc": 2,
+            "sic_sic_cmc": 1
         }
     )
     print(status)
     for blade in sequence:
         print(blade.name, end=" ")
     print()
 ```
@@ -98,12 +98,12 @@
         7,
         1,
         {
             "connector": 0  # Enabling connectors can lead to invalid designs.
         }
     )
     print(status)
-    for y in range(configuration.cols):
-        for x in range(configuration.cols):
-            print(configuration[x, y].name, end=" ")
+    for y in range(configuration.dims[0]):
+        for x in range(configuration.dims[1]):
+            print(configuration[y, x].name, end=" ")
         print()
 ```
```

### Comparing `nuclearcraft_designer-0.3.0/README.md` & `nuclearcraft_designer-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # NuclearCraft Designer
 Generates multiblock designs for NuclearCraft.
 
 ## Installation
 NuclearCraft Designer can be installed via pip using the following command:
 ```shell
-pip install git+https://github.com/MtCelesteMa/nuclearcraft-designer.git@v0.3.0
+pip install nuclearcraft-designer
 ```
 
 ## Usage
 Design the best rotor blade sequence of length 10 optimized for 400% expansion using a maximum of 1 SiC-SiC-CMC blade.
 ```python
 from nuclearcraft_designer.overhauled import turbine_rotor_blade
 
@@ -41,17 +41,17 @@
             "connector": 0  # Enabling connectors can lead to invalid designs.
         }
     )
     seq = []
     for seq in gen:
         pass
 
-    for y in range(seq.cols):
-        for x in range(seq.cols):
-            print(seq[x, y].name, end=" ")
+    for y in range(seq.dims[0]):
+        for x in range(seq.dims[1]):
+            print(seq[y, x].name, end=" ")
         print()
 ```
 
 ### OR-Tools Powered Designers
 Certain NuclearCraft Designer designers have OR-Tools powered alternatives. They are generally faster than the normal designers, but are less reliable and may have fewer features.
 
 OR-Tools is not a required dependency. Use the following command to install it:
@@ -63,15 +63,15 @@
 from nuclearcraft_designer.overhauled import turbine_rotor_blade
 
 if __name__ == "__main__":
     status, sequence = turbine_rotor_blade.beta_designer.RotorBladeSequenceDesigner().design(
         10,
         4.0,
         {
-            "sic_sic_cmc": 2,
+            "sic_sic_cmc": 1
         }
     )
     print(status)
     for blade in sequence:
         print(blade.name, end=" ")
     print()
 ```
@@ -84,12 +84,12 @@
         7,
         1,
         {
             "connector": 0  # Enabling connectors can lead to invalid designs.
         }
     )
     print(status)
-    for y in range(configuration.cols):
-        for x in range(configuration.cols):
-            print(configuration[x, y].name, end=" ")
+    for y in range(configuration.dims[0]):
+        for x in range(configuration.dims[1]):
+            print(configuration[y, x].name, end=" ")
         print()
 ```
```

### Comparing `nuclearcraft_designer-0.3.0/pyproject.toml` & `nuclearcraft_designer-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nuclearcraft_designer"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Celeste Ma", email="gerry.y.ma@gmail.com" },
 ]
 description = "Generates multiblock designs for NuclearCraft."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/beta_designer.py` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/beta_designer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """NuclearCraft: Overhauled turbine dynamo coil configuration designer."""
 
 from . import DynamoCoil, DYNAMO_COIL_TYPES
-from ... import utils
-
-import uuid
+from ... import utils, common
 
 try:
     from ortools.sat.python import cp_model
 except ImportError:
     cp_model = None
 
 
@@ -23,27 +21,28 @@
         :param dynamo_coil_types: A list of dynamo coil types.
         :param scaling_factor: The number of digits to scale decimals by.
         """
         self.dynamo_coil_types = dynamo_coil_types
         self.scaling_factor = scaling_factor
         self.sc = utils.scaled_calculator.ScaledCalculator(self.scaling_factor)
 
-    def ids_to_coils(self, sequence: list[int]) -> utils.ndim_sequence.Sequence2D[DynamoCoil]:
+    def ids_to_coils(self, sequence: list[int]) -> common.multi_sequence.MultiSequence[DynamoCoil]:
         """Converts a sequence of IDs to a sequence of rotor blades.
 
         :param sequence: A sequence of IDs.
         :return: A sequence of rotor blades.
         """
-        return utils.ndim_sequence.Sequence2D([
+        side_length = round(len(sequence) ** (1 / 2))
+        return common.multi_sequence.MultiSequence([
             self.dynamo_coil_types[i] if i >= 0 else None
             for i in sequence
-        ], round(len(sequence) ** (1 / 2)))
+        ], (side_length, side_length))
 
     def coil_attributes(self, model: cp_model.CpModel, n_coils: int) -> tuple[
-        list[cp_model.IntVar], list[cp_model.IntVar]
+        common.multi_sequence.MultiSequence[cp_model.IntVar], list[cp_model.IntVar]
     ]:
         """Registers dynamo coils as well as their attributes to the model.
 
         :param model: The model to register dynamo coils to.
         :param n_coils: The number of coils to register.
         :return: Two lists of IntVars, representing the coils and their conductivities.
         """
@@ -58,15 +57,16 @@
         ]
         for coil, conductivity in zip(coils, conductivities):
             model.AddElement(coil, [
                 round(coil_type.conductivity * (10 ** self.scaling_factor))
                 for coil_type in self.dynamo_coil_types
             ], conductivity)
 
-        return coils, conductivities
+        side_length = round(n_coils ** (1 / 2))
+        return common.multi_sequence.MultiSequence(coils, (side_length, side_length)), conductivities
 
     def total_efficiency(self, model: cp_model.CpModel, conductivities: list[cp_model.IntVar]) -> cp_model.IntVar:
         """Calculates the total efficiency of a dynamo coil configuration.
 
         :param model: The optimization model.
         :param conductivities: A list of IntVars representing each coil's conductivity.
         :return: An IntVar representing the total efficiency.
@@ -104,44 +104,53 @@
         return total_efficiency
 
     def design(
             self,
             side_length: int,
             shaft_width: int,
             type_limits: dict[str, int],
+            symmetric: bool = False,
             time_limit: float = None
-    ) -> tuple[int, utils.ndim_sequence.Sequence2D[DynamoCoil]]:
+    ) -> tuple[int, common.multi_sequence.MultiSequence[DynamoCoil]]:
         """Designs the optimal dynamo coil configuration if possible.
 
         :param side_length: The side length of the turbine.
         :param shaft_width: The width of the rotor shaft.
         :param type_limits: The maximum number of each type of dynamo coil.
+        :param symmetric: Whether to force the result to be symmetric.
         :param time_limit: The maximum time in seconds to run for.
         :return: The status as well as a dynamo coil configuration.
         """
         model = cp_model.CpModel()
 
         coils, conductivities = self.coil_attributes(model, side_length ** 2)
 
         total_efficiency = self.total_efficiency(model, conductivities)
 
         for target_name, quantity in type_limits.items():
-            utils.constraints.MaxQuantityConstraint(target_name, quantity).apply_to_model(
+            common.constraints.MaxQuantityConstraint(target_name, quantity).apply_to_model(
+                model,
+                coils,
+                self.dynamo_coil_types
+            )
+
+        if symmetric:
+            common.constraints.SymmetryConstraint().apply_to_model(
                 model,
                 coils,
                 self.dynamo_coil_types
             )
 
-        utils.constraints.CenteredBearingsConstraint(shaft_width).apply_to_model(
+        common.constraints.CenteredBearingsConstraint(shaft_width).apply_to_model(
             model,
             coils,
             self.dynamo_coil_types
         )
 
-        utils.constraints.PlacementRuleConstraint().apply_to_model(
+        common.constraints.PlacementRuleConstraint().apply_to_model(
             model,
             coils,
             self.dynamo_coil_types
         )
 
         model.Maximize(total_efficiency)
```

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/data_structures.py` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/data_structures.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 """NuclearCraft: Overhauled turbine dynamo coil data structures."""
 
-from ... import utils
+from ... import common
 
 
-class DynamoCoil(utils.component.Component):
+class DynamoCoil(common.component.Component):
     """An object representing a NuclearCraft: Overhauled turbine dynamo coil."""
     def __init__(
             self,
             name: str,
             conductivity: float,
-            placement_rule: utils.placement_rule.PlacementRule
+            placement_rule: common.placement_rule.PlacementRule
     ) -> None:
         """Constructs a DynamoCoil object.
 
         :param name: The name of the dynamo coil.
         :param conductivity: The conductivity of the dynamo coil.
         :param placement_rule: The placement rule of the dynamo coil.
         """
         super().__init__(name, {"conductivity": conductivity}, placement_rule)
 
     @property
     def conductivity(self) -> float:
         return self.stats["conductivity"]
 
 
-CASING = DynamoCoil("casing", -1.0, utils.placement_rule.PlacementRule())
-BEARING = DynamoCoil("bearing", -1.0, utils.placement_rule.PlacementRule())
-CONNECTOR = DynamoCoil("connector", -1.0, utils.placement_rule.CompoundPlacementRule([
-    utils.placement_rule.SimplePlacementRule("magnesium", 1),
-    utils.placement_rule.SimplePlacementRule("beryllium", 1),
-    utils.placement_rule.SimplePlacementRule("aluminum", 1),
-    utils.placement_rule.SimplePlacementRule("gold", 1),
-    utils.placement_rule.SimplePlacementRule("copper", 1),
-    utils.placement_rule.SimplePlacementRule("silver", 1)
-], utils.placement_rule.LogicMode.OR))
-MAGNESIUM = DynamoCoil("magnesium", 0.88, utils.placement_rule.CompoundPlacementRule([
-    utils.placement_rule.SimplePlacementRule("bearing", 1),
-    utils.placement_rule.SimplePlacementRule("connector", 1)
-], utils.placement_rule.LogicMode.OR))
-BERYLLIUM = DynamoCoil("beryllium", 0.9, utils.placement_rule.SimplePlacementRule("magnesium", 1))
-ALUMINUM = DynamoCoil("aluminum", 1.0, utils.placement_rule.SimplePlacementRule("magnesium", 2))
-GOLD = DynamoCoil("gold", 1.04, utils.placement_rule.SimplePlacementRule("aluminum", 1))
-COPPER = DynamoCoil("copper", 1.06, utils.placement_rule.SimplePlacementRule("beryllium", 1))
-SILVER = DynamoCoil("silver", 1.12, utils.placement_rule.CompoundPlacementRule([
-    utils.placement_rule.SimplePlacementRule("gold", 1),
-    utils.placement_rule.SimplePlacementRule("copper", 1)
-], utils.placement_rule.LogicMode.AND))
+CASING = DynamoCoil("casing", -1.0, common.placement_rule.PlacementRule())
+BEARING = DynamoCoil("bearing", -1.0, common.placement_rule.PlacementRule())
+CONNECTOR = DynamoCoil("connector", -1.0, common.placement_rule.CompoundPlacementRule([
+    common.placement_rule.SimplePlacementRule("magnesium", 1),
+    common.placement_rule.SimplePlacementRule("beryllium", 1),
+    common.placement_rule.SimplePlacementRule("aluminum", 1),
+    common.placement_rule.SimplePlacementRule("gold", 1),
+    common.placement_rule.SimplePlacementRule("copper", 1),
+    common.placement_rule.SimplePlacementRule("silver", 1)
+], common.placement_rule.LogicMode.OR))
+MAGNESIUM = DynamoCoil("magnesium", 0.88, common.placement_rule.CompoundPlacementRule([
+    common.placement_rule.SimplePlacementRule("bearing", 1),
+    common.placement_rule.SimplePlacementRule("connector", 1)
+], common.placement_rule.LogicMode.OR))
+BERYLLIUM = DynamoCoil("beryllium", 0.9, common.placement_rule.SimplePlacementRule("magnesium", 1))
+ALUMINUM = DynamoCoil("aluminum", 1.0, common.placement_rule.SimplePlacementRule("magnesium", 2))
+GOLD = DynamoCoil("gold", 1.04, common.placement_rule.SimplePlacementRule("aluminum", 1))
+COPPER = DynamoCoil("copper", 1.06, common.placement_rule.SimplePlacementRule("beryllium", 1))
+SILVER = DynamoCoil("silver", 1.12, common.placement_rule.CompoundPlacementRule([
+    common.placement_rule.SimplePlacementRule("gold", 1),
+    common.placement_rule.SimplePlacementRule("copper", 1)
+], common.placement_rule.LogicMode.AND))
 
 DYNAMO_COIL_TYPES = [
     CASING,
     BEARING,
     CONNECTOR,
     MAGNESIUM,
     BERYLLIUM,
```

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/designer.py` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/designer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """NuclearCraft: Overhauled turbine dynamo coil configuration designer."""
 
 from . import DynamoCoil, DYNAMO_COIL_TYPES
-from ... import utils
+from ... import utils, common
 
 import typing
 
 
 class DynamoCoilConfigurationDesigner:
     """Designs NuclearCraft: Overhauled turbine dynamo coil configurations."""
     def __init__(
@@ -14,26 +14,27 @@
     ) -> None:
         """Constructs a DynamoCoilConfigurationDesigner object.
 
         :param dynamo_coil_types: A list of dynamo coil types.
         """
         self.dynamo_coil_types = dynamo_coil_types
 
-    def ids_to_coils(self, sequence: list[int]) -> utils.ndim_sequence.Sequence2D[DynamoCoil]:
+    def ids_to_coils(self, sequence: list[int]) -> common.multi_sequence.MultiSequence[DynamoCoil]:
         """Converts a sequence of IDs to a sequence of rotor blades.
 
         :param sequence: A sequence of IDs.
         :return: A sequence of rotor blades.
         """
-        return utils.ndim_sequence.Sequence2D([
+        side_length = round(len(sequence) ** (1 / 2))
+        return common.multi_sequence.MultiSequence([
             self.dynamo_coil_types[i] if i >= 0 else None
             for i in sequence
-        ], round(len(sequence) ** (1 / 2)))
+        ], (side_length, side_length))
 
-    def total_efficiency(self, sequence: utils.ndim_sequence.Sequence2D[DynamoCoil]) -> float:
+    def total_efficiency(self, sequence: common.multi_sequence.MultiSequence[DynamoCoil]) -> float:
         """Calculates the total efficiency of a sequence of dynamo coils.
 
         :param sequence: A sequence of dynamo coils.
         :return: The total efficiency of the sequence.
         """
         total_efficiency = 0.0
         n_coils = 0
@@ -43,32 +44,36 @@
                 n_coils += 1
         return total_efficiency / n_coils if n_coils > 0 else 0
 
     def design_generator(
             self,
             side_length: int,
             shaft_width: int,
-            type_limits: dict[str, int]
-    ) -> typing.Generator[utils.ndim_sequence.Sequence2D[DynamoCoil], None, None]:
+            type_limits: dict[str, int],
+            symmetric: bool = False
+    ) -> typing.Generator[common.multi_sequence.MultiSequence[DynamoCoil], None, None]:
         """Constructs a generator that iteratively generates better dynamo coil sequences.
 
         :param side_length: The side length of the turbine.
         :param shaft_width: The width of the rotor shaft.
         :param type_limits: The maximum number of each type of dynamo coil.
+        :param symmetric: Whether to force the result to be symmetric.
         :return: A generator object.
         """
         gen = utils.optimizer.SequenceOptimizer(
             utils.optimizer.ConstrainedIntegerSequence(
                 side_length ** 2,
                 len(self.dynamo_coil_types),
                 [
-                    lambda seq: utils.constraints.CenteredBearingsConstraint(shaft_width)(self.ids_to_coils(seq)),
-                    lambda seq: utils.constraints.PlacementRuleConstraint()(self.ids_to_coils(seq))
+                    lambda seq: common.constraints.CenteredBearingsConstraint(shaft_width)(self.ids_to_coils(seq)),
+                    lambda seq: common.constraints.PlacementRuleConstraint()(self.ids_to_coils(seq))
                 ] + [
-                    lambda seq: utils.constraints.MaxQuantityConstraint(target_name, quantity)(self.ids_to_coils(seq))
+                    lambda seq: common.constraints.MaxQuantityConstraint(target_name, quantity)(self.ids_to_coils(seq))
                     for target_name, quantity in type_limits.items()
-                ]
+                ] + ([
+                    lambda seq: common.constraints.SymmetryConstraint()(self.ids_to_coils(seq))
+                ] if symmetric else [])
             ).generator(),
             lambda seq: self.total_efficiency(self.ids_to_coils(seq))
         ).generator()
         for sequence in gen:
             yield self.ids_to_coils(sequence)
```

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/beta_designer.py` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/beta_designer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """NuclearCraft: Overhauled turbine rotor blade sequence designer."""
 
 from . import RotorBlade, ROTOR_BLADE_TYPES
-from ... import utils
+from ... import utils, common
 
 import uuid
 
 try:
     from ortools.sat.python import cp_model
 except ImportError:
     cp_model = None
@@ -23,27 +23,30 @@
         :param rotor_blade_types: A list of rotor blade types.
         :param scaling_factor: The number of digits to scale decimals by.
         """
         self.rotor_blade_types = rotor_blade_types
         self.scaling_factor = scaling_factor
         self.sc = utils.scaled_calculator.ScaledCalculator(self.scaling_factor)
 
-    def ids_to_blades(self, sequence: list[int]) -> list[RotorBlade]:
+    def ids_to_blades(self, sequence: list[int]) -> common.multi_sequence.MultiSequence[RotorBlade]:
         """Converts a sequence of IDs to a sequence of rotor blades.
 
         :param sequence: A sequence of IDs.
         :return: A sequence of rotor blades.
         """
-        return [
+        return common.multi_sequence.MultiSequence([
             self.rotor_blade_types[i] if i >= 0 else None
             for i in sequence
-        ]
+        ], (len(sequence),))
 
     def blade_attributes(self, model: cp_model.CpModel, n_blades: int) -> tuple[
-        list[cp_model.IntVar], list[cp_model.IntVar], list[cp_model.IntVar], list[cp_model.IntVar]
+        common.multi_sequence.MultiSequence[cp_model.IntVar],
+        list[cp_model.IntVar],
+        list[cp_model.IntVar],
+        list[cp_model.IntVar]
     ]:
         """Registers rotor blades as well as their attributes to the model.
 
         :param model: The model to register rotor blades to.
         :param n_blades: The number of blades to register.
         :return: Four lists of IntVars, representing the blades, the efficiencies, and the expansions and their
         square roots.
@@ -79,15 +82,15 @@
         ]
         for blade, expansion_sqrt in zip(blades, expansions_sqrt):
             model.AddElement(blade, [
                 round(blade_type.expansion ** (1 / 2) * (10 ** self.scaling_factor))
                 for blade_type in self.rotor_blade_types
             ], expansion_sqrt)
 
-        return blades, efficiencies, expansions, expansions_sqrt
+        return common.multi_sequence.MultiSequence(blades, (len(blades),)), efficiencies, expansions, expansions_sqrt
 
     def expansion_levels(
             self,
             model: cp_model.CpModel,
             expansions: list[cp_model.IntVar],
             expansions_sqrt: list[cp_model.IntVar]
     ) -> list[cp_model.IntVar]:
@@ -178,15 +181,15 @@
 
     def design(
             self,
             length: int,
             opt_expansion: float,
             type_limits: dict[str, int],
             time_limit: float = None
-    ) -> tuple[int, list[RotorBlade]]:
+    ) -> tuple[int, common.multi_sequence.MultiSequence[RotorBlade]]:
         """Designs the optimal sequence of rotor blades if possible.
 
         :param length: The length of the rotor blade sequence.
         :param opt_expansion: The expansion level to optimize for.
         :param type_limits: The maximum number of each type of rotor blade.
         :param time_limit: The maximum time in seconds to run for.
         :return: The status as well as a sequence of rotor blades.
@@ -196,15 +199,15 @@
         blades, efficiencies, expansions, expansions_sqrt = self.blade_attributes(model, length)
 
         expansion_levels = self.expansion_levels(model, expansions, expansions_sqrt)
 
         total_efficiency = self.total_efficiency(model, efficiencies, expansion_levels, opt_expansion)
 
         for target_name, quantity in type_limits.items():
-            utils.constraints.MaxQuantityConstraint(target_name, quantity).apply_to_model(
+            common.constraints.MaxQuantityConstraint(target_name, quantity).apply_to_model(
                 model,
                 blades,
                 self.rotor_blade_types
             )
 
         model.Maximize(total_efficiency)
```

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/data_structures.py` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/data_structures.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """NuclearCraft: Overhauled turbine rotor blades."""
 
-from ... import utils
+from ... import common
 
 
-class RotorBlade(utils.component.Component):
+class RotorBlade(common.component.Component):
     """An object representing a NuclearCraft: Overhauled turbine rotor blade."""
     def __init__(self, name: str, efficiency: float, expansion: float) -> None:
         """Constructs a RotorBlade object.
 
         :param name: The name of the rotor blade.
         :param efficiency: The efficiency of the rotor blade.
         :param expansion: The expansion of the rotor blade.
         """
         super().__init__(name, {
             "efficiency": efficiency,
             "expansion": expansion
-        }, utils.placement_rule.PlacementRule())
+        }, common.placement_rule.PlacementRule())
 
     @property
     def efficiency(self) -> float:
         return self.stats["efficiency"]
 
     @property
     def expansion(self) -> float:
```

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/designer.py` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/overhauled/turbine_rotor_blade/designer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """NuclearCraft: Overhauled turbine rotor blade sequence designer."""
 
 from . import RotorBlade, ROTOR_BLADE_TYPES
-from ... import utils
+from ... import utils, common
 
 import typing
 
 
 class RotorBladeSequenceDesigner:
     """Designs NuclearCraft: Overhauled turbine rotor blade sequences."""
     def __init__(
@@ -14,39 +14,43 @@
     ) -> None:
         """Constructs a RotorBladeSequenceDesigner object.
 
         :param rotor_blade_types: A list of rotor blade types.
         """
         self.rotor_blade_types = rotor_blade_types
 
-    def ids_to_blades(self, sequence: list[int]) -> list[RotorBlade]:
+    def ids_to_blades(self, sequence: list[int]) -> common.multi_sequence.MultiSequence[RotorBlade]:
         """Converts a sequence of IDs to a sequence of rotor blades.
 
         :param sequence: A sequence of IDs.
         :return: A sequence of rotor blades.
         """
-        return [
+        return common.multi_sequence.MultiSequence([
             self.rotor_blade_types[i] if i >= 0 else None
             for i in sequence
-        ]
+        ], (len(sequence),))
 
-    def expansion_levels(self, sequence: list[RotorBlade]) -> list[float]:
+    def expansion_levels(self, sequence: common.multi_sequence.MultiSequence[RotorBlade]) -> list[float]:
         """Calculates the expansion levels of a sequence of rotor blades.
 
         :param sequence: A sequence of rotor blades.
         :return: A list of expansion levels.
         """
         total_expansion_level = 1.0
         expansion_levels = []
         for rotor_blade in sequence:
             expansion_levels.append(total_expansion_level * rotor_blade.expansion ** (1 / 2))
             total_expansion_level *= rotor_blade.expansion
         return expansion_levels
 
-    def total_efficiency(self, sequence: list[RotorBlade], opt_expansion: float) -> float:
+    def total_efficiency(
+            self,
+            sequence: common.multi_sequence.MultiSequence[RotorBlade],
+            opt_expansion: float
+    ) -> float:
         """Calculates the total efficiency of a sequence of rotor blades.
 
         :param sequence: A sequence of rotor blades.
         :param opt_expansion: The optimal expansion.
         :return: The total efficiency of the sequence.
         """
         expansion_levels = self.expansion_levels(sequence)
@@ -77,15 +81,15 @@
         :return: A generator object.
         """
         gen = utils.optimizer.SequenceOptimizer(
             utils.optimizer.ConstrainedIntegerSequence(
                 length,
                 len(self.rotor_blade_types),
                 [
-                    lambda seq: utils.constraints.MaxQuantityConstraint(target_name, quantity)(self.ids_to_blades(seq))
+                    lambda seq: common.constraints.MaxQuantityConstraint(target_name, quantity)(self.ids_to_blades(seq))
                     for target_name, quantity in type_limits.items()
                 ]
             ).generator(),
             lambda seq: self.total_efficiency(self.ids_to_blades(seq), opt_expansion)
         ).generator()
         for sequence in gen:
             yield self.ids_to_blades(sequence)
```

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/optimizer.py` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/placement_rule.py` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/common/placement_rule.py`

 * *Files identical despite different names*

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer/utils/scaled_calculator.py` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer/utils/scaled_calculator.py`

 * *Files identical despite different names*

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer.egg-info/PKG-INFO` & `nuclearcraft_designer-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
-Name: nuclearcraft-designer
-Version: 0.3.0
+Name: nuclearcraft_designer
+Version: 0.4.0
 Summary: Generates multiblock designs for NuclearCraft.
 Author-email: Celeste Ma <gerry.y.ma@gmail.com>
 Project-URL: Homepage, https://github.com/MtCelesteMa/nuclearcraft-designer
 Project-URL: Bug Tracker, https://github.com/MtCelesteMa/nuclearcraft-designer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NuclearCraft Designer
 Generates multiblock designs for NuclearCraft.
 
 ## Installation
 NuclearCraft Designer can be installed via pip using the following command:
 ```shell
-pip install git+https://github.com/MtCelesteMa/nuclearcraft-designer.git@v0.3.0
+pip install nuclearcraft-designer
 ```
 
 ## Usage
 Design the best rotor blade sequence of length 10 optimized for 400% expansion using a maximum of 1 SiC-SiC-CMC blade.
 ```python
 from nuclearcraft_designer.overhauled import turbine_rotor_blade
 
@@ -55,17 +55,17 @@
             "connector": 0  # Enabling connectors can lead to invalid designs.
         }
     )
     seq = []
     for seq in gen:
         pass
 
-    for y in range(seq.cols):
-        for x in range(seq.cols):
-            print(seq[x, y].name, end=" ")
+    for y in range(seq.dims[0]):
+        for x in range(seq.dims[1]):
+            print(seq[y, x].name, end=" ")
         print()
 ```
 
 ### OR-Tools Powered Designers
 Certain NuclearCraft Designer designers have OR-Tools powered alternatives. They are generally faster than the normal designers, but are less reliable and may have fewer features.
 
 OR-Tools is not a required dependency. Use the following command to install it:
@@ -77,15 +77,15 @@
 from nuclearcraft_designer.overhauled import turbine_rotor_blade
 
 if __name__ == "__main__":
     status, sequence = turbine_rotor_blade.beta_designer.RotorBladeSequenceDesigner().design(
         10,
         4.0,
         {
-            "sic_sic_cmc": 2,
+            "sic_sic_cmc": 1
         }
     )
     print(status)
     for blade in sequence:
         print(blade.name, end=" ")
     print()
 ```
@@ -98,12 +98,12 @@
         7,
         1,
         {
             "connector": 0  # Enabling connectors can lead to invalid designs.
         }
     )
     print(status)
-    for y in range(configuration.cols):
-        for x in range(configuration.cols):
-            print(configuration[x, y].name, end=" ")
+    for y in range(configuration.dims[0]):
+        for x in range(configuration.dims[1]):
+            print(configuration[y, x].name, end=" ")
         print()
 ```
```

### Comparing `nuclearcraft_designer-0.3.0/src/nuclearcraft_designer.egg-info/SOURCES.txt` & `nuclearcraft_designer-0.4.0/src/nuclearcraft_designer.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 README.md
 pyproject.toml
 src/nuclearcraft_designer/__init__.py
 src/nuclearcraft_designer.egg-info/PKG-INFO
 src/nuclearcraft_designer.egg-info/SOURCES.txt
 src/nuclearcraft_designer.egg-info/dependency_links.txt
 src/nuclearcraft_designer.egg-info/top_level.txt
+src/nuclearcraft_designer/common/__init__.py
+src/nuclearcraft_designer/common/component.py
+src/nuclearcraft_designer/common/constraints.py
+src/nuclearcraft_designer/common/multi_sequence.py
+src/nuclearcraft_designer/common/placement_rule.py
 src/nuclearcraft_designer/overhauled/__init__.py
 src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/__init__.py
 src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/beta_designer.py
 src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/data_structures.py
 src/nuclearcraft_designer/overhauled/turbine_dynamo_coil/designer.py
 src/nuclearcraft_designer/overhauled/turbine_rotor_blade/__init__.py
 src/nuclearcraft_designer/overhauled/turbine_rotor_blade/beta_designer.py
 src/nuclearcraft_designer/overhauled/turbine_rotor_blade/data_structures.py
 src/nuclearcraft_designer/overhauled/turbine_rotor_blade/designer.py
 src/nuclearcraft_designer/utils/__init__.py
-src/nuclearcraft_designer/utils/component.py
-src/nuclearcraft_designer/utils/constraints.py
-src/nuclearcraft_designer/utils/ndim_sequence.py
 src/nuclearcraft_designer/utils/optimizer.py
-src/nuclearcraft_designer/utils/placement_rule.py
 src/nuclearcraft_designer/utils/scaled_calculator.py
```

