# Comparing `tmp/SafeURL-Python-1.2.tar.gz` & `tmp/SafeURL-Python-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SafeURL-Python-1.2.tar", last modified: Thu Jan 26 01:36:01 2023, max compression
+gzip compressed data, was "SafeURL-Python-1.3.tar", last modified: Fri Jun 23 22:02:22 2023, max compression
```

## Comparing `SafeURL-Python-1.2.tar` & `SafeURL-Python-1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 kris      (1000) kris      (1000)        0 2023-01-26 01:36:01.365618 SafeURL-Python-1.2/
--rwxr-xr-x   0 kris      (1000) kris      (1000)     1083 2023-01-17 21:10:55.000000 SafeURL-Python-1.2/LICENSE
--rw-r--r--   0 kris      (1000) kris      (1000)     1827 2023-01-26 01:36:01.365618 SafeURL-Python-1.2/PKG-INFO
--rwxr-xr-x   0 kris      (1000) kris      (1000)     1541 2023-01-17 21:10:55.000000 SafeURL-Python-1.2/README.md
-drwxr-xr-x   0 kris      (1000) kris      (1000)        0 2023-01-26 01:36:01.365618 SafeURL-Python-1.2/SafeURL_Python.egg-info/
--rw-r--r--   0 kris      (1000) kris      (1000)     1827 2023-01-26 01:36:01.000000 SafeURL-Python-1.2/SafeURL_Python.egg-info/PKG-INFO
--rw-r--r--   0 kris      (1000) kris      (1000)      285 2023-01-26 01:36:01.000000 SafeURL-Python-1.2/SafeURL_Python.egg-info/SOURCES.txt
--rw-r--r--   0 kris      (1000) kris      (1000)        1 2023-01-26 01:36:01.000000 SafeURL-Python-1.2/SafeURL_Python.egg-info/dependency_links.txt
--rw-r--r--   0 kris      (1000) kris      (1000)       15 2023-01-26 01:36:01.000000 SafeURL-Python-1.2/SafeURL_Python.egg-info/requires.txt
--rw-r--r--   0 kris      (1000) kris      (1000)        8 2023-01-26 01:36:01.000000 SafeURL-Python-1.2/SafeURL_Python.egg-info/top_level.txt
--rw-r--r--   0 kris      (1000) kris      (1000)      338 2023-01-26 01:35:13.000000 SafeURL-Python-1.2/pyproject.toml
-drwxr-xr-x   0 kris      (1000) kris      (1000)        0 2023-01-26 01:36:01.365618 SafeURL-Python-1.2/safeurl/
--rwxr-xr-x   0 kris      (1000) kris      (1000)        1 2023-01-17 21:10:55.000000 SafeURL-Python-1.2/safeurl/__init__.py
--rwxr-xr-x   0 kris      (1000) kris      (1000)    20065 2023-01-26 01:19:44.000000 SafeURL-Python-1.2/safeurl/safeurl.py
--rwxr-xr-x   0 kris      (1000) kris      (1000)     1381 2023-01-26 01:19:44.000000 SafeURL-Python-1.2/safeurl/safeurl_tests.py
--rw-r--r--   0 kris      (1000) kris      (1000)       38 2023-01-26 01:36:01.365618 SafeURL-Python-1.2/setup.cfg
+drwxr-xr-x   0 kris      (1000) kris      (1000)        0 2023-06-23 22:02:22.969294 SafeURL-Python-1.3/
+-rwxr-xr-x   0 kris      (1000) kris      (1000)     1083 2023-01-17 21:10:55.000000 SafeURL-Python-1.3/LICENSE
+-rw-r--r--   0 kris      (1000) kris      (1000)     2413 2023-06-23 22:02:22.969294 SafeURL-Python-1.3/PKG-INFO
+-rwxr-xr-x   0 kris      (1000) kris      (1000)     2129 2023-06-23 22:01:20.000000 SafeURL-Python-1.3/README.md
+drwxr-xr-x   0 kris      (1000) kris      (1000)        0 2023-06-23 22:02:22.965961 SafeURL-Python-1.3/SafeURL_Python.egg-info/
+-rw-r--r--   0 kris      (1000) kris      (1000)     2413 2023-06-23 22:02:22.000000 SafeURL-Python-1.3/SafeURL_Python.egg-info/PKG-INFO
+-rw-r--r--   0 kris      (1000) kris      (1000)      302 2023-06-23 22:02:22.000000 SafeURL-Python-1.3/SafeURL_Python.egg-info/SOURCES.txt
+-rw-r--r--   0 kris      (1000) kris      (1000)        1 2023-06-23 22:02:22.000000 SafeURL-Python-1.3/SafeURL_Python.egg-info/dependency_links.txt
+-rw-r--r--   0 kris      (1000) kris      (1000)       15 2023-06-23 22:02:22.000000 SafeURL-Python-1.3/SafeURL_Python.egg-info/requires.txt
+-rw-r--r--   0 kris      (1000) kris      (1000)        8 2023-06-23 22:02:22.000000 SafeURL-Python-1.3/SafeURL_Python.egg-info/top_level.txt
+-rw-r--r--   0 kris      (1000) kris      (1000)      390 2023-06-23 22:01:20.000000 SafeURL-Python-1.3/pyproject.toml
+-rwxr-xr-x   0 kris      (1000) kris      (1000)       15 2023-06-23 22:01:20.000000 SafeURL-Python-1.3/requirements.txt
+drwxr-xr-x   0 kris      (1000) kris      (1000)        0 2023-06-23 22:02:22.969294 SafeURL-Python-1.3/safeurl/
+-rwxr-xr-x   0 kris      (1000) kris      (1000)        1 2023-01-17 21:10:55.000000 SafeURL-Python-1.3/safeurl/__init__.py
+-rwxr-xr-x   0 kris      (1000) kris      (1000)    20087 2023-06-23 22:01:20.000000 SafeURL-Python-1.3/safeurl/safeurl.py
+-rwxr-xr-x   0 kris      (1000) kris      (1000)     1621 2023-06-23 22:01:20.000000 SafeURL-Python-1.3/safeurl/safeurl_tests.py
+-rw-r--r--   0 kris      (1000) kris      (1000)       38 2023-06-23 22:02:22.969294 SafeURL-Python-1.3/setup.cfg
```

### Comparing `SafeURL-Python-1.2/LICENSE` & `SafeURL-Python-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SafeURL-Python-1.2/PKG-INFO` & `SafeURL-Python-1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: SafeURL-Python
-Version: 1.2
+Version: 1.3
 Summary: SafeURL is a library that aids developers in protecting against a class of vulnerabilities known as Server Side Request Forgery.
 Project-URL: Homepage, https://github.com/IncludeSecurity/safeurl-python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SafeURL for Python
 ### Ported by [@nicolasrod](https://github.com/nicolasrod) and docs by [@momopranto](https://github.com/momopranto)
 
 ## Overview
-SafeURL is a library that aids developers in protecting against a class of vulnerabilities known as [Server Side Request Forgery](http://www.acunetix.com/blog/articles/server-side-request-forgery-vulnerability/). It does this by validating each part of the URL against a configurable white or black list before making an HTTP request. SafeURL is open-source and licensed under MIT.
+SafeURL is a library that aids developers in protecting against a class of vulnerabilities known as [Server Side Request Forgery (SSRF)](http://www.acunetix.com/blog/articles/server-side-request-forgery-vulnerability/). It does this by validating each part of the URL against a configurable white or black list before making an HTTP request. SafeURL is open-source and licensed under MIT.
+
+Note that for mitigating SSRF vulnerabilities, we first recommend routing outbound requests from your infrastructure through a proxy such as [Smokescreen](https://github.com/stripe/smokescreen). Alternately, ensure that all services which can make outbound requests to potentially user-controlled URLs are firewalled from talking to other internal hosts. Application-layer defences such as this library should only be used if those options are not practical. Please see [our blog post](https://blog.includesecurity.com/2023/03/mitigating-ssrf-in-2023/) for further information.
 
 ## Installation
 Clone this repository and import it into your project.
 
 ## Implementation
 SafeURL serves as a replacement wrapper for [PyCurl](http://pycurl.io/) in Python.
```

### Comparing `SafeURL-Python-1.2/SafeURL_Python.egg-info/PKG-INFO` & `SafeURL-Python-1.3/SafeURL_Python.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: SafeURL-Python
-Version: 1.2
+Version: 1.3
 Summary: SafeURL is a library that aids developers in protecting against a class of vulnerabilities known as Server Side Request Forgery.
 Project-URL: Homepage, https://github.com/IncludeSecurity/safeurl-python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SafeURL for Python
 ### Ported by [@nicolasrod](https://github.com/nicolasrod) and docs by [@momopranto](https://github.com/momopranto)
 
 ## Overview
-SafeURL is a library that aids developers in protecting against a class of vulnerabilities known as [Server Side Request Forgery](http://www.acunetix.com/blog/articles/server-side-request-forgery-vulnerability/). It does this by validating each part of the URL against a configurable white or black list before making an HTTP request. SafeURL is open-source and licensed under MIT.
+SafeURL is a library that aids developers in protecting against a class of vulnerabilities known as [Server Side Request Forgery (SSRF)](http://www.acunetix.com/blog/articles/server-side-request-forgery-vulnerability/). It does this by validating each part of the URL against a configurable white or black list before making an HTTP request. SafeURL is open-source and licensed under MIT.
+
+Note that for mitigating SSRF vulnerabilities, we first recommend routing outbound requests from your infrastructure through a proxy such as [Smokescreen](https://github.com/stripe/smokescreen). Alternately, ensure that all services which can make outbound requests to potentially user-controlled URLs are firewalled from talking to other internal hosts. Application-layer defences such as this library should only be used if those options are not practical. Please see [our blog post](https://blog.includesecurity.com/2023/03/mitigating-ssrf-in-2023/) for further information.
 
 ## Installation
 Clone this repository and import it into your project.
 
 ## Implementation
 SafeURL serves as a replacement wrapper for [PyCurl](http://pycurl.io/) in Python.
```

### Comparing `SafeURL-Python-1.2/safeurl/safeurl.py` & `SafeURL-Python-1.3/safeurl/safeurl.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
             if lst == "whitelist":
                 return True
             else:
                 return False
 
         if type_ == "domain":
             for domain in dst:
-                if domain.lower() == value.lower():
+                if domain.lower().strip(".") == value.lower().strip("."):
                     return True
             return False
         else:
             return value in dst
 
     def getList(self, lst, type_=None):
         """"
```

### Comparing `SafeURL-Python-1.2/safeurl/safeurl_tests.py` & `SafeURL-Python-1.3/safeurl/safeurl_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,7 +64,21 @@
 
     res = sc.execute("https://example.com/")
 
 except:
     print("Error:", sys.exc_info())
 
 
+# fqdn
+try:
+    sc = safeurl.SafeURL()
+
+    opt = safeurl.Options()
+    opt.setList("blacklist", ["example.com"], "domain")
+    sc.setOptions(opt)
+
+    res = sc.execute("https://example.com.")
+
+except:
+    print("Error:", sys.exc_info())
+
+
```

