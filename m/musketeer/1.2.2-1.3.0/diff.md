# Comparing `tmp/musketeer-1.2.2.tar.gz` & `tmp/musketeer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musketeer-1.2.2.tar", last modified: Thu Mar 16 16:44:22 2023, max compression
+gzip compressed data, was "musketeer-1.3.0.tar", last modified: Sat Jun 24 19:40:04 2023, max compression
```

## Comparing `musketeer-1.2.2.tar` & `musketeer-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 16:44:22.610246 musketeer-1.2.2/
--rw-rw-rw-   0        0        0       66 2023-01-17 16:05:36.000000 musketeer-1.2.2/.flake8
--rw-rw-rw-   0        0        0       58 2023-02-06 20:47:27.000000 musketeer-1.2.2/.gitignore
--rw-rw-rw-   0        0        0     1093 2021-05-07 10:14:54.000000 musketeer-1.2.2/LICENSE
--rw-rw-rw-   0        0        0       35 2021-07-24 12:56:15.000000 musketeer-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      890 2023-03-16 16:44:22.606247 musketeer-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-02-23 14:24:54.000000 musketeer-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-16 16:44:22.530271 musketeer-1.2.2/musketeer/
--rw-rw-rw-   0        0        0       23 2023-03-16 16:43:23.000000 musketeer-1.2.2/musketeer/__init__.py
--rw-rw-rw-   0        0        0    10662 2023-03-15 16:52:22.000000 musketeer-1.2.2/musketeer/__main__.py
--rw-rw-rw-   0        0        0     1020 2023-03-09 17:15:19.000000 musketeer-1.2.2/musketeer/combineResiduals.py
--rw-rw-rw-   0        0        0    13143 2023-03-15 17:20:39.000000 musketeer-1.2.2/musketeer/contributors.py
--rw-rw-rw-   0        0        0     8304 2023-02-06 20:04:34.000000 musketeer-1.2.2/musketeer/editData.py
--rw-rw-rw-   0        0        0    13484 2023-03-15 17:11:13.000000 musketeer-1.2.2/musketeer/equilibriumConstants.py
--rw-rw-rw-   0        0        0     6654 2023-03-09 17:15:19.000000 musketeer-1.2.2/musketeer/fitSignals.py
--rw-rw-rw-   0        0        0     3581 2023-03-16 16:26:03.000000 musketeer-1.2.2/musketeer/knownSignals.py
--rw-rw-rw-   0        0        0      937 2021-01-06 01:52:42.000000 musketeer-1.2.2/musketeer/logo small.png
--rw-rw-rw-   0        0        0     5452 2023-03-16 16:26:03.000000 musketeer-1.2.2/musketeer/moduleFrame.py
--rw-rw-rw-   0        0        0     8595 2023-03-16 16:26:03.000000 musketeer-1.2.2/musketeer/patchMatplotlib.py
--rw-rw-rw-   0        0        0      961 2023-03-09 17:15:19.000000 musketeer-1.2.2/musketeer/proportionality.py
--rw-rw-rw-   0        0        0    12401 2023-02-17 10:34:11.000000 musketeer-1.2.2/musketeer/scrolledFrame.py
--rw-rw-rw-   0        0        0    15039 2023-03-15 17:27:11.000000 musketeer-1.2.2/musketeer/speciation.py
--rw-rw-rw-   0        0        0      607 2023-03-14 16:14:53.000000 musketeer-1.2.2/musketeer/style.py
--rw-rw-rw-   0        0        0    16954 2023-03-10 11:41:30.000000 musketeer-1.2.2/musketeer/table.py
--rw-rw-rw-   0        0        0     8918 2023-03-16 16:24:47.000000 musketeer-1.2.2/musketeer/titration.py
--rw-rw-rw-   0        0        0    46737 2023-03-16 16:26:03.000000 musketeer-1.2.2/musketeer/titrationFrame.py
--rw-rw-rw-   0        0        0     8908 2023-02-24 14:27:02.000000 musketeer-1.2.2/musketeer/titrationReader.py
--rw-rw-rw-   0        0        0    17120 2023-03-15 16:30:48.000000 musketeer-1.2.2/musketeer/totalConcentrations.py
--rw-rw-rw-   0        0        0     2903 2023-03-09 17:30:25.000000 musketeer-1.2.2/musketeer/windowsHighDpiPatch.py
-drwxrwxrwx   0        0        0        0 2023-03-16 16:44:22.603243 musketeer-1.2.2/musketeer.egg-info/
--rw-rw-rw-   0        0        0      890 2023-03-16 16:44:20.000000 musketeer-1.2.2/musketeer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      770 2023-03-16 16:44:21.000000 musketeer-1.2.2/musketeer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 16:44:20.000000 musketeer-1.2.2/musketeer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-03-16 16:44:20.000000 musketeer-1.2.2/musketeer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-16 16:44:20.000000 musketeer-1.2.2/musketeer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 16:44:22.610246 musketeer-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1836 2023-03-10 14:26:02.000000 musketeer-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:40:04.397315 musketeer-1.3.0/
+-rw-rw-rw-   0        0        0       66 2023-01-17 16:05:36.000000 musketeer-1.3.0/.flake8
+-rw-rw-rw-   0        0        0       70 2023-06-24 19:22:11.000000 musketeer-1.3.0/.gitignore
+-rw-rw-rw-   0        0        0     1093 2021-05-07 10:14:54.000000 musketeer-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0       35 2021-07-24 12:56:15.000000 musketeer-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      867 2023-06-24 19:40:04.394317 musketeer-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-02-23 14:24:54.000000 musketeer-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 19:40:04.352317 musketeer-1.3.0/musketeer/
+-rw-rw-rw-   0        0        0       23 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/__init__.py
+-rw-rw-rw-   0        0        0    10662 2023-05-04 16:25:02.000000 musketeer-1.3.0/musketeer/__main__.py
+-rw-rw-rw-   0        0        0     1082 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/combineResiduals.py
+-rw-rw-rw-   0        0        0     8000 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/contributingSpecies.py
+-rw-rw-rw-   0        0        0    19032 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/contributors.py
+-rw-rw-rw-   0        0        0     8404 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/editData.py
+-rw-rw-rw-   0        0        0    13925 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/equilibriumConstants.py
+-rw-rw-rw-   0        0        0     8433 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/fitSignals.py
+-rw-rw-rw-   0        0        0    10506 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/knownSignals.py
+-rw-rw-rw-   0        0        0      937 2021-01-06 01:52:42.000000 musketeer-1.3.0/musketeer/logo small.png
+-rw-rw-rw-   0        0        0     5452 2023-06-24 19:16:36.000000 musketeer-1.3.0/musketeer/moduleFrame.py
+-rw-rw-rw-   0        0        0     8875 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/patchMatplotlib.py
+-rw-rw-rw-   0        0        0     1266 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/proportionality.py
+-rw-rw-rw-   0        0        0    12401 2023-05-04 16:25:44.000000 musketeer-1.3.0/musketeer/scrolledFrame.py
+-rw-rw-rw-   0        0        0    22687 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/speciation.py
+-rw-rw-rw-   0        0        0      607 2023-04-19 11:14:04.000000 musketeer-1.3.0/musketeer/style.py
+-rw-rw-rw-   0        0        0    17174 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/table.py
+-rw-rw-rw-   0        0        0     9381 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/titration.py
+-rw-rw-rw-   0        0        0    48125 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/titrationFrame.py
+-rw-rw-rw-   0        0        0     8950 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/titrationReader.py
+-rw-rw-rw-   0        0        0    17120 2023-04-19 11:14:04.000000 musketeer-1.3.0/musketeer/totalConcentrations.py
+-rw-rw-rw-   0        0        0     2903 2023-03-09 17:30:25.000000 musketeer-1.3.0/musketeer/windowsHighDpiPatch.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:40:04.391317 musketeer-1.3.0/musketeer.egg-info/
+-rw-rw-rw-   0        0        0      867 2023-06-24 19:40:03.000000 musketeer-1.3.0/musketeer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2023-06-24 19:40:03.000000 musketeer-1.3.0/musketeer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 19:40:03.000000 musketeer-1.3.0/musketeer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-24 19:40:03.000000 musketeer-1.3.0/musketeer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-24 19:40:03.000000 musketeer-1.3.0/musketeer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 19:40:04.397315 musketeer-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1836 2023-04-19 11:14:04.000000 musketeer-1.3.0/setup.py
```

### Comparing `musketeer-1.2.2/LICENSE` & `musketeer-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `musketeer-1.2.2/PKG-INFO` & `musketeer-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: musketeer
-Version: 1.2.2
+Version: 1.3.0
 Summary: A tool for fitting data from titration experiments.
 Home-page: https://github.com/daniilS/Musketeer
 Author: Daniil Soloviev
 Author-email: dos23@cam.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry
@@ -24,9 +23,7 @@
 ```
 python -m pip install musketeer
 ```
 ### Usage
 ```
 python -m musketeer
 ```
-
-
```

### Comparing `musketeer-1.2.2/musketeer/__main__.py` & `musketeer-1.3.0/musketeer/__main__.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.2.2/musketeer/combineResiduals.py` & `musketeer-1.3.0/musketeer/combineResiduals.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,23 +11,23 @@
     @abstractmethod
     def run(self, residuals):
         pass
 
 
 class ResidualsSum(combineResiduals):
     def run(self, residuals):
-        return np.sum(residuals)
+        return np.sqrt(np.sum(residuals))
 
 
 class ResidualsSumScaled(combineResiduals):
-    # TODO: test
+    # Provided for legacy reasons, not currently recommended
     # sum of the residuals, scaled by the number of data points for each signal
     def run(self, residuals):
         numPoints = self.titration.processedData.count(axis=0)
-        return np.sum(residuals / numPoints)
+        return np.sqrt(np.sum(residuals / numPoints))
 
 
 class ResidualsSumNormalised(combineResiduals):
     def run(self, residuals):
         raise NotImplementedError
```

### Comparing `musketeer-1.2.2/musketeer/editData.py` & `musketeer-1.3.0/musketeer/editData.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,15 @@
             rawData = data[:, 1:]
         elif titration.hasSignalTitles:
             titration.signalTitles = data[0, :]
             rawData = data[1:, :]
         else:
             rawData = data
 
+        rawData = rawData.astype(object)  # to allow setting values to "nan"
         rawData[rawData == ""] = "nan"
         return ma.masked_invalid(rawData.astype(float))
 
     def saveData(self):
         self.titration.rawData = self.processData()
         for param in Params._fields:
             setattr(self.titration, param, getattr(self, param).get())
@@ -212,12 +213,12 @@
             master=self,
             title="Load from CSV",
             filetypes=[("All files", "*.*"), ("CSV files", "*.csv")],
             typevariable=fileType,
         )
         if filePath == "":
             return
-        with open(filePath) as file:
+        with open(filePath, encoding="utf-8-sig") as file:
             d = csv.Sniffer().sniff(file.readline() + file.readline())
             file.seek(0)
             data = list(csv.reader(file, dialect=d))
         self.sheet.set_sheet_data(data)
```

### Comparing `musketeer-1.2.2/musketeer/equilibriumConstants.py` & `musketeer-1.3.0/musketeer/equilibriumConstants.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,19 +164,28 @@
             trans = str.maketrans("0123456789", "⁰¹²³⁴⁵⁶⁷⁸⁹")
             variables = self.rowTitles[1:]
             for globalK, statFactor, variableFactors in zip(
                 self.columnTitles[:-1],
                 self.data[0, :-1],
                 self.data[1:, :-1].T.astype(int),
             ):
-                label = f"Global K for {globalK} = {statFactor}"
+                if (int(statFactor) != 1) or all(variableFactors == 0):
+                    label = f"Global K for {globalK} = {statFactor}"
+                    needsCross = True
+                else:
+                    label = f"Global K for {globalK} ="
+                    needsCross = False
                 for variable, factor in zip(variables, variableFactors):
                     if factor == 0 or factor == "":
                         continue
-                    label += f" × {variable}"
+                    if needsCross:
+                        label += " ×"
+                    else:
+                        needsCross = True
+                    label += f" {variable}"
                     if factor == 1:
                         continue
                     label += str(factor).translate(trans)
                 labels.append(label)
             self.equationsLabel.configure(text="\n".join(labels))
         except Exception:
             pass
@@ -195,20 +204,20 @@
         height = int(self.master.winfo_height() * 0.4)
         self.frame = ttk.Frame(self, height=height)
         self.frame.pack(expand=True, fill="both")
 
         customKsLabel = WrappedLabel(
             self.frame,
             text=(
-                "Each row represents a variable that will be optimised. The global K"
-                " for each complex is the product of a statistical factor and all the"
-                " variables raised to the exponent specified in the cells.\n\nIn the"
-                " final column, specify a value to fix the variable, leave empty to"
-                " optimise the variable, or write ~number to provide an initial guess"
-                " for the optimisation."
+                "Each row represents a variable that will be optimised. Each column"
+                " represents a complex. The global K for each complex is the product of"
+                " a statistical factor, and all the variables raised to the exponents"
+                " specified in that column.\n\nIn the final column, specify a value to"
+                " fix the variable, leave empty to optimise the variable, or write"
+                " ~number to provide an initial guess for the optimisation."
             ),
             padding=5,
         )
         customKsLabel.pack(expand=False, fill="both")
 
         scrolledFrame = ScrolledFrame(self.frame, max_width=1500)
         scrolledFrame.pack(expand=True, fill="both")
@@ -270,14 +279,15 @@
         "statisticalFactors",
         "kNames",
         "knownKs",
         "initialKs",
     )
 
     def run(self, kVars):
+        # print(kVars)
         # microKs as a column vector, with the unknown values filled in
         microKs = self.knownKs.copy()
         microKs[self.knownMask] = kVars
         microKs = np.atleast_2d(microKs).T
 
         # perform the calculation as previewed in the popup
         globalKs = self.statisticalFactors * np.prod(microKs**self.ksMatrix, 0)
```

### Comparing `musketeer-1.2.2/musketeer/logo small.png` & `musketeer-1.3.0/musketeer/logo small.png`

 * *Files identical despite different names*

### Comparing `musketeer-1.2.2/musketeer/moduleFrame.py` & `musketeer-1.3.0/musketeer/moduleFrame.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.2.2/musketeer/patchMatplotlib.py` & `musketeer-1.3.0/musketeer/patchMatplotlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 import tkinter as tk
 import tkinter.ttk as ttk
 
 import matplotlib
 from matplotlib import cbook, offsetbox
 from matplotlib.backend_bases import NavigationToolbar2, _Mode, cursors
 from matplotlib.backends._backend_tk import (
@@ -139,20 +140,24 @@
 def __init__(self, ref_artist, use_blit=False):
     self.ref_artist = ref_artist
     if not ref_artist.pickable():
         ref_artist.set_picker(True)
     self.got_artist = False
     self._hover = False
     self._use_blit = use_blit and self.canvas.supports_blit
-    self.cids = [
-        self.canvas.callbacks._connect_picklable("pick_event", self.on_pick),
-        self.canvas.callbacks._connect_picklable(
-            "button_release_event", self.on_release
-        ),
-        self.canvas.callbacks._connect_picklable("motion_notify_event", self.on_motion),
+    callbacks = ref_artist.figure._canvas_callbacks
+    self._disconnectors = [
+        functools.partial(
+            callbacks.disconnect, callbacks._connect_picklable(name, func)
+        )
+        for name, func in [
+            ("pick_event", self.on_pick),
+            ("button_release_event", self.on_release),
+            ("motion_notify_event", self.on_motion),
+        ]
     ]
 
 
 def on_motion(self, evt):
     # Only check if the widget lock is available, setting it would prevent
     # picking.
     if not (self._check_still_parented() and self.canvas.widgetlock.available(self)):
@@ -211,16 +216,16 @@
 
         if self._use_blit:
             self.ref_artist.set_animated(False)
 
 
 def disconnect(self):
     """Disconnect the callbacks."""
-    for cid in self.cids:
-        self.canvas.mpl_disconnect(cid)
+    for disconnector in self._disconnectors:
+        disconnector()
     if self._hover:
         self.canvas.set_cursor(cursors.POINTER)
 
 
 original_scroll_event_windows = FigureCanvasTk.scroll_event_windows
 
 
@@ -232,16 +237,19 @@
 
 def applyPatch():
     # makes buttons use ttk widgets
     NavigationToolbar2Tk._Button = _Button
     NavigationToolbar2Tk._Spacer = _Spacer
     NavigationToolbar2Tk._update_buttons_checked = _update_buttons_checked
 
-    # implements PR #25412
+    # implements PR #25412, and #25442 below mpl version 3.7.2
     offsetbox.DraggableBase.__init__ = __init__
+    offsetbox.DraggableBase.cids = property(
+        lambda self: [disconnect.args[0] for disconnect in self._disconnectors[:2]]
+    )
     offsetbox.DraggableBase.on_motion = on_motion
     offsetbox.DraggableBase.on_pick = on_pick
     offsetbox.DraggableBase.on_release = on_release
     offsetbox.DraggableBase.disconnect = disconnect
     # implements PR #25413
     cursord[cursors.SELECT_REGION] = "crosshair"
```

### Comparing `musketeer-1.2.2/musketeer/scrolledFrame.py` & `musketeer-1.3.0/musketeer/scrolledFrame.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.2.2/musketeer/speciation.py` & `musketeer-1.3.0/musketeer/totalConcentrations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,445 +1,500 @@
+import re
+import tkinter as tk
 import tkinter.ttk as ttk
 from abc import abstractmethod
+from decimal import Decimal
 
 import numpy as np
 from numpy import ma
 
 from . import moduleFrame
 from .scrolledFrame import ScrolledFrame
-from .table import ButtonFrame, Table
+from .table import ButtonFrame, Table, WrappedLabel
 
+DEFAULT_INITIAL_CONC = 1e-4
 
-def stoichiometriesToBoundNames(freeNames, stoichiometries, polymerMode):
-    polymerModes = ("unchanged", "dimer+polymer", "terminal+internal")
+prefixesDecimal = {
+    "": Decimal(1),
+    "m": Decimal(1e-3),
+    "u": Decimal(1e-6),
+    "μ": Decimal(1e-6),
+    "n": Decimal(1e-9),
+}
+
+prefixes = dict([key, float(value)] for key, value in prefixesDecimal.items())
+
+
+def convertConc(conc, fromUnit, toUnit):
+    if conc is ma.masked:
+        return ""
+    conc = Decimal(conc)
+    convertedConc = float(
+        conc * prefixesDecimal[fromUnit.strip("M")] / prefixesDecimal[toUnit.strip("M")]
+    )
+    return f"{convertedConc:g}"  # strip trailing zeroes
+
+
+class totalConcentrations(moduleFrame.Strategy):
+    requiredAttributes = (
+        "concsUnit",
+        "totalConcs",
+        "freeNames",
+        "variableNames",
+    )
 
-    if polymerMode not in polymerModes:
-        raise ValueError(
-            f"Unknown polymer mode {polymerMode}: must be one of {polymerModes}."
-        )
-    trans = str.maketrans("0123456789", "₀₁₂₃₄₅₆₇₈₉")
-
-    boundNames = []
-    for row in stoichiometries:
-        boundName = ""
-        for freeName, stoichiometry in zip(freeNames, row):
-            if stoichiometry == 0:
-                continue
-
-            if boundName != "":
-                boundName += "·"
-
-            if stoichiometry == 1:
-                boundName += freeName
-            elif stoichiometry == -1:
-                boundName += freeName + "ₙ"
-            else:
-                boundName += freeName + str(stoichiometry).translate(trans)
-        if "ₙ" in boundName and polymerMode == "dimer+polymer":
-            # insert a dimer before the polymer entry
-            boundNames.append(boundName.replace("ₙ", "₂"))
-            boundNames.append(boundName)
-        elif "ₙ" in boundName and polymerMode == "terminal+internal":
-            # separate the terminal and internal parts of the polymer
-            boundNames.append(boundName + " terminal")
-            boundNames.append(boundName + " internal")
-        else:
-            boundNames.append(boundName)
-    return np.array(boundNames)
-
-
-class Speciation(moduleFrame.Strategy):
-    requiredAttributes = ("stoichiometries",)
-
-    @abstractmethod
-    def run(self, variables, totalConcs):
-        pass
-
-    # Other modules need to access freeNames and freeCount, but totalConcentrations
-    # may not yet be loaded.
+    # TODO: support entering initial guesses
     @property
-    def freeNames(self):
-        try:
-            return self.titration.totalConcentrations.freeNames
-        except AttributeError:
-            return np.array(["Host", "Guest"])
+    def variableInitialGuesses(self):
+        return np.full(len(self.variableNames), DEFAULT_INITIAL_CONC)
 
     @property
     def freeCount(self):
         return len(self.freeNames)
 
-    @property
-    def boundCount(self):
-        return self.stoichiometries.shape[0]
-
-    @property
-    def speciesCount(self):
-        return self.freeCount + self.boundCount
+    @abstractmethod
+    def run(self, totalConcVars):
+        pass
 
-    @property
-    def polymerIndices(self):
-        return np.any(self.stoichiometries < 0, 1)
 
-    @property
-    def polymerCount(self):
-        return np.count_nonzero(self.stoichiometries < 0)
+class StockTable(Table):
+    def __init__(self, master, titration):
+        try:
+            stockTitles = titration.totalConcentrations.stockTitles
+        except AttributeError:
+            stockTitles = ("Stock 1", "Stock 2")
 
-    @property
-    def complexCount(self):
-        return self.boundCount - self.polymerCount
+        try:
+            freeNames = titration.totalConcentrations.freeNames
+        except AttributeError:
+            freeNames = ("Host", "Guest")
 
-    @property
-    def boundNames(self):
-        return stoichiometriesToBoundNames(
-            self.freeNames,
-            self.stoichiometries,
-            "unchanged",
+        super().__init__(
+            master,
+            2,
+            0,
+            stockTitles,
+            maskBlanks=True,
+            rowOptions=("titles", "new", "delete"),
+            columnOptions=("titles", "new", "delete"),
         )
 
-    @property
-    def variableNames(self):
-        return stoichiometriesToBoundNames(
-            self.freeNames,
-            self.stoichiometries,
-            "dimer+polymer",
+        self.titration = titration
+
+        self.label(0 - self.headerGridRows, 0, "Stock concentrations:", 4)
+        self.label(1 - self.headerGridRows, 2, "Unit:")
+        _, self.concsUnit = self.dropdown(
+            1 - self.headerGridRows, 3, ("nM", "μM", "mM", "M"), "mM"
         )
+        try:
+            self.concsUnit.set(titration.totalConcentrations.concsUnit)
+        except AttributeError:
+            pass
 
-    @property
-    def outputNames(self):
-        return np.append(
-            self.freeNames,
-            stoichiometriesToBoundNames(
-                self.freeNames,
-                self.stoichiometries,
-                "terminal+internal",
-            ),
-        )
-
-    def variablesToKs(self, variables):
-        # The rest of the UI should be agnostic towards the treatment of polymers, so
-        # this function is used to separate out the double K values (dimer and 3+_mer)
-        # for polymers.
-        ks = np.empty(self.boundCount)
-        polymerKs = np.empty(self.boundCount)
-
-        polymersCounted = 0
-        for i in range(self.boundCount):
-            ks[i] = variables[i + polymersCounted]
-            if self.polymerIndices[i]:
-                polymerKs[i] = variables[i + polymersCounted + 1]
-                polymersCounted += 1
-        polymerKs = ma.masked_array(polymerKs, ~self.polymerIndices)
-        if not len(variables) == self.boundCount + polymersCounted:
-            raise ValueError(
-                f"Expected {self.boundCount + polymersCounted} variables, got"
-                f" {len(variables)}."
+        try:
+            self.populate(freeNames, titration.totalConcentrations.stockConcs)
+        except AttributeError:
+            self.populateDefault(freeNames)
+
+    def populate(self, freeNames, stockConcs):
+        for name, row in zip(freeNames, stockConcs):
+            self.addRow(
+                name, [convertConc(conc, "M", self.concsUnit.get()) for conc in row]
             )
-        return ks, polymerKs
+
+    def populateDefault(self, freeNames):
+        for name in freeNames:
+            self.addRow(name)
 
 
-class SpeciationTable(Table):
+class VolumesTable(Table):
     def __init__(self, master, titration):
+        try:
+            stockTitles = titration.totalConcentrations.stockTitles
+        except AttributeError:
+            stockTitles = ("Stock 1", "Stock 2")
         super().__init__(
             master,
-            0,
-            0,
-            titration.totalConcentrations.freeNames,
-            rowOptions=("readonlyTitles", "new", "delete"),
-            columnOptions=("readonlyTitles",),
-            boldTitles=True,
-            callback=self.updateTitles,
+            2,
+            2,
+            stockTitles,
+            rowOptions=("readonlyTitles", "delete"),
+            columnOptions=(),
         )
-        for boundName, stoichiometry in zip(
-            titration.speciation.boundNames, titration.speciation.stoichiometries
-        ):
-            self.addRow(boundName, stoichiometry)
 
-    def updateTitles(self, *args, **kwargs):
-        for cell, title in zip(
-            self.cells[2 : self.headerCells :, 1], self.columnTitles
-        ):
-            cell.set(title)
+        self.titration = titration
 
-        self.rowTitles = stoichiometriesToBoundNames(
-            self.columnTitles, self.data, polymerMode="unchanged"
+        self.label(0 - self.headerGridRows, 0, "Cumulative addition volumes:", 4)
+        self.label(1 - self.headerGridRows, 2, "Unit:")
+        _, self.volumesUnit = self.dropdown(
+            1 - self.headerGridRows, 3, ("nL", "μL", "mL", "L"), "μL"
         )
+        try:
+            self.volumesUnit.set(titration.totalConcentrations.volumesUnit)
+        except AttributeError:
+            pass
 
-    def addFreeRow(self, index=-1):
-        row = self.cells.shape[0]
-        freeRow = np.full(self.cells.shape[1], None)
+        self.readonlyEntry(self.headerCells - 1, 1, "Addition title:", align="left")
 
-        freeRow[0] = self.deleteRowButton(row, 0, "Delete Row", state="disabled")
-        freeRow[1] = self.readonlyEntry(
-            row, 1, self.columnTitles[index], font=self.titleFont
-        )
-
-        freeRow[2:] = [
-            self.readonlyEntry(row, 2 + column, "0", align="right")
-            for column in range(self.cells.shape[1] - 2)
-        ]
-        freeRow[-1].set("1")
+        if (
+            self.titration.totalConcentrations is not None
+            and hasattr(titration.totalConcentrations, "volumes")
+            and (
+                self.titration.totalConcentrations.volumes.shape[0]
+                == len(self.titration.additionTitles)
+            )
+        ):
+            self.populate(titration.totalConcentrations.volumes)
+        else:
+            self.populateDefault()
 
-        self.cells = np.insert(self.cells, self.headerCells, freeRow, axis=0)
-        self.headerCells += 1
+    # TODO: instead make the columnspan of the titles 2
+    def deleteRowButton(self, *args, **kwargs):
+        button = super().deleteRowButton(*args, **kwargs)
+        button.state(["disabled"])
+        return button
+
+    def populate(self, volumes):
+        for name, row in zip(self.titration.additionTitles, volumes):
+            self.addRow(
+                name,
+                [
+                    self.convertVolume(volume, "L", self.volumesUnit.get())
+                    for volume in row
+                ],
+            )
 
-        self.redraw()
+    def populateDefault(self):
+        for name in self.titration.additionTitles:
+            self.addRow(name)
 
     def addColumn(self, firstEntry="", data=None):
         super().addColumn(firstEntry, data)
-
-        for row in range(2, self.headerCells):
-            self.cells[row, -1] = self.readonlyEntry(
-                row, self.cells.shape[-1], "0", align="right"
+        column = self.cells.shape[1] - 1
+        copyFirstButton = self.button(self.headerCells - 2, column, "Copy first")
+        copyFirstButton.configure(
+            command=lambda button=copyFirstButton: self.copyFirst(
+                button.grid_info()["column"]
             )
+        )
+        self.cells[self.headerCells - 2, column] = copyFirstButton
 
-        self.addFreeRow()
+        copyTitlesButton = self.button(self.headerCells - 1, column, "Copy from titles")
+        copyTitlesButton.configure(
+            command=lambda button=copyTitlesButton: self.copyFromTitles(
+                button.grid_info()["column"]
+            )
+        )
+        self.cells[self.headerCells - 1, column] = copyTitlesButton
 
-    def deleteColumn(self, column):
-        super().deleteColumn(column)
-        self.headerCells -= 1
-        self.deleteRow(column)
-        self.updateTitles()
-
-    def convertData(self, number):
-        if number == "n":
-            return -1
-        elif number == "":
-            return 0
-        else:
-            return int(number)
+    def copyFirst(self, column):
+        cells = self.cells[self.headerCells :, column]
+        first = cells[0].get()
+        for cell in cells:
+            cell.set(first)
+
+    def copyFromTitles(self, column):
+        cells = self.cells[self.headerCells :]
+        for row in cells:
+            title = row[1].get()
+            volume = self.getVolumeFromString(title, self.volumesUnit.get())
+            if volume is not None:
+                row[column].set(volume)
+
+    def getVolumeFromString(self, string, toUnit="L"):
+        searchResult = re.search(r"([0-9.]+) ?([nuμm]?)[lL]", string)
+        if not searchResult:
+            return None
+        volume, prefix = searchResult.group(1, 2)
+        return self.convertVolume(volume, prefix, toUnit)
+
+    def convertVolume(self, volume, fromUnit, toUnit):
+        volume = Decimal(volume)
+        convertedVolume = float(
+            volume
+            * prefixesDecimal[fromUnit.strip("L")]
+            / prefixesDecimal[toUnit.strip("L")]
+        )
+        return f"{convertedVolume:g}"  # strip trailing zeroes
 
 
-class SpeciationPopup(moduleFrame.Popup):
+class VolumesPopup(moduleFrame.Popup):
     def __init__(self, titration, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.titration = titration
-        self.title("Enter speciation table")
+        self.title("Enter volumes")
 
-        height = int(self.master.winfo_height() * 0.4)
+        height = int(self.master.winfo_height() * 0.8)
         frame = ScrolledFrame(self, height=height, max_width=1500)
         frame.pack(expand=True, fill="both")
 
-        self.innerFrame = frame.display_widget(ttk.Frame, stretch=True)
-
-        self.speciationTable = SpeciationTable(self.innerFrame, titration)
-        self.speciationTable.pack(expand=True, fill="both")
+        innerFrame = frame.display_widget(ttk.Frame, stretch=True)
 
-        buttonFrame = ButtonFrame(
-            self.innerFrame, self.reset, self.saveData, self.destroy
+        unknownConcsFrame = ttk.Frame(innerFrame, borderwidth=5)
+        unknownConcsFrame.pack(expand=True, fill="both")
+        unknownConcsLabel = WrappedLabel(
+            unknownConcsFrame,
+            text="Leave cells blank to optimise that concentration as a variable.\n",
         )
-        buttonFrame.pack(expand=False, fill="both", side="bottom")
+        unknownConcsLabel.pack(expand=False, fill="both")
+        self.unknownTotalConcsLinkedVar = tk.BooleanVar()
+        try:
+            self.unknownTotalConcsLinkedVar.set(
+                self.titration.totalConcentrations.unknownTotalConcsLinked
+            )
+        except AttributeError:
+            self.unknownTotalConcsLinkedVar.set(True)
+        unknownTotalConcsCheckbutton = ttk.Checkbutton(
+            unknownConcsFrame,
+            variable=self.unknownTotalConcsLinkedVar,
+            text="Link unknown concentrations in the same row?",
+        )
+        unknownTotalConcsCheckbutton.pack()
+
+        self.stockTable = StockTable(innerFrame, titration)
+        self.stockTable.pack(expand=True, fill="both")
+        self.volumesTable = VolumesTable(innerFrame, titration)
+        self.volumesTable.pack(expand=True, fill="both")
+
+        self.stockTable.newColumnButton.configure(command=self.addColumns)
+        self.stockTable._deleteColumn = self.stockTable.deleteColumn
+        self.stockTable.deleteColumn = self.deleteColumns
+
+        buttonFrame = ButtonFrame(innerFrame, self.reset, self.saveData, self.destroy)
+        buttonFrame.pack(expand=False, fill="both")
+
+    def addColumns(self):
+        self.stockTable.addColumn()
+        self.volumesTable.addColumn()
+
+    def deleteColumns(self, column):
+        self.stockTable._deleteColumn(column)
+        self.volumesTable.deleteColumn(column)
 
     def reset(self):
-        self.speciationTable.destroy()
-        self.speciationTable = SpeciationTable(self.innerFrame, self.titration)
-        self.speciationTable.pack(expand=True, fill="both")
+        for table in (self.stockTable, self.volumesTable):
+            table.resetData()
+            table.columnTitles = ("Stock 1", "Stock 2")
+            table.populateDefault()
 
     def saveData(self):
-        self.stoichiometries = self.speciationTable.data
+        self.freeNames = self.stockTable.rowTitles
+
+        self.stockTitles = self.stockTable.columnTitles
+        self.unknownTotalConcsLinked = self.unknownTotalConcsLinkedVar.get()
+
+        self.concsUnit = self.stockTable.concsUnit.get()
+        self.stockConcs = self.stockTable.data * prefixes[self.concsUnit.strip("M")]
+
+        self.volumesUnit = self.volumesTable.volumesUnit.get()
+        self.volumes = self.volumesTable.data * prefixes[self.volumesUnit.strip("L")]
 
         self.saved = True
         self.destroy()
 
 
-class SpeciationDimerisation(Speciation):
-    freeNames = np.array(["Host"])
-    stoichiometries = np.array([[2]])
-
-    def run(self, variables, totalConcs):
-        K = variables[0]
-        Htot = totalConcs.T[0]
-        H = (-1 + np.sqrt(1 + 8 * Htot * K)) / (4 * K)
-        H2 = (1 + 4 * Htot * K - np.sqrt(1 + 8 * Htot * K)) / (8 * K)
-
-        free = np.atleast_2d(H).T
-        bound = np.atleast_2d(H2).T
-        return free, bound
-
-
-class SpeciationHG(Speciation):
-    stoichiometries = np.array([[1, 1]])
-
-    def run(self, variables, totalConcs):
-        K = variables[0]
-        Htot, Gtot = totalConcs.T
-        H = (
-            np.sqrt(
-                Gtot**2 * K**2 - 2 * Gtot * K * (Htot * K - 1) + (Htot * K + 1) ** 2
-            )
-            - Gtot * K
-            + Htot * K
-            - 1
-        ) / (2 * K)
-        G = (
-            np.sqrt(
-                Htot**2 * K**2 - 2 * Htot * K * (Gtot * K - 1) + (Gtot * K + 1) ** 2
-            )
-            - Htot * K
-            + Gtot * K
-            - 1
-        ) / (2 * K)
-        HG = H * G * K
-
-        free = np.vstack((H, G)).T
-        bound = np.atleast_2d(HG).T
-        return free, bound
-
-
-class SpeciationCOGS(Speciation):
-    # TODO: see if this can be sped up using numba
-    def COGS(self, M, y, ks, polymerKs):
-        free = y.copy()
-        bound = np.empty(len(ks))
-        polymers = np.any(M < 0, 1)
-        # the index of the species making up each of the polymers
-        polymerParents = np.nonzero(M[polymers])[1]
-        complexes = ~polymers
-
-        P = np.empty(len(ks))
-        P[complexes] = np.sum(M[complexes, :], 1)
-        P[polymers] = 2 * ks[polymers] * y[polymerParents]
-        P = 1 / max(P)
-        tol = 1e-7
-        while True:
-            bound[complexes] = ks[complexes] * np.prod(free ** M[complexes, :], 1)
-            # cap the maximum guess to avoid divergence
-            bound[polymers] = np.where(
-                free[polymerParents] * polymerKs[polymers] >= 1,
-                free[polymerParents] ** 2 * polymerKs[polymers] / P,
-                (2 - polymerKs[polymers] * free[polymerParents])
-                * (ks[polymers] * free[polymerParents] ** 2)
-                / ((1 - polymerKs[polymers] * free[polymerParents]) ** 2),
-            )
-            total = free + abs(M.T) @ bound  # total concentrations of species
-            if all((total - y) <= tol * y):
-                break
-            # to handle 0 total concentration
-            invTotal = np.where(total == 0, 1, 1 / total)
-            free *= (y * invTotal) ** P
-
-        # For polymers, return separate entries for terminal and internal groups
-        bound = []
-        paddedPolymerParents = ma.array(np.empty(len(ks)), mask=True)
-        paddedPolymerParents[polymers] = polymerParents
-        for k, polymerK, stoichiometries, isPolymer, parent in zip(
-            ks, polymerKs, M, self.polymerIndices, paddedPolymerParents
+class GetTotalConcsFromVolumes(totalConcentrations):
+    Popup = VolumesPopup
+    popupAttributes = (
+        "stockTitles",
+        "unknownTotalConcsLinked",
+        "concsUnit",
+        "stockConcs",
+        "volumesUnit",
+        "volumes",
+        "freeNames",
+    )
+
+    def run(self, totalConcVars):
+        stockConcs = np.copy(self.stockConcs)
+        if self.unknownTotalConcsLinked:
+            # For each row (= species), all blank cells are assigned to a
+            # single unknown variable.
+            for rowIndex, totalConcVar in zip(
+                np.where(self.rowsWithBlanks)[0], totalConcVars
+            ):
+                stockConcs[rowIndex, np.isnan(stockConcs[rowIndex])] = totalConcVar
+        else:
+            stockConcs[np.isnan(stockConcs)] = totalConcVars
+
+        moles = self.volumes @ stockConcs.T
+        totalVolumes = np.atleast_2d(np.sum(self.volumes, 1)).T
+        totalConcs = moles / totalVolumes
+
+        return totalConcs
+
+    @property
+    def totalConcs(self):
+        # If all total concentrations are known, they can be used by other strategies.
+        if len(self.variableNames) != 0:
+            return np.empty((0, 0))
+        else:
+            return self.run(np.empty((0,)))
+
+    @property
+    def rowsWithBlanks(self):
+        return np.any(ma.getmaskarray(self.stockConcs), axis=1)
+
+    @property
+    def variableNames(self):
+        if self.unknownTotalConcsLinked:
+            # return the number of rows (= species) with blank cells
+            concVarsNames = self.freeNames[self.rowsWithBlanks]
+            return np.array([f"[{name}]" for name in concVarsNames])
+        else:
+            concVarsNames = []
+            for freeName, concs in zip(self.freeNames, self.stockConcs):
+                concVarsNames.extend(
+                    [
+                        f"[{freeName}] in {stock}"
+                        for stock in self.stockTitles[ma.getmaskarray(concs)]
+                    ]
+                )
+            return np.array(concVarsNames)
+
+
+class ConcsTable(Table):
+    # TODO: merge with VolumesTable
+    def __init__(self, master, titration):
+        self.titration = titration
+
+        try:
+            freeNames = titration.totalConcentrations.freeNames
+        except AttributeError:
+            freeNames = ("Host", "Guest")
+
+        super().__init__(
+            master,
+            2,
+            2,
+            freeNames,
+            rowOptions=("readonlyTitles",),
+            columnOptions=("titles", "new", "delete"),
+        )
+
+        self.populateDefault()
+
+    def populateDefault(self):
+        self.label(0 - self.headerGridRows, 0, "Concentrations:", 4)
+        self.label(1 - self.headerGridRows, 2, "Unit:")
+        _, self.concsUnit = self.dropdown(
+            1 - self.headerGridRows, 3, ("nM", "μM", "mM", "M"), "mM"
+        )
+
+        self.readonlyEntry(self.headerCells - 1, 1, "Addition title:", align="left")
+
+        if (
+            self.titration.totalConcentrations is not None
+            and self.titration.totalConcentrations.totalConcs.shape[0]
+            == len(self.titration.additionTitles)
         ):
-            if not isPolymer:
-                bound.append(k * np.prod(free**stoichiometries))
-            else:
-                # terminal
-                bound.append(2 * free[parent] ** 2 * k / (1 - free[parent] * polymerK))
-                # internal
-                bound.append(
-                    (free[parent] ** 3 * k * polymerK)
-                    / (1 - free[parent] * polymerK) ** 2
+            self.concsUnit.set(self.titration.totalConcentrations.concsUnit)
+            for name, row in zip(
+                self.titration.additionTitles,
+                self.titration.totalConcentrations.totalConcs,
+            ):
+                self.addRow(
+                    name, [convertConc(conc, "M", self.concsUnit.get()) for conc in row]
                 )
+        else:
+            for name in self.titration.additionTitles:
+                self.addRow(name)
 
-        return free, np.array(bound)
+    def addColumn(self, firstEntry="", data=None):
+        super().addColumn(firstEntry, data)
+        column = self.cells.shape[1] - 1
+        copyFirstButton = self.button(self.headerCells - 2, column, "Copy first")
+        copyFirstButton.configure(
+            command=lambda button=copyFirstButton: self.copyFirst(
+                button.grid_info()["column"]
+            )
+        )
+        self.cells[self.headerCells - 2, column] = copyFirstButton
 
-    def run(self, variables, totalConcs):
-        ks, polymerKs = self.variablesToKs(variables)
-        numPoints = totalConcs.shape[0]
-        free = np.zeros((numPoints, self.titration.totalConcentrations.freeCount))
-        bound = np.zeros((numPoints, self.complexCount + 2 * self.polymerCount))
-        for i in range(numPoints):
-            free[i], bound[i] = self.COGS(
-                self.stoichiometries, totalConcs[i], ks, polymerKs
+        copyTitlesButton = self.button(self.headerCells - 1, column, "Copy from titles")
+        copyTitlesButton.configure(
+            command=lambda button=copyTitlesButton: self.copyFromTitles(
+                button.grid_info()["column"]
             )
-        return free, bound
+        )
+        self.cells[self.headerCells - 1, column] = copyTitlesButton
 
+    def copyFirst(self, column):
+        cells = self.cells[self.headerCells :, column]
+        first = cells[0].get()
+        for cell in cells:
+            cell.set(first)
+
+    def copyFromTitles(self, column):
+        cells = self.cells[self.headerCells :]
+        for row in cells:
+            title = row[1].get()
+            conc = self.getConcFromString(title, self.concsUnit.get())
+            if conc is not None:
+                row[column].set(conc)
+
+    def getConcFromString(self, string, toUnit="M"):
+        searchResult = re.search(r"([0-9.]+) ?([nuμm]?)M", string)
+        if not searchResult:
+            return None
+        conc, prefix = searchResult.group(1, 2)
+        return convertConc(conc, prefix, toUnit)
 
-"""
-class SpeciationSolver:
-    def __init__(self, parent):
-        self.parent = parent
-
-    def speciationLog(self, logFree, ks, total, M):
-        free = 10 ** logFree
-        return (
-            np.sum(free)
-            - total @ logFree * 2.30258509299
-            + ks @ np.prod(free ** M.T, 1)
-        )
-
-    def jacobianCalculatorLog(self, logFree, ks, total, M):
-        free = 10 ** logFree
-        return ((M @ (ks * np.prod(free ** M.T, 1))) + free - total) * 2.30258509299
-
-    def getLowerBounds(self, ks, total, M):
-        return np.log10(total ** 2 / (total + M @ (ks * np.prod(total ** M.T, 1))))
-
-    def getUpperBounds(self, ks, total, M):
-        return np.log10(total)
-
-    def run(self, ks, alphas, totalConcs):
-        numPoints = totalConcs.shape[0]
-        M = self.parent.stoichiometries
-        free = np.empty((numPoints, M.shape[1]))
-        bound = np.empty((numPoints, M.shape[0]))
-
-        for i in range(numPoints):
-            additionTotalConcs = totalConcs[i]
-
-            # Filter the to exclude species and complexes that will have a concentration
-            # of 0
-            zeroTotalConcs = additionTotalConcs == 0
-            zeroBound = np.any(self.parent.stoichiometries[:, zeroTotalConcs], 1)
-            filteredKs = ks[~zeroBound]
-            filteredTotal = additionTotalConcs[~zeroTotalConcs]
-            filteredM = self.parent.stoichiometries[~zeroBound, :][:, ~zeroTotalConcs]
-
-            lb = self.getLowerBounds(filteredKs, filteredTotal, filteredM)
-            ub = self.getLowerBounds(filteredKs, filteredTotal, filteredM)
-
-            logFree = minimize(
-                self.speciationLog,
-                x0=ub,
-                args=(filteredKs, filteredTotal, filteredM),
-                jac=self.jacobianCalculatorLog,
-                bounds=np.vstack((lb, ub)).T,
-                tol=1e-8 / 10 ** (len(filteredTotal)),
-            ).x
-
-            free[i, ~zeroTotalConcs] = 10 ** logFree
-            free[i, zeroTotalConcs] = 0
-
-            # get the concentrations of the bound species from those of the free
-            bound[i] = ks * np.prod(free[i] ** M, 1)
-        return free, bound
-
-
-class speciationGrad(moduleFrame.Strategy):
-    def run(self, ks, alphas, totalConcs):
-        if self.polymerCount == 0:
-            algorithm = SpeciationAlgorithm()
-        else:
-            algorithm = SpeciationAlgorithmWithPolymers()
-        return algorithm.run(ks, alphas, totalConcs)
 
+class ConcsPopup(moduleFrame.Popup):
+    def __init__(self, titration, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.titration = titration
+        self.title("Enter concentrations")
+
+        height = int(self.master.winfo_height() * 0.8)
+        frame = ScrolledFrame(self, height=height, max_width=1500)
+        frame.pack(expand=True, fill="both")
+
+        innerFrame = frame.display_widget(ttk.Frame, stretch=True)
+
+        self.concsTable = ConcsTable(innerFrame, titration)
+        self.concsTable.pack(expand=True, fill="both")
 
-class SpeciationCustomGrad(speciationGrad):
-    Popup = SpeciationPopup
-    popupAttributes = ("stoichiometries", "freeNames", "boundNames")
-"""
+        buttonFrame = ButtonFrame(innerFrame, self.reset, self.saveData, self.destroy)
+        buttonFrame.pack(expand=False, fill="both")
+
+    def reset(self):
+        self.concsTable.resetData()
+        try:
+            self.concsTable.columnTitles = self.titration.totalConcentrations.freeNames
+        except AttributeError:
+            self.concsTable.columnTitles = ("Host", "Guest")
+        self.concsTable.populateDefault()
+
+    def saveData(self):
+        self.concsUnit = self.concsTable.concsUnit.get()
+        self.totalConcs = self.concsTable.data * prefixes[self.concsUnit.strip("M")]
+        self.freeNames = self.concsTable.columnTitles
+
+        self.saved = True
+        self.destroy()
 
 
-class SpeciationHG2(SpeciationCOGS):
-    stoichiometries = np.array([[1, 1], [1, 2]])
+class GetTotalConcs(totalConcentrations):
+    Popup = ConcsPopup
+    popupAttributes = (
+        "concsUnit",
+        "totalConcs",
+        "freeNames",
+    )
 
+    def run(self, totalConcVars):
+        return self.totalConcs
 
-class SpeciationCustom(SpeciationCOGS):
-    Popup = SpeciationPopup
-    popupAttributes = ("stoichiometries",)
+    variableNames = np.array([])
 
 
 class ModuleFrame(moduleFrame.ModuleFrame):
-    group = "Equilibria"
-    dropdownLabelText = "Select a binding isotherm:"
+    group = "Experiment"
+    dropdownLabelText = "Enter concentrations or volumes:"
     dropdownOptions = {
-        "1:1 binding": SpeciationHG,
-        "1:2 binding": SpeciationHG2,
-        "Dimerisation": SpeciationDimerisation,
-        "Custom": SpeciationCustom,
-        # "Custom Grad": SpeciationCustomGrad,
+        "Volumes": GetTotalConcsFromVolumes,
+        "Concentrations": GetTotalConcs,
     }
-    attributeName = "speciation"
+    attributeName = "totalConcentrations"
+    setDefault = False
```

### Comparing `musketeer-1.2.2/musketeer/style.py` & `musketeer-1.3.0/musketeer/style.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.2.2/musketeer/table.py` & `musketeer-1.3.0/musketeer/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from . import style
 from .style import cellWidth, padding
 
 
 class Table(ttk.Frame):
     width = cellWidth
+    rowTitleWidth = None
 
     titleFont = None
     italicFont = None
     fitToText = "New column"
 
     def __init__(
         self,
@@ -85,19 +86,20 @@
         row,
         column,
         text="",
         align="left",
         columnspan=1,
         *,
         addCallback=True,
+        width=None,
         **kwargs,
     ):
         entry = ttk.Entry(
             self,
-            width=self.width * columnspan,
+            width=width or self.width * columnspan,
             justify=align,
             **kwargs,
         )
 
         entry.stringVar = tk.StringVar(entry)
         entry.configure(textvariable=entry.stringVar)
         if self.callback is not None and addCallback:
@@ -227,20 +229,25 @@
         for (row, column), cell in np.ndenumerate(self.cells):
             if cell is not None:
                 cell.grid(row=self.headerGridRows + row, column=column)
 
     def addRow(self, firstEntry="", data=None):
         row = self.cells.shape[0]
         newRow = np.full(self.cells.shape[1], None)
+        rowTitleWidth = self.rowTitleWidth or self.width
         if "delete" in self.rowOptions:
             newRow[0] = self.deleteRowButton(row, 0, "Delete Row")
         if "readonlyTitles" in self.rowOptions:
-            newRow[1] = self.readonlyEntry(row, 1, firstEntry, font=self.titleFont)
+            newRow[1] = self.readonlyEntry(
+                row, 1, firstEntry, font=self.titleFont, width=rowTitleWidth
+            )
         elif "titles" in self.rowOptions:
-            newRow[1] = self.entry(row, 1, firstEntry, font=self.titleFont)
+            newRow[1] = self.entry(
+                row, 1, firstEntry, font=self.titleFont, width=rowTitleWidth
+            )
         for column in range(self.cells.shape[1] - 2):
             entry = self.entry(row, 2 + column, align="right")
             if data is not None:
                 entry.set(data[column])
             newRow[2 + column] = entry
 
         self.cells = np.vstack((self.cells, newRow))
```

### Comparing `musketeer-1.2.2/musketeer/titration.py` & `musketeer-1.3.0/musketeer/titration.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,18 @@
             return self.signalTitles[self.columnFilter]
         else:
             return np.array(
                 ["Signal " + str(i + 1) for i in range(self.processedData.shape[1])]
             )
 
     @property
+    def processedSignalCount(self):
+        return self.processedData.shape[1]
+
+    @property
     def signalTitles(self):
         if self.hasSignalTitles:
             return self._signalTitles
         else:
             return np.array(
                 ["Signal " + str(i + 1) for i in range(self.rawData.shape[1])]
             )
@@ -148,19 +152,23 @@
     def additionTitles(self, additionTitles):
         if additionTitles.size == 0:
             return
         self.hasAdditionTitles = True
         self._additionTitles = additionTitles
 
     def getPeakIndices(self, maxPeaks=4, maxShoulderPeaks=2, threshold=0.1):
+        numSignals = self.processedData.shape[1]
+        if numSignals <= maxPeaks + maxShoulderPeaks:
+            return np.arange(numSignals)
         # get the total movement for each signal
         movement = abs(np.diff(self.processedData, axis=0)).sum(axis=0)
-        # get the largest difference from the first point for each signal
-        diff = self.processedData - self.processedData[0]
-        maxDiff = np.max(abs(diff), axis=0)
+        # get the range for each signal
+        totalRange = np.abs(
+            np.max(self.processedData, axis=0) - np.min(self.processedData, axis=0)
+        )
         # find the signals with the largest total movement
         peakIndices, peakProperties = find_peaks(movement, prominence=0)
         prominences = peakProperties["prominences"]
         # select the four most prominent peaks
         largestFilter = prominences.argsort()[-maxPeaks:]
         largestPeakIndices = peakIndices[largestFilter]
 
@@ -184,19 +192,20 @@
         inflectionFilter = inflectionProminences.argsort()[-maxShoulderPeaks:]
         largestInflectionsIndices = inflectionIndices[inflectionFilter]
 
         # combine the two arrays, without duplicates, and sort them
         largestPeakIndices = np.sort(
             np.unique(np.concatenate((largestPeakIndices, largestInflectionsIndices)))
         )
+        if len(largestPeakIndices) == 0:
+            return np.array([np.argmax(movement)])
 
-        # discard peaks that don't move far enough away from the baseline
-        # compared to the other peaks
-        peaksDiff = maxDiff[largestPeakIndices]
-        return largestPeakIndices[peaksDiff >= np.max(peaksDiff) * threshold]
+        # discard peaks that don't move far enough compared to the other peaks
+        peaksRange = totalRange[largestPeakIndices]
+        return largestPeakIndices[peaksRange >= np.max(peaksRange) * threshold]
 
     def optimisationFunc(self, ksAndTotalConcs):
         # scipy.optimize optimizes everything as a single array, so split it
         kVars = ksAndTotalConcs[: self.equilibriumConstants.variableCount]
         self.lastKVars = kVars
         totalConcVars = ksAndTotalConcs[self.equilibriumConstants.variableCount :]
         self.lastTotalConcVars = totalConcVars
@@ -207,18 +216,23 @@
         self.lastKs = speciationVars
         totalConcs = self.totalConcentrations.run(totalConcVars)
         self.lastTotalConcs = totalConcs
 
         freeConcs, boundConcs = self.speciation.run(speciationVars, totalConcs)
         self.lastFreeConcs, self.lastBoundConcs = freeConcs, boundConcs
 
-        signalVars = self.contributors.run(freeConcs, boundConcs)
+        contributingSpeciesFilter = self.contributingSpecies.run()
+        signalVars, contributorsCountPerMolecule = self.contributors.run(
+            freeConcs, boundConcs
+        )
         self.lastSignalVars = signalVars
 
-        proportionalSignalVars = self.proportionality.run(signalVars, totalConcs)
+        proportionalSignalVars = self.proportionality.run(
+            signalVars, contributorsCountPerMolecule
+        )
 
         knownSpectra = self.knownSignals.run()
 
         self.lastFittedSpectra, residuals, self.lastFittedCurves = self.fitSignals.run(
             proportionalSignalVars, knownSpectra
         )
```

### Comparing `musketeer-1.2.2/musketeer/titrationFrame.py` & `musketeer-1.3.0/musketeer/titrationFrame.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 import tkinter.filedialog as fd
 import tkinter.messagebox as mb
 import tkinter.ttk as ttk
 from copy import deepcopy
 from pathlib import PurePath
 
 import matplotlib as mpl
+import matplotlib.ticker as mtick
 import numpy as np
 import packaging.version
 import tksheet
 from cycler import cycler
 from matplotlib.backend_bases import ResizeEvent
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib.figure import Figure
 from numpy import ma
 from scipy.interpolate import make_interp_spline
 from ttkbootstrap.widgets import InteractiveNotebook
 
 from . import (
     __version__,
     combineResiduals,
+    contributingSpecies,
     contributors,
     editData,
     equilibriumConstants,
     fitSignals,
     knownSignals,
     proportionality,
     speciation,
@@ -42,14 +44,15 @@
 COPY_ORIGINAL_ARRAY = "COPY_OGIRINAL_ARRAY"
 
 titrationModules = [
     totalConcentrations,
     proportionality,
     speciation,
     equilibriumConstants,
+    contributingSpecies,
     contributors,
     knownSignals,
     fitSignals,
     combineResiduals,
 ]
 
 
@@ -332,16 +335,16 @@
                 strategy = getattr(titration, moduleFrame.attributeName)
                 if strategy is None:
                     continue
 
                 options[f"{fit}.{moduleFrame.attributeName}"] = list(
                     moduleFrame.dropdownOptions.keys()
                 )[
-                    list(moduleFrame.dropdownOptions.values()).index(
-                        type(getattr(titration, moduleFrame.attributeName))
+                    [x.__name__ for x in moduleFrame.dropdownOptions.values()].index(
+                        type(getattr(titration, moduleFrame.attributeName)).__name__
                     )
                 ]
 
                 for popupAttributeName in strategy.popupAttributes:
                     key = f"{fit}.{moduleFrame.attributeName}.{popupAttributeName}"
                     data = getattr(strategy, popupAttributeName)
 
@@ -563,33 +566,36 @@
         rangeSelection = ttk.Frame(self)
         rangeSelection.grid(row=0, column=1, sticky="s")
 
         ttk.Label(rangeSelection, text=f"Range of {titration.xQuantity} to fit:").pack(
             side="left"
         )
 
-        minWL, maxWL = self.titration.continuousRange
-        minWL = max(minWL, self.titration.signalTitles.min())
-        maxWL = min(maxWL, self.titration.signalTitles.max())
+        signalMin = self.titration.signalTitles.min()
+        signalMax = self.titration.signalTitles.max()
+
+        currentMin, currentMax = self.titration.continuousRange
+        currentMin = max(currentMin, signalMin)
+        currentMax = min(currentMax, signalMax)
 
         decimals = self.titration.signalTitlesDecimals
         step = 1 / (10**decimals)
 
         self.fromSpinbox = ttk.Spinbox(
-            rangeSelection, from_=minWL, to=maxWL, width=5, increment=step
+            rangeSelection, from_=signalMin, to=signalMax, width=5, increment=step
         )
-        self.fromSpinbox.set(f"{minWL:.{decimals}f}")
+        self.fromSpinbox.set(f"{currentMin:.{decimals}f}")
         self.fromSpinbox.pack(padx=padding, side="left")
 
         ttk.Label(rangeSelection, text="to").pack(side="left")
 
         self.toSpinbox = ttk.Spinbox(
-            rangeSelection, from_=minWL, to=maxWL, width=5, increment=step
+            rangeSelection, from_=signalMin, to=signalMax, width=5, increment=step
         )
-        self.toSpinbox.set(f"{maxWL:.{decimals}f}")
+        self.toSpinbox.set(f"{currentMax:.{decimals}f}")
         self.toSpinbox.pack(padx=padding, side="left")
 
         self.fig = Figure(
             layout="constrained", figsize=(self.figwidth, self.figheight), dpi=self.dpi
         )
         self.ax = self.fig.add_subplot()
 
@@ -685,16 +691,16 @@
             "Deconvolution at start",
             "Deconvolution at endpoint",
         )
         self.deconvolutionDropdown = ttk.OptionMenu(
             self.optionsFrame,
             self.deconvolutionVar,
             deconvolutionOptions[0],
-            command=lambda *args: self.plot(),
             *deconvolutionOptions,
+            command=lambda *args: self.plot(),
             style="primary.Outline.TMenubutton",
         )
         self.deconvolutionDropdown.pack()
 
         self.columnconfigure(
             0,
             weight=1000,
@@ -716,27 +722,29 @@
         self.grid_anchor("center")
 
     def plot(self):
         self.ax.clear()
 
         titration = self.titration
         spectra = titration.lastFittedSpectra
-        names = titration.contributors.contributorNames
+        names = titration.contributors.outputNames
         wavelengths = titration.processedSignalTitles
 
         deconvolution = self.deconvolutionVar.get()
         if deconvolution == f"Molar {titration.yQuantity}":
             for spectrum, name in zip(spectra, names):
                 self.ax.plot(wavelengths, spectrum, label=name)
             self.ax.set_ylabel(f"molar {titration.yQuantity} / {titration.yUnit} M⁻¹")
         else:
             if deconvolution == "Deconvolution at start":
                 deconvolutionPoint = 0
             elif deconvolution == "Deconvolution at endpoint":
                 deconvolutionPoint = -1
+            else:
+                raise ValueError(f"Unknown deconvolution option {deconvolution}")
 
             self.ax.plot(
                 wavelengths,
                 titration.processedData[deconvolutionPoint],
                 color="0.5",
                 label="Observed",
             )
@@ -764,15 +772,14 @@
 
 class FittedFrame(PlotFrame):
     def __init__(self, parent, titration, *args, **kwargs):
         super().__init__(parent, *args, **kwargs)
         self.titration = titration
         self.xQuantity = titration.totalConcentrations.freeNames[-1]
         self.xConcs = titration.lastTotalConcs.T[-1]
-        self.normalisation = False
         self.smooth = True
         self.logScale = False
 
     def populate(self):
         self.fig = Figure(
             layout="constrained", figsize=(self.figwidth, self.figheight), dpi=self.dpi
         )
@@ -784,21 +791,31 @@
 
         self.toolbar = NavigationToolbarVertical(self.canvas, self, pack_toolbar=False)
         self.toolbar.update()
         self.toolbar.grid(row=1, column=0, sticky="ne")
 
         self.toggleButtonsFrame = ttk.Frame(self)
         self.toggleButtonsFrame.grid(row=1, column=2, sticky="w")
-        self.normalisationButton = ttk.Checkbutton(
+
+        self.plotTypeVar = tk.StringVar()
+        self.plotTypes = {
+            f"Absolute {self.titration.yQuantity}": "absolute",
+            f"Change in {self.titration.yQuantity}": "relative",
+            f"Normalised change in {self.titration.yQuantity}": "normalised",
+        }
+        self.plotTypeDropdown = ttk.OptionMenu(
             self.toggleButtonsFrame,
-            text="Normalise movement",
-            command=self.toggleNormalisation,
-            style="Outline.Toolbutton",
+            self.plotTypeVar,
+            [k for (k, v) in self.plotTypes.items() if v == "relative"][0],
+            *self.plotTypes.keys(),
+            command=lambda *args: self.plot(),
+            style="primary.Outline.TMenubutton",
         )
-        self.normalisationButton.pack(pady=padding, fill="x")
+        self.plotTypeDropdown.pack()
+
         self.logScaleButton = ttk.Checkbutton(
             self.toggleButtonsFrame,
             text="Logarithmic x axis",
             command=self.toggleLogScale,
             style="Outline.Toolbutton",
         )
         self.logScaleButton.pack(pady=padding, fill="x")
@@ -838,17 +855,17 @@
             ),
         )
         self.rowconfigure(0, weight=1000, uniform="row")
         self.rowconfigure(1, weight=1)
         self.rowconfigure(2, weight=1000, uniform="row")
         self.grid_anchor("center")
 
-    def toggleNormalisation(self):
-        self.normalisation = not self.normalisation
-        self.plot()
+    @property
+    def plotType(self):
+        return self.plotTypes[self.plotTypeVar.get()]
 
     def toggleLogScale(self):
         self.logScale = not self.logScale
         if self.logScale:
             self.ax.set_xscale("log")
         else:
             self.ax.set_xscale("linear")
@@ -883,15 +900,24 @@
         # xQuantity and xUnit for the fitted plot. Different from the xQuantity
         # and xUnit in the titration object, which are used for the input
         # spectra.
         xQuantity = self.xQuantity
         xUnit = titration.totalConcentrations.concsUnit
         xConcs = self.xConcs / totalConcentrations.prefixes[xUnit.strip("M")]
 
-        if self.normalisation:
+        if self.plotType == "absolute":
+            curves = self.curves
+            fittedCurves = self.fittedCurves
+            self.ax.set_ylabel(f"{titration.yQuantity} / {titration.yUnit}")
+        elif self.plotType == "relative":
+            fittedZeros = self.fittedCurves[:, [0]]
+            curves = self.curves - fittedZeros
+            fittedCurves = self.fittedCurves - fittedZeros
+            self.ax.set_ylabel(f"Δ{titration.yQuantity} / {titration.yUnit}")
+        elif self.plotType == "normalised":
             curves = self.curves.T
             fittedCurves = self.fittedCurves.T
             # normalise so that all the fitted curves have the same amplitude
             fittedDiff = self.fittedCurves.T - self.fittedCurves.T[0]
             maxFittedDiff = np.max(abs(fittedDiff), axis=0)
             curves = curves / maxFittedDiff
 
@@ -899,24 +925,23 @@
             negatives = abs(np.amin(diff, axis=0)) > abs(np.amax(diff, axis=0))
             curves[:, negatives] *= -1
             curves = curves.T * 100
 
             fittedCurves = fittedCurves / maxFittedDiff
             fittedCurves[:, negatives] *= -1
             fittedCurves = fittedCurves.T * 100
+
+            fittedZeros = fittedCurves[:, [0]]
+            curves = curves - fittedZeros
+            fittedCurves = fittedCurves - fittedZeros
             self.ax.set_ylabel(f"Normalised Δ{titration.yQuantity} / %")
         else:
-            curves = self.curves
-            fittedCurves = self.fittedCurves
-            self.ax.set_ylabel(f"Δ{titration.yQuantity} / {titration.yUnit}")
+            raise ValueError(f"Unknown plot type: {self.plotType}")
 
         for curve, fittedCurve, name in zip(curves, fittedCurves, self.names):
-            fittedZero = fittedCurve[0]
-            curve -= fittedZero
-            fittedCurve -= fittedZero
             self.ax.scatter(xConcs, curve)
 
             # add step - 1 points between each data point
             step = 10
             smoothXCount = (xConcs.size - 1) * step + 1
             smoothX = np.interp(
                 np.arange(smoothXCount), np.arange(smoothXCount, step=step), xConcs
@@ -1086,25 +1111,26 @@
             self.xConcs[additionsFilter]
             / totalConcentrations.prefixes[xUnit.strip("M")]
         )
 
         freeConcs = titration.lastFreeConcs[additionsFilter, :][:, self.freeIndex]
         freeName = self.speciesVar.get()
 
-        factor = abs(titration.speciation.stoichiometries[:, self.freeIndex])
+        factor = abs(titration.speciation.outputStoichiometries[:, self.freeIndex])
         boundFilter = factor.astype(bool)
 
         boundConcs = titration.lastBoundConcs * factor
         boundConcs = boundConcs[additionsFilter, :][:, boundFilter]
-        # TODO: make this work with polymers
-        boundNames = titration.speciation.boundNames[boundFilter]
+        boundNames = titration.speciation.outputBoundNames[boundFilter]
 
         curves = 100 * np.vstack((freeConcs, boundConcs.T)) / totalConcs
         names = np.append(freeName, boundNames)
         self.ax.set_ylabel(f"% of {freeName}")
+        self.ax.yaxis.set_major_formatter(mtick.PercentFormatter(xmax=100))
+        self.ax.set_ylim(bottom=-5, top=105)
 
         for curve, name in zip(curves, names):
             # add step - 1 points between each data point
             step = 10
             smoothXCount = (xConcs.size - 1) * step + 1
             smoothX = np.interp(
                 np.arange(smoothXCount), np.arange(smoothXCount, step=step), xConcs
@@ -1212,21 +1238,27 @@
                         )
                     ],
                 )
             concsTable.pack(side="top", pady=15)
 
         sheet = tksheet.Sheet(
             self,
+            empty_vertical=0,
+            empty_horizontal=0,
             data=list(np.around(titration.lastFittedSpectra, 2)),
             headers=list(titration.processedSignalTitlesStrings),
-            row_index=list(titration.contributors.contributorNames),
+            row_index=list(titration.contributors.outputNames),
             set_all_heights_and_widths=True,
         )
+        sheet.MT.configure(height=0)
+        sheet.RI.configure(height=0)
+
         sheet.enable_bindings()
-        sheet.pack(side="top", pady=15, fill="x")
+        sheet.set_width_of_index_to_text()
+        sheet.pack(side="top", pady=15, fill="both", expand=True)
 
         saveButton = ttk.Button(
             self,
             text="Save fitted spectra to CSV",
             command=self.saveCSV,
             style="success.TButton",
         )
@@ -1237,14 +1269,14 @@
         fileName = fd.asksaveasfilename(
             title="Save fitted spectra",
             initialfile=initialfile,
             filetypes=[("CSV file", "*.csv")],
             defaultextension=".csv",
         )
         data = self.titration.lastFittedSpectra
-        rowTitles = np.atleast_2d(self.titration.contributors.contributorNames).T
-        columnTitles = np.append("", self.titration.processedSignalTitles)
+        rowTitles = np.atleast_2d(self.titration.contributors.outputNames).T
+        columnTitles = np.append("", self.titration.processedSignalTitlesStrings)
         output = np.vstack((columnTitles, np.hstack((rowTitles, data))))
         try:
             np.savetxt(fileName, output, fmt="%s", delimiter=",", encoding="utf-8-sig")
         except Exception as e:
             mb.showerror(title="Could not save file", message=e, parent=self)
```

### Comparing `musketeer-1.2.2/musketeer/titrationReader.py` & `musketeer-1.3.0/musketeer/titrationReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 # TODO: convert to classes, register using ABC
 def readUV(filePath):
     titration = Titration()
     # set default parameters for UV-Vis titrations
     fillPredefinedParams(titration, predefinedParams["UV-Vis"])
 
-    with open(filePath, "r", newline="") as inFile:
-
+    with open(filePath, "r", newline="", encoding="utf-8-sig") as inFile:
         reader = csv.reader(inFile)
 
         titleRow = next(reader)[::2]
         # the title row can contain an extra blank entry, this gets rid of it
         if not titleRow[-1]:
             titleRow.pop(-1)
 
@@ -112,15 +111,15 @@
     # reads an MNova 1D peaks list
     additionTitles = []
     frequencies = []
     intensities = []
     plotFrequencies = []
     plotIntensities = []
 
-    with open(filePath, "r", newline="") as inFile:
+    with open(filePath, "r", newline="", encoding="utf-8-sig") as inFile:
         reader = csv.reader(inFile, delimiter="\t")
         for row in reader:
             if not row or not row[0]:
                 break
             additionTitles.append(row[1])
             currentFrequencies = [float(f) for f in row[2::2]]
             currentIntensities = [float(i) for i in row[3::2]]
```

### Comparing `musketeer-1.2.2/musketeer/windowsHighDpiPatch.py` & `musketeer-1.3.0/musketeer/windowsHighDpiPatch.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.2.2/musketeer.egg-info/PKG-INFO` & `musketeer-1.3.0/musketeer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: musketeer
-Version: 1.2.2
+Version: 1.3.0
 Summary: A tool for fitting data from titration experiments.
 Home-page: https://github.com/daniilS/Musketeer
 Author: Daniil Soloviev
 Author-email: dos23@cam.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry
@@ -24,9 +23,7 @@
 ```
 python -m pip install musketeer
 ```
 ### Usage
 ```
 python -m musketeer
 ```
-
-
```

### Comparing `musketeer-1.2.2/musketeer.egg-info/SOURCES.txt` & `musketeer-1.3.0/musketeer.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 musketeer/__init__.py
 musketeer/__main__.py
 musketeer/combineResiduals.py
+musketeer/contributingSpecies.py
 musketeer/contributors.py
 musketeer/editData.py
 musketeer/equilibriumConstants.py
 musketeer/fitSignals.py
 musketeer/knownSignals.py
 musketeer/logo small.png
 musketeer/moduleFrame.py
```

### Comparing `musketeer-1.2.2/setup.py` & `musketeer-1.3.0/setup.py`

 * *Files identical despite different names*

