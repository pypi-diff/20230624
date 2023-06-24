# Comparing `tmp/sdqrcode-0.2.8.tar.gz` & `tmp/sdqrcode-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.2.8.tar", max compression
+gzip compressed data, was "sdqrcode-0.2.9.tar", max compression
```

## Comparing `sdqrcode-0.2.8.tar` & `sdqrcode-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-06-24 20:55:15.127856 sdqrcode-0.2.8/LICENSE
--rw-r--r--   0        0        0     3778 2023-06-24 20:55:15.127856 sdqrcode-0.2.8/README.md
--rw-r--r--   0        0        0      474 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2410 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/src/sdqrcode/Engines/AutoEngine.py
--rw-r--r--   0        0        0     1867 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/src/sdqrcode/Engines/DiffusersEngine.py
--rw-r--r--   0        0        0      186 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/src/sdqrcode/Engines/Engine.py
--rw-r--r--   0        0        0      426 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/src/sdqrcode/Engines/engine_util.py
--rw-r--r--   0        0        0       32 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0       22 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/src/sdqrcode/configs/custom.yaml
--rw-r--r--   0        0        0      737 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/src/sdqrcode/configs/default.yaml
--rw-r--r--   0        0        0      628 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/src/sdqrcode/configs/default_auto.yaml
--rw-r--r--   0        0        0      713 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/src/sdqrcode/configs/default_diffusers.yaml
--rw-r--r--   0        0        0     8920 2023-06-24 20:55:15.147856 sdqrcode-0.2.8/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 sdqrcode-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-24 20:59:52.797309 sdqrcode-0.2.9/LICENSE
+-rw-r--r--   0        0        0     3778 2023-06-24 20:59:52.797309 sdqrcode-0.2.9/README.md
+-rw-r--r--   0        0        0      474 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2410 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     1867 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      426 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      628 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      713 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0     8930 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 sdqrcode-0.2.9/PKG-INFO
```

### Comparing `sdqrcode-0.2.8/LICENSE` & `sdqrcode-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.8/README.md` & `sdqrcode-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.8/src/sdqrcode/Engines/AutoEngine.py` & `sdqrcode-0.2.9/src/sdqrcode/Engines/AutoEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.8/src/sdqrcode/Engines/DiffusersEngine.py` & `sdqrcode-0.2.9/src/sdqrcode/Engines/DiffusersEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.8/src/sdqrcode/configs/default.yaml` & `sdqrcode-0.2.9/src/sdqrcode/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.8/src/sdqrcode/configs/default_auto.yaml` & `sdqrcode-0.2.9/src/sdqrcode/configs/default_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.8/src/sdqrcode/configs/default_diffusers.yaml` & `sdqrcode-0.2.9/src/sdqrcode/configs/default_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.8/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.2.9/src/sdqrcode/sdqrcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         auto_api_https=auto_api_https,
         auto_api_username=auto_api_username,
         auto_api_password=auto_api_password,
     )
 
 
 def init_and_generate_sd_qrcode(
-    config_name_or_path: str = "default",
+    config_name_or_path: str = "default_diffusers",
     auto_api_hostname: str = "",
     auto_api_port: int = 7860,
     auto_api_https: bool = True,
     auto_api_username: str = "",
     auto_api_password: str = "",
     **config_kwargs,
 ) -> tuple[PIL.Image.Image, Sdqrcode]:
```

### Comparing `sdqrcode-0.2.8/PKG-INFO` & `sdqrcode-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.2.8
+Version: 0.2.9
 Summary: Generate ai qr codes with stable diffusion and controlnet with standardised methods
 License: MIT
 Author: PhilSad
 Author-email: philippe.henri.saade@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

