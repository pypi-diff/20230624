# Comparing `tmp/sdqrcode-0.1.0.tar.gz` & `tmp/sdqrcode-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.1.0.tar", max compression
+gzip compressed data, was "sdqrcode-0.2.5.tar", max compression
```

## Comparing `sdqrcode-0.1.0.tar` & `sdqrcode-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-06-21 11:45:08.323732 sdqrcode-0.1.0/LICENSE
--rw-r--r--   0        0        0     3086 2023-06-21 21:03:53.711341 sdqrcode-0.1.0/README.md
--rw-r--r--   0        0        0      456 2023-06-21 21:22:16.649401 sdqrcode-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-06-21 17:09:33.012024 sdqrcode-0.1.0/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0     8371 2023-06-21 13:34:35.627954 sdqrcode-0.1.0/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 sdqrcode-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-24 20:10:49.255413 sdqrcode-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3778 2023-06-24 20:10:49.255413 sdqrcode-0.2.5/README.md
+-rw-r--r--   0        0        0      474 2023-06-24 20:11:04.215432 sdqrcode-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2410 2023-06-24 20:10:49.279413 sdqrcode-0.2.5/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     1867 2023-06-24 20:10:49.279413 sdqrcode-0.2.5/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-06-24 20:10:49.279413 sdqrcode-0.2.5/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      426 2023-06-24 20:10:49.279413 sdqrcode-0.2.5/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-06-24 20:10:49.279413 sdqrcode-0.2.5/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-24 20:10:49.279413 sdqrcode-0.2.5/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-06-24 20:10:49.279413 sdqrcode-0.2.5/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      628 2023-06-24 20:10:49.279413 sdqrcode-0.2.5/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      713 2023-06-24 20:10:49.279413 sdqrcode-0.2.5/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0     8920 2023-06-24 20:10:49.279413 sdqrcode-0.2.5/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 sdqrcode-0.2.5/PKG-INFO
```

### Comparing `sdqrcode-0.1.0/LICENSE` & `sdqrcode-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.1.0/README.md` & `sdqrcode-0.2.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 
 # Stable Diffusion QR Code
-alpha version
+alpha version, expect breaking changes
 
-call [Automatic1111 webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) api to generate qrcodes, will add a pure diffusers version once [this PR is completed](https://github.com/huggingface/diffusers/pull/3770)
+call diffusers pipeline or [Automatic1111 webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) api to generate qrcodes, will add a pure diffusers version once [this PR is completed](https://github.com/huggingface/diffusers/pull/3770)
+
+**June 23 update: a colab with a pure diffusers version without automatic1111 dependencie is now available !** It will be added to the package soon
 
 # tldr
-**Colab:**  <a target="_blank" href="https://colab.research.google.com/github/koll-ai/stable-difusion-qrcode/blob/master/colabs/demo_sdqrcode.ipynb">
+**Diffusers Colab:**  <a target="_blank" href="https://colab.research.google.com/github/koll-ai/stable-difusion-qrcode/blob/master/colabs/diffusers_qrcode_test_multicontrolnet_guidance_start_end.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
+**Automatic1111 Colab:**  <a target="_blank" href="https://colab.research.google.com/github/koll-ai/stable-difusion-qrcode/blob/master/colabs/demo_sdqrcode.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 # Motivation
 There is multiple methodes availables to generate ai qr code with differents controlnets models and params. Some parameters might works better with some stable diffusion checkpoints and it's a pain to find somethings that works consistanly.
 This repo aims to easily try and evaluate differents methods, models, params and share them with a simple config file 
 
 # Exemple
 (cherry picked, will add more results later)
-![file (4)](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/435d4a3c-5eca-498e-a8bd-47d2658e6305)
+![Dalmatian qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/a33a7ae9-3842-4290-b5b2-0104f5339323)
+
+![Swimming pool girl qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/435d4a3c-5eca-498e-a8bd-47d2658e6305)
 
 # Install
 ```
 pip install sdqrcode
 ```
 
 # Usage
 ```python
-import sdqrcode.sdqrcode as sdqrcode
+import sdqrcode
 
 # generate with default params
 sd_qr_code = sdqrcode.generate_sd_qrcode(
             config_name_or_path="./configs/default.yaml",
             auto_api_hostname=os.getenv("AUTO_API_HOSTNAME"),
             auto_api_port=os.getenv("AUTO_API_PORT"),
             auto_api_https=os.getenv("AUTO_API_HTTPS") == "true",
@@ -37,15 +45,15 @@
         )
 ```
 
 This lib uses a yaml file to describe the qrcode generation process. Exemple:
 ``` yaml
 global:
   prompt: "a beautiful landscape"
-  model_name_or_path_or_api_name: "6ce0161689"
+#  model_name_or_path_or_api_name: "6ce0161689" (not implemented)
   steps: 20
   sampler_name: Euler a
   cfg_scale: 7
   width: 512
   height: 512
   seed: -1
 
@@ -76,17 +84,17 @@
 This method seem to be the best for me, I use it with the model [realistic_visionV2](https://civitai.com/models/4201/realistic-vision-v20).
 It uses [Controlnet Brightness](https://huggingface.co/ioclab/control_v1p_sd15_brightness) and [Controlnet Tile](https://huggingface.co/lllyasviel/control_v11f1e_sd15_tile)
 Here are my firsts thoughts:
 * CN brightness should be left as is
 * You can play with CN tile parameters to get an image more or less "grid like"
 
 # Todos
-[] fix weird import
-[] add more configs
-[] allow to set the config without having the file in local path
-[] more tests
-[] try to install the webui in demo colab
-[] add diffusers backend
-[] add docs
+- [ ] allow to set the model in the config
+- [ ] add more configs
+- [ ] allow to set the config without having the file in local path
+- [ ] more tests
+- [ ] try to install the webui in demo colab
+- [ ] add diffusers backend
+- [ ] add docs
 
 # Contrib
 Please don't hesitate to submit a PR to improve the code or submit a config
```

### Comparing `sdqrcode-0.1.0/PKG-INFO` & `sdqrcode-0.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.1.0
+Version: 0.2.5
 Summary: Generate ai qr codes with stable diffusion and controlnet with standardised methods
 License: MIT
 Author: PhilSad
 Author-email: philippe.henri.saade@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: qrcode[pil] (>=7.4.2,<8.0.0)
+Requires-Dist: accelerate (>=0.20.0,<0.21.0)
+Requires-Dist: qrcode (>=7.4.1,<8.0.0)
+Requires-Dist: transformers (==4.30.0)
 Requires-Dist: webuiapi (>=0.9.3,<0.10.0)
 Description-Content-Type: text/markdown
 
 
 # Stable Diffusion QR Code
-alpha version
+alpha version, expect breaking changes
 
-call [Automatic1111 webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) api to generate qrcodes, will add a pure diffusers version once [this PR is completed](https://github.com/huggingface/diffusers/pull/3770)
+call diffusers pipeline or [Automatic1111 webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) api to generate qrcodes, will add a pure diffusers version once [this PR is completed](https://github.com/huggingface/diffusers/pull/3770)
+
+**June 23 update: a colab with a pure diffusers version without automatic1111 dependencie is now available !** It will be added to the package soon
 
 # tldr
-**Colab:**  <a target="_blank" href="https://colab.research.google.com/github/koll-ai/stable-difusion-qrcode/blob/master/colabs/demo_sdqrcode.ipynb">
+**Diffusers Colab:**  <a target="_blank" href="https://colab.research.google.com/github/koll-ai/stable-difusion-qrcode/blob/master/colabs/diffusers_qrcode_test_multicontrolnet_guidance_start_end.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
+**Automatic1111 Colab:**  <a target="_blank" href="https://colab.research.google.com/github/koll-ai/stable-difusion-qrcode/blob/master/colabs/demo_sdqrcode.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 # Motivation
 There is multiple methodes availables to generate ai qr code with differents controlnets models and params. Some parameters might works better with some stable diffusion checkpoints and it's a pain to find somethings that works consistanly.
 This repo aims to easily try and evaluate differents methods, models, params and share them with a simple config file 
 
 # Exemple
 (cherry picked, will add more results later)
-![file (4)](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/435d4a3c-5eca-498e-a8bd-47d2658e6305)
+![Dalmatian qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/a33a7ae9-3842-4290-b5b2-0104f5339323)
+
+![Swimming pool girl qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/435d4a3c-5eca-498e-a8bd-47d2658e6305)
 
 # Install
 ```
 pip install sdqrcode
 ```
 
 # Usage
 ```python
-import sdqrcode.sdqrcode as sdqrcode
+import sdqrcode
 
 # generate with default params
 sd_qr_code = sdqrcode.generate_sd_qrcode(
             config_name_or_path="./configs/default.yaml",
             auto_api_hostname=os.getenv("AUTO_API_HOSTNAME"),
             auto_api_port=os.getenv("AUTO_API_PORT"),
             auto_api_https=os.getenv("AUTO_API_HTTPS") == "true",
@@ -56,15 +66,15 @@
         )
 ```
 
 This lib uses a yaml file to describe the qrcode generation process. Exemple:
 ``` yaml
 global:
   prompt: "a beautiful landscape"
-  model_name_or_path_or_api_name: "6ce0161689"
+#  model_name_or_path_or_api_name: "6ce0161689" (not implemented)
   steps: 20
   sampler_name: Euler a
   cfg_scale: 7
   width: 512
   height: 512
   seed: -1
 
@@ -95,18 +105,18 @@
 This method seem to be the best for me, I use it with the model [realistic_visionV2](https://civitai.com/models/4201/realistic-vision-v20).
 It uses [Controlnet Brightness](https://huggingface.co/ioclab/control_v1p_sd15_brightness) and [Controlnet Tile](https://huggingface.co/lllyasviel/control_v11f1e_sd15_tile)
 Here are my firsts thoughts:
 * CN brightness should be left as is
 * You can play with CN tile parameters to get an image more or less "grid like"
 
 # Todos
-[] fix weird import
-[] add more configs
-[] allow to set the config without having the file in local path
-[] more tests
-[] try to install the webui in demo colab
-[] add diffusers backend
-[] add docs
+- [ ] allow to set the model in the config
+- [ ] add more configs
+- [ ] allow to set the config without having the file in local path
+- [ ] more tests
+- [ ] try to install the webui in demo colab
+- [ ] add diffusers backend
+- [ ] add docs
 
 # Contrib
 Please don't hesitate to submit a PR to improve the code or submit a config
```

