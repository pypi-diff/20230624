# Comparing `tmp/rapidocr_web-0.1.7-py3-none-any.whl.zip` & `tmp/rapidocr_web-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 41052 bytes, number of entries: 12
--rw-r--r--  2.0 unx       73 b- defN 23-Jun-18 12:05 rapidocr_web/__init__.py
--rw-r--r--  2.0 unx     1264 b- defN 23-Jun-18 12:05 rapidocr_web/ocrweb.py
--rw-r--r--  2.0 unx     3043 b- defN 23-Jun-18 12:05 rapidocr_web/task.py
--rw-r--r--  2.0 unx    16958 b- defN 23-Jun-18 12:05 rapidocr_web/static/css/favicon.ico
--rw-r--r--  2.0 unx     2065 b- defN 23-Jun-18 12:05 rapidocr_web/static/css/main.css
--rw-r--r--  2.0 unx    86341 b- defN 23-Jun-18 12:05 rapidocr_web/static/js/jquery-3.0.0.min.js
--rw-r--r--  2.0 unx     8202 b- defN 23-Jun-18 12:05 rapidocr_web/templates/index.html
--rw-r--r--  2.0 unx     2008 b- defN 23-Jun-18 12:05 rapidocr_web-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 12:05 rapidocr_web-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Jun-18 12:05 rapidocr_web-0.1.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-18 12:05 rapidocr_web-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1025 b- defN 23-Jun-18 12:05 rapidocr_web-0.1.7.dist-info/RECORD
-12 files, 121143 bytes uncompressed, 39316 bytes compressed:  67.5%
+Zip file size: 41042 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-24 02:28 rapidocr_web/__init__.py
+-rw-r--r--  2.0 unx     1216 b- defN 23-Jun-24 02:28 rapidocr_web/ocrweb.py
+-rw-r--r--  2.0 unx     3043 b- defN 23-Jun-24 02:28 rapidocr_web/task.py
+-rw-r--r--  2.0 unx    16958 b- defN 23-Jun-24 02:28 rapidocr_web/static/css/favicon.ico
+-rw-r--r--  2.0 unx     2065 b- defN 23-Jun-24 02:28 rapidocr_web/static/css/main.css
+-rw-r--r--  2.0 unx    86341 b- defN 23-Jun-24 02:28 rapidocr_web/static/js/jquery-3.0.0.min.js
+-rw-r--r--  2.0 unx     8202 b- defN 23-Jun-24 02:28 rapidocr_web/templates/index.html
+-rw-r--r--  2.0 unx     2008 b- defN 23-Jun-24 02:28 rapidocr_web-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 02:28 rapidocr_web-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-24 02:28 rapidocr_web-0.1.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-24 02:28 rapidocr_web-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1025 b- defN 23-Jun-24 02:28 rapidocr_web-0.1.8.dist-info/RECORD
+12 files, 121095 bytes uncompressed, 39306 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: rapidocr_web/static/js/jquery-3.0.0.min.js
 Comment: 
 
 Filename: rapidocr_web/templates/index.html
 Comment: 
 
-Filename: rapidocr_web-0.1.7.dist-info/METADATA
+Filename: rapidocr_web-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_web-0.1.7.dist-info/WHEEL
+Filename: rapidocr_web-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_web-0.1.7.dist-info/entry_points.txt
+Filename: rapidocr_web-0.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.7.dist-info/top_level.txt
+Filename: rapidocr_web-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.7.dist-info/RECORD
+Filename: rapidocr_web-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapidocr_web/ocrweb.py

```diff
@@ -10,40 +10,38 @@
 try:
     from rapidocr_web.task import OCRWebUtils
 except:
     from task import OCRWebUtils
 
 root_dir = Path(__file__).resolve().parent
 
-app = Flask(__name__, template_folder='templates')
-app.config['MAX_CONTENT_LENGTH'] = 3 * 1024 * 1024
+app = Flask(__name__, template_folder="templates")
+app.config["MAX_CONTENT_LENGTH"] = 3 * 1024 * 1024
 processor = OCRWebUtils()
 
 
-@app.route('/')
+@app.route("/")
 def index():
-    return render_template('index.html')
+    return render_template("index.html")
 
 
-@app.route('/ocr', methods=['POST'])
+@app.route("/ocr", methods=["POST"])
 def ocr():
-    if request.method == 'POST':
-        img_str = request.get_json().get('file', None)
+    if request.method == "POST":
+        img_str = request.get_json().get("file", None)
         ocr_res = processor(img_str)
         return ocr_res
 
 
 def main():
-    parser = argparse.ArgumentParser('rapidocr_web')
-    parser.add_argument('-ip', '--ip', type=str, default='0.0.0.0',
-                        help='IP Address')
-    parser.add_argument('-p', '--port', type=int, default=9003,
-                        help='IP port')
+    parser = argparse.ArgumentParser("rapidocr_web")
+    parser.add_argument("-ip", "--ip", type=str, default="0.0.0.0", help="IP Address")
+    parser.add_argument("-p", "--port", type=int, default=9003, help="IP port")
     args = parser.parse_args()
 
-    print(f'Successfully launched and visit https://{args.ip}:{args.port} to view.')
+    print(f"Successfully launched and visit https://{args.ip}:{args.port} to view.")
     server = make_server(args.ip, args.port, app)
     server.serve_forever()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

## Comparing `rapidocr_web-0.1.7.dist-info/METADATA` & `rapidocr_web-0.1.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidocr-web
-Version: 0.1.7
+Version: 0.1.8
 Summary: A cross platform OCR Library based on OnnxRuntime.
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
-Metadata-Version: 2.1 Name: rapidocr-web Version: 0.1.7 Summary: A cross
+Metadata-Version: 2.1 Name: rapidocr-web Version: 0.1.8 Summary: A cross
 platform OCR Library based on OnnxRuntime. Home-page: https://github.com/
 RapidAI/RapidOCR Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Download-URL: https://github.com/RapidAI/RapidOCR.git Keywords:
 ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
 Platform: Any Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

## Comparing `rapidocr_web-0.1.7.dist-info/RECORD` & `rapidocr_web-0.1.8.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 rapidocr_web/__init__.py,sha256=JmySAOGOURKrbjdme2lVdTbDKaclr00IBKeVIa0_n30,73
-rapidocr_web/ocrweb.py,sha256=2YUp91COzzuJW5_XKwfng0-9VwtGXeRSOA3Kw_DAyfg,1264
+rapidocr_web/ocrweb.py,sha256=IMF9-6CeaEbKsy5YJCBbF2rV_lyZaeR7ZZlMeFdUVbE,1216
 rapidocr_web/task.py,sha256=UVgdPds1NeZTtBnh_hjZiULUKOs_J1cU_hcQDm1Y5ts,3043
 rapidocr_web/static/css/favicon.ico,sha256=CBE1NF6iiIax8WqZVR-vPRaPTcmWjlTWsk1fzEbSd8c,16958
 rapidocr_web/static/css/main.css,sha256=2HcVvoa5oSQONnuC6IjjmBd127Jv9Y5EFJGy32nTEZk,2065
 rapidocr_web/static/js/jquery-3.0.0.min.js,sha256=JmvOoLtYsmqlsWxa7mDSLMwa6dZ9rrIdtrrVYRnDRH0,86341
 rapidocr_web/templates/index.html,sha256=xUe3Xce289Of4XTfeafPTX5JMRsOTdgv2Md5EQwxm48,8202
-rapidocr_web-0.1.7.dist-info/METADATA,sha256=h1DtauYNAwI-zqCb9P8zzL46hN9wY1kmT8Dxahb9t34,2008
-rapidocr_web-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapidocr_web-0.1.7.dist-info/entry_points.txt,sha256=ivlPn9JP6ziblPQyG6N4H4cXfrJZ9FD5rvSYhnEc8cU,59
-rapidocr_web-0.1.7.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
-rapidocr_web-0.1.7.dist-info/RECORD,,
+rapidocr_web-0.1.8.dist-info/METADATA,sha256=aijyn005_9sWdQ9AwqTQRcYtC9BnS3J-nMpGQCbAeZE,2008
+rapidocr_web-0.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapidocr_web-0.1.8.dist-info/entry_points.txt,sha256=ivlPn9JP6ziblPQyG6N4H4cXfrJZ9FD5rvSYhnEc8cU,59
+rapidocr_web-0.1.8.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
+rapidocr_web-0.1.8.dist-info/RECORD,,
```

