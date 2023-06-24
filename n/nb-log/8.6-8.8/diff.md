# Comparing `tmp/nb_log-8.6.tar.gz` & `tmp/nb_log-8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_log-8.6.tar", last modified: Mon May  8 07:37:23 2023, max compression
+gzip compressed data, was "nb_log-8.8.tar", last modified: Sat Jun 24 15:59:50 2023, max compression
```

## Comparing `nb_log-8.6.tar` & `nb_log-8.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 07:37:23.000000 nb_log-8.6/
--rw-rw-rw-   0        0        0    27863 2023-05-08 07:37:23.000000 nb_log-8.6/PKG-INFO
--rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log/
--rw-rw-rw-   0        0        0     2369 2023-04-28 10:24:28.000000 nb_log-8.6/nb_log/__init__.py
--rw-rw-rw-   0        0        0    50691 2023-04-28 10:26:55.000000 nb_log-8.6/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.6/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0      247 2023-04-18 01:17:35.000000 nb_log-8.6/nb_log/helper.py
--rw-rw-rw-   0        0        0    30621 2023-04-18 02:30:56.000000 nb_log-8.6/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     7782 2023-04-18 01:50:08.000000 nb_log-8.6/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0     9455 2023-04-17 07:36:14.000000 nb_log-8.6/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-8.6/nb_log/set_nb_log_config.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/
--rw-rw-rw-   0        0        0    27863 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 07:37:23.000000 nb_log-8.6/setup.cfg
--rw-rw-rw-   0        0        0     2345 2023-05-08 07:37:15.000000 nb_log-8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:59:50.323320 nb_log-8.8/
+-rw-rw-rw-   0        0        0    27859 2023-06-24 15:59:50.320319 nb_log-8.8/PKG-INFO
+-rw-rw-rw-   0        0        0    26926 2023-05-13 11:59:47.000000 nb_log-8.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 15:59:50.299320 nb_log-8.8/nb_log/
+-rw-rw-rw-   0        0        0     2369 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/__init__.py
+-rw-rw-rw-   0        0        0    50691 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-8.8/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0      247 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/helper.py
+-rw-rw-rw-   0        0        0    30621 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     7782 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0     9470 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     7710 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/set_nb_log_config.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:59:50.316305 nb_log-8.8/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    27859 2023-06-24 15:59:50.000000 nb_log-8.8/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-06-24 15:59:50.000000 nb_log-8.8/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 15:59:50.000000 nb_log-8.8/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-24 15:59:50.000000 nb_log-8.8/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 15:59:50.000000 nb_log-8.8/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 15:59:50.323320 nb_log-8.8/setup.cfg
+-rw-rw-rw-   0        0        0     2345 2023-06-24 15:59:45.000000 nb_log-8.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nb_log-8.6/PKG-INFO` & `nb_log-8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 8.6
+Version: 8.8
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -495,9 +495,7 @@
 [nb_log readthedocs文档链接](https://nb-log-doc.readthedocs.io/zh_CN/latest)
 
 [nb_log 源码链接](https://github.com/ydf0509/nb_log)
 
 ![](https://visitor-badge.glitch.me/badge?page_id=nb_log)
 
 <div> </div>
-
-
```

### Comparing `nb_log-8.6/README.md` & `nb_log-8.8/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-8.6/nb_log/__init__.py` & `nb_log-8.8/nb_log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.6/nb_log/handlers.py` & `nb_log-8.8/nb_log/handlers.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.6/nb_log/handlers0000.py` & `nb_log-8.8/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.6/nb_log/log_manager.py` & `nb_log-8.8/nb_log/log_manager.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.6/nb_log/monkey_print.py` & `nb_log-8.8/nb_log/monkey_print.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.6/nb_log/nb_log_config_default.py` & `nb_log-8.8/nb_log/nb_log_config_default.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,13 +127,13 @@
 
     9: logging.Formatter(
         '[p%(process)d_t%(thread)d] %(asctime)s - %(name)s - "%(pathname)s:%(lineno)d" - %(funcName)s - %(levelname)s - %(message)s',
         "%Y-%m-%d %H:%M:%S"),  # 对5改进，带进程和线程显示的日志模板。
     10: logging.Formatter(
         '[p%(process)d_t%(thread)d] %(asctime)s - %(name)s - "%(filename)s:%(lineno)d" - %(levelname)s - %(message)s', "%Y-%m-%d %H:%M:%S"),  # 对7改进，带进程和线程显示的日志模板。
     11: logging.Formatter(
-        f'({computer_ip},{computer_name})-[p%(process)d_t%(thread)d] %(asctime)s - %(name)s - "%(filename)s:%(lineno)d" - %(levelname)s - %(message)s', "%Y-%m-%d %H:%M:%S"),  # 对7改进，带进程和线程显示的日志模板以及ip和主机名。
+        f'({computer_ip},{computer_name})-[p%(process)d_t%(thread)d] %(asctime)s - %(name)s - "%(filename)s:%(lineno)d" - %(funcName)s - %(levelname)s - %(message)s', "%Y-%m-%d %H:%M:%S"),  # 对7改进，带进程和线程显示的日志模板以及ip和主机名。
 }
 
 FORMATTER_KIND = 5  # 如果get_logger不指定日志模板，则默认选择第几个模板
```

### Comparing `nb_log-8.6/nb_log/set_nb_log_config.py` & `nb_log-8.8/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.6/nb_log.egg-info/PKG-INFO` & `nb_log-8.8/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 8.6
+Version: 8.8
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -495,9 +495,7 @@
 [nb_log readthedocs文档链接](https://nb-log-doc.readthedocs.io/zh_CN/latest)
 
 [nb_log 源码链接](https://github.com/ydf0509/nb_log)
 
 ![](https://visitor-badge.glitch.me/badge?page_id=nb_log)
 
 <div> </div>
-
-
```

### Comparing `nb_log-8.6/setup.py` & `nb_log-8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="8.6",
+    version="8.8",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -62,14 +62,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-8.6.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-8.8.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

