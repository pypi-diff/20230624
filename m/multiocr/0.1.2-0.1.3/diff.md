# Comparing `tmp/multiocr-0.1.2.tar.gz` & `tmp/multiocr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiocr-0.1.2.tar", max compression
+gzip compressed data, was "multiocr-0.1.3.tar", max compression
```

## Comparing `multiocr-0.1.2.tar` & `multiocr-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2647 2023-06-19 22:14:53.371351 multiocr-0.1.2/README.md
--rw-r--r--   0        0        0       35 2023-06-10 13:04:19.610231 multiocr-0.1.2/multiocr/__init__.py
--rw-r--r--   0        0        0      338 2023-06-19 22:04:10.847491 multiocr-0.1.2/multiocr/base_class.py
--rw-r--r--   0        0        0     2276 2023-06-21 01:06:27.978422 multiocr-0.1.2/multiocr/main.py
--rw-r--r--   0        0        0      202 2023-06-19 21:48:38.816200 multiocr-0.1.2/multiocr/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-06-10 04:58:23.910390 multiocr-0.1.2/multiocr/pipelines/aws_textract/__init__.py
--rw-r--r--   0        0        0     4383 2023-06-19 22:00:05.907425 multiocr-0.1.2/multiocr/pipelines/aws_textract/engine.py
--rw-r--r--   0        0        0     2535 2023-06-19 21:57:53.639183 multiocr-0.1.2/multiocr/pipelines/easy_ocr/engine.py
--rw-r--r--   0        0        0        0 2023-06-10 04:58:45.721303 multiocr-0.1.2/multiocr/pipelines/paddle_ocr/__init__.py
--rw-r--r--   0        0        0     2707 2023-06-19 21:58:41.369725 multiocr-0.1.2/multiocr/pipelines/paddle_ocr/engine.py
--rw-r--r--   0        0        0        0 2023-06-10 04:55:24.885038 multiocr-0.1.2/multiocr/pipelines/tesseract/__init__.py
--rw-r--r--   0        0        0     3405 2023-06-21 01:17:26.126369 multiocr-0.1.2/multiocr/pipelines/tesseract/engine.py
--rw-r--r--   0        0        0     1319 2023-06-10 08:55:37.312478 multiocr-0.1.2/multiocr/utils.py
--rw-r--r--   0        0        0      378 2023-06-21 01:21:53.829613 multiocr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3281 1970-01-01 00:00:00.000000 multiocr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2647 2023-06-19 22:14:53.371351 multiocr-0.1.3/README.md
+-rw-r--r--   0        0        0       35 2023-06-10 13:04:19.610231 multiocr-0.1.3/multiocr/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-19 22:04:10.847491 multiocr-0.1.3/multiocr/base_class.py
+-rw-r--r--   0        0        0     2276 2023-06-24 05:22:03.118012 multiocr-0.1.3/multiocr/main.py
+-rw-r--r--   0        0        0      202 2023-06-19 21:48:38.816200 multiocr-0.1.3/multiocr/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 04:58:23.910390 multiocr-0.1.3/multiocr/pipelines/aws_textract/__init__.py
+-rw-r--r--   0        0        0     4678 2023-06-24 05:27:10.673761 multiocr-0.1.3/multiocr/pipelines/aws_textract/engine.py
+-rw-r--r--   0        0        0     2717 2023-06-24 05:23:30.977149 multiocr-0.1.3/multiocr/pipelines/easy_ocr/engine.py
+-rw-r--r--   0        0        0        0 2023-06-10 04:58:45.721303 multiocr-0.1.3/multiocr/pipelines/paddle_ocr/__init__.py
+-rw-r--r--   0        0        0     2827 2023-06-24 05:24:28.226298 multiocr-0.1.3/multiocr/pipelines/paddle_ocr/engine.py
+-rw-r--r--   0        0        0        0 2023-06-10 04:55:24.885038 multiocr-0.1.3/multiocr/pipelines/tesseract/__init__.py
+-rw-r--r--   0        0        0     3535 2023-06-24 05:28:02.597428 multiocr-0.1.3/multiocr/pipelines/tesseract/engine.py
+-rw-r--r--   0        0        0     1319 2023-06-10 08:55:37.312478 multiocr-0.1.3/multiocr/utils.py
+-rw-r--r--   0        0        0      378 2023-06-24 05:29:10.612232 multiocr-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3281 1970-01-01 00:00:00.000000 multiocr-0.1.3/PKG-INFO
```

### Comparing `multiocr-0.1.2/README.md` & `multiocr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `multiocr-0.1.2/multiocr/main.py` & `multiocr-0.1.3/multiocr/main.py`

 * *Files identical despite different names*

### Comparing `multiocr-0.1.2/multiocr/pipelines/aws_textract/engine.py` & `multiocr-0.1.3/multiocr/pipelines/aws_textract/engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 from multiocr.base_class import OCR
 import boto3
 import pandas as pd
 import json
 from typing import Union
 from PIL import Image
+import os
 
 class AwsTextractOcr(OCR):
     """
 
     The TextractOcr class takes an image file path as input and an optional AWS region. It has four methods:
 
     text_extraction(): This method extracts text from the image using AWS Textract and returns the text as a dictionary with the block IDs as keys and the text, confidence score, and bounding box coordinates as values.
     text_extraction_to_json(text_dict): This method takes the dictionary output from text_extraction() as input and saves it to a JSON file.
     """
 
     def __init__(self, config: Union[dict, None]=None):
 
         self.config = config
+        if not self.config:
+            self.config = {
+            "region_name":os.getenv("region_name"),
+            "aws_access_key_id":os.getenv("aws_access_key_id"),
+            "aws_secret_access_key":os.getenv("aws_secret_access_key")
+        }
         self.client = boto3.client('textract', **self.config)
     
     def text_extraction(self, image_file):
         try:
             img = Image.open(image_file)
             with open(image_file, 'rb') as f:
                 image_bytes = f.read()
         except Exception as e:
             raise Exception(f"Error reading image file: {e}")
         
         try:
             response = self.client.detect_document_text(Document={'Bytes': image_bytes})
             self.raw_ocr = response
             # with open("./aws_response.json","r") as f:
-            #     response = json.loads(f.read())
+            #     response = json.  loads(f.read())
         except Exception as e:
             raise Exception(f"Error detecting text in image: {e}")
         
         text_dict = []
         
         for block in response['Blocks']:
             if block['BlockType'] == 'LINE':
@@ -63,40 +70,40 @@
                     text_dict.append(word_dict)
         return text_dict
     
     def text_extraction_to_json(self, text_dict):
         try:
             return json.dumps(text_dict)
         except Exception as e:
-            raise Exception(f"Error saving output to JSON file: {e}")
+            raise Exception(f"Error converting text extraction to JSON: {e}")
         
     def text_extraction_to_df(self, text_dict):
         rows = []
         
         for v in text_dict:
             rows.append([v['text'], v['confidence'], v['coordinates']['xmin'], v['coordinates']['ymin'],
                          v['coordinates']['xmax'], v['coordinates']['ymax']])
         
         df = pd.DataFrame(rows, columns=['text', 'confidence', 'xmin', 'ymin', 'xmax', 'ymax'])
         
         try:
             return df
         except Exception as e:
-            raise Exception(f"Error saving output to CSV file: {e}")
+            raise Exception(f"Error converting text extraction to dataframe: {e}")
         
     def extract_plain_text(self, text_dict):
         plain_text = ''
         
         for v in text_dict:
             plain_text += v['text'] + ' '
         
         try:
             return plain_text
         except Exception as e:
-            raise Exception(f"Error saving output to plain text file: {e}")
+            raise Exception(f"Error converting text extraction to plain text: {e}")
 
 if __name__ == "__main__":
     import os
     config = {
         "region_name":os.getenv("region_name"),
         "aws_access_key_id":os.getenv("aws_access_key_id"),
         "aws_secret_access_key":os.getenv("aws_secret_access_key")
```

### Comparing `multiocr-0.1.2/multiocr/pipelines/easy_ocr/engine.py` & `multiocr-0.1.3/multiocr/pipelines/easy_ocr/engine.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import json
 import pandas as pd
 from easyocr import Reader
+from typing import Union
 
 class EasyOcr:
-    def __init__(self, config):
+    def __init__(self, config: Union[dict, None]=None):
         self.config = config
-        self.ocr = Reader(**config)
+        if not self.config:
+            self.config = {
+            "lang_list": ["en"]
+        }
+        self.ocr = Reader(**self.config)
 
     def text_extraction(self, image_file):
         try:
             result = self.ocr.readtext(image_file)
             self.raw_ocr = result
         except Exception as e:
             raise Exception(f"Error detecting text in image: {e}")
@@ -36,37 +41,37 @@
 
         return text_dict
 
     def text_extraction_to_json(self, text_dict):
         try:
             return json.dumps(text_dict)
         except Exception as e:
-            raise Exception(f"Error saving output to JSON file: {e}")
+            raise Exception(f"Error converting text extraction to JSON: {e}")
 
     def text_extraction_to_df(self, text_dict):
         rows = []
         for v in text_dict:
             rows.append([v['text'], v['confidence'], v['coordinates']['xmin'], v['coordinates']['ymin'],
                          v['coordinates']['xmax'], v['coordinates']['ymax']])
         df = pd.DataFrame(rows, columns=['text', 'confidence', 'xmin', 'ymin', 'xmax', 'ymax'])
 
         try:
             return df
         except Exception as e:
-            raise Exception(f"Error saving output to CSV file: {e}")
+            raise Exception(f"Error converting text extraction to dataframe: {e}")
 
     def extract_plain_text(self, text_dict):
         plain_text = ''
         for v in text_dict:
             plain_text += v['text'] + ' '
 
         try:
             return plain_text
         except Exception as e:
-            raise Exception(f"Error saving output to plain text file: {e}")
+            raise Exception(f"Error converting text extraction to plain text: {e}")
 
 if __name__ == "__main__":
     config = {
         "lang_list": ["en"]
     }
     image_file = "/Users/aravindh/Documents/GitHub/multiocr/tests/data/test-european.jpg"
     ocr = EasyOcr(config)
```

### Comparing `multiocr-0.1.2/multiocr/pipelines/paddle_ocr/engine.py` & `multiocr-0.1.3/multiocr/pipelines/paddle_ocr/engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from PIL import Image
 from paddleocr import draw_ocr
 from typing import Union
 
 class PaddleOcr:
     def __init__(self, config:Union[dict, None]=None):
         self.config = config
+        if not self.config:
+            self.config = {
+            "lang":"en"
+        }
         self.ocr = paddleocr.PaddleOCR(**self.config)
 
     def text_extraction(self, image_file):
         try:
             text = self.ocr.ocr(image_file)
             self.raw_ocr = text
         except Exception as e:
@@ -39,40 +43,40 @@
 
         return text_dict
 
     def text_extraction_to_json(self, text_dict):
         try:
             return json.dumps(text_dict)
         except Exception as e:
-            raise Exception(f"Error saving output to JSON file: {e}")
+            raise Exception(f"Error converting text extraction to JSON: {e}")
         
     def text_extraction_to_df(self, text_dict):
         rows = []
         
         for v in text_dict:
             rows.append([v['text'], v['confidence'], v['coordinates']['xmin'], v['coordinates']['ymin'],
                          v['coordinates']['xmax'], v['coordinates']['ymax']])
         
         df = pd.DataFrame(rows, columns=['text', 'confidence', 'xmin', 'ymin', 'xmax', 'ymax'])
         
         try:
             return df
         except Exception as e:
-            raise Exception(f"Error saving output to CSV file: {e}")
+            raise Exception(f"Error converting text extraction to dataframe: {e}")
         
     def extract_plain_text(self, text_dict):
         plain_text = ''
         
         for v in text_dict:
             plain_text += v['text'] + ' '
         
         try:
             return plain_text
         except Exception as e:
-            raise Exception(f"Error saving output to plain text file: {e}")
+            raise Exception(f"Error converting text extraction to plain text: {e}")
 
 if __name__ == "__main__":
     config = {
         "lang":"en"
     }
     image_file = "/Users/aravindh/Documents/GitHub/multiocr/tests/data/test-european.jpg"
     ocr = PaddleOcr(config)
```

### Comparing `multiocr-0.1.2/multiocr/pipelines/tesseract/engine.py` & `multiocr-0.1.3/multiocr/pipelines/tesseract/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     text_extraction(): This method extracts text from the image using Tesseract OCR and returns the text as a dictionary with the block IDs as keys and the text, confidence score, and bounding box coordinates as values.
     text_extraction_to_json(text_dict): This method takes the dictionary output from text_extraction() as input and saves it to a JSON file.
     text_extraction_to_df(text_dict): This method takes the dictionary output from text_extraction() as input and saves it to a Pandas DataFrame with columns for the text, confidence score, and bounding box coordinates.
     extract_plain_text(text_dict): This method takes the dictionary output from text_extraction() as input and saves the plain text to a text file.
     """
     def __init__(self, config:Union[dict, None]=None):
         self.config = config
+        if not self.config:
+            self.config = {
+                "lang": "eng"
+            }
         self.config.pop("output_type", None)
     
     def text_extraction(self, image_file):
         try:
             text = pytesseract.image_to_data( Image.open(image_file), output_type='dict', **self.config)
             self.raw_ocr = text
         except Exception as e:
@@ -35,40 +39,40 @@
         
         return text_dict
     
     def text_extraction_to_json(self, text_dict):
         try:
             return json.dumps(text_dict)
         except Exception as e:
-            raise Exception(f"Error saving output to JSON file: {e}")
+            raise Exception(f"Error converting text extraction to JSON: {e}")
         
     def text_extraction_to_df(self, text_dict):
         rows = []
         
         for v in text_dict:
             rows.append([v['text'], v['confidence'], v['coordinates']['xmin'], v['coordinates']['ymin'],
                          v['coordinates']['xmax'], v['coordinates']['ymax']])
         
         df = pd.DataFrame(rows, columns=['text', 'confidence', 'xmin', 'ymin', 'xmax', 'ymax'])
         
         try:
             return df
         except Exception as e:
-            raise Exception(f"Error saving output to CSV file: {e}")
+            raise Exception(f"Error converting text extraction to dataframe: {e}")
         
     def extract_plain_text(self, text_dict):
         plain_text = ''
         
         for v in text_dict:
             plain_text += v['text'] + ' '
         
         try:
             return plain_text
         except Exception as e:
-            raise Exception(f"Error saving output to plain text file: {e}")
+            raise Exception(f"Error converting text extraction to plain text: {e}")
 
 if __name__ == "__main__":
     image_file = "/Users/aravindh/Documents/GitHub/multiocr/tests/data/test-european.jpg"
     config = {
         "lang": "eng",
         "config" : "--psm 6"
     }
```

### Comparing `multiocr-0.1.2/multiocr/utils.py` & `multiocr-0.1.3/multiocr/utils.py`

 * *Files identical despite different names*

### Comparing `multiocr-0.1.2/PKG-INFO` & `multiocr-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiocr
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Aravindh
 Author-email: 32878238+s-aravindh@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

