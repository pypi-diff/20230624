# Comparing `tmp/anticaptchaofficial-1.0.52-py3-none-any.whl.zip` & `tmp/anticaptchaofficial-1.0.53-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 17490 bytes, number of entries: 23
+Zip file size: 17670 bytes, number of entries: 23
 -rw-r--r--  2.0 unx      172 b- defN 20-Mar-11 07:55 anticaptchaofficial/__init__.py
 -rw-r--r--  2.0 unx     1013 b- defN 23-Jan-07 03:37 anticaptchaofficial/antibotcookietask.py
 -rw-r--r--  2.0 unx     2720 b- defN 22-Sep-27 14:01 anticaptchaofficial/antigatetask.py
--rw-r--r--  2.0 unx     6743 b- defN 23-May-24 09:17 anticaptchaofficial/antinetworking.py
+-rw-r--r--  2.0 unx     6995 b- defN 23-Jun-24 09:26 anticaptchaofficial/antinetworking.py
 -rw-r--r--  2.0 unx     1149 b- defN 22-Jun-01 07:46 anticaptchaofficial/funcaptchaproxyless.py
 -rw-r--r--  2.0 unx     1430 b- defN 22-Jun-01 07:46 anticaptchaofficial/funcaptchaproxyon.py
 -rw-r--r--  2.0 unx     1619 b- defN 22-Jun-01 07:46 anticaptchaofficial/geetestproxyless.py
 -rw-r--r--  2.0 unx     1900 b- defN 22-Jun-01 07:46 anticaptchaofficial/geetestproxyon.py
 -rw-r--r--  2.0 unx     1215 b- defN 23-May-24 09:17 anticaptchaofficial/hcaptchaproxyless.py
 -rw-r--r--  2.0 unx     1491 b- defN 23-May-24 09:17 anticaptchaofficial/hcaptchaproxyon.py
 -rw-r--r--  2.0 unx     1750 b- defN 23-May-24 09:11 anticaptchaofficial/imagecaptcha.py
@@ -14,12 +14,12 @@
 -rw-r--r--  2.0 unx     1278 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2enterpriseproxyon.py
 -rw-r--r--  2.0 unx     1045 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2proxyless.py
 -rw-r--r--  2.0 unx     1339 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2proxyon.py
 -rw-r--r--  2.0 unx     1318 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav3enterpriseproxyless.py
 -rw-r--r--  2.0 unx     1270 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav3proxyless.py
 -rw-r--r--  2.0 unx      943 b- defN 23-May-24 09:17 anticaptchaofficial/turnstileproxyless.py
 -rw-r--r--  2.0 unx     1252 b- defN 23-May-24 09:17 anticaptchaofficial/turnstileproxyon.py
--rw-r--r--  2.0 unx     9712 b- defN 23-Jun-03 08:32 anticaptchaofficial-1.0.52.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 08:32 anticaptchaofficial-1.0.52.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jun-03 08:32 anticaptchaofficial-1.0.52.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2208 b- defN 23-Jun-03 08:32 anticaptchaofficial-1.0.52.dist-info/RECORD
-23 files, 42635 bytes uncompressed, 13804 bytes compressed:  67.6%
+-rw-r--r--  2.0 unx    10166 b- defN 23-Jun-24 09:33 anticaptchaofficial-1.0.53.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 09:33 anticaptchaofficial-1.0.53.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-24 09:33 anticaptchaofficial-1.0.53.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2209 b- defN 23-Jun-24 09:33 anticaptchaofficial-1.0.53.dist-info/RECORD
+23 files, 43342 bytes uncompressed, 13984 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: anticaptchaofficial/turnstileproxyless.py
 Comment: 
 
 Filename: anticaptchaofficial/turnstileproxyon.py
 Comment: 
 
-Filename: anticaptchaofficial-1.0.52.dist-info/METADATA
+Filename: anticaptchaofficial-1.0.53.dist-info/METADATA
 Comment: 
 
-Filename: anticaptchaofficial-1.0.52.dist-info/WHEEL
+Filename: anticaptchaofficial-1.0.53.dist-info/WHEEL
 Comment: 
 
-Filename: anticaptchaofficial-1.0.52.dist-info/top_level.txt
+Filename: anticaptchaofficial-1.0.53.dist-info/top_level.txt
 Comment: 
 
-Filename: anticaptchaofficial-1.0.52.dist-info/RECORD
+Filename: anticaptchaofficial-1.0.53.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anticaptchaofficial/antinetworking.py

```diff
@@ -45,14 +45,21 @@
     def get_balance(self):
         result = self.make_request("getBalance", {"clientKey": self.client_key})
         if result != 0:
             return result["balance"]
         else:
             return -1
 
+    def get_credits_balance(self):
+        result = self.make_request("getBalance", {"clientKey": self.client_key})
+        if result != 0 and "captchaCredits" in result:
+            return result["captchaCredits"]
+        else:
+            return -1
+
     def create_task(self, post_data):
         new_task = self.make_request("createTask", post_data)
         if new_task == 0:
             return 0
         else:
             if new_task["errorId"] == 0:
                 self.task_id = new_task["taskId"]
```

## Comparing `anticaptchaofficial-1.0.52.dist-info/METADATA` & `anticaptchaofficial-1.0.53.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anticaptchaofficial
-Version: 1.0.52
+Version: 1.0.53
 Summary: Official anti-captcha.com library
 Home-page: https://git.anti-captcha.com/sup/anticaptcha-python
 Author: Anti Admin
 Author-email: admin@anti-captcha.com
 License: MIT
 Keywords: anticaptcha anti captcha recognition solve bypass recaptcha enterprise funcaptcha arkoselabs geetest hcaptcha antigate turnstile
 Description-Content-Type: text/markdown
@@ -14,37 +14,54 @@
 anticaptchaofficial
 ===================
 
 Official https://anti-captcha.com/ library for solving images with text, Recaptcha v2/v3 Enterprise or non-Enterprise, Funcaptcha Arcoselabs, GeeTest and hCaptcha Enterprise or non-Enterprise.
 Anti-Captcha is the most popular and reliable captcha solving service, working since 2007.
 Prices for solving captchas start from $0.0005 per item.
 
-Python 3:
-
-
 ```bash
 pip3 install anticaptchaofficial
 ```
 
-Python 2 not supported.
-___
-
+&nbsp;
+Check API key balance before creating tasks:
+```python
+balance = solver.get_balance()
+if balance <= 0:
+    print("too low balance!")
+    return
+```
+&nbsp;
+<br>
+Check subscription credits balance if you have one:
+```python
+credits = solver.get_credits_balance()
+if credits <= 0:
+    print("too low credits balance!")
+    return
+```
 &nbsp;
 
 Example how to create [Recaptcha V2](https://anti-captcha.com/apidoc/task-types/RecaptchaV2TaskProxyless) task and receive g-response:
 
 ```python
 from anticaptchaofficial.recaptchav2proxyless import *
 
 solver = recaptchaV2Proxyless()
 solver.set_verbose(1)
 solver.set_key("YOUR_API_KEY")
 solver.set_website_url("https://website.com")
 solver.set_website_key("SITE_KEY")
 
+# Set True if it is Recaptcha V2-invisible
+#solver.set_is_invisible(True)
+
+# Set data-s value for google.com pages
+#solver.set_data_s('a_long_string_here')
+
 # Specify softId to earn 10% commission with your app.
 # Get your softId here: https://anti-captcha.com/clients/tools/devcenter
 solver.set_soft_id(0)
 
 g_response = solver.solve_and_return_solution()
 if g_response != 0:
     print "g-response: "+g_response
```

## Comparing `anticaptchaofficial-1.0.52.dist-info/RECORD` & `anticaptchaofficial-1.0.53.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 anticaptchaofficial/__init__.py,sha256=cVWkoYa7AggYHfknWykrbVxEW70AWFOrwY0Z5_maznY,172
 anticaptchaofficial/antibotcookietask.py,sha256=Sqy6bfaRsrXh2nzPnjxhHUn2Rc6G4IBibPwZ6iARGpw,1013
 anticaptchaofficial/antigatetask.py,sha256=A9yzevmMuyXiH6Ixlu_bcxxzvp4MLQpl3DwFNXU_Gek,2720
-anticaptchaofficial/antinetworking.py,sha256=c1bvffSv_k5iQSRDHc-TB8bfyClTZj92QvClfyCxx7w,6743
+anticaptchaofficial/antinetworking.py,sha256=VdZBoICFK1H-AbkVlZX0lxzewmW-Ku9dR3wS9QLU9HU,6995
 anticaptchaofficial/funcaptchaproxyless.py,sha256=5ORFsWFo_xZK1TRpBnP2R1ELkyG3HsBuyqKb88fmGls,1149
 anticaptchaofficial/funcaptchaproxyon.py,sha256=7LNgSSAvNfdeDUXEtZrOdjY5iYVgvq3ocxIzgNx_5Ac,1430
 anticaptchaofficial/geetestproxyless.py,sha256=ggfg6PcTlPO6Ri9vsO9nZ_23d9rFvUapWjzi-cUojFk,1619
 anticaptchaofficial/geetestproxyon.py,sha256=q6YVGLc3IIPzhzCVx_ayLujTFVej1h3rvaX2KNWKXBQ,1900
 anticaptchaofficial/hcaptchaproxyless.py,sha256=3YPVqMlLUUJR0bXDtfwFwyWkPR054smwKoSvDp10DvE,1215
 anticaptchaofficial/hcaptchaproxyon.py,sha256=6aBwVWBqS1hGS6h0P95QMFW3EAOgidFjq-s8v3ZQm3I,1491
 anticaptchaofficial/imagecaptcha.py,sha256=52_YD4ezf0IqewCEz7egynLnclSCmwhUo0ApfjQdRtk,1750
@@ -13,11 +13,11 @@
 anticaptchaofficial/recaptchav2enterpriseproxyon.py,sha256=p7sdV0qHScbrIrhw00624pH_2hQeG95RTGjRQDutxs4,1278
 anticaptchaofficial/recaptchav2proxyless.py,sha256=12fviOgw1waeeRbyzwvSctIoc1w3qCBYJY7GYi0FSJc,1045
 anticaptchaofficial/recaptchav2proxyon.py,sha256=KKjm72dfxdCChyj3Qn5y5Twm8qT3sZsvSGSfjbdrIM8,1339
 anticaptchaofficial/recaptchav3enterpriseproxyless.py,sha256=exQ-sgvOdcSpsh0mWsUDKEGudM4k23SrROVZ9p0pU5M,1318
 anticaptchaofficial/recaptchav3proxyless.py,sha256=Fv0nfDG-Jp8Vzz8C4-vccz3BJ0hm89MTAs3y9Okzctw,1270
 anticaptchaofficial/turnstileproxyless.py,sha256=nK737Ccr8mZy0_CL6_gB1P5UiCWLaJ0gM9SoCVshMpg,943
 anticaptchaofficial/turnstileproxyon.py,sha256=0HpomUlH1PuLglzrtMBEu5R4287oE3cpp3QnsDhfF2k,1252
-anticaptchaofficial-1.0.52.dist-info/METADATA,sha256=ps0gFvyNGFaNyDcK3g766bH4vBt_uhUGSrrtAw6IecU,9712
-anticaptchaofficial-1.0.52.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-anticaptchaofficial-1.0.52.dist-info/top_level.txt,sha256=lLc0em6A2B5BH-M8v9OP54jTh3u65A4xb2trGoI2_5A,20
-anticaptchaofficial-1.0.52.dist-info/RECORD,,
+anticaptchaofficial-1.0.53.dist-info/METADATA,sha256=XXRCsSgXCYbIcX9MKT3lGvjpTBZV0Du_LIV1eKcmfd4,10166
+anticaptchaofficial-1.0.53.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+anticaptchaofficial-1.0.53.dist-info/top_level.txt,sha256=lLc0em6A2B5BH-M8v9OP54jTh3u65A4xb2trGoI2_5A,20
+anticaptchaofficial-1.0.53.dist-info/RECORD,,
```

