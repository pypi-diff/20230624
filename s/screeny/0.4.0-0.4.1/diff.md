# Comparing `tmp/screeny-0.4.0.tar.gz` & `tmp/screeny-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screeny-0.4.0.tar", last modified: Thu Jun 22 19:52:37 2023, max compression
+gzip compressed data, was "screeny-0.4.1.tar", last modified: Sat Jun 24 11:33:04 2023, max compression
```

## Comparing `screeny-0.4.0.tar` & `screeny-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-06-22 19:52:37.276400 screeny-0.4.0/
--rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.4.0/LICENSE
--rw-r--r--   0 paulpol    (501) staff       (20)    25695 2023-05-12 15:40:17.000000 screeny-0.4.0/LICENSE-3RD-Party.txt
--rw-r--r--   0 paulpol    (501) staff       (20)     3557 2023-06-22 19:52:37.276584 screeny-0.4.0/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)     3176 2023-06-22 19:43:27.000000 screeny-0.4.0/README.md
--rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.4.0/pyproject.toml
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-06-22 19:52:37.273563 screeny-0.4.0/screeny/
--rw-r--r--   0 paulpol    (501) staff       (20)      239 2023-06-22 19:28:07.000000 screeny-0.4.0/screeny/__init__.py
--rw-r--r--   0 paulpol    (501) staff       (20)     7260 2023-06-22 19:43:27.000000 screeny-0.4.0/screeny/image.py
--rw-r--r--   0 paulpol    (501) staff       (20)      445 2023-05-12 15:40:04.000000 screeny-0.4.0/screeny/mouse.py
--rw-r--r--   0 paulpol    (501) staff       (20)     2294 2023-05-12 18:59:44.000000 screeny-0.4.0/screeny/screeny.py
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-06-22 19:52:37.275978 screeny-0.4.0/screeny.egg-info/
--rw-r--r--   0 paulpol    (501) staff       (20)     3557 2023-06-22 19:52:37.000000 screeny-0.4.0/screeny.egg-info/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)      291 2023-06-22 19:52:37.000000 screeny-0.4.0/screeny.egg-info/SOURCES.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-06-22 19:52:37.000000 screeny-0.4.0/screeny.egg-info/dependency_links.txt
--rw-r--r--   0 paulpol    (501) staff       (20)       55 2023-06-22 19:52:37.000000 screeny-0.4.0/screeny.egg-info/requires.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-06-22 19:52:37.000000 screeny-0.4.0/screeny.egg-info/top_level.txt
--rw-r--r--   0 paulpol    (501) staff       (20)      528 2023-06-22 19:52:37.277384 screeny-0.4.0/setup.cfg
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-06-24 11:33:04.845539 screeny-0.4.1/
+-rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.4.1/LICENSE
+-rw-r--r--   0 paulpol    (501) staff       (20)    25695 2023-05-12 15:40:17.000000 screeny-0.4.1/LICENSE-3RD-Party.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)     3998 2023-06-24 11:33:04.845770 screeny-0.4.1/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)     3617 2023-06-24 11:31:29.000000 screeny-0.4.1/README.md
+-rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.4.1/pyproject.toml
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-06-24 11:33:04.842065 screeny-0.4.1/screeny/
+-rw-r--r--   0 paulpol    (501) staff       (20)      239 2023-06-22 19:57:12.000000 screeny-0.4.1/screeny/__init__.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     7536 2023-06-24 11:29:45.000000 screeny-0.4.1/screeny/image.py
+-rw-r--r--   0 paulpol    (501) staff       (20)      445 2023-05-12 15:40:04.000000 screeny-0.4.1/screeny/mouse.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     2294 2023-05-12 18:59:44.000000 screeny-0.4.1/screeny/screeny.py
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-06-24 11:33:04.845178 screeny-0.4.1/screeny.egg-info/
+-rw-r--r--   0 paulpol    (501) staff       (20)     3998 2023-06-24 11:33:04.000000 screeny-0.4.1/screeny.egg-info/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)      291 2023-06-24 11:33:04.000000 screeny-0.4.1/screeny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-06-24 11:33:04.000000 screeny-0.4.1/screeny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)       55 2023-06-24 11:33:04.000000 screeny-0.4.1/screeny.egg-info/requires.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-06-24 11:33:04.000000 screeny-0.4.1/screeny.egg-info/top_level.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)      528 2023-06-24 11:33:04.846517 screeny-0.4.1/setup.cfg
```

### Comparing `screeny-0.4.0/LICENSE` & `screeny-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `screeny-0.4.0/LICENSE-3RD-Party.txt` & `screeny-0.4.1/LICENSE-3RD-Party.txt`

 * *Files identical despite different names*

### Comparing `screeny-0.4.0/PKG-INFO` & `screeny-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screeny
-Version: 0.4.0
+Version: 0.4.1
 Summary: A simple python library for working with screens and images.
 Author: Paul Pol
 Author-email: mail@paul-pol.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -34,26 +34,27 @@
 * [Screeny.get_mouse_pos](#screenyget_mouse_pos)
 * [Screeny.locate_image](#screenylocate_imageimage-str--npndarray--image--rect-rect-confidence-float)
 * [Screeny.read_text](#screenyread_textrect-rect)
 * [Screeny.take_screenshot](#screenytake_screenshotrect-rect)
 ####
 * [Image.__init__](#imageinitimage-str--npndarray--image)
 * [Image.binarize](#imagebinarizemethod-str-threshold-int)
-* Image.compute_descriptors
+* [Image.compute_descriptors](#imagecompute_descriptors)
 * [Image.denoise](#imagedenoise)
-* Image.detect_features
-* Image.detect_keypoints
+* [Image.detect_features](#imagedetect_features)
+* [Image.detect_keypoints](#imagedetect_keypoints)
 * [Image.get_data](#imageget_data)
 * [Image.invert](#imageinvert)
 * [Image.locate_image](#imagelocate_imageimage_to_find-str--npndarray--image-confidence-float)
-* Image.match_features
+* [Image.match_features](#imagematch_featuresimage_to_find-str--npndarray--image)
 * [Image.read_text](#imageread_textresize_factor-int-whitelist-str)
 * [Image.resize](#imageresizefactor-int)
+* [Image.save](#imagesavetitle-str-path-str)
 * [Image.show](#imageshowtitle-str)
-* Image.show_matches
+* [Image.show_matches](#imageshow_matchesimage_to_find-str--npndarray--image-matches-list)
 * [Image.to_grayscale](#imageto_grayscale)
 * [Image.to_hsv](#imageto_hsv)
 
 ### Screeny-class
 
 #### Screeny.get_mouse_pos()
         
@@ -133,14 +134,20 @@
 
 ---
 #### Image.resize(factor: int)
 
 Resizes the image with a given factor.
 
 ---
+#### Image.save(title: str[, path: str])
+
+Saves the image on the disk in a given path with a given title.
+If no path is specified, the file be saved in the current active directory.
+
+---
 #### Image.show([title: str])
 
 Displays the image.
 
 ---
 #### Image.show_matches(image_to_find: str | np.ndarray | Image, matches: list)
```

### Comparing `screeny-0.4.0/README.md` & `screeny-0.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 * [Screeny.get_mouse_pos](#screenyget_mouse_pos)
 * [Screeny.locate_image](#screenylocate_imageimage-str--npndarray--image--rect-rect-confidence-float)
 * [Screeny.read_text](#screenyread_textrect-rect)
 * [Screeny.take_screenshot](#screenytake_screenshotrect-rect)
 ####
 * [Image.__init__](#imageinitimage-str--npndarray--image)
 * [Image.binarize](#imagebinarizemethod-str-threshold-int)
-* Image.compute_descriptors
+* [Image.compute_descriptors](#imagecompute_descriptors)
 * [Image.denoise](#imagedenoise)
-* Image.detect_features
-* Image.detect_keypoints
+* [Image.detect_features](#imagedetect_features)
+* [Image.detect_keypoints](#imagedetect_keypoints)
 * [Image.get_data](#imageget_data)
 * [Image.invert](#imageinvert)
 * [Image.locate_image](#imagelocate_imageimage_to_find-str--npndarray--image-confidence-float)
-* Image.match_features
+* [Image.match_features](#imagematch_featuresimage_to_find-str--npndarray--image)
 * [Image.read_text](#imageread_textresize_factor-int-whitelist-str)
 * [Image.resize](#imageresizefactor-int)
+* [Image.save](#imagesavetitle-str-path-str)
 * [Image.show](#imageshowtitle-str)
-* Image.show_matches
+* [Image.show_matches](#imageshow_matchesimage_to_find-str--npndarray--image-matches-list)
 * [Image.to_grayscale](#imageto_grayscale)
 * [Image.to_hsv](#imageto_hsv)
 
 ### Screeny-class
 
 #### Screeny.get_mouse_pos()
         
@@ -120,14 +121,20 @@
 
 ---
 #### Image.resize(factor: int)
 
 Resizes the image with a given factor.
 
 ---
+#### Image.save(title: str[, path: str])
+
+Saves the image on the disk in a given path with a given title.
+If no path is specified, the file be saved in the current active directory.
+
+---
 #### Image.show([title: str])
 
 Displays the image.
 
 ---
 #### Image.show_matches(image_to_find: str | np.ndarray | Image, matches: list)
```

### Comparing `screeny-0.4.0/screeny/image.py` & `screeny-0.4.1/screeny/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from screeny import *
 from typing import Union
 
 import copy
 import numpy as np, cv2, pytesseract
-# pytesseract.pytesseract.tesseract_cmd = r'/usr/local/Cellar/tesseract/5.3.1/bin/tesseract'
 
 
 class Image:
 
     data: np.ndarray = np.array([])
     color_code: str = ""
     orb_detector: cv2.ORB = None
@@ -30,42 +29,65 @@
             self.descriptors = image.descriptors
         else:
             raise Exception("Unknown image-type!")
 
     def get_data(self):
         return self.data
 
-    def to_grayscale(self) -> 'Image':
-        if self.color_code == "RGB":
-            self.data = cv2.cvtColor(self.data, cv2.COLOR_RGB2GRAY)
-        elif self.color_code == "BGR":
-            self.data = cv2.cvtColor(self.data, cv2.COLOR_BGR2GRAY)
-        elif self.color_code == "HSV":
-            self.data = cv2.cvtColor(self.data, cv2.COLOR_HSV2GRAY)
-        elif self.color_code == "GRAY":
-            pass
+    def binarize(self, method: str = "otsus_thresholding", threshold: int = 127) -> "Image":
+        if self.color_code != "GRAY":
+            raise Exception("Colorcode should be 'GRAY' for binarizing image!")
+
+        if method == "simple_thresholding":
+            ret, self.data = cv2.threshold(self.data, threshold, 255, cv2.THRESH_BINARY_INV)
+        elif method == "adaptive_thresholding":
+            self.data = cv2.adaptiveThreshold(self.data, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 11, 2)
+        elif method == "otsus_thresholding":
+            # The threshold-value will be automatically detected
+            ret, self.data = cv2.threshold(self.data, 0, 255, cv2.THRESH_BINARY_INV + cv2.THRESH_OTSU)
         else:
-            raise Exception(f"Colorcode {self.color_code} is unknown!")
+            raise Exception(f"Binarization-metho '{method}' is unknown!")
 
-        self.color_code = "GRAY"
         return self
 
-    def to_hsv(self) -> "Image":
-        if self.color_code == "RGB":
-            self.data = cv2.cvtColor(self.data, cv2.COLOR_RGB2HSV)
-        elif self.color_code == "BGR":
-            self.data = cv2.cvtColor(self.data, cv2.COLOR_BGR2HSV)
-        elif self.color_code == "HSV":
-            pass
-        elif self.color_code == "GRAY":
-            self.data = cv2.cvtColor(self.data, cv2.COLOR_GRAY2HSV)
-        else:
-            raise Exception(f"Colorcode {self.color_code} is unknown!")
+    def compute_descriptors(self) -> "Image":
+        """
+        Computes the descriptors of the image.
 
-        self.color_code = "HSV"
+        :return: Image
+        """
+        # compute the descriptors with ORB
+        self.keypoints, self.descriptors = self.orb_detector.compute(self.data, self.keypoints)
+        return self
+
+    def denoise(self) -> "Image":
+        self.data = cv2.fastNlMeansDenoising(self.data, None, 10, 21, 7)
+        return self
+
+    def detect_features(self) -> "Image":
+        """
+        Finds feature in the image.
+
+        :return: Image
+        """
+        self.keypoints, self.descriptors = self.orb_detector.detectAndCompute(self.data, None)
+        return self
+
+    def detect_keypoints(self) -> "Image":
+        """
+        Finds the keypoints of the image.
+
+        :return: Image
+        """
+        # find the keypoints with ORB
+        self.keypoints = self.orb_detector.detect(self.data, None)
+        return self
+
+    def invert(self) -> "Image":
+        self.data = cv2.bitwise_not(self.data)
         return self
 
     def locate_image(self, image_to_find: Union[str, np.ndarray, "Image"], confidence: float = 0.8) -> Point | bool:
         template = Image(image_to_find).to_grayscale()
         image = copy.copy(self)
         image.to_grayscale()
 
@@ -73,37 +95,33 @@
         min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(heat_map)
         if max_val >= confidence:
             w, h = template.get_data().shape
             return Point(max_loc[0] + (w / 2), max_loc[1] + (h / 2))
         else:
             return False
 
-    def resize(self, factor: int) -> "Image":
-        self.data = cv2.resize(self.data, None, fx=factor, fy=factor, interpolation=cv2.INTER_CUBIC)
-        return self
+    def match_features(self, image_to_find: Union[str, np.ndarray, "Image"]) -> list:
+        """
+        Matches the features of the image with another image.
 
-    def binarize(self, method: str = "otsus_thresholding", threshold: int = 127) -> "Image":
-        if self.color_code != "GRAY":
-            raise Exception("Colorcode should be 'GRAY' for binarizing image!")
+        :param image_to_find: str | np.ndarray | Image
+        :return: list
+        """
+        template = Image(image_to_find)  #.to_grayscale()
 
-        if method == "simple_thresholding":
-            ret, self.data = cv2.threshold(self.data, threshold, 255, cv2.THRESH_BINARY_INV)
-        elif method == "adaptive_thresholding":
-            self.data = cv2.adaptiveThreshold(self.data, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 11, 2)
-        elif method == "otsus_thresholding":
-            # The threshold-value will be automatically detected
-            ret, self.data = cv2.threshold(self.data, 0, 255, cv2.THRESH_BINARY_INV + cv2.THRESH_OTSU)
-        else:
-            raise Exception(f"Binarization-metho '{method}' is unknown!")
+        if len(template.descriptors) <= 0:
+            template.detect_features()
 
-        return self
+        if len(self.descriptors) <= 0:
+            self.detect_features()
 
-    def denoise(self) -> "Image":
-        self.data = cv2.fastNlMeansDenoising(self.data, None, 10, 21, 7)
-        return self
+        bf = cv2.BFMatcher(cv2.NORM_HAMMING, crossCheck=True)
+        matches = bf.match(self.descriptors, template.descriptors)  # Match descriptors.
+        matches = sorted(matches, key=lambda x: x.distance)  # Sort them in the order of their distance.
+        return matches
 
     def read_text(
             self, resize_factor: int = None,
             whitelist: str = "._0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
     ):
         image = copy.copy(self)
         image.to_grayscale()
@@ -119,86 +137,78 @@
         # 13    - (Raw line. Treat the image as a single text line, bypassing hacks that are Tesseract-specific.)
         text = pytesseract.image_to_string(
             image.get_data(),
             config="-c tessedit_char_whitelist=" + whitelist + " --psm 3 load_system_dawg=0 load_freq_dawg=0"
         ).strip("\n\r")
         return text
 
+    def resize(self, factor: int) -> "Image":
+        self.data = cv2.resize(self.data, None, fx=factor, fy=factor, interpolation=cv2.INTER_CUBIC)
+        return self
+
+    def save(self, title: str, path: str = "") -> bool:
+        """
+        Saves the image on the disk in a given path with a given title.
+        If no path is specified, the file be saved in the current active directory.
+
+        :param title: str
+        :param path: str
+        :return: bool
+        """
+        return cv2.imwrite(path + title, self.get_data())
+
     def show(self, title: str = "", with_keypoints: bool = False):
         if with_keypoints:
             img2 = cv2.drawKeypoints(self.data, self.keypoints, None, color=(0, 255, 0), flags=0)
             cv2.imshow(title, img2)
             cv2.waitKey(0)
 
             """plt.imshow(img2)
             plt.show()"""
         else:
             cv2.imshow(title, self.data)
             cv2.waitKey(0)
 
-    def invert(self) -> "Image":
-        self.data = cv2.bitwise_not(self.data)
-        return self
-
-    def detect_keypoints(self) -> "Image":
-        """
-        Finds the keypoints of the image.
-
-        :return: Image
-        """
-        # find the keypoints with ORB
-        self.keypoints = self.orb_detector.detect(self.data, None)
-        return self
-
-    def compute_descriptors(self) -> "Image":
-        """
-        Computes the descriptors of the image.
-
-        :return: Image
-        """
-        # compute the descriptors with ORB
-        self.keypoints, self.descriptors = self.orb_detector.compute(self.data, self.keypoints)
-        return self
-
-    def detect_features(self) -> "Image":
-        """
-        Finds feature in the image.
-
-        :return: Image
-        """
-        self.keypoints, self.descriptors = self.orb_detector.detectAndCompute(self.data, None)
-        return self
-
-    def match_features(self, image_to_find: Union[str, np.ndarray, "Image"]) -> list:
-        """
-        Matches the features of the image with another image.
-
-        :param image_to_find: str | np.ndarray | Image
-        :return: list
-        """
-        template = Image(image_to_find)  #.to_grayscale()
-
-        if len(template.descriptors) <= 0:
-            template.detect_features()
-
-        if len(self.descriptors) <= 0:
-            self.detect_features()
-
-        bf = cv2.BFMatcher(cv2.NORM_HAMMING, crossCheck=True)
-        matches = bf.match(self.descriptors, template.descriptors)  # Match descriptors.
-        matches = sorted(matches, key=lambda x: x.distance)  # Sort them in the order of their distance.
-        return matches
-
     def show_matches(self, image_to_find: Union[str, np.ndarray, "Image"], matches: list) -> None:
         """
         Show the two images with matches as lines connect points.
 
         :param image_to_find: str | np.ndarray | Image
         :param matches: list
         :return:
         """
         template = Image(image_to_find)
 
         Image(cv2.drawMatches(
             self.data, self.keypoints, template.get_data(),
             template.keypoints, matches, None, flags=cv2.DrawMatchesFlags_NOT_DRAW_SINGLE_POINTS
         )).show("Matched images")
+
+    def to_grayscale(self) -> 'Image':
+        if self.color_code == "RGB":
+            self.data = cv2.cvtColor(self.data, cv2.COLOR_RGB2GRAY)
+        elif self.color_code == "BGR":
+            self.data = cv2.cvtColor(self.data, cv2.COLOR_BGR2GRAY)
+        elif self.color_code == "HSV":
+            self.data = cv2.cvtColor(self.data, cv2.COLOR_HSV2GRAY)
+        elif self.color_code == "GRAY":
+            pass
+        else:
+            raise Exception(f"Colorcode {self.color_code} is unknown!")
+
+        self.color_code = "GRAY"
+        return self
+
+    def to_hsv(self) -> "Image":
+        if self.color_code == "RGB":
+            self.data = cv2.cvtColor(self.data, cv2.COLOR_RGB2HSV)
+        elif self.color_code == "BGR":
+            self.data = cv2.cvtColor(self.data, cv2.COLOR_BGR2HSV)
+        elif self.color_code == "HSV":
+            pass
+        elif self.color_code == "GRAY":
+            self.data = cv2.cvtColor(self.data, cv2.COLOR_GRAY2HSV)
+        else:
+            raise Exception(f"Colorcode {self.color_code} is unknown!")
+
+        self.color_code = "HSV"
+        return self
```

### Comparing `screeny-0.4.0/screeny/screeny.py` & `screeny-0.4.1/screeny/screeny.py`

 * *Files identical despite different names*

### Comparing `screeny-0.4.0/screeny.egg-info/PKG-INFO` & `screeny-0.4.1/screeny.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screeny
-Version: 0.4.0
+Version: 0.4.1
 Summary: A simple python library for working with screens and images.
 Author: Paul Pol
 Author-email: mail@paul-pol.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -34,26 +34,27 @@
 * [Screeny.get_mouse_pos](#screenyget_mouse_pos)
 * [Screeny.locate_image](#screenylocate_imageimage-str--npndarray--image--rect-rect-confidence-float)
 * [Screeny.read_text](#screenyread_textrect-rect)
 * [Screeny.take_screenshot](#screenytake_screenshotrect-rect)
 ####
 * [Image.__init__](#imageinitimage-str--npndarray--image)
 * [Image.binarize](#imagebinarizemethod-str-threshold-int)
-* Image.compute_descriptors
+* [Image.compute_descriptors](#imagecompute_descriptors)
 * [Image.denoise](#imagedenoise)
-* Image.detect_features
-* Image.detect_keypoints
+* [Image.detect_features](#imagedetect_features)
+* [Image.detect_keypoints](#imagedetect_keypoints)
 * [Image.get_data](#imageget_data)
 * [Image.invert](#imageinvert)
 * [Image.locate_image](#imagelocate_imageimage_to_find-str--npndarray--image-confidence-float)
-* Image.match_features
+* [Image.match_features](#imagematch_featuresimage_to_find-str--npndarray--image)
 * [Image.read_text](#imageread_textresize_factor-int-whitelist-str)
 * [Image.resize](#imageresizefactor-int)
+* [Image.save](#imagesavetitle-str-path-str)
 * [Image.show](#imageshowtitle-str)
-* Image.show_matches
+* [Image.show_matches](#imageshow_matchesimage_to_find-str--npndarray--image-matches-list)
 * [Image.to_grayscale](#imageto_grayscale)
 * [Image.to_hsv](#imageto_hsv)
 
 ### Screeny-class
 
 #### Screeny.get_mouse_pos()
         
@@ -133,14 +134,20 @@
 
 ---
 #### Image.resize(factor: int)
 
 Resizes the image with a given factor.
 
 ---
+#### Image.save(title: str[, path: str])
+
+Saves the image on the disk in a given path with a given title.
+If no path is specified, the file be saved in the current active directory.
+
+---
 #### Image.show([title: str])
 
 Displays the image.
 
 ---
 #### Image.show_matches(image_to_find: str | np.ndarray | Image, matches: list)
```

### Comparing `screeny-0.4.0/setup.cfg` & `screeny-0.4.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = screeny
-version = 0.4.0
+version = 0.4.1
 author = Paul Pol
 author_email = mail@paul-pol.de
 description = A simple python library for working with screens and images.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers =
```

