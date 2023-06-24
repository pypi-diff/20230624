# Comparing `tmp/labelprinterkit-0.4.2.tar.gz` & `tmp/labelprinterkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelprinterkit-0.4.2.tar", max compression
+gzip compressed data, was "labelprinterkit-0.5.1.tar", max compression
```

## Comparing `labelprinterkit-0.4.2.tar` & `labelprinterkit-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.4.2/LICENSE
--rw-r--r--   0        0        0     2247 2023-06-24 10:59:26.674400 labelprinterkit-0.4.2/README.md
--rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.4.2/labelprinterkit/__init__.py
--rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.4.2/labelprinterkit/backends/__init__.py
--rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.4.2/labelprinterkit/backends/bluetooth.py
--rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.4.2/labelprinterkit/backends/network.py
--rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.4.2/labelprinterkit/backends/usb.py
--rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.4.2/labelprinterkit/constants.py
--rw-r--r--   0        0        0     1878 2023-06-24 10:56:51.609529 labelprinterkit-0.4.2/labelprinterkit/doc/examples/complex_label_with_qrcode.py
--rw-r--r--   0        0        0     1864 2023-06-23 21:07:41.480689 labelprinterkit-0.4.2/labelprinterkit/job.py
--rw-r--r--   0        0        0     6822 2023-06-24 10:59:15.379263 labelprinterkit-0.4.2/labelprinterkit/label.py
--rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.4.2/labelprinterkit/page.py
--rw-r--r--   0        0        0     8578 2023-06-24 10:59:26.675400 labelprinterkit-0.4.2/labelprinterkit/printers.py
--rw-r--r--   0        0        0      667 2023-06-24 10:59:26.677400 labelprinterkit-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 labelprinterkit-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.1/README.md
+-rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.5.1/labelprinterkit/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.5.1/labelprinterkit/backends/__init__.py
+-rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.1/labelprinterkit/backends/bluetooth.py
+-rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.1/labelprinterkit/backends/network.py
+-rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.1/labelprinterkit/backends/usb.py
+-rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.5.1/labelprinterkit/constants.py
+-rw-r--r--   0        0        0     2006 2023-06-24 11:52:16.204326 labelprinterkit-0.5.1/labelprinterkit/doc/examples/complex_label_with_qrcode.py
+-rw-r--r--   0        0        0     1864 2023-06-23 21:07:41.480689 labelprinterkit-0.5.1/labelprinterkit/job.py
+-rw-r--r--   0        0        0     6450 2023-06-24 11:50:05.192647 labelprinterkit-0.5.1/labelprinterkit/label.py
+-rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.1/labelprinterkit/page.py
+-rw-r--r--   0        0        0     8578 2023-06-24 10:59:26.675400 labelprinterkit-0.5.1/labelprinterkit/printers.py
+-rw-r--r--   0        0        0      667 2023-06-24 11:52:16.204326 labelprinterkit-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 labelprinterkit-0.5.1/PKG-INFO
```

### Comparing `labelprinterkit-0.4.2/LICENSE` & `labelprinterkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.2/README.md` & `labelprinterkit-0.5.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from labelprinterkit.job import Job
 from labelprinterkit.constants import MediaType, MediaSize
 from labelprinterkit.page import Page
 from PIL import Image
 
 # Create text for the label
 
-text1 = Text("First line", 45, 'comic.ttf', padding=Padding(0, 0, 1, 0))
-text2 = Text("Some text", 25, 'comic.ttf')
-text3 = Text("Other text", 25, 'comic.ttf')
+text1 = Text(45, "First line", 'comic.ttf', padding=Padding(0, 0, 1, 0))
+text2 = Text(25, "Some text", 'comic.ttf')
+text3 = Text(25, "Other text", 'comic.ttf')
 
 # Insert Text into boxes
 box1 = Box(45, text1)
 box2 = Box(25, text2, text3)
 
 # Create label with rows from above
 label = Label(box1, box2)
```

### Comparing `labelprinterkit-0.4.2/labelprinterkit/backends/bluetooth.py` & `labelprinterkit-0.5.1/labelprinterkit/backends/bluetooth.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.2/labelprinterkit/backends/network.py` & `labelprinterkit-0.5.1/labelprinterkit/backends/network.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.2/labelprinterkit/backends/usb.py` & `labelprinterkit-0.5.1/labelprinterkit/backends/usb.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.2/labelprinterkit/constants.py` & `labelprinterkit-0.5.1/labelprinterkit/constants.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.2/labelprinterkit/doc/examples/complex_label_with_qrcode.py` & `labelprinterkit-0.5.1/labelprinterkit/doc/examples/complex_label_with_qrcode.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,31 +24,32 @@
 qrcode = QrCode(70, "https://pypi.org/project/labelprinterkit/")
 
 # Create text for the label
 # The upper text is 25 pixels height and the lower text is 45 pixels height.
 # Both together have the 70 points width of the label.
 # The lower label gets 1 pixel padding on the top for some spacing.
 # If the font_size is not given, the font_size is calculated automatically to fit in the width
-text1 = Text("This label is proudly presented by", 25, 'comic.ttf')
-text2 = Text("labelprinterkit", 45, 'comic.ttf', padding=Padding(0, 1, 0, 0))
+text1 = Text(25, "This label is proudly presented by", 'comic.ttf')
+text2 = Text(45, "labelprinterkit", 'comic.ttf', padding=Padding(0, 1, 0, 0))
 
-# Insert Text into boxes
-box = Box(70, text1, text2, vertical=True)
+# Insert Text into boxes, add left_padding to get some space to the qr code
+right_box = Box(70, text1, text2, vertical=True, left_padding=10)
 
-# Create label with rows from above
-label = Label(qrcode, box)
+# Now we can put the qrcode and the box with text together
+full_box = Box(70, qrcode, right_box)
+
+# Create label with box from above
+label = Label(full_box)
+
+# For debugging purpose you can render an PIL image from the label and save it
+label.image.save('/tmp/label.png')
 
 # Create job with configuration and add label as page
 job = Job(MediaSize.W12, MediaType.LAMINATED_TAPE)
 job.add_page(label)
 
-# Create a page from a Pillow image and add it to the job
-image = Image.new("1", (70, 200), "white")
-page = Page.from_image(image)
-job.add_page(page)
-
 # Use TCP backend to connect to printer
-backend = TCPBackend('labelprinter-1.net.scc.kit.edu')
+backend = TCPBackend('labelprinter-1.example.com')
 printer = P750W(backend)
 
 # Print job
 printer.print(job)
```

### Comparing `labelprinterkit-0.4.2/labelprinterkit/job.py` & `labelprinterkit-0.5.1/labelprinterkit/job.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.2/labelprinterkit/label.py` & `labelprinterkit-0.5.1/labelprinterkit/label.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,16 +39,16 @@
         ...
 
 
 ItemType = TypeVar('ItemType', bound=Item)
 
 
 class Text(Item):
-    def __init__(self, text: str, height: int, font_path: str, font_index: int = 0, font_size: int | None = None,
-            padding: Padding = Padding(0, 0, 0, 0)):
+    def __init__(self, height: int, text: str, font_path: str, font_index: int = 0, font_size: int | None = None,
+                 padding: Padding = Padding(0, 0, 0, 0)):
         self.text = text
         self.height = height
         self.font_path = font_path
         self.font_index = font_index
         self.font_size = font_size
 
         if any([i < 0 for i in padding]):
@@ -101,16 +101,15 @@
             else:
                 return test
 
 
 class QrCode(Item):
     def __init__(self, width: int, data: str,
                  error_correction: qrcode.constants.ERROR_CORRECT_L | qrcode.constants.ERROR_CORRECT_M |
-                                   qrcode.constants.ERROR_CORRECT_H | qrcode.constants.ERROR_CORRECT_Q
-                                    = qrcode.constants.ERROR_CORRECT_M,
+                 qrcode.constants.ERROR_CORRECT_H | qrcode.constants.ERROR_CORRECT_Q = qrcode.constants.ERROR_CORRECT_M,
                  box_size: int | None = None, border: int = 0):
         self._width = width
         self._data = data
         self._error_correction = error_correction
         self._box_size = box_size
         self._border = border
 
@@ -121,15 +120,15 @@
             box_size = self._box_size
         probe_box_size = box_size
         qr_image = None
         while True:
             logger.debug(f"qrcode: {self._data}, probe_box_size: {probe_box_size}")
             qr = qrcode.QRCode(error_correction=self._error_correction, box_size=probe_box_size, border=self._border)
             qr.add_data(self._data)
-            new_image = qr.make_image()._img
+            new_image = qr.make_image()
             if new_image.size[0] <= self._width:
                 qr_image = new_image
                 probe_box_size += 1
             elif qr_image is None:
                 raise RuntimeError("Data does not fit in qrcode")
             else:
                 break
@@ -142,52 +141,43 @@
         image = Image.new("1", (qr_image.size[0], self._width), "white")
         image.paste(qr_image, (0, rest // 2))
 
         return image
 
 
 class Box:
-    def __init__(self, height: int, *items: ItemType, vertical: bool = False):
+    def __init__(self, height: int, *items: ItemType, vertical: bool = False, left_padding: int = 0):
         self.height = height
-        self.length = 0
         self.items = items
         self._vertical = vertical
+        self._left_padding = left_padding
 
     def render(self) -> Image:
         rendered_images = [item.render() for item in self.items]
         if self._vertical:
-            length = max([rendered_image.size[0] for rendered_image in rendered_images])
+            length = max([rendered_image.size[0] for rendered_image in rendered_images]) + self._left_padding
             assert self.height == sum([rendered_image.size[1] for rendered_image in rendered_images])
             image = Image.new("1", (length, self.height), "white")
             xpos = 0
             for rendered_image in rendered_images:
-                image.paste(rendered_image, (0, xpos))
+                image.paste(rendered_image, (self._left_padding, xpos))
                 xpos += rendered_image.size[1]
         else:
-            length = sum([rendered_image.size[0] for rendered_image in rendered_images])
+            length = sum([rendered_image.size[0] for rendered_image in rendered_images]) + self._left_padding
             image = Image.new("1", (length, self.height), "white")
-            ypos = 0
+            ypos = self._left_padding
             for rendered_image in rendered_images:
                 image.paste(rendered_image, (ypos, 0))
                 ypos += rendered_image.size[0]
         return image
 
 
 class Label(BasePage):
-    def __init__(self, *boxes: Box):
-        self.boxes = boxes
-
-        rendered_images = [box.render() for box in self.boxes]
-        length = max([rendered_image.size[0] for rendered_image in rendered_images])
-        width = sum([rendered_image.size[1] for rendered_image in rendered_images])
-        image = Image.new("1", (length, width), "white")
-        xpos = 0
-        for rendered_image in rendered_images:
-            image.paste(rendered_image, (0, xpos))
-            xpos += rendered_image.size[1]
-        self._bitmap, self._width , self._length = image_to_bitmap(image)
+    def __init__(self, item: ItemType):
+        self.item = item
+        self._bitmap, self._width, self._length = image_to_bitmap(self.item.render())
         self._resolution = Resolution.LOW
 
         logger.debug(f"label width {self._width}")
         logger.debug(f"label length {self._length}")
 
         super().__init__()
```

### Comparing `labelprinterkit-0.4.2/labelprinterkit/page.py` & `labelprinterkit-0.5.1/labelprinterkit/page.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.2/labelprinterkit/printers.py` & `labelprinterkit-0.5.1/labelprinterkit/printers.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.2/pyproject.toml` & `labelprinterkit-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labelprinterkit"
-version = "0.4.2"
+version = "0.5.1"
 description = "A library for creating and printing labels for Brother P-Touch devices"
 authors = ["Adrian Tschira <packages@notafile.com>", "Benedikt Neuffer <benedikt.neuffer@kit.edu>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `labelprinterkit-0.4.2/PKG-INFO` & `labelprinterkit-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelprinterkit
-Version: 0.4.2
+Version: 0.5.1
 Summary: A library for creating and printing labels for Brother P-Touch devices
 License: Apache License, Version 2.0
 Author: Adrian Tschira
 Author-email: packages@notafile.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -34,17 +34,17 @@
 from labelprinterkit.job import Job
 from labelprinterkit.constants import MediaType, MediaSize
 from labelprinterkit.page import Page
 from PIL import Image
 
 # Create text for the label
 
-text1 = Text("First line", 45, 'comic.ttf', padding=Padding(0, 0, 1, 0))
-text2 = Text("Some text", 25, 'comic.ttf')
-text3 = Text("Other text", 25, 'comic.ttf')
+text1 = Text(45, "First line", 'comic.ttf', padding=Padding(0, 0, 1, 0))
+text2 = Text(25, "Some text", 'comic.ttf')
+text3 = Text(25, "Other text", 'comic.ttf')
 
 # Insert Text into boxes
 box1 = Box(45, text1)
 box2 = Box(25, text2, text3)
 
 # Create label with rows from above
 label = Label(box1, box2)
```

