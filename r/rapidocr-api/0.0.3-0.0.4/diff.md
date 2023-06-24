# Comparing `tmp/rapidocr_api-0.0.3-py3-none-any.whl.zip` & `tmp/rapidocr_api-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4225 bytes, number of entries: 7
--rw-r--r--  2.0 unx       74 b- defN 23-Jun-18 12:05 rapidocr_api/__init__.py
--rw-r--r--  2.0 unx     2082 b- defN 23-Jun-18 12:05 rapidocr_api/api.py
--rw-r--r--  2.0 unx     4652 b- defN 23-Jun-18 12:06 rapidocr_api-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 12:06 rapidocr_api-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 23-Jun-18 12:06 rapidocr_api-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-18 12:06 rapidocr_api-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      573 b- defN 23-Jun-18 12:06 rapidocr_api-0.0.3.dist-info/RECORD
-7 files, 7542 bytes uncompressed, 3199 bytes compressed:  57.6%
+Zip file size: 4216 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-24 02:28 rapidocr_api/__init__.py
+-rw-r--r--  2.0 unx     1997 b- defN 23-Jun-24 02:28 rapidocr_api/api.py
+-rw-r--r--  2.0 unx     4652 b- defN 23-Jun-24 02:28 rapidocr_api-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 02:28 rapidocr_api-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-24 02:28 rapidocr_api-0.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-24 02:28 rapidocr_api-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      573 b- defN 23-Jun-24 02:28 rapidocr_api-0.0.4.dist-info/RECORD
+7 files, 7457 bytes uncompressed, 3190 bytes compressed:  57.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: rapidocr_api/__init__.py
 Comment: 
 
 Filename: rapidocr_api/api.py
 Comment: 
 
-Filename: rapidocr_api-0.0.3.dist-info/METADATA
+Filename: rapidocr_api-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_api-0.0.3.dist-info/WHEEL
+Filename: rapidocr_api-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_api-0.0.3.dist-info/entry_points.txt
+Filename: rapidocr_api-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_api-0.0.3.dist-info/top_level.txt
+Filename: rapidocr_api-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_api-0.0.3.dist-info/RECORD
+Filename: rapidocr_api-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapidocr_api/api.py

```diff
@@ -15,67 +15,66 @@
 from PIL import Image
 from rapidocr_onnxruntime import RapidOCR
 
 
 sys.path.append(str(Path(__file__).resolve().parent.parent))
 
 
-class OCRAPIUtils():
+class OCRAPIUtils:
     def __init__(self) -> None:
         self.ocr = RapidOCR()
 
     def __call__(self, img):
         img = np.array(img)
         img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
 
         ocr_res, _ = self.ocr(img)
         if not ocr_res:
             return json.dumps({})
 
-        out_dict = {str(i): {'rec_txt': rec,
-                             'dt_boxes': dt_box,
-                             'score': score}
-                    for i, (dt_box, rec, score) in enumerate(ocr_res)}
+        out_dict = {
+            str(i): {"rec_txt": rec, "dt_boxes": dt_box, "score": score}
+            for i, (dt_box, rec, score) in enumerate(ocr_res)
+        }
         return out_dict
 
 
 app = FastAPI()
 processor = OCRAPIUtils()
 
 
 @app.get("/")
 async def root():
-    return {'message': 'Welcome to RapidOCR Server!'}
+    return {"message": "Welcome to RapidOCR Server!"}
 
 
-@app.post('/ocr')
+@app.post("/ocr")
 async def ocr(image_file: UploadFile = None, image_data: str = Form(None)):
     if image_file:
         img = Image.open(image_file.file)
     elif image_data:
         img_bytes = str.encode(image_data)
         img_b64decode = base64.b64decode(img_bytes)
         img = Image.open(io.BytesIO(img_b64decode))
     else:
         raise ValueError(
-            'When sending a post request, data or files must have a value.')
+            "When sending a post request, data or files must have a value."
+        )
 
     ocr_res = processor(img)
     return ocr_res
 
 
 def main():
-    parser = argparse.ArgumentParser('rapidocr_api')
-    parser.add_argument('-ip', '--ip', type=str, default='0.0.0.0',
-                        help='IP Address')
-    parser.add_argument('-p', '--port', type=int, default=9003,
-                        help='IP port')
+    parser = argparse.ArgumentParser("rapidocr_api")
+    parser.add_argument("-ip", "--ip", type=str, default="0.0.0.0", help="IP Address")
+    parser.add_argument("-p", "--port", type=int, default=9003, help="IP port")
     args = parser.parse_args()
 
     cur_file_path = Path(__file__).resolve()
-    app_path = f'{cur_file_path.parent.name}.{cur_file_path.stem}:app'
+    app_path = f"{cur_file_path.parent.name}.{cur_file_path.stem}:app"
     print(app_path)
     uvicorn.run(app_path, host=args.ip, port=args.port, reload=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

## Comparing `rapidocr_api-0.0.3.dist-info/METADATA` & `rapidocr_api-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidocr-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A cross platform OCR API Library based on OnnxRuntime.
 Home-page: https://github.com/RapidAI/RapidOCR
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Download-URL: https://github.com/RapidAI/RapidOCR.git
 Keywords: ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidocr-api Version: 0.0.3 Summary: A cross
+Metadata-Version: 2.1 Name: rapidocr-api Version: 0.0.4 Summary: A cross
 platform OCR API Library based on OnnxRuntime. Home-page: https://github.com/
 RapidAI/RapidOCR Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Download-URL: https://github.com/RapidAI/RapidOCR.git Keywords:
 ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
 Platform: Any Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

