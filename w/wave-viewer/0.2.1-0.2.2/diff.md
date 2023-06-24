# Comparing `tmp/wave_viewer-0.2.1.tar.gz` & `tmp/wave_viewer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wave_viewer-0.2.1.tar", max compression
+gzip compressed data, was "wave_viewer-0.2.2.tar", max compression
```

## Comparing `wave_viewer-0.2.1.tar` & `wave_viewer-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-18 02:42:58.397916 wave_viewer-0.2.1/LICENSE
--rw-r--r--   0        0        0      837 2023-05-28 11:56:12.971870 wave_viewer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1424 2023-05-28 11:53:04.265234 wave_viewer-0.2.1/README.md
--rw-r--r--   0        0        0      714 2023-05-22 20:04:53.097291 wave_viewer-0.2.1/wave_viewer/__init__.py
--rw-r--r--   0        0        0     5017 2023-05-28 11:42:11.245757 wave_viewer-0.2.1/wave_viewer/_controller.py
--rw-r--r--   0        0        0     7110 2023-05-28 11:31:20.511591 wave_viewer-0.2.1/wave_viewer/_viewer.py
--rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 wave_viewer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-18 02:42:58.397916 wave_viewer-0.2.2/LICENSE
+-rw-r--r--   0        0        0      837 2023-06-24 14:49:49.186099 wave_viewer-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1424 2023-05-28 11:53:04.265234 wave_viewer-0.2.2/README.md
+-rw-r--r--   0        0        0      714 2023-05-22 20:04:53.097291 wave_viewer-0.2.2/wave_viewer/__init__.py
+-rw-r--r--   0        0        0     5160 2023-06-24 14:47:31.215651 wave_viewer-0.2.2/wave_viewer/_controller.py
+-rw-r--r--   0        0        0     7110 2023-06-24 14:14:24.442339 wave_viewer-0.2.2/wave_viewer/_viewer.py
+-rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 wave_viewer-0.2.2/PKG-INFO
```

### Comparing `wave_viewer-0.2.1/LICENSE` & `wave_viewer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wave_viewer-0.2.1/pyproject.toml` & `wave_viewer-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wave-viewer"
-version = "0.2.1"
+version = "0.2.2"
 description = "A simple GUI for viewing waveforms."
 authors = ["Jiahao Yuan <kaho0769@qq.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/kahojyun/wave-viewer"
 packages = [{include = "wave_viewer"}]
```

### Comparing `wave_viewer-0.2.1/README.md` & `wave_viewer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `wave_viewer-0.2.1/wave_viewer/__init__.py` & `wave_viewer-0.2.2/wave_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `wave_viewer-0.2.1/wave_viewer/_controller.py` & `wave_viewer-0.2.2/wave_viewer/_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 provides methods for adding and removing lines from the plot, clearing the plot,
 and closing the GUI.
 """
 import multiprocessing as mp
 
 import numpy as np
 
-from ._viewer import main
+
+def _entrypoint(rconn: mp.Queue):
+    """Entry point for the wave_viewer process."""
+    from ._viewer import main
+
+    main(rconn)
 
 
 class WaveViewer:
     """A simple GUI for viewing waveforms.
 
     It plots the waveform with vispy in a separate process. The GUI is built with
     PySide6.
@@ -25,15 +30,17 @@
         viewer process will continue to run after the main process exits. In this
         case, the viewer process must be closed manually by calling the `close`
         method. The default is True.
     """
 
     def __init__(self, daemon: bool = True) -> None:
         self._conn = mp.Queue()
-        self._process = mp.Process(target=main, args=(self._conn,), daemon=daemon)
+        self._process = mp.Process(
+            target=_entrypoint, args=(self._conn,), daemon=daemon
+        )
         self._process.start()
 
     def _ensure_open(self) -> None:
         if not self._process.is_alive():
             raise RuntimeError("WaveViewer is closed")
 
     def add_line(self, name: str, t: np.ndarray, ys: list, offset: float) -> None:
```

### Comparing `wave_viewer-0.2.1/wave_viewer/_viewer.py` & `wave_viewer-0.2.2/wave_viewer/_viewer.py`

 * *Files identical despite different names*

### Comparing `wave_viewer-0.2.1/PKG-INFO` & `wave_viewer-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wave-viewer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple GUI for viewing waveforms.
 Home-page: https://github.com/kahojyun/wave-viewer
 License: MIT
 Author: Jiahao Yuan
 Author-email: kaho0769@qq.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

