# Comparing `tmp/vision6D-0.2.5.tar.gz` & `tmp/vision6D-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.2.5.tar", last modified: Sat Jun  3 17:58:00 2023, max compression
+gzip compressed data, was "dist\vision6D-0.2.6.tar", last modified: Sat Jun 24 04:19:13 2023, max compression
```

## Comparing `vision6D-0.2.5.tar` & `vision6D-0.2.6.tar`

### file list

```diff
@@ -1,33 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 17:57:59.774731 vision6D-0.2.5/
--rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.2.5/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1361 2023-06-03 17:57:59.774731 vision6D-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.2.5/README.md
--rw-rw-rw-   0        0        0      406 2023-06-02 21:40:49.000000 vision6D-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0     2050 2023-06-03 17:57:59.780997 vision6D-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      282 2023-06-02 21:40:49.000000 vision6D-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 17:57:59.629091 vision6D-0.2.5/test/
--rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.5/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.5/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-06-03 17:57:59.657094 vision6D-0.2.5/vision6D/
--rw-rw-rw-   0        0        0    52546 2023-06-03 17:56:36.000000 vision6D-0.2.5/vision6D/GUI.py
--rw-rw-rw-   0        0        0      913 2023-06-02 21:40:49.000000 vision6D-0.2.5/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.2.5/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-06-02 21:40:49.000000 vision6D-0.2.5/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-06-03 17:57:59.771936 vision6D-0.2.5/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.5/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.2.5/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.2.5/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.2.5/vision6D/interface.py
--rw-rw-rw-   0        0        0    27853 2023-06-03 17:53:50.000000 vision6D-0.2.5/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.2.5/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.2.5/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.2.5/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.2.5/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-03 17:57:59.727091 vision6D-0.2.5/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1361 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 04:19:13.112982 vision6D-0.2.6/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1361 2023-06-24 04:19:13.113980 vision6D-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.2.6/README.md
+-rw-rw-rw-   0        0        0      406 2023-06-02 21:40:49.000000 vision6D-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0     2050 2023-06-24 04:19:13.116981 vision6D-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      277 2023-06-24 04:13:08.000000 vision6D-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 04:19:12.903985 vision6D-0.2.6/test/
+-rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.6/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.6/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-06-24 04:19:12.968980 vision6D-0.2.6/vision6D/
+-rw-rw-rw-   0        0        0    65799 2023-06-24 04:12:06.000000 vision6D-0.2.6/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      910 2023-06-24 04:12:06.000000 vision6D-0.2.6/vision6D/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 04:19:13.086981 vision6D-0.2.6/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.6/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.2.6/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-06-06 19:10:46.000000 vision6D-0.2.6/vision6D/data/style.qss
+drwxrwxrwx   0        0        0        0 2023-06-24 04:19:13.110981 vision6D-0.2.6/vision6D/entry/
+-rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.2.6/vision6D/entry/__init__.py
+-rw-rw-rw-   0        0        0      422 2023-06-24 04:14:35.000000 vision6D-0.2.6/vision6D/entry/main.py
+-rw-rw-rw-   0        0        0    17032 2023-06-24 04:12:06.000000 vision6D-0.2.6/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    15676 2023-06-24 04:12:06.000000 vision6D-0.2.6/vision6D/utils.py
+-rw-rw-rw-   0        0        0    24790 2023-06-24 04:12:06.000000 vision6D-0.2.6/vision6D/widgets_gui.py
+drwxrwxrwx   0        0        0        0 2023-06-24 04:19:13.030981 vision6D-0.2.6/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1361 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.2.5/LICENSE` & `vision6D-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.5/PKG-INFO` & `vision6D-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.5
+Version: 0.2.6
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.2.5/README.md` & `vision6D-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.5/setup.cfg` & `vision6D-0.2.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e32 2e35 0d0a 7572  sion = 0.2.5..ur
+00000020: 7369 6f6e 203d 2030 2e32 2e36 0d0a 7572  sion = 0.2.6..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.2.5/test/test_create_dataset.py` & `vision6D-0.2.6/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.5/test/test_projection.py` & `vision6D-0.2.6/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.5/vision6D/GUI.py` & `vision6D-0.2.6/vision6D/GUI.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,353 +1,406 @@
-# General import
+import os
+import re
 import numpy as np
 import pyvista as pv
-import functools
 import trimesh
 import pathlib
 import PIL
 import ast
 import json
 import math
 import copy
-from skimage.metrics import peak_signal_noise_ratio, structural_similarity
+import cv2
+import vtk
+import pyvista as pv
+
+# Setting the Qt bindings for QtPy
+import os
+os.environ["QT_API"] = "pyqt5"
 
-# Qt5 import
 from PyQt5 import QtWidgets, QtGui
-from pyvistaqt import QtInteractor, MainWindow
-from PyQt5.QtCore import Qt, QPoint
+from PyQt5.QtCore import QPoint
+from .mainwindow import MyMainWindow
 
-# self defined package import
-import vision6D as vis
+from . import utils
+from . import widgets_gui
 
 np.set_printoptions(suppress=True)
 
-class YesNoBox(QtWidgets.QMessageBox):
-    def __init__(self, *args, **kwargs):
-        super(YesNoBox, self).__init__(*args, **kwargs)
-        self.canceled = False
-
-    def closeEvent(self, event: QtGui.QCloseEvent):
-        self.canceled = True
-        super(YesNoBox, self).closeEvent(event)
-
-class PopUpDialog(QtWidgets.QDialog):
-    def __init__(self, parent=None, on_button_click=None):
-        super().__init__(parent)
-
-        self.setWindowTitle("Vision6D - Colors")
-        self.setWindowFlags(self.windowFlags() & ~Qt.WindowContextHelpButtonHint) # Disable the question mark
-
-        button_grid = QtWidgets.QGridLayout()
-        colors = ["nocs", "cyan", "magenta", 
-                "yellow", "lime", "deepskyblue", "latlon", "salmon", 
-                "silver", "aquamarine", "plum", "blueviolet"]
-
-        button_count = 0
-        for i in range(2):
-            for j in range(6):
-                name = f"{colors[button_count]}"
-                button = QtWidgets.QPushButton(name)
-                button.clicked.connect(lambda _, idx=name: on_button_click(str(idx)))
-                button_grid.addWidget(button, j, i)
-                button_count += 1
-
-        self.setLayout(button_grid)
-
-class CameraPropsInputDialog(QtWidgets.QDialog):
-    def __init__(self, parent=None, 
-                    line1=(None, None), 
-                    line2=(None, None), 
-                    line3=(None, None), 
-                    line4=(None, None), 
-                    line5=(None, None),
-                    line6=(None, None)):
-        super().__init__(parent)
-
-        self.args1 = QtWidgets.QLineEdit(self, text=str(line1[1]))
-        self.args2 = QtWidgets.QLineEdit(self, text=str(line2[1]))
-        self.args3 = QtWidgets.QLineEdit(self, text=str(line3[1]))
-        self.args4 = QtWidgets.QLineEdit(self, text=str(line4[1]))
-        self.args5 = QtWidgets.QLineEdit(self, text=str(line5[1]))
-        self.args6 = QtWidgets.QLineEdit(self, text=str(line6[1]))
-
-        buttonBox = QtWidgets.QDialogButtonBox(QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel, self)
-
-        layout = QtWidgets.QFormLayout(self)
-        layout.addRow(f"{line1[0]}", self.args1)
-        layout.addRow(f"{line2[0]}", self.args2)
-        layout.addRow(f"{line3[0]}", self.args3)
-        layout.addRow(f"{line4[0]}", self.args4)
-        layout.addRow(f"{line5[0]}", self.args5)
-        layout.addRow(f"{line6[0]}", self.args6)
-        layout.addWidget(buttonBox)
-
-        buttonBox.accepted.connect(self.accept)
-        buttonBox.rejected.connect(self.reject)
-
-    def getInputs(self):
-        return (self.args1.text(), 
-                self.args2.text(), 
-                self.args3.text(),
-                self.args4.text(),
-                self.args5.text(),
-                self.args6.text())
-    
-class CalibrationPopWindow(QtWidgets.QDialog):
-    def __init__(self, calibrated_image, original_image, parent=None):
-        super(CalibrationPopWindow, self).__init__(parent)
-        self.setWindowFlags(self.windowFlags() & ~Qt.WindowContextHelpButtonHint)
-
-        self.calibrated_image = calibrated_image
-        self.original_image = original_image
-
-        self.setWindowTitle("Vision6D")
-        self.setFixedSize(960, 540)
-
-        overall = QtWidgets.QVBoxLayout()
-        layout = QtWidgets.QHBoxLayout()
-
-        vbox1layout = QtWidgets.QVBoxLayout()
-        label1 = QtWidgets.QLabel("Calibrated image", self)
-        label1.setAlignment(Qt.AlignCenter)
-        pixmap_label1 = QtWidgets.QLabel(self)
-        qimage1 = QtGui.QImage(self.calibrated_image, self.calibrated_image.shape[1], self.calibrated_image.shape[0], QtGui.QImage.Format_RGB888)
-        pixmap1 = QtGui.QPixmap.fromImage(qimage1).scaled(960, 540, Qt.KeepAspectRatio)
-        pixmap_label1.setPixmap(pixmap1)
-        pixmap_label1.setAlignment(Qt.AlignCenter)
-        vbox1layout.addWidget(label1)
-        vbox1layout.addWidget(pixmap_label1)
-
-        vbox2layout = QtWidgets.QVBoxLayout()
-        label2 = QtWidgets.QLabel("Original image", self)
-        label2.setAlignment(Qt.AlignCenter)
-        pixmap_label2 = QtWidgets.QLabel(self)
-        qimage2 = QtGui.QImage(self.original_image, self.original_image.shape[1], self.original_image.shape[0], QtGui.QImage.Format_RGB888)
-        pixmap2 = QtGui.QPixmap.fromImage(qimage2).scaled(960, 540, Qt.KeepAspectRatio)
-        pixmap_label2.setPixmap(pixmap2)
-        pixmap_label2.setAlignment(Qt.AlignCenter)
-
-        vbox2layout.addWidget(label2)
-        vbox2layout.addWidget(pixmap_label2)
-
-        layout.addLayout(vbox1layout)
-        layout.addLayout(vbox2layout)
-
-        psnr, ssim = self.calculate_similarity()
-        similarity_label = QtWidgets.QLabel(f"PSNR is {psnr} and SSIM is {ssim}", self)
-        similarity_label.setAlignment(Qt.AlignCenter)
-
-        overall.addLayout(layout)
-        overall.addWidget(similarity_label)
-
-        self.setLayout(overall)
-
-    def calculate_similarity(self):
-        psnr = peak_signal_noise_ratio(self.calibrated_image, self.original_image, data_range=255)
-        ssim = structural_similarity(self.calibrated_image, self.original_image, data_range=255, channel_axis=2)
-        return psnr, ssim
-
-class GetTextDialog(QtWidgets.QDialog):
-    def __init__(self, parent=None):
-        super(GetTextDialog, self).__init__(parent)
+class Interface(MyMainWindow):
+    def __init__(self):
+        super().__init__()
+        # initialize
+        self.reference = None
+        self.transformation_matrix = np.eye(4)
+        self.initial_pose = None
 
-        layout = QtWidgets.QVBoxLayout(self)
-        
-        self.setWindowTitle("Vision6D")
-        self.introLabel = QtWidgets.QLabel("Input the Ground Truth Pose:")
-        self.btnloadfromfile = QtWidgets.QPushButton("Load from file", self)
-
-        hbox = QtWidgets.QHBoxLayout()
-        hbox.addWidget(self.introLabel)
-        hbox.addWidget(self.btnloadfromfile)
-        hbox.setContentsMargins(0, 0, 0, 0)
-        self.hboxWidget = QtWidgets.QWidget()
-        self.hboxWidget.setLayout(hbox)
-
-        self.btnloadfromfile.clicked.connect(self.load_from_file)
-        self.textEdit = QtWidgets.QTextEdit(self)
-        self.textEdit.setPlainText(f"[[1, 0, 0, 0], \n[0, 1, 0, 0], \n[0, 0, 1, 0], \n[0, 0, 0, 1]]")
-        self.btnSubmit = QtWidgets.QPushButton("Submit", self)
-        self.btnSubmit.clicked.connect(self.submit_text)
-
-        layout.addWidget(self.hboxWidget)
-        layout.addWidget(self.textEdit)
-        layout.addWidget(self.btnSubmit)
-
-    def submit_text(self):
-        self.user_text = self.textEdit.toPlainText()
-        self.accept()
-
-    def load_from_file(self):
-        file_dialog = QtWidgets.QFileDialog()
-        pose_path, _ = file_dialog.getOpenFileName(None, "Open file", "", "Files (*.npy)")
-        if pose_path != '':
-            gt_pose = np.load(pose_path)
-            self.textEdit.setPlainText(f"[[{np.around(gt_pose[0, 0], 8)}, {np.around(gt_pose[0, 1], 8)}, {np.around(gt_pose[0, 2], 8)}, {np.around(gt_pose[0, 3], 8)}],\n"
-                                    f"[{np.around(gt_pose[1, 0], 8)}, {np.around(gt_pose[1, 1], 8)}, {np.around(gt_pose[1, 2], 8)}, {np.around(gt_pose[1, 3], 8)}],\n"
-                                    f"[{np.around(gt_pose[2, 0], 8)}, {np.around(gt_pose[2, 1], 8)}, {np.around(gt_pose[2, 2], 8)}, {np.around(gt_pose[2, 3], 8)}],\n"
-                                    f"[{np.around(gt_pose[3, 0], 8)}, {np.around(gt_pose[3, 1], 8)}, {np.around(gt_pose[3, 2], 8)}, {np.around(gt_pose[3, 3], 8)}]]")
-
-    def get_text(self):
-        return self.user_text
-
-class MyMainWindow(MainWindow):
-    def __init__(self, parent=None):
-        QtWidgets.QMainWindow.__init__(self, parent)
-        
-        # Set up the main window layout
-        self.setWindowTitle("Vision6D")
-        self.window_size = (1920, 1080)
-        self.main_widget = QtWidgets.QWidget()
-        self.setCentralWidget(self.main_widget)
-        self.setAcceptDrops(True)
+        self.mirror_x = False
+        self.mirror_y = False
 
-        self.track_actors_names = []
-        self.button_group_actors_names = QtWidgets.QButtonGroup(self)
+        self.image_actor = None
+        self.mask_actor = None
+        self.mesh_actors = {}
+        self.meshdict = {}
+        
+        self.undo_poses = {}
+        self.latlon = utils.load_latitude_longitude()
 
-        self.toggle_hide_actors_flag = False
+        self.colors = ["cyan", "magenta", "yellow", "lime", "dodgerblue", "darkviolet", "darkorange", "forestgreen"]
+        self.used_colors = []
+        self.mesh_colors = {}
 
-        # Set panel bar
-        self.set_panel_bar()
+        self.mesh_opacity = {}
+        self.store_mesh_opacity = {}
+        self.image_opacity = 0.8
+        self.mask_opacity = 0.3
+        self.surface_opacity = self.opacity_spinbox.value()
         
-        # Set menu bar
-        self.set_menu_bars()
-
-        # Create the plotter
-        self.create_plotter()
+        # Set mesh spacing
+        self.mesh_spacing = [1, 1, 1]
         
         # Set the camera
         self.camera = pv.Camera()
         self.fx = 50000
         self.fy = 50000
-        self.cx = 960
-        self.cy = 540
+        self.cx = self.window_size[0] // 2
+        self.cy = self.window_size[1] // 2
         self.cam_viewup = (0, -1, 0)
         self.cam_position = -500
         self.set_camera_props()
 
-        # Set up the main layout with the left panel and the render window using QSplitter
-        self.main_layout = QtWidgets.QHBoxLayout(self.main_widget)
-        self.splitter = QtWidgets.QSplitter()
-        self.splitter.addWidget(self.panel_widget)
-        self.splitter.addWidget(self.plotter)
-        self.main_layout.addWidget(self.splitter)
-
-        # Add a QLabel as an overlay hint label
-        self.hintLabel = QtWidgets.QLabel(self.plotter)
-        self.hintLabel.setText("Drag and drop a file here...")
-        self.hintLabel.setStyleSheet("""
-                                    color: white; 
-                                    background-color: rgba(0, 0, 0, 127); 
-                                    padding: 10px;
-                                    border: 2px dashed gray;
-                                    """)
-        self.hintLabel.setAlignment(Qt.AlignCenter)
-
-        # Show the plotter
-        self.show_plot()
-
-    def dragEnterEvent(self, e):
-        if e.mimeData().hasUrls():
-            e.accept()
-            self.hintLabel.hide()  # Hide hint when dragging
-        else:
-            e.ignore()
-
-    def dropEvent(self, e):
-        for url in e.mimeData().urls():
-            file_path = url.toLocalFile()
-            if file_path.endswith(('.mesh', '.ply', '.stl', '.obj', '.off', '.dae', '.fbx', '.3ds', '.x3d')):  # add mesh
-                self.mesh_path = file_path
-                self.add_mesh_file(prompt=False)
-            elif file_path.endswith(('.png', '.jpg', 'jpeg', '.tiff', '.bmp', '.webp', '.ico')):  # add image/mask
-                yes_no_box = YesNoBox()
-                yes_no_box.setIcon(QtWidgets.QMessageBox.Question)
-                yes_no_box.setWindowTitle("Vision6D")
-                yes_no_box.setText("Do you want to load the image as mask?")
-                yes_no_box.setStandardButtons(QtWidgets.QMessageBox.Yes | QtWidgets.QMessageBox.No)
-                button_clicked = yes_no_box.exec_()
-                if not yes_no_box.canceled:
-                    if button_clicked == QtWidgets.QMessageBox.Yes:
-                        self.mask_path = file_path
-                        self.add_mask_file(prompt=False)
-                    elif button_clicked == QtWidgets.QMessageBox.No:
-                        self.image_path = file_path
-                        self.add_image_file(prompt=False)
-            elif file_path.endswith('.npy'):
-                self.pose_path = file_path
-                self.add_pose_file()
+        self.track_actors_names = []
+        self.button_group_actors_names = QtWidgets.QButtonGroup(self)
+        self.toggle_hide_meshes_flag = False
+
+        # Shortcut key bindings
+        # camera related key bindings
+        QtWidgets.QShortcut(QtGui.QKeySequence("c"), self).activated.connect(self.reset_camera)
+        QtWidgets.QShortcut(QtGui.QKeySequence("z"), self).activated.connect(self.zoom_out)
+        QtWidgets.QShortcut(QtGui.QKeySequence("x"), self).activated.connect(self.zoom_in)
+
+        # registration related key bindings
+        QtWidgets.QShortcut(QtGui.QKeySequence("k"), self).activated.connect(self.reset_gt_pose)
+        QtWidgets.QShortcut(QtGui.QKeySequence("l"), self).activated.connect(self.update_gt_pose)
+        QtWidgets.QShortcut(QtGui.QKeySequence("s"), self).activated.connect(self.undo_pose)
+
+        # Reset the mask location
+        QtWidgets.QShortcut(QtGui.QKeySequence("t"), self).activated.connect(self.add_mask_file)
+
+        # change image opacity key bindings
+        QtWidgets.QShortcut(QtGui.QKeySequence("b"), self).activated.connect(lambda up=True: self.toggle_image_opacity(up))
+        QtWidgets.QShortcut(QtGui.QKeySequence("n"), self).activated.connect(lambda up=False: self.toggle_image_opacity(up))
+
+        # change mask opacity key bindings
+        QtWidgets.QShortcut(QtGui.QKeySequence("g"), self).activated.connect(lambda up=True: self.toggle_mask_opacity(up))
+        QtWidgets.QShortcut(QtGui.QKeySequence("h"), self).activated.connect(lambda up=False: self.toggle_mask_opacity(up))
+
+        # change mesh opacity key bindings
+        QtWidgets.QShortcut(QtGui.QKeySequence("y"), self).activated.connect(lambda up=True: self.toggle_surface_opacity(up))
+        QtWidgets.QShortcut(QtGui.QKeySequence("u"), self).activated.connect(lambda up=False: self.toggle_surface_opacity(up))
+
+        # Add shortcut to the right, left, space buttons
+        QtWidgets.QShortcut(QtGui.QKeySequence("Right"), self).activated.connect(self.next_frame)
+        QtWidgets.QShortcut(QtGui.QKeySequence("Left"), self).activated.connect(self.prev_frame)
+        QtWidgets.QShortcut(QtGui.QKeySequence("Space"), self).activated.connect(self.play_video)
+
+    def button_actor_name_clicked(self, text):
+        if text in self.mesh_actors:
+            # set the current mesh color
+            self.color_button.setText(self.mesh_colors[text])
+            # set mesh reference
+            self.reference = text
+            self.current_pose()
+            curr_opacity = self.mesh_actors[self.reference].GetProperty().opacity
+            self.opacity_spinbox.setValue(curr_opacity)
+        else:
+            self.color_button.setText("Color")
+            if text == 'image': curr_opacity = self.image_opacity
+            elif text == 'mask': curr_opacity = self.mask_opacity
+            else: curr_opacity = self.opacity_spinbox.value()
+            self.opacity_spinbox.setValue(curr_opacity)
+            # self.reference = None
+        
+        output = f"-> Actor {text}, and its opacity is {curr_opacity}"
+        if output not in self.output_text.toPlainText(): self.output_text.append(output)
+                                            
+    def set_image_opacity(self, image_opacity: float):
+        assert image_opacity>=0 and image_opacity<=1, "image opacity should range from 0 to 1!"
+        self.image_opacity = image_opacity
+        self.image_actor.GetProperty().opacity = image_opacity
+        self.plotter.add_actor(self.image_actor, pickable=False, name='image')
+
+    def set_mask_opacity(self, mask_opacity: float):
+        assert mask_opacity>=0 and mask_opacity<=1, "image opacity should range from 0 to 1!"
+        self.mask_opacity = mask_opacity
+        self.mask_actor.GetProperty().opacity = mask_opacity
+        self.plotter.add_actor(self.mask_actor, pickable=True, name='mask')
+
+    def set_mesh_opacity(self, name: str, surface_opacity: float):
+        assert surface_opacity>=0 and surface_opacity<=1, "mesh opacity should range from 0 to 1!"
+        self.mesh_opacity[name] = surface_opacity
+        self.mesh_actors[name].user_matrix = pv.array_from_vtkmatrix(self.mesh_actors[name].GetMatrix())
+        self.mesh_actors[name].GetProperty().opacity = surface_opacity
+        self.plotter.add_actor(self.mesh_actors[name], pickable=True, name=name)
+
+    def add_image(self, image_source):
+
+        if isinstance(image_source, pathlib.WindowsPath) or isinstance(image_source, str):
+            image_source = np.array(PIL.Image.open(image_source), dtype='uint8')
+        if len(image_source.shape) == 2: image_source = image_source[..., None]
+
+        if self.mirror_x: image_source = image_source[:, ::-1, :]
+        if self.mirror_y: image_source = image_source[::-1, :, :]
+
+        dim = image_source.shape
+        h, w, channel = dim[0], dim[1], dim[2]
+
+        # Create the render based on the image size
+        self.render = pv.Plotter(window_size=[w, h], lighting=None, off_screen=True) 
+        self.render.set_background('black'); assert self.render.background_color == "black", "render's background need to be black"
+
+        image = pv.UniformGrid(dimensions=(w, h, 1), spacing=[0.01, 0.01, 1], origin=(0.0, 0.0, 0.0))
+        image.point_data["values"] = image_source.reshape((w * h, channel)) # order = 'C
+        image = image.translate(-1 * np.array(image.center), inplace=False)
+
+        # Then add it to the plotter
+        image = self.plotter.add_mesh(image, cmap='gray', opacity=self.image_opacity, name='image') if channel == 1 else self.plotter.add_mesh(image, rgb=True, opacity=self.image_opacity, name='image')
+        actor, _ = self.plotter.add_actor(image, pickable=False, name='image')
+        # Save actor for later
+        self.image_actor = actor
+        
+        # get the image scalar
+        image_data = utils.get_image_actor_scalars(self.image_actor)
+        assert (image_data == image_source).all() or (image_data*255 == image_source).all(), "image_data and image_source should be equal"
+
+        # add remove current image to removeMenu
+        if 'image' not in self.track_actors_names:
+            self.track_actors_names.append('image')
+            self.add_button_actor_name('image')
+
+        self.check_button('image')
+
+    def add_mask(self, mask_source):
+
+        if isinstance(mask_source, pathlib.WindowsPath) or isinstance(mask_source, str):
+            mask_source = np.array(PIL.Image.open(mask_source), dtype='uint8')
+
+        if mask_source.shape[-1] == 3: mask_source = cv2.cvtColor(mask_source, cv2.COLOR_RGB2GRAY)
+
+        # Get the segmentation contour points
+        contours, _ = cv2.findContours(mask_source, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+        points2d = contours[0].squeeze()
+        
+        # Mirror points
+        h, w = mask_source.shape[0], mask_source.shape[1]
+        if self.mirror_x: points2d[:, 0] = w - points2d[:, 0]
+        if self.mirror_y: points2d[:, 1] = h - points2d[:, 1]
+
+        bottom_point = points2d[np.argmax(points2d[:, 1])]
+
+        mask_center = (mask_source.shape[1] // 2, mask_source.shape[0] // 2)
+
+        self.mask_offset = np.hstack(((bottom_point - mask_center)*0.01, 0))
+
+        # Pad points a z dimension
+        points = np.hstack((points2d*0.01, np.zeros(points2d.shape[0]).reshape((-1, 1))))
+        # Find the bottom point on mask
+        self.mask_bottom_point = points[np.argmax(points[:, 1])]
+
+        # Create the mesh surface object
+        cells = np.hstack([[points.shape[0]], np.arange(points.shape[0]), 0])
+        mask_surface = pv.PolyData(points, cells).triangulate()
+        mask_surface = mask_surface.translate(-self.mask_bottom_point+self.mask_offset, inplace=False)
+
+        # Add mask surface object to the plot
+        mask_mesh = self.plotter.add_mesh(mask_surface, color="white", style='surface', opacity=self.mask_opacity)
+        actor, _ = self.plotter.add_actor(mask_mesh, pickable=True, name='mask')
+        self.mask_actor = actor
+
+        mask_point_data = utils.get_mask_actor_points(self.mask_actor)
+        assert np.isclose(((mask_point_data+self.mask_bottom_point-self.mask_offset) - points), 0).all(), "mask_point_data and points should be equal"
+
+        # Add remove current image to removeMenu
+        if 'mask' not in self.track_actors_names:
+            self.track_actors_names.append('mask')
+            self.add_button_actor_name('mask')
+
+        self.check_button('mask')
+
+    def add_mesh(self, mesh_name, mesh_source, transformation_matrix=None):
+        """ add a mesh to the pyqt frame """
+
+        flag = False
+                              
+        if isinstance(mesh_source, pathlib.WindowsPath) or isinstance(mesh_source, str):
+            # Load the '.mesh' file
+            if pathlib.Path(mesh_source).suffix == '.mesh': mesh_source = utils.load_trimesh(mesh_source)
+            # Load the '.ply' file
+            else: mesh_source = pv.read(mesh_source)
+
+        if isinstance(mesh_source, trimesh.Trimesh):
+            assert (mesh_source.vertices.shape[1] == 3 and mesh_source.faces.shape[1] == 3), "it should be N by 3 matrix"
+            mesh_data = pv.wrap(mesh_source)
+            source_verts = mesh_source.vertices * self.mesh_spacing
+            source_faces = mesh_source.faces
+            flag = True
+
+        if isinstance(mesh_source, pv.PolyData):
+            mesh_data = mesh_source
+            source_verts = mesh_source.points * self.mesh_spacing
+            source_faces = mesh_source.faces.reshape((-1, 4))[:, 1:]
+            flag = True
+
+        if flag:
+            # consider the mesh verts spacing
+            mesh_data.points = mesh_data.points * self.mesh_spacing
+
+            # assign a color to every mesh
+            if len(self.colors) != 0: mesh_color = self.colors.pop(0)
             else:
-                QtWidgets.QMessageBox.warning(self, 'vision6D', "File format is not supported!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-                return 0
+                self.colors = self.used_colors
+                mesh_color = self.colors.pop(0)
+                self.used_colors = []
+
+            self.used_colors.append(mesh_color)
+            self.mesh_colors[mesh_name] = mesh_color
+            self.color_button.setText(self.mesh_colors[mesh_name])
+            mesh = self.plotter.add_mesh(mesh_data, color=mesh_color, opacity=self.mesh_opacity[mesh_name], name=mesh_name)
+
+            mesh.user_matrix = self.transformation_matrix if transformation_matrix is None else transformation_matrix
+            if self.initial_pose is None: self.initial_pose = self.transformation_matrix
+                    
+            # Add and save the actor
+            actor, _ = self.plotter.add_actor(mesh, pickable=True, name=mesh_name)
+
+            actor_vertices, actor_faces = utils.get_mesh_actor_vertices_faces(actor)
+            assert (actor_vertices == source_verts).all(), "vertices should be the same"
+            assert (actor_faces == source_faces).all(), "faces should be the same"
+            assert actor.name == mesh_name, "actor's name should equal to mesh_name"
+            
+            self.mesh_actors[mesh_name] = actor
+
+            # add remove current mesh to removeMenu
+            if mesh_name not in self.track_actors_names:
+                self.track_actors_names.append(mesh_name)
+                self.add_button_actor_name(mesh_name)
+
+            self.check_button(mesh_name)
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "The mesh format is not supported!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            return 0
+
+    def reset_camera(self):
+        self.plotter.camera = self.camera.copy()
+
+    def zoom_in(self):
+        self.plotter.camera.zoom(2)
+
+    def zoom_out(self):
+        self.plotter.camera.zoom(0.5)
 
-    def resizeEvent(self, e):
-        x = (self.plotter.size().width() - self.hintLabel.width()) // 2
-        y = (self.plotter.size().height() - self.hintLabel.height()) // 2
-        self.hintLabel.move(x, y)
-        super().resizeEvent(e)
-
-    # ^Main Menu
-    def set_menu_bars(self):
-        mainMenu = self.menuBar()
-        # simple dialog to record users input info
-        self.input_dialog = QtWidgets.QInputDialog()
-        self.file_dialog = QtWidgets.QFileDialog()
-        self.get_text_dialog = GetTextDialog()
+    def check_button(self, actor_name):
+        for button in self.button_group_actors_names.buttons():
+            if button.text() == actor_name: 
+                button.setChecked(True)
+                self.button_actor_name_clicked(actor_name)
+                break
+
+    def add_button_actor_name(self, actor_name):
+        button = QtWidgets.QPushButton(actor_name)
+        button.setCheckable(True)  # Set the button to be checkable
+        button.clicked.connect(lambda _, text=actor_name: self.button_actor_name_clicked(text))
+        button.setChecked(True)
+        button.setFixedSize(self.display.size().width(), 50)
+        self.button_layout.insertWidget(0, button) # insert from the top # self.button_layout.addWidget(button)
+        self.button_group_actors_names.addButton(button)
+        self.button_actor_name_clicked(actor_name)
+
+    def toggle_image_opacity(self, up):
+        if up:
+            self.image_opacity += 0.05
+            if self.image_opacity > 1: self.image_opacity = 1
+        else:
+            self.image_opacity -= 0.05
+            if self.image_opacity < 0: self.image_opacity = 0
+        self.image_actor.GetProperty().opacity = self.image_opacity
+        self.plotter.add_actor(self.image_actor, pickable=False, name="image")
+        self.ignore_spinbox_value_change = True
+        self.opacity_spinbox.setValue(self.image_opacity)
+        self.ignore_spinbox_value_change = False
+
+    def toggle_mask_opacity(self, up):
+        if up:
+            self.mask_opacity += 0.05
+            if self.mask_opacity > 1: self.mask_opacity = 1
+        else:
+            self.mask_opacity -= 0.05
+            if self.mask_opacity < 0: self.mask_opacity = 0
+        self.mask_actor.GetProperty().opacity = self.mask_opacity
+        self.plotter.add_actor(self.mask_actor, pickable=True, name="mask")
+        self.ignore_spinbox_value_change = True
+        self.opacity_spinbox.setValue(self.mask_opacity)
+        self.ignore_spinbox_value_change = False
+
+    def toggle_surface_opacity(self, up):
+        current_opacity = self.opacity_spinbox.value()
+        if up:
+            current_opacity += 0.05
+            if current_opacity > 1: current_opacity = 1
+        else:
+            current_opacity -= 0.05
+            if current_opacity < 0: current_opacity = 0
+        self.opacity_spinbox.setValue(current_opacity)
+
+    def opacity_value_change(self, value):
+        if self.ignore_spinbox_value_change: return 0
+        checked_button = self.button_group_actors_names.checkedButton()
+        if checked_button:
+            actor_name = checked_button.text()
+            if actor_name == 'image': 
+                self.set_image_opacity(value)
+            elif actor_name == 'mask': 
+                self.set_mask_opacity(value)
+            elif actor_name in self.mesh_actors: 
+                self.store_mesh_opacity[actor_name] = copy.deepcopy(self.mesh_opacity[actor_name])
+                self.mesh_opacity[actor_name] = value
+                self.set_mesh_opacity(actor_name, self.mesh_opacity[actor_name])
+        else:
+            self.ignore_spinbox_value_change = True
+            self.opacity_spinbox.setValue(value)
+            self.ignore_spinbox_value_change = False
+            return 0
         
-        self.image_path = None
-        self.mask_path = None
-        self.mesh_path = None
-        self.pose_path = None
-        self.meshdict = {}
-            
-        # allow to add files
-        fileMenu = mainMenu.addMenu('File')
-        fileMenu.addAction('Add Workspace', self.add_workspace)
-        fileMenu.addAction('Add Image', self.add_image_file)
-        fileMenu.addAction('Add Mask', self.add_mask_file)
-        fileMenu.addAction('Add Mesh', self.add_mesh_file)
-        fileMenu.addAction('Clear', self.clear_plot)
-
-        # allow to export files
-        exportMenu = mainMenu.addMenu('Export')
-        exportMenu.addAction('Image Render', self.export_image_plot)
-        exportMenu.addAction('Mask Render', self.export_mask_plot)
-        exportMenu.addAction('Mesh Render', self.export_mesh_plot)
-        exportMenu.addAction('SegMesh Render', self.export_segmesh_plot)
-        exportMenu.addAction('Pose', self.export_pose)
-                
-        # Add camera related actions
-        CameraMenu = mainMenu.addMenu('Camera')
-        CameraMenu.addAction('Calibrate', self.camera_calibrate)
-        CameraMenu.addAction('Reset Camera (c)', self.reset_camera)
-        CameraMenu.addAction('Zoom In (x)', self.zoom_in)
-        CameraMenu.addAction('Zoom Out (z)', self.zoom_out)
-
-        # add mirror actors related actions
-        mirrorMenu = mainMenu.addMenu('Mirror')
-        mirror_x = functools.partial(self.mirror_actors, direction='x')
-        mirrorMenu.addAction('Mirror X axis', mirror_x)
-        mirror_y = functools.partial(self.mirror_actors, direction='y')
-        mirrorMenu.addAction('Mirror Y axis', mirror_y)
+    def toggle_hide_meshes_button(self):
+        self.toggle_hide_meshes_flag = not self.toggle_hide_meshes_flag
         
-        # Add register related actions
-        RegisterMenu = mainMenu.addMenu('Register')
-        RegisterMenu.addAction('Reset GT Pose (k)', self.reset_gt_pose)
-        RegisterMenu.addAction('Update GT Pose (l)', self.update_gt_pose)
-        RegisterMenu.addAction('Current Pose (t)', self.current_pose)
-        RegisterMenu.addAction('Undo Pose (s)', self.undo_pose)
-
-        # Add pnp algorithm related actions
-        PnPMenu = mainMenu.addMenu('Run')
-        PnPMenu.addAction('EPnP with mesh', self.epnp_mesh)
-        epnp_nocs_mask = functools.partial(self.epnp_mask, True)
-        PnPMenu.addAction('EPnP with nocs mask', epnp_nocs_mask)
-        epnp_latlon_mask = functools.partial(self.epnp_mask, False)
-        PnPMenu.addAction('EPnP with latlon mask', epnp_latlon_mask)
+        if self.toggle_hide_meshes_flag:
+            for button in self.button_group_actors_names.buttons():
+                if button.text() in self.mesh_actors:
+                    button.setChecked(True); self.opacity_value_change(0)
+    
+            checked_button = self.button_group_actors_names.checkedButton()
+            if checked_button: 
+                self.ignore_spinbox_value_change = True
+                self.opacity_spinbox.setValue(0.0)
+                self.ignore_spinbox_value_change = False
+            else: QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+        
+        else:
+            for button in self.button_group_actors_names.buttons():
+                if button.text() in self.mesh_actors:
+                    button.setChecked(True)
+                    self.opacity_value_change(self.store_mesh_opacity[button.text()])
+
+            checked_button = self.button_group_actors_names.checkedButton()
+            if checked_button:
+                self.ignore_spinbox_value_change = True
+                if checked_button.text() in self.mesh_actors: self.opacity_spinbox.setValue(self.mesh_opacity[checked_button.text()])
+                self.ignore_spinbox_value_change = False
+            else: QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def set_camera_extrinsics(self):
         self.camera.SetPosition((0,0,self.cam_position))
         self.camera.SetFocalPoint((*self.camera.GetWindowCenter(),0)) # Get the camera window center
         self.camera.SetViewUp(self.cam_viewup)
     
     def set_camera_intrinsics(self):
@@ -370,29 +423,33 @@
  
     def set_camera_props(self):
         self.set_camera_intrinsics()
         self.set_camera_extrinsics()
         self.plotter.camera = self.camera.copy()
 
     def camera_calibrate(self):
-        if self.image_path != '' and self.image_path is not None:
+        if self.image_path:
             original_image = np.array(PIL.Image.open(self.image_path), dtype='uint8')
             # make the the original image shape is [h, w, 3] to match with the rendered calibrated_image
+            original_image = original_image[..., :3]
             if len(original_image.shape) == 2: original_image = original_image[..., None]
             if original_image.shape[-1] == 1: original_image = np.dstack((original_image, original_image, original_image))
-            calibrated_image = np.array(self.render_image(self.image_actor, self.plotter.camera.copy()), dtype='uint8')
+            calibrated_image = np.array(self.render_image(self.plotter.camera.copy()), dtype='uint8')
+            if original_image.shape != calibrated_image.shape:
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "Original image shape is not equal to calibrated image shape!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+                return 0
         else:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         
-        calibrate_pop = CalibrationPopWindow(calibrated_image, original_image)
+        calibrate_pop = widgets_gui.CalibrationPopWindow(calibrated_image, original_image)
         calibrate_pop.exec_()
 
     def set_camera(self):
-        dialog = CameraPropsInputDialog(
+        dialog = widgets_gui.CameraPropsInputDialog(
             line1=("Fx", self.fx), 
             line2=("Fy", self.fy), 
             line3=("Cx", self.cx), 
             line4=("Cy", self.cy), 
             line5=("View Up", self.cam_viewup), 
             line6=("Cam Position", self.cam_position))
         if dialog.exec():
@@ -427,655 +484,752 @@
                     return 0
             except: 
                 QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                 return None
         else: 
             return None
 
-    def set_spacing(self):
-        checked_button = self.button_group_actors_names.checkedButton()
-        if checked_button is not None:
-            if checked_button.text() == 'image':
-                spacing, ok = self.input_dialog.getText(self, 'Input', "Set Spacing", text=str(self.image_spacing))
-                if ok:
-                    try: self.image_spacing = ast.literal_eval(spacing)
-                    except: QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-                    self.add_image(self.image_path)
-            elif checked_button.text() == 'mask':
-                spacing, ok = self.input_dialog.getText(self, 'Input', "Set Spacing", text=str(self.mask_spacing))
-                if ok:
-                    try: self.mask_spacing = ast.literal_eval(spacing)
-                    except: QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-                    self.add_mask(self.mask_path)
-            else:
-                spacing, ok = self.input_dialog.getText(self, 'Input', "Set Spacing", text=str(self.mesh_spacing))
-                if ok:
-                    actor_name = checked_button.text()
-                    try: self.mesh_spacing = ast.literal_eval(spacing)
-                    except: QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-                    self.add_mesh(actor_name, self.meshdict[actor_name])
-        else:
-            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-
-    def add_workspace(self):
-        workspace_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.json)")
-        if workspace_path != '':
-            # Clear the plot automatically if loading a new workspace
-            self.clear_plot()
+    def add_workspace(self, prompt=False):
+        if prompt:
+            self.workspace_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.json)")
+        if self.workspace_path:
             self.hintLabel.hide()
-            with open(str(workspace_path), 'r') as f: 
+            with open(str(self.workspace_path), 'r') as f: 
                 workspace = json.load(f)
 
-            self.image_path = workspace['image_path']
-            self.mask_path = workspace['mask_path']
-            self.pose_path = workspace['pose_path']
-            mesh_paths = workspace['mesh_path']
-
-            self.add_image_file(prompt=False)
-            self.add_mask_file(prompt=False)
-            self.add_pose_file()
-
-            for mesh_path in mesh_paths:
-                self.mesh_path = mesh_path
-                self.add_mesh_file(prompt=False)
-
+            if 'image_path' in workspace:
+                self.image_path = workspace['image_path']
+                self.add_image_file()
+            if 'video_path' in workspace:
+                self.video_path = workspace['video_path']
+                self.add_video_file()
+            if 'mask_path' in workspace:
+                self.mask_path = workspace['mask_path']
+                self.add_mask_file()
+            if 'pose_path' in workspace: # need to load pose before loading meshes
+                self.pose_path = workspace['pose_path']
+                self.add_pose_file()
+            if 'mesh_path' in workspace:
+                mesh_path = workspace['mesh_path']
+                for path in mesh_path:
+                    self.mesh_path = path
+                    self.add_mesh_file()
+            
             # reset camera
             self.reset_camera()
 
-    def add_image_file(self, prompt=True):
-        if prompt:
-            if self.image_path == None or self.image_path == '':
-                self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg *.jpeg *.tiff *.bmp *.webp *.ico)")
+    def get_files_from_folder(self, category):
+        dir = pathlib.Path(self.folder_path) / category
+        folders = [d for d in os.listdir(dir) if os.path.isdir(os.path.join(dir, d))]
+        if len(folders) == 1: dir = pathlib.Path(self.folder_path) / category / folders[0]
+        # Retrieve files
+        files = [f for f in os.listdir(dir) if os.path.isfile(os.path.join(dir, f))]
+        self.total_count = len(files)
+        # Sort files
+        files.sort(key=lambda f: int(re.sub('\D', '', f)))
+        return files, dir
+   
+    def add_folder(self, prompt=False):
+        if prompt: 
+            self.folder_path = QtWidgets.QFileDialog.getExistingDirectory(self, "Select Folder")
+        
+        if self.folder_path:
+            folders = [d for d in os.listdir(self.folder_path) if os.path.isdir(os.path.join(self.folder_path, d))]
+            flag = True
+
+            if 'images' in folders:
+                flag = False
+                image_files, image_dir = self.get_files_from_folder('images')
+                self.image_path = str(image_dir / image_files[self.current_frame])
+                if os.path.isfile(self.image_path): self.add_image_file()
+
+            if 'masks' in folders:
+                flag = False
+                mask_files, mask_dir = self.get_files_from_folder('masks')
+                self.mask_path = str(mask_dir / mask_files[self.current_frame])
+                if os.path.isfile(self.mask_path): self.add_mask_file()
+                    
+            if 'poses' in folders:
+                flag = False
+                pose_files, pose_dir = self.get_files_from_folder('poses')
+                self.pose_path = str(pose_dir / pose_files[self.current_frame])
+                if os.path.isfile(self.pose_path): self.add_pose_file()
+                    
+            if self.current_frame == 0:
+                if 'meshes' in folders:
+                    flag = False
+                    dir = pathlib.Path(self.folder_path) / "meshes"
+                    if os.path.isfile(dir / 'mesh_path.txt'):
+                        with open(dir / 'mesh_path.txt', 'r') as f: mesh_path = f.read().splitlines()
+                        for path in mesh_path:
+                            self.mesh_path = path
+                            self.add_mesh_file()
+
+            if flag:
+                self.delete_video_folder()
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "Not a valid folder, please reload a folder", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+                return 0
             else:
-                self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.image_path).parent), "Files (*.png *.jpg *.jpeg *.tiff *.bmp *.webp *.ico)")
+                self.video_path = None # make sure video_path and folder_path are exclusive
+                self.output_text.append(f"-> After reset GT pose, current slide is ({self.current_frame}/{self.total_count})")
+                self.reset_camera()
 
-        if self.image_path != '' and self.image_path is not None:
+    def add_video_file(self, prompt=False):
+        if prompt:
+            self.video_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.avi *.mp4 *.mkv *.mov *.fly *.wmv *.mpeg *.asf *.webm)")
+        if self.video_path:
+            self.hintLabel.hide()
+            self.folder_path = None # make sure video_path and folder_path are exclusive
+            self.video_player = widgets_gui.VideoPlayer(self.video_path, self.current_frame)
+            self.play_video_button.setText("Play Video")
+            self.output_text.append(f"-> Load video {self.video_path} into vision6D")
+            self.output_text.append(f"-> Current frame is ({self.current_frame}/{self.video_player.frame_count})")
+            self.fps = round(self.video_player.fps)
+            self.load_per_frame_info(True)
+            self.sample_video()
+            
+    def add_image_file(self, prompt=False):
+        if prompt:
+            self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg *.jpeg *.tiff *.bmp *.webp *.ico)")
+        if self.image_path:
             self.hintLabel.hide()
             image_source = np.array(PIL.Image.open(self.image_path), dtype='uint8')
             if len(image_source.shape) == 2: image_source = image_source[..., None]
             self.add_image(image_source)
             
-    def add_mask_file(self, prompt=True):
+    def add_mask_file(self, prompt=False):
         if prompt:
-            if self.mask_path == None or self.mask_path == '':
-                self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg *.jpeg *.tiff *.bmp *.webp *.ico)")
-            else:
-                self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.mask_path).parent), "Files (*.png *.jpg *.jpeg *.tiff *.bmp *.webp *.ico)")
-        
-        if self.mask_path != '' and self.mask_path is not None:
+            self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg *.jpeg *.tiff *.bmp *.webp *.ico)") 
+        if self.mask_path:
             self.hintLabel.hide()
             mask_source = np.array(PIL.Image.open(self.mask_path), dtype='uint8')
-            if len(mask_source.shape) == 2: mask_source = mask_source[..., None]
             self.add_mask(mask_source)
 
-    def add_mesh_file(self, prompt=True):
-        if prompt:
-            if self.mesh_path == None or self.mesh_path == '':
-                self.mesh_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.mesh *.ply *.stl *.obj *.off *.dae *.fbx *.3ds *.x3d)")
-            else:
-                self.mesh_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.mesh_path).parent), "Files (*.mesh *.ply)")
-        
-        if self.mesh_path != '' and self.mesh_path is not None:
+    def add_mesh_file(self, prompt=False):
+        if prompt: 
+            self.mesh_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.mesh *.ply *.stl *.obj *.off *.dae *.fbx *.3ds *.x3d)") 
+        if self.mesh_path:
             self.hintLabel.hide()
             mesh_name = pathlib.Path(self.mesh_path).stem
             self.meshdict[mesh_name] = self.mesh_path
             self.mesh_opacity[mesh_name] = self.surface_opacity
             transformation_matrix = self.transformation_matrix
             if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix                   
             self.add_mesh(mesh_name, self.mesh_path, transformation_matrix)
-                      
+
+    def add_pose(self, matrix:np.ndarray=None, rot:np.ndarray=None, trans:np.ndarray=None):
+        if matrix is not None: 
+            self.initial_pose = matrix
+            self.reset_gt_pose()
+            self.reset_camera()
+        else:
+            if (rot and trans): matrix = np.vstack((np.hstack((rot, trans)), [0, 0, 0, 1]))
+
     def add_pose_file(self):
-        if self.pose_path != '' and self.pose_path is not None:
+        if self.pose_path:
             self.hintLabel.hide()
             transformation_matrix = np.load(self.pose_path)
             self.transformation_matrix = transformation_matrix
             if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             self.add_pose(matrix=transformation_matrix)
     
+    def register_pose(self, pose):
+        for actor_name, actor in self.mesh_actors.items():
+            actor.user_matrix = pose
+            self.plotter.add_actor(actor, pickable=True, name=actor_name)
+
+    def reset_gt_pose(self):
+        self.output_text.append(f"-> Reset the GT pose to: \n{self.initial_pose}")
+        self.register_pose(self.initial_pose)
+
+    def update_gt_pose(self):
+        self.initial_pose = self.transformation_matrix
+        self.current_pose()
+        self.output_text.append(f"Update the GT pose to: \n{self.initial_pose}")
+            
+    def current_pose(self):
+        if len(self.mesh_actors) == 1: self.reference = list(self.mesh_actors.keys())[0]
+        if self.reference:
+            self.transformation_matrix = self.mesh_actors[self.reference].user_matrix
+            self.output_text.append(f"-> Current reference mesh is: <span style='background-color:yellow; color:black;'>{self.reference}</span>")
+            self.output_text.append(f"Current pose is: \n{self.transformation_matrix}")
+            self.register_pose(self.transformation_matrix)
+
+    def undo_pose(self):
+        if self.button_group_actors_names.checkedButton():
+            actor_name = self.button_group_actors_names.checkedButton().text()
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Choose a mesh actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            return 0
+        if len(self.undo_poses[actor_name]) != 0: 
+            self.transformation_matrix = self.undo_poses[actor_name].pop()
+            if (self.transformation_matrix == self.mesh_actors[actor_name].user_matrix).all():
+                if len(self.undo_poses[actor_name]) != 0: 
+                    self.transformation_matrix = self.undo_poses[actor_name].pop()
+
+            self.output_text.append(f"-> Current reference mesh is: <span style='background-color:yellow; color:black;'>{actor_name}</span>")
+            self.output_text.append(f"Undo pose to: \n{self.transformation_matrix}")
+                
+            self.mesh_actors[actor_name].user_matrix = self.transformation_matrix
+            self.plotter.add_actor(self.mesh_actors[actor_name], pickable=True, name=actor_name)
+
     def mirror_actors(self, direction):
 
         if direction == 'x': self.mirror_x = not self.mirror_x
         elif direction == 'y': self.mirror_y = not self.mirror_y
 
         #^ mirror the image actor
-        if self.image_actor is not None:
+        if self.image_actor:
             original_image_data = np.array(PIL.Image.open(self.image_path), dtype='uint8')
             if len(original_image_data.shape) == 2: original_image_data = original_image_data[..., None]
             self.add_image(original_image_data)
 
         #^ mirror the mask actor
-        if self.mask_actor is not None:
+        if self.mask_actor:
             original_mask_data = np.array(PIL.Image.open(self.mask_path), dtype='uint8')
             if len(original_mask_data.shape) == 2: original_mask_data = original_mask_data[..., None]
             self.add_mask(original_mask_data)
 
         #^ mirror the mesh actors
-        if len(self.mesh_actors) != 0:
-            for actor_name, _ in self.mesh_actors.items():
-                transformation_matrix = self.transformation_matrix
-                if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
-                if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
-                self.add_mesh(actor_name, self.meshdict[actor_name], transformation_matrix)
-            
+        if self.reference:
+            transformation_matrix = self.initial_pose
+            if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
+            if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
+            self.add_mesh(self.reference, self.meshdict[self.reference], transformation_matrix)
             # Output the mirrored transformation matrix
             self.output_text.append(f"-> Mirrored transformation matrix is: \n{transformation_matrix}")
              
     def remove_actor(self, button):
         name = button.text()
         if name == 'image': 
             actor = self.image_actor
             self.image_actor = None
             self.image_path = None
         elif name == 'mask':
             actor = self.mask_actor
             self.mask_actor = None
             self.mask_path = None
-        else: 
+        elif name in self.mesh_actors: 
             actor = self.mesh_actors[name]
             del self.mesh_actors[name] # remove the item from the mesh dictionary
             del self.mesh_colors[name]
             del self.mesh_opacity[name]
             del self.meshdict[name]
             self.reference = None
             self.color_button.setText("Color")
             self.mesh_spacing = [1, 1, 1]
 
         self.plotter.remove_actor(actor)
         self.track_actors_names.remove(name)
-        self.output_text.append(f"-> Remove actor: <span style='background-color:yellow; color:black;'>{name}</span>")
+        self.output_text.append(f"-> Remove actor: {name}")
         # remove the button from the button group
         self.button_group_actors_names.removeButton(button)
         # remove the button from the self.button_layout widget
         self.button_layout.removeWidget(button)
         # offically delete the button
         button.deleteLater()
 
         # clear out the plot if there is no actor
         if self.image_actor is None and self.mask_actor is None and len(self.mesh_actors) == 0: self.clear_plot()
-   
+
+    def remove_actors_button(self):
+        checked_button = self.button_group_actors_names.checkedButton()
+        if checked_button: self.remove_actor(checked_button)
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            return 0
+
     def clear_plot(self):
         
         # Clear out everything in the remove menu
         for button in self.button_group_actors_names.buttons():
             name = button.text()
             if name == 'image': actor = self.image_actor
             elif name == 'mask': actor = self.mask_actor
-            else: actor = self.mesh_actors[name]
+            elif name in self.mesh_actors: actor = self.mesh_actors[name]
             self.plotter.remove_actor(actor)
             # remove the button from the button group
             self.button_group_actors_names.removeButton(button)
             # remove the button from the self.button_layout widget
             self.button_layout.removeWidget(button)
             # offically delete the button
             button.deleteLater()
 
         self.hintLabel.show()
 
         # Re-initial the dictionaries
+        self.delete_video_folder()
+        self.workspace_path = None
         self.image_path = None
         self.mask_path = None
         self.mesh_path = None
         self.pose_path = None
         self.meshdict = {}
         self.mesh_colors = {}
 
         # reset everything to original actor opacity
         self.mesh_opacity = {}
-        self.image_opacity = 0.99
-        self.mask_opacity = 0.5
+        self.store_mesh_opacity = {}
+        self.image_opacity = 0.8
+        self.mask_opacity = 0.3
+        self.surface_opacity = self.opacity_spinbox.value()
 
-        self.image_spacing = [0.01, 0.01, 1]
-        self.mask_spacing = [0.01, 0.01, 1]
         self.mesh_spacing = [1, 1, 1]
 
         self.mirror_x = False
         self.mirror_y = False
 
         self.reference = None
         self.transformation_matrix = np.eye(4)
         self.image_actor = None
         self.mask_actor = None
         self.mesh_actors = {}
         self.undo_poses = {}
         self.track_actors_names = []
 
-        self.colors = ["cyan", "magenta", "yellow", "lime", "deepskyblue", "salmon", "silver", "aquamarine", "plum", "blueviolet"]
+        self.colors = ["cyan", "magenta", "yellow", "lime", "dodgerblue", "darkviolet", "darkorange", "forestgreen"]
         self.used_colors = []
         self.color_button.setText("Color")
 
-        self.ignore_slider_value_change = True
-        self.opacity_slider.setValue(100)
-        self.ignore_slider_value_change = False
-
         self.clear_output_text()
 
-    def render_image(self, actor, camera):
+    def render_image(self, camera):
         self.render.clear()
-        render_actor = actor.copy(deep=True)
+        render_actor = self.image_actor.copy(deep=True)
         render_actor.GetProperty().opacity = 1
         self.render.add_actor(render_actor, pickable=False)
         self.render.camera = camera
         self.render.disable()
         self.render.show(auto_close=False)
         image = self.render.last_image
         return image
     
-    def render_mesh(self, render_all_meshes, camera, point_clouds):
+    def render_mask(self, camera):
         self.render.clear()
-        for mesh_name, mesh_actor in self.mesh_actors.items():
-            if not render_all_meshes:
-                if mesh_name != self.reference: continue
-            vertices, faces = vis.utils.get_mesh_actor_vertices_faces(mesh_actor)
-            mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
-            colors = vis.utils.get_mesh_actor_scalars(mesh_actor)
-            if colors is not None: 
-                assert colors.shape == vertices.shape, "colors shape should be the same as vertices shape"
-                mesh = self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='surface', opacity=1, name=mesh_name) if not point_clouds else self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=mesh_name)
-            else:
-                mesh = self.render.add_mesh(mesh_data, color=self.mesh_colors[mesh_name], style='surface', opacity=1, name=mesh_name) if not point_clouds else self.render.add_mesh(mesh_data, color=self.mesh_colors[mesh_name], style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=mesh_name)
-            mesh.user_matrix = self.mesh_actors[self.reference].user_matrix
+        render_actor = self.mask_actor.copy(deep=True)
+        render_actor.GetProperty().opacity = 1
+        self.render.add_actor(render_actor, pickable=False)
         self.render.camera = camera
         self.render.disable()
         self.render.show(auto_close=False)
         image = self.render.last_image
         return image
 
-    def export_image_plot(self):
+    def render_mesh(self, camera):
+        self.render.clear()
+        vertices, faces = utils.get_mesh_actor_vertices_faces(self.mesh_actors[self.reference])
+        mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
+        colors = utils.get_mesh_actor_scalars(self.mesh_actors[self.reference])
+        if colors is not None: 
+            assert colors.shape == vertices.shape, "colors shape should be the same as vertices shape"
+            mesh = self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='surface', opacity=1, name=self.reference)
+        else:
+            mesh = self.render.add_mesh(mesh_data, color=self.mesh_colors[self.reference], style='surface', opacity=1, name=self.reference)
+        mesh.user_matrix = self.mesh_actors[self.reference].user_matrix
+        
+        self.render.camera = camera
+        self.render.disable()
+        self.render.show(auto_close=False)
+        image = self.render.last_image
+        return image
+
+    def export_image(self):
 
-        if self.image_actor is None:
+        if self.image_actor:
+            image = self.render_image(camera=self.camera.copy())
+            output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Image Files (*.png)")
+            if output_path:
+                if pathlib.Path(output_path).suffix == '': output_path = output_path.parent / (output_path.stem + '.png')
+                rendered_image = PIL.Image.fromarray(image)
+                rendered_image.save(output_path)
+                self.output_text.append(f"-> Export image render to:\n {str(output_path)}")
+        else:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
-        
-        reply = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
-        if reply == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
-        else: camera = self.plotter.camera.copy()
-
-        image = self.render_image(self.image_actor, camera)
-        output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Image Files (*.png)")
-        if output_path: 
-            rendered_image = PIL.Image.fromarray(image)
-            rendered_image.save(output_path)
-            self.output_text.append(f"-> Export image render to:\n {str(output_path)}")
 
-    def export_mask_plot(self):
-        if self.mask_actor is None:
+    def export_mask(self):
+        if self.mask_actor:
+            image = self.render_mask(camera=self.camera.copy())
+            output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Mask Files (*.png)")
+            if output_path:
+                if pathlib.Path(output_path).suffix == '': output_path = output_path.parent / (output_path.stem + '.png')
+                rendered_image = PIL.Image.fromarray(image)
+                rendered_image.save(output_path)
+                self.output_text.append(f"-> Export mask render to:\n {str(output_path)}")
+        else:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a mask first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
-        
-        reply = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
-        if reply == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
-        else: camera = self.plotter.camera.copy()
-
-        image = self.render_image(self.mask_actor, camera)
-        output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Mask Files (*.png)")
-        if output_path:
-            rendered_image = PIL.Image.fromarray(image)
-            rendered_image.save(output_path)
-            self.output_text.append(f"-> Export mask render to:\n {str(output_path)}")
-
-    def export_mesh_plot(self, reply_reset_camera=None, reply_render_mesh=None, reply_export_surface=None, save_render=True):
+   
+    def export_pose(self):
+        if self.reference: 
+            self.update_gt_pose()
+            output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Pose Files (*.npy)")
+            if output_path:
+                if pathlib.Path(output_path).suffix == '': output_path = output_path.parent / (output_path.stem + '.npy')
+                np.save(output_path, self.transformation_matrix)
+                self.output_text.append(f"-> Saved:\n{self.transformation_matrix}\nExport to:\n {str(output_path)}")
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            return 0
+    
+    def export_mesh_render(self, save_render=True):
 
-        if self.reference is None:
+        if self.reference:
+            image = self.render_mesh(camera=self.camera.copy())
+            if save_render:
+                output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Mesh Files (*.png)")
+                if output_path:
+                    if pathlib.Path(output_path).suffix == '': output_path = output_path.parent / (output_path.stem + '.png')
+                    rendered_image = PIL.Image.fromarray(image)
+                    rendered_image.save(output_path)
+                    self.output_text.append(f"-> Export reference mesh render to:\n {str(output_path)}")
+            return image
+        else:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
-        if reply_reset_camera is None and reply_render_mesh is None and reply_export_surface is None:
-            reply_reset_camera = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
-            reply_render_mesh = QtWidgets.QMessageBox.question(self,"vision6D", "Only render the reference mesh?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
-            reply_export_surface = QtWidgets.QMessageBox.question(self,"vision6D", "Export the mesh as surface?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
-            
-        if reply_reset_camera == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
-        else: camera = self.plotter.camera.copy()
-        if reply_render_mesh == QtWidgets.QMessageBox.No: render_all_meshes = True
-        else: render_all_meshes = False
-        if reply_export_surface == QtWidgets.QMessageBox.No: point_clouds = True
-        else: point_clouds = False
-        
-        image = self.render_mesh(render_all_meshes, camera, point_clouds)
-        
-        if save_render:
-            output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Mesh Files (*.png)")
+    def export_segmesh_render(self):
+
+        if self.reference and self.mask_actor:
+            segmask = self.render_mask(camera=self.camera.copy())
+            if np.max(segmask) > 1: segmask = segmask / 255
+            image = self.render_mesh(camera=self.camera.copy())
+            image = (image * segmask).astype(np.uint8)
+            output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "SegMesh Files (*.png)")
             if output_path:
+                if pathlib.Path(output_path).suffix == '': output_path = output_path.parent / (output_path.stem + '.png')
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_path)
-                self.output_text.append(f"-> Export reference mesh render to:\n {str(output_path)}")
-
-        return image
-
-    def export_segmesh_plot(self):
-
-        if self.reference is None:
-            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-            return 0
-        
-        if self.mask_actor is None: 
-            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a segmentation mask first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+                self.output_text.append(f"-> Export segmask render:\n to {str(output_path)}")
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a mesh or mask first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
-        reply_reset_camera = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
-        reply_export_surface = QtWidgets.QMessageBox.question(self,"vision6D", "Export the mesh as surface?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
+    def set_spacing(self):
+        checked_button = self.button_group_actors_names.checkedButton()
+        if checked_button:
+            actor_name = checked_button.text()
+            if actor_name in self.mesh_actors:
+                spacing, ok = self.input_dialog.getText(self, 'Input', "Set Spacing", text=str(self.mesh_spacing))
+                if ok:
+                    try: self.mesh_spacing = ast.literal_eval(spacing)
+                    except: QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+                    self.add_mesh(actor_name, self.meshdict[actor_name])
+            else:
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select a mesh object instead", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select a mesh actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
-        if reply_reset_camera == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
-        else: camera = self.plotter.camera.copy()
-        if reply_export_surface == QtWidgets.QMessageBox.No: point_clouds = True
-        else: point_clouds = False
-
-        segmask = self.render_image(self.mask_actor, camera)
-        if np.max(segmask) > 1: segmask = segmask / 255
-        image = self.render_mesh(False, camera, point_clouds)
-        image = (image * segmask).astype(np.uint8)
-        output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "SegMesh Files (*.png)")
-        if output_path:
-            rendered_image = PIL.Image.fromarray(image)
-            rendered_image.save(output_path)
-            self.output_text.append(f"-> Export segmask render:\n to {str(output_path)}")
-        
-    def export_pose(self):
-        if self.reference is None: 
-            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+    def set_scalar(self, nocs, actor_name):
+        vertices, faces = utils.get_mesh_actor_vertices_faces(self.mesh_actors[actor_name])
+        vertices_color = vertices
+        if self.mirror_x: vertices_color = utils.transform_vertices(vertices_color, np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]))
+        if self.mirror_y: vertices_color = utils.transform_vertices(vertices_color, np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]))
+        # get the corresponding color
+        colors = utils.color_mesh(vertices_color, nocs=nocs)
+        if colors.shape != vertices.shape: 
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Cannot set the selected color", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
-        self.update_gt_pose()
-        output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Pose Files (*.npy)")
-        if output_path:
-            np.save(output_path, self.transformation_matrix)
-            self.output_text.append(f"-> Saved:\n{self.transformation_matrix}\nExport to:\n {str(output_path)}")
+        assert colors.shape == vertices.shape, "colors shape should be the same as vertices shape"
+        # color the mesh and actor
+        mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
+        mesh = self.plotter.add_mesh(mesh_data, scalars=colors, rgb=True, opacity=self.mesh_opacity[actor_name], name=actor_name)
+        transformation_matrix = pv.array_from_vtkmatrix(self.mesh_actors[actor_name].GetMatrix())
+        mesh.user_matrix = transformation_matrix
+        actor, _ = self.plotter.add_actor(mesh, pickable=True, name=actor_name)
+        actor_colors = utils.get_mesh_actor_scalars(actor)
+        assert (actor_colors == colors).all(), "actor_colors should be the same as colors"
+        assert actor.name == actor_name, "actor's name should equal to actor_name"
+        self.mesh_actors[actor_name] = actor
+
+    def set_color(self, color, actor_name):
+        vertices, faces = utils.get_mesh_actor_vertices_faces(self.mesh_actors[actor_name])
+        mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
+        mesh = self.plotter.add_mesh(mesh_data, color=color, opacity=self.mesh_opacity[actor_name], name=actor_name)
+        transformation_matrix = pv.array_from_vtkmatrix(self.mesh_actors[actor_name].GetMatrix())
+        mesh.user_matrix = transformation_matrix
+        actor, _ = self.plotter.add_actor(mesh, pickable=True, name=actor_name)
+        assert actor.name == actor_name, "actor's name should equal to actor_name"
+        self.mesh_actors[actor_name] = actor
+        
+    def nocs_epnp(self, color_mask, mesh):
+        vertices = mesh.vertices
+        pts3d, pts2d = utils.create_2d_3d_pairs(color_mask, vertices)
+        pts2d = pts2d.astype('float32')
+        pts3d = pts3d.astype('float32')
+        camera_intrinsics = self.camera_intrinsics.astype('float32')
+        predicted_pose = utils.solve_epnp_cv2(pts2d, pts3d, camera_intrinsics, self.camera.position)
+        return predicted_pose
+
+    def latlon_epnp(self, color_mask, mesh):
+        binary_mask = utils.color2binary_mask(color_mask)
+        idx = np.where(binary_mask == 1)
+        # swap the points for opencv, maybe because they handle RGB image differently (RGB -> BGR in opencv)
+        idx = idx[:2][::-1]
+        pts2d = np.stack((idx[0], idx[1]), axis=1)
+        pts3d = []
+        
+        # Obtain the rg color
+        color = color_mask[pts2d[:,1], pts2d[:,0]][..., :2]
+        if np.max(color) > 1: color = color / 255
+        gx = color[:, 0]
+        gy = color[:, 1]
+
+        lat = np.array(self.latlon[..., 0])
+        lon = np.array(self.latlon[..., 1])
+        lonf = lon[mesh.faces]
+        msk = (np.sum(lonf>=0, axis=1)==3) & (np.sum(lat[mesh.faces]>=0, axis=1)==3)
+        for i in range(len(pts2d)):
+            pt = utils.latLon2xyz(mesh, lat, lonf, msk, gx[i], gy[i])
+            pts3d.append(pt)
+       
+        pts3d = np.array(pts3d).reshape((len(pts3d), 3))
+
+        pts2d = pts2d.astype('float32')
+        pts3d = pts3d.astype('float32')
+        camera_intrinsics = self.camera_intrinsics.astype('float32')
+        
+        predicted_pose = utils.solve_epnp_cv2(pts2d, pts3d, camera_intrinsics, self.camera.position)
+
+        return predicted_pose
+
+    def epnp_mesh(self):
+        if len(self.mesh_actors) == 1: self.reference = list(self.mesh_actors.keys())[0]
+        if self.reference:
+            colors = utils.get_mesh_actor_scalars(self.mesh_actors[self.reference])
+            if colors is not None and (not np.all(colors == colors[0])):
+                color_mask = self.export_mesh_render(save_render=False)
+                gt_pose = self.mesh_actors[self.reference].user_matrix
+                if self.mirror_x: gt_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
+                if self.mirror_y: gt_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
+
+                if np.sum(color_mask):
+                    if self.mesh_colors[self.reference] == 'nocs':
+                        vertices, faces = utils.get_mesh_actor_vertices_faces(self.mesh_actors[self.reference])
+                        mesh = trimesh.Trimesh(vertices, faces, process=False)
+                        predicted_pose = self.nocs_epnp(color_mask, mesh)
+                        if self.mirror_x: predicted_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+                        if self.mirror_y: predicted_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+                        error = np.sum(np.abs(predicted_pose - gt_pose))
+                        self.output_text.append(f"-> PREDICTED POSE WITH <span style='background-color:yellow; color:black;'>NOCS COLOR</span>: ")
+                        self.output_text.append(f"{predicted_pose}\nGT POSE: \n{gt_pose}\nERROR: \n{error}")
+                    else:
+                        QtWidgets.QMessageBox.warning(self, 'vision6D', "Only works using EPnP with latlon mask", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+                else:
+                    QtWidgets.QMessageBox.warning(self, 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            else:
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "The mesh need to be colored, with gradient color", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "A mesh need to be loaded/mesh reference need to be set", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+
+    def epnp_mask(self, nocs_method):
+        if self.mask_actor:
+            mask_data = self.render_mask(camera=self.camera.copy())
+            if np.max(mask_data) > 1: mask_data = mask_data / 255
+
+            # current shown mask is binary mask
+            if np.all(np.logical_or(mask_data == 0, mask_data == 1)):
+                if len(self.mesh_actors) == 1: 
+                    self.reference = list(self.mesh_actors.keys())[0]
+                if self.reference:
+                    colors = utils.get_mesh_actor_scalars(self.mesh_actors[self.reference])
+                    if colors is not None and (not np.all(colors == colors[0])):
+                        color_mask = self.export_mesh_render(save_render=False)
+                        nocs_color = (self.mesh_colors[self.reference] == 'nocs')
+                        gt_pose = self.mesh_actors[self.reference].user_matrix
+                        if self.mirror_x: gt_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
+                        if self.mirror_y: gt_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
+                        vertices, faces = utils.get_mesh_actor_vertices_faces(self.mesh_actors[self.reference])
+                        mesh = trimesh.Trimesh(vertices, faces, process=False)
+                    else:
+                        QtWidgets.QMessageBox.warning(self, 'vision6D', "The mesh need to be colored, with gradient color", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+                        return 0
+                else: 
+                    QtWidgets.QMessageBox.warning(self, 'vision6D', "A mesh need to be loaded/mesh reference need to be set", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+                    return 0
+                color_mask = (color_mask * mask_data).astype(np.uint8)
+            
+            if np.sum(color_mask):
+                if nocs_method == nocs_color:
+                    if nocs_method: 
+                        color_theme = 'NOCS'
+                        predicted_pose = self.nocs_epnp(color_mask, mesh)
+                        if self.mirror_x: predicted_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+                        if self.mirror_y: predicted_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+                    else: 
+                        color_theme = 'LATLON'
+                        if self.mirror_x: color_mask = color_mask[:, ::-1, :]
+                        if self.mirror_y: color_mask = color_mask[::-1, :, :]
+                        predicted_pose = self.latlon_epnp(color_mask, mesh)
+                    error = np.sum(np.abs(predicted_pose - gt_pose))
+                    self.output_text.append(f"-> PREDICTED POSE WITH <span style='background-color:yellow; color:black;'>{color_theme} COLOR (MASKED)</span>: ")
+                    self.output_text.append(f"{predicted_pose}\nGT POSE: \n{gt_pose}\nERROR: \n{error}")
+                else:
+                    QtWidgets.QMessageBox.warning(self,"vision6D", "Clicked the wrong method")
+            else:
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+        else:
+            QtWidgets.QMessageBox.warning(self,"vision6D", "please load a mask first")
 
     def copy_output_text(self):
         self.clipboard.setText(self.output_text.toPlainText())
         
     def clear_output_text(self):
         self.output_text.clear()
 
-    # ^Panel
-    def set_panel_bar(self):
-        # Create a left panel layout
-        self.panel_widget = QtWidgets.QWidget()
-        self.panel_layout = QtWidgets.QVBoxLayout(self.panel_widget)
-
-        # Create a top panel bar with a toggle button
-        self.panel_bar = QtWidgets.QMenuBar()
-        self.toggle_action = QtWidgets.QAction("Panel", self)
-        self.toggle_action.triggered.connect(self.toggle_panel)
-        self.panel_bar.addAction(self.toggle_action)
-        self.setMenuBar(self.panel_bar)
-
-        self.panel_display()
-        self.panel_output()
-        
-        # Set the stretch factor for each section to be equal
-        self.panel_layout.setStretchFactor(self.display, 1)
-        self.panel_layout.setStretchFactor(self.output, 1)
-
-    def toggle_panel(self):
-
-        if self.panel_widget.isVisible():
-            # self.panel_widget width changes when the panel is visiable or hiden
-            self.panel_widget_width = self.panel_widget.width()
-            self.panel_widget.hide()
-            x = (self.plotter.size().width() + self.panel_widget_width - self.hintLabel.width()) // 2
-            y = (self.plotter.size().height() - self.hintLabel.height()) // 2
-            self.hintLabel.move(x, y)
-        else:
-            self.panel_widget.show()
-            x = (self.plotter.size().width() - self.panel_widget_width - self.hintLabel.width()) // 2
-            y = (self.plotter.size().height() - self.hintLabel.height()) // 2
-            self.hintLabel.move(x, y)
-
-    def add_button_actor_name(self, actor_name):
-        button = QtWidgets.QPushButton(actor_name)
-        button.setCheckable(True)  # Set the button to be checkable
-        button.clicked.connect(lambda _, text=actor_name: self.button_actor_name_clicked(text))
-        button.setChecked(True)
-        button.setFixedSize(self.display.size().width(), 50)
-        self.button_layout.insertWidget(0, button) # insert from the top # self.button_layout.addWidget(button)
-        self.button_group_actors_names.addButton(button)
-        self.button_actor_name_clicked(actor_name)
-
     def update_color_button_text(self, text, popup):
         self.color_button.setText(text)
         popup.close() # automatically close the popup window
 
     def show_color_popup(self):
 
         checked_button = self.button_group_actors_names.checkedButton()
-        if checked_button is None:
+        if checked_button:
+            actor_name = checked_button.text()
+            if actor_name in self.mesh_actors:
+                popup = widgets_gui.PopUpDialog(self, on_button_click=lambda text: self.update_color_button_text(text, popup))
+                button_position = self.color_button.mapToGlobal(QPoint(0, 0))
+                popup.move(button_position + QPoint(self.color_button.width(), 0))
+                popup.exec_()
+
+                text = self.color_button.text()
+                self.mesh_colors[actor_name] = text
+                if text == 'nocs': self.set_scalar(True, actor_name)
+                elif text == 'latlon': self.set_scalar(False, actor_name)
+                else: self.set_color(text, actor_name)
+            else:
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "Only be able to color mesh actors", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+        else:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-            return 0
-
-        actor_name = checked_button.text()
 
-        if actor_name not in self.mesh_actors:
-            QtWidgets.QMessageBox.warning(self, 'vision6D', "Only be able to color mesh actors", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+    def load_per_frame_info(self, save=False):
+        if self.video_path:
+            self.video_player.cap.set(cv2.CAP_PROP_POS_FRAMES, self.current_frame)
+            ret, frame = self.video_player.cap.read()
+            if ret: 
+                video_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+                self.add_image(video_frame)
+                if save:
+                    os.makedirs(pathlib.Path(self.video_path).parent / f"{pathlib.Path(self.video_path).stem}_vision6D", exist_ok=True)
+                    os.makedirs(pathlib.Path(self.video_path).parent / f"{pathlib.Path(self.video_path).stem}_vision6D" / "frames", exist_ok=True)
+                    output_frame_path = pathlib.Path(self.video_path).parent / f"{pathlib.Path(self.video_path).stem}_vision6D" / "frames" / f"frame_{self.current_frame}.png"
+                    save_frame = PIL.Image.fromarray(video_frame)
+                    
+                    # save each frame
+                    save_frame.save(output_frame_path)
+                    self.output_text.append(f"-> Save frame {self.current_frame}: ({self.current_frame}/{self.video_player.frame_count})")
+                    self.image_path = str(output_frame_path)
+
+                    # save gt_pose for each frame
+                    os.makedirs(pathlib.Path(self.video_path).parent / f"{pathlib.Path(self.video_path).stem}_vision6D" / "poses", exist_ok=True)
+                    output_pose_path = pathlib.Path(self.video_path).parent / f"{pathlib.Path(self.video_path).stem}_vision6D" / "poses" / f"pose_{self.current_frame}.npy"
+                    self.current_pose()
+                    np.save(output_pose_path, self.transformation_matrix)
+                    self.output_text.append(f"-> Save frame {self.current_frame} pose: \n{self.transformation_matrix}")
+        elif self.folder_path:
+            # save gt_pose for specific frame
+            os.makedirs(pathlib.Path(self.folder_path) / "vision6D", exist_ok=True)
+            os.makedirs(pathlib.Path(self.folder_path) / "vision6D" / "poses", exist_ok=True)
+            output_pose_path = pathlib.Path(self.folder_path) / "vision6D" / "poses" / f"{pathlib.Path(self.pose_path).stem}.npy"
+            self.current_pose()
+            np.save(output_pose_path, self.transformation_matrix)
+            self.output_text.append(f"-> Save frame {pathlib.Path(self.pose_path).stem} pose: \n{self.transformation_matrix}")
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a video or folder!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            return 0
+    
+    def sample_video(self):
+        if self.video_path:
+            self.video_sampler = widgets_gui.VideoSampler(self.video_player, self.fps)
+            res = self.video_sampler.exec_()
+            if res == QtWidgets.QDialog.Accepted: self.fps = round(self.video_sampler.fps)
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
-        popup = PopUpDialog(self, on_button_click=lambda text: self.update_color_button_text(text, popup))
-        button_position = self.color_button.mapToGlobal(QPoint(0, 0))
-        popup.move(button_position + QPoint(self.color_button.width(), 0))
-        popup.exec_()
-
-        text = self.color_button.text()
-        self.mesh_colors[actor_name] = text
-        if text == 'nocs': self.set_scalar(True, actor_name)
-        elif text == 'latlon': self.set_scalar(False, actor_name)
-        else: self.set_color(text, actor_name)
-
-    def remove_actors_button(self):
-        checked_button = self.button_group_actors_names.checkedButton()
-        if checked_button is None: 
-            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-        else: self.remove_actor(checked_button)
-
-    def opacity_value_change(self, value):
-        if self.ignore_slider_value_change: return 0
-        checked_button = self.button_group_actors_names.checkedButton()
-        if checked_button is not None:
-            actor_name = checked_button.text()
-            if actor_name == 'image': 
-                self.store_image_opacity = copy.deepcopy(self.image_opacity)
-                self.set_image_opacity(value / 100)
-            elif actor_name == 'mask': 
-                self.store_mask_opacity = copy.deepcopy(self.mask_opacity)
-                self.set_mask_opacity(value / 100)
-            else: 
-                self.store_mesh_opacity[actor_name] = copy.deepcopy(self.mesh_opacity[actor_name])
-                self.mesh_opacity[actor_name] = value / 100
-                self.set_mesh_opacity(actor_name, self.mesh_opacity[actor_name])
+    def play_video(self):
+        if self.video_path:
+            res = self.video_player.exec_()
+            if res == QtWidgets.QDialog.Accepted:
+                self.current_frame = self.video_player.current_frame
+                self.output_text.append(f"-> Current frame is ({self.current_frame}/{self.video_player.frame_count})")
+                self.play_video_button.setText(f"Play ({self.current_frame}/{self.video_player.frame_count})")
+                self.load_per_frame_info()
         else:
-            self.ignore_slider_value_change = True
-            self.opacity_slider.setValue(value)
-            self.ignore_slider_value_change = False
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
-        
-    def toggle_hide_actors_button(self):
-        self.toggle_hide_actors_flag = not self.toggle_hide_actors_flag
-        
-        if self.toggle_hide_actors_flag:
-            for button in self.button_group_actors_names.buttons():
-                button.setChecked(True)
-                actor_name = button.text()
-                self.opacity_value_change(0)
     
-            checked_button = self.button_group_actors_names.checkedButton()
-            if checked_button is not None: 
-                self.ignore_slider_value_change = True
-                self.opacity_slider.setValue(0)
-                self.ignore_slider_value_change = False
-            else: QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-        
+    def prev_frame(self):
+        if self.video_path:
+            current_frame = self.current_frame - self.fps
+            if current_frame >= 0: 
+                self.current_frame = current_frame
+                self.output_text.append(f"-> Current frame is ({self.current_frame}/{self.video_player.frame_count})")
+                pose_path = pathlib.Path(self.video_path).parent / f"{pathlib.Path(self.video_path).stem}_vision6D" / "poses" / f"pose_{self.current_frame}.npy"
+                if os.path.isfile(pose_path): 
+                    self.transformation_matrix = np.load(pose_path)
+                    self.register_pose(self.transformation_matrix)
+                    self.output_text.append(f"-> Load saved frame {self.current_frame} pose: \n{self.transformation_matrix}")
+                else: self.output_text.append(f"-> No saved pose for frame {self.current_frame}")
+                self.play_video_button.setText(f"Play ({self.current_frame}/{self.video_player.frame_count})")
+                self.video_player.slider.setValue(self.current_frame)
+                self.load_per_frame_info()
+        elif self.folder_path:
+            if self.current_frame > 0:
+                self.current_frame -= 1
+                self.add_folder()
         else:
-            for button in self.button_group_actors_names.buttons():
-                button.setChecked(True)
-                actor_name = button.text()
-                if actor_name == 'image': self.opacity_value_change(self.store_image_opacity * 100)
-                elif actor_name == 'mask': self.opacity_value_change(self.store_mask_opacity * 100)
-                else: self.opacity_value_change(self.store_mesh_opacity[actor_name] * 100)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a video or folder!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            return 0
 
-            checked_button = self.button_group_actors_names.checkedButton()
-            if checked_button is not None:
-                actor_name = checked_button.text()
-                self.ignore_slider_value_change = True
-                if actor_name == 'image': self.opacity_slider.setValue(int(self.image_opacity * 100))
-                elif actor_name == 'mask': self.opacity_slider.setValue(int(self.mask_opacity * 100))
-                else: self.opacity_slider.setValue(int(self.mesh_opacity[actor_name] * 100))
-                self.ignore_slider_value_change = False
-            else: QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+    def next_frame(self):
+        if self.video_path:
+            current_frame = self.current_frame + self.fps
+            if current_frame <= self.video_player.frame_count: 
+                # save pose from the previous frame 
+                self.load_per_frame_info(save=True)
+                self.current_frame = current_frame
+                self.output_text.append(f"-> Current frame is ({self.current_frame}/{self.video_player.frame_count})")
+                # load pose for the current frame if the pose exist
+                pose_path = pathlib.Path(self.video_path).parent / f"{pathlib.Path(self.video_path).stem}_vision6D" / "poses" / f"pose_{self.current_frame}.npy"
+                if os.path.isfile(pose_path): 
+                    self.transformation_matrix = np.load(pose_path)
+                    self.register_pose(self.transformation_matrix)
+                    self.output_text.append(f"-> Load saved frame {self.current_frame} pose: \n{self.transformation_matrix}")
+                self.play_video_button.setText(f"Play ({self.current_frame}/{self.video_player.frame_count})")
+                self.video_player.slider.setValue(self.current_frame)
+                self.load_per_frame_info()
+        elif self.folder_path:
+            if self.current_frame < self.total_count:
+                self.current_frame += 1
+                self.add_folder()
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a video or folder!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            return 0
 
-    def panel_display(self):
-        self.display = QtWidgets.QGroupBox("Console")
-        display_layout = QtWidgets.QVBoxLayout()
-        display_layout.setContentsMargins(10, 20, 10, 10)
-
-        #* Create the top widgets (layout)
-        top_layout = QtWidgets.QHBoxLayout()
-        top_layout.setContentsMargins(0, 0, 0, 0)
-
-        # Create Grid layout for function buttons
-        grid_layout = QtWidgets.QGridLayout()
-
-        # Create the set camera button
-        set_camera_button = QtWidgets.QPushButton("Set Camera")
-        set_camera_button.clicked.connect(self.set_camera)
-        grid_layout.addWidget(set_camera_button, 0, 0)
-
-        # Create the actor pose button
-        actor_pose_button = QtWidgets.QPushButton("Set Pose")
-        actor_pose_button.clicked.connect(self.set_pose)
-        grid_layout.addWidget(actor_pose_button, 0, 1)
-
-        # Create the hide button
-        hide_button = QtWidgets.QPushButton("toggle hide")
-        hide_button.clicked.connect(self.toggle_hide_actors_button)
-        grid_layout.addWidget(hide_button, 0, 2)
-
-        # Create the remove button
-        remove_button = QtWidgets.QPushButton("Remove Actor")
-        remove_button.clicked.connect(self.remove_actors_button)
-        grid_layout.addWidget(remove_button, 0, 3)
-
-        # Create the color dropdown menu (comboBox)
-        self.color_button = QtWidgets.QPushButton("Color")
-        self.color_button.clicked.connect(self.show_color_popup)
-        grid_layout.addWidget(self.color_button, 1, 0)
-        
-        # Create the spacing button (comboBox)
-        self.spacing_button = QtWidgets.QPushButton("Spacing")
-        self.spacing_button.clicked.connect(self.set_spacing)
-        grid_layout.addWidget(self.spacing_button, 1, 1)
-
-        self.opacity_slider = QtWidgets.QSlider(Qt.Horizontal)
-        self.opacity_slider.setMinimum(0)
-        self.opacity_slider.setMaximum(100)
-        self.opacity_slider.setValue(100)
-        self.opacity_slider.setTickPosition(QtWidgets.QSlider.TicksBelow)
-        self.opacity_slider.setSingleStep(1)
-        self.ignore_slider_value_change = False 
-        self.opacity_slider.valueChanged.connect(self.opacity_value_change)
-        grid_layout.addWidget(self.opacity_slider, 1, 2, 1, 2)
-
-        grid_widget = QtWidgets.QWidget()
-        grid_widget.setLayout(grid_layout)
-        top_layout.addWidget(grid_widget)
-
-        display_layout.addLayout(top_layout)
-
-        #* Create the bottom widgets
-        actor_widget = QtWidgets.QLabel("Actors")
-        display_layout.addWidget(actor_widget)
-
-        # Create a scroll area for the buttons
-        scroll_area = QtWidgets.QScrollArea()
-        scroll_area.setWidgetResizable(True)
-        display_layout.addWidget(scroll_area)
-
-        # Create a container widget for the buttons
-        button_container = QtWidgets.QWidget()
-        self.button_layout = QtWidgets.QVBoxLayout()
-        self.button_layout.setSpacing(0)  # Remove spacing between buttons
-        button_container.setLayout(self.button_layout)
-
-        self.button_layout.addStretch()
-
-        # Set the container widget as the scroll area's widget
-        scroll_area.setWidget(button_container)
-
-        self.display.setLayout(display_layout)
-        self.panel_layout.addWidget(self.display)
-
-    def panel_output(self):
-        # Add a spacer to the top of the main layout
-        self.output = QtWidgets.QGroupBox("Output")
-        output_layout = QtWidgets.QVBoxLayout()
-        output_layout.setContentsMargins(10, 20, 10, 10)
-
-        #* Create the top widgets (layout)
-        top_layout = QtWidgets.QHBoxLayout()
-        top_layout.setContentsMargins(0, 0, 0, 0)
-
-        # Create Grid layout for function buttons
-        grid_layout = QtWidgets.QGridLayout()
-
-        # Create the set camera button
-        copy_text_button = QtWidgets.QPushButton("Copy")
-        copy_text_button.clicked.connect(self.copy_output_text)
-        grid_layout.addWidget(copy_text_button, 0, 2, 1, 1)
-
-        # Create the actor pose button
-        clear_text_button = QtWidgets.QPushButton("Clear")
-        clear_text_button.clicked.connect(self.clear_output_text)
-        grid_layout.addWidget(clear_text_button, 0, 3, 1, 1)
-
-        grid_widget = QtWidgets.QWidget()
-        grid_widget.setLayout(grid_layout)
-        top_layout.addWidget(grid_widget)
-        output_layout.addLayout(top_layout)
-
-        self.output_text = QtWidgets.QTextEdit()
-        self.output_text.setReadOnly(False)
-        # Access to the system clipboard
-        self.clipboard = QtGui.QGuiApplication.clipboard()
-        output_layout.addWidget(self.output_text)
-        self.output.setLayout(output_layout)
-        self.panel_layout.addWidget(self.output)
-
-    #^ Show plot
-    def create_plotter(self):
-        self.frame = QtWidgets.QFrame()
-        self.frame.setFixedSize(*self.window_size)
-        self.plotter = QtInteractor(self.frame)
-        # self.plotter.setFixedSize(*self.window_size)
-        self.signal_close.connect(self.plotter.close)
-
-    def show_plot(self):
-        self.plotter.enable_joystick_actor_style()
-        self.plotter.enable_trackball_actor_style()
-        self.plotter.iren.interactor.AddObserver("LeftButtonPressEvent", self.pick_callback)
+    def delete_video_folder(self):
+        # self.video_path and self.folder_path should be exclusive
+        if self.video_path:
+            self.output_text.append(f"-> Delete video {self.video_path} from vision6D")
+            self.play_video_button.setText("Play Video")
+            self.video_path = None
+        elif self.folder_path:
+            self.output_text.append(f"-> Delete folder {self.folder_path} from vision6D")
+            self.folder_path = None
+            
+        self.current_frame = 0
 
-        # camera related key bindings
-        self.plotter.add_key_event('c', self.reset_camera)
-        self.plotter.add_key_event('z', self.zoom_out)
-        self.plotter.add_key_event('x', self.zoom_in)
+    def draw_mask(self):
+        def handle_output_path_change(output_path):
+            if output_path:
+                self.mask_path = output_path
+                self.add_mask(self.mask_path)
+        if self.image_path:
+            self.label_window = widgets_gui.LabelWindow(self.image_path)
+            self.label_window.show()
+            self.label_window.image_label.output_path_changed.connect(handle_output_path_change)
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            return 0
 
-        # registration related key bindings
-        self.plotter.add_key_event('k', self.reset_gt_pose)
-        self.plotter.add_key_event('l', self.update_gt_pose)
-        self.plotter.add_key_event('t', self.current_pose)
-        self.plotter.add_key_event('s', self.undo_pose)
-
-        # change opacity key bindings
-        self.plotter.add_key_event('b', functools.partial(self.toggle_image_opacity, up=True))
-        self.plotter.add_key_event('n', functools.partial(self.toggle_image_opacity, up=False))
-        self.plotter.add_key_event('g', functools.partial(self.toggle_mask_opacity, up=True))
-        self.plotter.add_key_event('h', functools.partial(self.toggle_mask_opacity, up=False))
-        self.plotter.add_key_event('y', functools.partial(self.toggle_surface_opacity, up=True))
-        self.plotter.add_key_event('u', functools.partial(self.toggle_surface_opacity, up=False))
-
-        self.plotter.add_axes()
-        self.plotter.add_camera_orientation_widget()
-
-        self.plotter.show()
-        self.show()
-
-    def showMaximized(self):
-        super(MyMainWindow, self).showMaximized()
-        self.splitter.setSizes([int(self.width() * 0.05), int(self.width() * 0.95)])
```

### Comparing `vision6D-0.2.5/vision6D/__init__.py` & `vision6D-0.2.6/vision6D/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,11 +25,11 @@
     #     }
     # },
 }
 
 # Setup the logging configuration
 logging.config.dictConfig(LOGGING_CONFIG)
 
-from .app import App
-from .interface import Interface
-from .interface_gui import Interface_GUI
-from . import utils
+from .mainwindow import MyMainWindow
+from .GUI import Interface
+from . import utils
+from . import widgets_gui
```

### Comparing `vision6D-0.2.5/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.2.6/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.5/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.2.6/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.5/vision6D/data/style.qss` & `vision6D-0.2.6/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.5/vision6D/utils.py` & `vision6D-0.2.6/vision6D/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,23 +349,37 @@
                 xyz.append(xyznode(m.vertices[f[0]] + c * (m.vertices[f[1]] - m.vertices[f[0]]),d1))
             elif d2 < d3:
                 xyz.append(xyznode(m.vertices[f[0]] + d * (m.vertices[f[2]] - m.vertices[f[0]]),d2))
             else:
                 xyz.append(xyznode(m.vertices[f[1]] + e * (m.vertices[f[2]] - m.vertices[f[1]]),d3))
     return np.min(xyz).pnt
 
-def get_image_mask_actor_scalars(actor):
+def get_image_actor_scalars(actor):
     input = actor.GetMapper().GetInput()
     shape = input.GetDimensions()[::-1]
     point_data = input.GetPointData().GetScalars()
     point_array = vtknp.vtk_to_numpy(point_data)
     if len(point_array.shape) == 1: point_array = point_array.reshape(*point_array.shape, 1)
     scalars = point_array.reshape(*shape[1:], point_array.shape[-1])
     return scalars
 
+def get_mask_actor_points(actor):
+    input = actor.GetMapper().GetInput()
+    point_data = input.GetPoints().GetData()
+    points_array = vtknp.vtk_to_numpy(point_data)
+    vtk_matrix = actor.GetMatrix()
+    matrix = np.array([[vtk_matrix.GetElement(i, j) for j in range(4)] for i in range(4)])
+    # Calculate points not with homogeneous form
+    points = (matrix[:3, :3] @ points_array.T).T + matrix[:3, 3:].T
+    # Calculate points with homogeneous coordinates
+    homogeneous_points = np.hstack((points_array, np.ones((points_array.shape[0], 1))))
+    transformed_points = ((matrix @ homogeneous_points.T).T)[:, :3]
+    assert np.isclose(transformed_points, points).all(), "points and transformed_points should be very very close!"
+    return transformed_points
+
 def get_mesh_actor_vertices_faces(actor):
     input = actor.GetMapper().GetInput()
     points = input.GetPoints().GetData()
     cells = input.GetPolys().GetData()
     vertices = vtknp.vtk_to_numpy(points)
     """
     # popular presentation
@@ -384,9 +398,9 @@
     faces = faces[:, 1:] # trim the first element in each row
     return vertices, faces
 
 def get_mesh_actor_scalars(actor):
     input = actor.GetMapper().GetInput()
     point_data = input.GetPointData()
     scalars = point_data.GetScalars()
-    if scalars is not None: scalars = vtknp.vtk_to_numpy(scalars)
+    if scalars: scalars = vtknp.vtk_to_numpy(scalars)
     return scalars
```

### Comparing `vision6D-0.2.5/vision6D.egg-info/PKG-INFO` & `vision6D-0.2.6/vision6D.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.5
+Version: 0.2.6
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

