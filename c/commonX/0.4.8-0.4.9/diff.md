# Comparing `tmp/commonX-0.4.8.tar.gz` & `tmp/commonX-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\commonX-0.4.8.tar", last modified: Thu Jun 22 17:04:59 2023, max compression
+gzip compressed data, was "dist\commonX-0.4.9.tar", last modified: Sat Jun 24 06:10:33 2023, max compression
```

## Comparing `commonX-0.4.8.tar` & `commonX-0.4.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/
--rw-rw-rw-   0        0        0      760 2023-06-22 17:04:59.000000 commonX-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-06-22 17:01:37.000000 commonX-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/common/
--rw-rw-rw-   0        0        0      107 2023-06-22 17:01:37.000000 commonX-0.4.8/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/common/base/
--rw-rw-rw-   0        0        0      622 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/entity.py
--rw-rw-rw-   0        0        0      359 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/factory.py
--rw-rw-rw-   0        0        0     2927 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/genor.py
--rw-rw-rw-   0        0        0     2916 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/hook.py
--rw-rw-rw-   0        0        0     4135 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/logger.py
--rw-rw-rw-   0        0        0     5710 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/mapper.py
--rw-rw-rw-   0        0        0     8399 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/multi_task.py
--rw-rw-rw-   0        0        0     5194 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/packer.py
--rw-rw-rw-   0        0        0     1968 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/registry.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/common/ext/
--rw-rw-rw-   0        0        0      187 2023-06-22 17:01:37.000000 commonX-0.4.8/common/ext/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-06-22 17:01:37.000000 commonX-0.4.8/common/ext/cookie_parser.py
--rw-rw-rw-   0        0        0     3845 2023-06-22 17:01:37.000000 commonX-0.4.8/common/ext/iphone_client.py
--rw-rw-rw-   0        0        0      220 2023-06-22 17:01:37.000000 commonX-0.4.8/common/ext/ocr_support.py
--rw-rw-rw-   0        0        0     1862 2023-06-22 17:01:37.000000 commonX-0.4.8/common/ext/qq_email.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/common/postman/
--rw-rw-rw-   0        0        0       87 2023-06-22 17:01:37.000000 commonX-0.4.8/common/postman/__init__.py
--rw-rw-rw-   0        0        0     5045 2023-06-22 17:01:37.000000 commonX-0.4.8/common/postman/postman_api.py
--rw-rw-rw-   0        0        0     5201 2023-06-22 17:01:37.000000 commonX-0.4.8/common/postman/postman_impl.py
--rw-rw-rw-   0        0        0     4782 2023-06-22 17:01:37.000000 commonX-0.4.8/common/postman/postman_proxy.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/common/util/
--rw-rw-rw-   0        0        0      304 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/__init__.py
--rw-rw-rw-   0        0        0      791 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/args_util.py
--rw-rw-rw-   0        0        0     2176 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/assert_util.py
--rw-rw-rw-   0        0        0     3273 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/decorator_util.py
--rw-rw-rw-   0        0        0     2725 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/exception_utll.py
--rw-rw-rw-   0        0        0     7244 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/file_util.py
--rw-rw-rw-   0        0        0     2935 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/image_util.py
--rw-rw-rw-   0        0        0     2921 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/json_util.py
--rw-rw-rw-   0        0        0     7041 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/requests_util.py
--rw-rw-rw-   0        0        0     4611 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/sys_util.py
--rw-rw-rw-   0        0        0      898 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/time_util.py
--rw-rw-rw-   0        0        0      715 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/typing_util.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/commonX.egg-info/
--rw-rw-rw-   0        0        0      760 2023-06-22 17:04:59.000000 commonX-0.4.8/commonX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-06-22 17:04:59.000000 commonX-0.4.8/commonX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 17:04:59.000000 commonX-0.4.8/commonX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 17:04:59.000000 commonX-0.4.8/commonX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 17:04:59.000000 commonX-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1410 2023-06-22 17:01:37.000000 commonX-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:10:33.000000 commonX-0.4.9/
+-rw-rw-rw-   0        0        0      760 2023-06-24 06:10:33.000000 commonX-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-06-24 06:10:04.000000 commonX-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 06:10:33.000000 commonX-0.4.9/common/
+-rw-rw-rw-   0        0        0      107 2023-06-24 06:10:04.000000 commonX-0.4.9/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:10:33.000000 commonX-0.4.9/common/base/
+-rw-rw-rw-   0        0        0      622 2023-06-24 06:10:04.000000 commonX-0.4.9/common/base/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-06-24 06:10:04.000000 commonX-0.4.9/common/base/entity.py
+-rw-rw-rw-   0        0        0      359 2023-06-24 06:10:04.000000 commonX-0.4.9/common/base/factory.py
+-rw-rw-rw-   0        0        0     2927 2023-06-24 06:10:04.000000 commonX-0.4.9/common/base/genor.py
+-rw-rw-rw-   0        0        0     2916 2023-06-24 06:10:04.000000 commonX-0.4.9/common/base/hook.py
+-rw-rw-rw-   0        0        0     4135 2023-06-24 06:10:04.000000 commonX-0.4.9/common/base/logger.py
+-rw-rw-rw-   0        0        0     5710 2023-06-24 06:10:04.000000 commonX-0.4.9/common/base/mapper.py
+-rw-rw-rw-   0        0        0     8399 2023-06-24 06:10:04.000000 commonX-0.4.9/common/base/multi_task.py
+-rw-rw-rw-   0        0        0     5194 2023-06-24 06:10:04.000000 commonX-0.4.9/common/base/packer.py
+-rw-rw-rw-   0        0        0     1968 2023-06-24 06:10:04.000000 commonX-0.4.9/common/base/registry.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:10:33.000000 commonX-0.4.9/common/ext/
+-rw-rw-rw-   0        0        0      187 2023-06-24 06:10:04.000000 commonX-0.4.9/common/ext/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-06-24 06:10:04.000000 commonX-0.4.9/common/ext/cookie_parser.py
+-rw-rw-rw-   0        0        0     3845 2023-06-24 06:10:04.000000 commonX-0.4.9/common/ext/iphone_client.py
+-rw-rw-rw-   0        0        0      220 2023-06-24 06:10:04.000000 commonX-0.4.9/common/ext/ocr_support.py
+-rw-rw-rw-   0        0        0     1862 2023-06-24 06:10:04.000000 commonX-0.4.9/common/ext/qq_email.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:10:33.000000 commonX-0.4.9/common/postman/
+-rw-rw-rw-   0        0        0       87 2023-06-24 06:10:04.000000 commonX-0.4.9/common/postman/__init__.py
+-rw-rw-rw-   0        0        0     5045 2023-06-24 06:10:04.000000 commonX-0.4.9/common/postman/postman_api.py
+-rw-rw-rw-   0        0        0     5201 2023-06-24 06:10:04.000000 commonX-0.4.9/common/postman/postman_impl.py
+-rw-rw-rw-   0        0        0     4782 2023-06-24 06:10:04.000000 commonX-0.4.9/common/postman/postman_proxy.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:10:33.000000 commonX-0.4.9/common/util/
+-rw-rw-rw-   0        0        0      304 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/args_util.py
+-rw-rw-rw-   0        0        0     2176 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/assert_util.py
+-rw-rw-rw-   0        0        0     2513 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/decorator_util.py
+-rw-rw-rw-   0        0        0     2725 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/exception_utll.py
+-rw-rw-rw-   0        0        0     7244 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/file_util.py
+-rw-rw-rw-   0        0        0     2935 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/image_util.py
+-rw-rw-rw-   0        0        0     2921 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/json_util.py
+-rw-rw-rw-   0        0        0     7041 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/requests_util.py
+-rw-rw-rw-   0        0        0     4611 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/sys_util.py
+-rw-rw-rw-   0        0        0      898 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/time_util.py
+-rw-rw-rw-   0        0        0      715 2023-06-24 06:10:04.000000 commonX-0.4.9/common/util/typing_util.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:10:33.000000 commonX-0.4.9/commonX.egg-info/
+-rw-rw-rw-   0        0        0      760 2023-06-24 06:10:33.000000 commonX-0.4.9/commonX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-06-24 06:10:33.000000 commonX-0.4.9/commonX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 06:10:33.000000 commonX-0.4.9/commonX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 06:10:33.000000 commonX-0.4.9/commonX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 06:10:33.000000 commonX-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1410 2023-06-24 06:10:04.000000 commonX-0.4.9/setup.py
```

### Comparing `commonX-0.4.8/PKG-INFO` & `commonX-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.8
+Version: 0.4.9
 Summary: python common toolkit
 Home-page: https://github.com/hect0x7/common
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `commonX-0.4.8/common/base/__init__.py` & `commonX-0.4.9/common/base/__init__.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/base/entity.py` & `commonX-0.4.9/common/base/entity.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/base/genor.py` & `commonX-0.4.9/common/base/genor.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/base/hook.py` & `commonX-0.4.9/common/base/hook.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/base/logger.py` & `commonX-0.4.9/common/base/logger.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/base/mapper.py` & `commonX-0.4.9/common/base/mapper.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/base/multi_task.py` & `commonX-0.4.9/common/base/multi_task.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/base/packer.py` & `commonX-0.4.9/common/base/packer.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/base/registry.py` & `commonX-0.4.9/common/base/registry.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/ext/cookie_parser.py` & `commonX-0.4.9/common/ext/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/ext/iphone_client.py` & `commonX-0.4.9/common/ext/iphone_client.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/ext/qq_email.py` & `commonX-0.4.9/common/ext/qq_email.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/postman/postman_api.py` & `commonX-0.4.9/common/postman/postman_api.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/postman/postman_impl.py` & `commonX-0.4.9/common/postman/postman_impl.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/postman/postman_proxy.py` & `commonX-0.4.9/common/postman/postman_proxy.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/util/args_util.py` & `commonX-0.4.9/common/util/args_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/util/assert_util.py` & `commonX-0.4.9/common/util/assert_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/util/exception_utll.py` & `commonX-0.4.9/common/util/exception_utll.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/util/file_util.py` & `commonX-0.4.9/common/util/file_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/util/image_util.py` & `commonX-0.4.9/common/util/image_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/util/json_util.py` & `commonX-0.4.9/common/util/json_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/util/requests_util.py` & `commonX-0.4.9/common/util/requests_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/util/sys_util.py` & `commonX-0.4.9/common/util/sys_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/util/time_util.py` & `commonX-0.4.9/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/common/util/typing_util.py` & `commonX-0.4.9/common/util/typing_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/commonX.egg-info/PKG-INFO` & `commonX-0.4.9/commonX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.8
+Version: 0.4.9
 Summary: python common toolkit
 Home-page: https://github.com/hect0x7/common
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `commonX-0.4.8/commonX.egg-info/SOURCES.txt` & `commonX-0.4.9/commonX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonX-0.4.8/setup.py` & `commonX-0.4.9/setup.py`

 * *Files identical despite different names*

