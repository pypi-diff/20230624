# Comparing `tmp/wpdetect-1.3.7.tar.gz` & `tmp/wpdetect-1.3.8.tar.gz`

## Comparing `wpdetect-1.3.7.tar` & `wpdetect-1.3.8.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wpdetect-1.3.7/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.3.7/wpdetect/__init__.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 wpdetect-1.3.7/wpdetect/__main__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wpdetect-1.3.7/LICENSE.txt
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 wpdetect-1.3.7/README.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 wpdetect-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 wpdetect-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wpdetect-1.3.8/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.3.8/wpdetect/__init__.py
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 wpdetect-1.3.8/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 wpdetect-1.3.8/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wpdetect-1.3.8/LICENSE.txt
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 wpdetect-1.3.8/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 wpdetect-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 wpdetect-1.3.8/PKG-INFO
```

### Comparing `wpdetect-1.3.7/wpdetect/__main__.py` & `wpdetect-1.3.8/wpdetect/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import urllib.request
+import requests
 import sys
 from pyfiglet import figlet_format
 
 header = "'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14 (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'"
-version = "1.3.7"
+version = "1.3.8"
 wp_domains = []
 
 
 def print_logo():
     print(figlet_format('     wpdetect     '))
     print("=================== version: " + version + " ===================\n")
 
@@ -29,23 +30,24 @@
     print("[+] Going with HTTP.\n")
     print("Checking: " + str(url))
 
     return url
 
 
 def check_redirect(url):
-    req = urllib.request.Request(url, headers={'User-Agent': header})
-    u = urllib.request.urlopen(req)
-
-    if url != u.geturl():
-        print("[!] " + url + " redirected to "+u.geturl())
-        url = u.geturl()
-        print("Checking: " + str(url))
-
-    return url
+    headers = {'User-Agent': 'Mozilla/5.0'}
+    response = requests.head(url, allow_redirects=True, headers=headers)
+    redirected_url = response.url
+
+    if url != redirected_url:
+        print("[!] {} redirected to {}".format(url, redirected_url))
+        # Recursively follow the redirect
+        return check_redirect(redirected_url)
+    else:
+        return redirected_url
 
 
 def check_HTTP(url):
     print("[!] Couldn't connect over HTTPS.")
     print("[+] Trying with HTTP.\n")
     url = "http://" + url[8:]
     print("Checking: " + str(url))
```

### Comparing `wpdetect-1.3.7/LICENSE.txt` & `wpdetect-1.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpdetect-1.3.7/README.md` & `wpdetect-1.3.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
 ## Changelog
 
+#### What's new in version 1.3.8
+
+-   Fixed [#8](https://github.com/IamLizu/wpdetect/issues)
+
 #### What's new in version 1.3.7
 
 -   Migrated to Hatchling build system
 -   Updated README
 
 #### What's new in version 1.3.6
```

### Comparing `wpdetect-1.3.7/pyproject.toml` & `wpdetect-1.3.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wpdetect"
-version = "1.3.7"
+version = "1.3.8"
 dependencies = [
-    "pyfiglet",
+    "pyfiglet", "requests"
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="thegeek@iamlizu.com" },
 ]
 description = "A WordPress detection tool, detects if a website is running WordPress"
 readme = "README.md"
 requires-python = ">=3.4"
```

### Comparing `wpdetect-1.3.7/PKG-INFO` & `wpdetect-1.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: wpdetect
-Version: 1.3.7
+Version: 1.3.8
 Summary: A WordPress detection tool, detects if a website is running WordPress
 Project-URL: Homepage, https://github.com/IamLizu/wpdetect
 Project-URL: Bug Tracker, https://github.com/IamLizu/wpdetect/issues
 Author-email: S M Mahmudul Hasan <thegeek@iamlizu.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.4
 Requires-Dist: pyfiglet
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # WP DETECT
 
 A WordPress detection tool, detects if a website is running WordPress. wpdetect is a great tool when you just want to check WordPress' presence but do not want to scan the site for vulnerabilities or issues.
 
 ## Installation
@@ -56,14 +57,18 @@
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
 ## Changelog
 
+#### What's new in version 1.3.8
+
+-   Fixed [#8](https://github.com/IamLizu/wpdetect/issues)
+
 #### What's new in version 1.3.7
 
 -   Migrated to Hatchling build system
 -   Updated README
 
 #### What's new in version 1.3.6
```

