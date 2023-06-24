# Comparing `tmp/ecghelper-0.3.0.tar.gz` & `tmp/ecghelper-0.3.1.tar.gz`

## Comparing `ecghelper-0.3.0.tar` & `ecghelper-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    46579 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000.csv
--rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000.dat
--rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000.edf
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000.hea
--rw-r--r--   0        0        0    18048 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000.xml
--rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000_wfdb.dat
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000_wfdb.hea
--rw-r--r--   0        0        0    82282 2020-02-02 00:00:00.000000 ecghelper-0.3.0/Untitled.ipynb
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.3.0/debug.py
--rw-r--r--   0        0        0    33302 2020-02-02 00:00:00.000000 ecghelper-0.3.0/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.3.0/.ipynb_checkpoints/debug-checkpoint.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/__main__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/convert.py
--rw-r--r--   0        0        0    17124 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/io.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/utils.py
--rw-r--r--   0        0        0    21595 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/waveform.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/test_io.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/test_timing.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/test_waveform.py
--rw-r--r--   0        0        0   149083 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/82000.xml
--rw-r--r--   0        0        0   185294 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/A0001.edf
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/A0001.hea
--rw-r--r--   0        0        0   180024 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/A0001.mat
--rw-r--r--   0        0        0   247499 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/A0001.xml
--rw-r--r--   0        0        0   108785 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/binary.csv
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ecghelper-0.3.0/.gitignore
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ecghelper-0.3.0/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ecghelper-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 ecghelper-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    46579 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000.csv
+-rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000.dat
+-rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000.edf
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000.hea
+-rw-r--r--   0        0        0    18048 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000.xml
+-rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000_wfdb.dat
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000_wfdb.hea
+-rw-r--r--   0        0        0    82282 2020-02-02 00:00:00.000000 ecghelper-0.3.1/Untitled.ipynb
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.3.1/debug.py
+-rw-r--r--   0        0        0    33302 2020-02-02 00:00:00.000000 ecghelper-0.3.1/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.3.1/.ipynb_checkpoints/debug-checkpoint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/__main__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/convert.py
+-rw-r--r--   0        0        0    17124 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/io.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/utils.py
+-rw-r--r--   0        0        0    21598 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/waveform.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/test_io.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/test_timing.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/test_waveform.py
+-rw-r--r--   0        0        0   149083 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/82000.xml
+-rw-r--r--   0        0        0   185294 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/A0001.edf
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/A0001.hea
+-rw-r--r--   0        0        0   180024 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/A0001.mat
+-rw-r--r--   0        0        0   247499 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/A0001.xml
+-rw-r--r--   0        0        0   108785 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/binary.csv
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ecghelper-0.3.1/.gitignore
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ecghelper-0.3.1/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ecghelper-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 ecghelper-0.3.1/PKG-INFO
```

### Comparing `ecghelper-0.3.0/82000.csv` & `ecghelper-0.3.1/82000.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/82000.dat` & `ecghelper-0.3.1/82000.dat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/82000.edf` & `ecghelper-0.3.1/82000.edf`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/82000.hea` & `ecghelper-0.3.1/82000.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/82000.xml` & `ecghelper-0.3.1/82000.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/82000_wfdb.dat` & `ecghelper-0.3.1/82000_wfdb.dat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/82000_wfdb.hea` & `ecghelper-0.3.1/82000_wfdb.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/Untitled.ipynb` & `ecghelper-0.3.1/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/debug.py` & `ecghelper-0.3.1/debug.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/.ipynb_checkpoints/Untitled-checkpoint.ipynb` & `ecghelper-0.3.1/.ipynb_checkpoints/Untitled-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/.ipynb_checkpoints/debug-checkpoint.py` & `ecghelper-0.3.1/.ipynb_checkpoints/debug-checkpoint.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/src/ecghelper/__main__.py` & `ecghelper-0.3.1/src/ecghelper/__main__.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/src/ecghelper/convert.py` & `ecghelper-0.3.1/src/ecghelper/convert.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/src/ecghelper/io.py` & `ecghelper-0.3.1/src/ecghelper/io.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/src/ecghelper/utils.py` & `ecghelper-0.3.1/src/ecghelper/utils.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/src/ecghelper/waveform.py` & `ecghelper-0.3.1/src/ecghelper/waveform.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
 
 
 @dataclass
 class WaveformMetadata:
     age: Optional[int] = None
     sex: Optional[str] = None
     race: Optional[str] = None
-    arrythmia: Optional[List[int]] = field(default_factory=list)
+    arrhythmia: Optional[List[int]] = field(default_factory=list)
     potassium:  Optional[float] = None
     lvef: Optional[int] = None
 
     @classmethod
     def from_edf(cls, record_filename: Union[str, Path]):
         """Load an EDF record."""
         # Open EDF file
@@ -547,14 +547,14 @@
         """Load metadata for a CSV record. Not implemented."""
         
         # TODO: get attributes dynamically
         data = {
             'age': self.age,
             'sex': self.sex,
             'race': self.race,
-            'arrythmia': self.arrythmia,
+            'arrhythmia': self.arrhythmia,
             'potassium': self.potassium,
             'lvef': self.lvef,
         }
 
         with open(record_name, 'w') as fp:
             json.dump(data, fp)
```

### Comparing `ecghelper-0.3.0/tests/test_io.py` & `ecghelper-0.3.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/tests/test_timing.py` & `ecghelper-0.3.1/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/tests/test_waveform.py` & `ecghelper-0.3.1/tests/test_waveform.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/tests/data/82000.xml` & `ecghelper-0.3.1/tests/data/82000.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/tests/data/A0001.edf` & `ecghelper-0.3.1/tests/data/A0001.edf`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/tests/data/A0001.hea` & `ecghelper-0.3.1/tests/data/A0001.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/tests/data/A0001.mat` & `ecghelper-0.3.1/tests/data/A0001.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/tests/data/A0001.xml` & `ecghelper-0.3.1/tests/data/A0001.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/tests/data/binary.csv` & `ecghelper-0.3.1/tests/data/binary.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/.gitignore` & `ecghelper-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.0/pyproject.toml` & `ecghelper-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ecghelper"
-version = "0.3.0"
+version = "0.3.1"
 description = "Tools to load and process electrocardiogram data."
 author = "Alistair Johnson"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

### Comparing `ecghelper-0.3.0/PKG-INFO` & `ecghelper-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecghelper
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tools to load and process electrocardiogram data.
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: cython>=0.29.34
 Requires-Dist: joblib>=1.2.0
 Requires-Dist: lxml>=4.9.2
```

