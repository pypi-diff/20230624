# Comparing `tmp/unitauto-0.8.2.tar.gz` & `tmp/unitauto-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-5aaued0h/unitauto-0.8.2.tar", last modified: Sun Jun 18 16:32:04 2023, max compression
+gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-oje2c6rl/unitauto-0.9.0.tar", last modified: Sat Jun 24 15:58:55 2023, max compression
```

## Comparing `unitauto-0.8.2.tar` & `unitauto-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:32:04.000000 unitauto-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 16:31:41.000000 unitauto-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-18 16:32:04.000000 unitauto-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-18 16:31:41.000000 unitauto-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-18 16:31:41.000000 unitauto-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-18 16:32:04.000000 unitauto-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:32:04.000000 unitauto-0.8.2/unitauto/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 16:31:41.000000 unitauto-0.8.2/unitauto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-06-18 16:31:41.000000 unitauto-0.8.2/unitauto/methodutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-18 16:31:41.000000 unitauto-0.8.2/unitauto/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:32:04.000000 unitauto-0.8.2/unitauto/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-18 16:31:41.000000 unitauto-0.8.2/unitauto/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-18 16:31:41.000000 unitauto-0.8.2/unitauto/test/testutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:32:04.000000 unitauto-0.8.2/unitauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-18 16:32:04.000000 unitauto-0.8.2/unitauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 16:32:04.000000 unitauto-0.8.2/unitauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:32:04.000000 unitauto-0.8.2/unitauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 16:32:04.000000 unitauto-0.8.2/unitauto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:58:55.000000 unitauto-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-24 15:58:41.000000 unitauto-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-24 15:58:55.000000 unitauto-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-24 15:58:41.000000 unitauto-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 15:58:41.000000 unitauto-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-24 15:58:55.000000 unitauto-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 15:58:41.000000 unitauto-0.9.0/unitauto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20666 2023-06-24 15:58:41.000000 unitauto-0.9.0/unitauto/methodutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-24 15:58:41.000000 unitauto-0.9.0/unitauto/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-24 15:58:41.000000 unitauto-0.9.0/unitauto/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-24 15:58:41.000000 unitauto-0.9.0/unitauto/test/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 15:58:55.000000 unitauto-0.9.0/unitauto.egg-info/top_level.txt
```

### Comparing `unitauto-0.8.2/LICENSE` & `unitauto-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitauto-0.8.2/PKG-INFO` & `unitauto-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 0.8.2
+Version: 0.9.0
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,28 +17,28 @@
 UnitAuto Python Library for remote dependencies with pip, etc.
 
 #### 1. 在你的项目中添加依赖
 #### 1. Add dependency to your project
 ```sh
 	pip install unitauto
 ```
-如果执行以上命令未成功，则将 pip 换成 pip3 试试：
+如果执行以上命令未成功，则将 pip 换成 pip3 试试：<br />
 if you cannot run the command successfully, try pip3:
 ```sh
 	pip3 install unitauto
 ```
 
 <br />
 
 #### 2. 运行 main.py
 #### 2. Run main.py
 ```sh
 	python main.py
 ```
-如果执行以上命令未成功，则将 python 换成 python3 试试：
+如果执行以上命令未成功，则将 python 换成 python3 试试：<br />
 if you cannot run the command successfully, try python3:
 ```sh
 	python3 main.py
 ```
 
 <br />
```

### Comparing `unitauto-0.8.2/README.md` & `unitauto-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 UnitAuto Python Library for remote dependencies with pip, etc.
 
 #### 1. 在你的项目中添加依赖
 #### 1. Add dependency to your project
 ```sh
 	pip install unitauto
 ```
-如果执行以上命令未成功，则将 pip 换成 pip3 试试：
+如果执行以上命令未成功，则将 pip 换成 pip3 试试：<br />
 if you cannot run the command successfully, try pip3:
 ```sh
 	pip3 install unitauto
 ```
 
 <br />
 
 #### 2. 运行 main.py
 #### 2. Run main.py
 ```sh
 	python main.py
 ```
-如果执行以上命令未成功，则将 python 换成 python3 试试：
+如果执行以上命令未成功，则将 python 换成 python3 试试：<br />
 if you cannot run the command successfully, try python3:
 ```sh
 	python3 main.py
 ```
 
 <br />
```

### Comparing `unitauto-0.8.2/setup.cfg` & `unitauto-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unitauto
-version = 0.8.2
+version = 0.9.0
 author = TommyLemon
 author_email = tommylemon@qq.com
 description = An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TommyLemon/unitauto-py
 classifiers =
```

### Comparing `unitauto-0.8.2/unitauto.egg-info/PKG-INFO` & `unitauto-0.9.0/unitauto.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 0.8.2
+Version: 0.9.0
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,28 +17,28 @@
 UnitAuto Python Library for remote dependencies with pip, etc.
 
 #### 1. 在你的项目中添加依赖
 #### 1. Add dependency to your project
 ```sh
 	pip install unitauto
 ```
-如果执行以上命令未成功，则将 pip 换成 pip3 试试：
+如果执行以上命令未成功，则将 pip 换成 pip3 试试：<br />
 if you cannot run the command successfully, try pip3:
 ```sh
 	pip3 install unitauto
 ```
 
 <br />
 
 #### 2. 运行 main.py
 #### 2. Run main.py
 ```sh
 	python main.py
 ```
-如果执行以上命令未成功，则将 python 换成 python3 试试：
+如果执行以上命令未成功，则将 python 换成 python3 试试：<br />
 if you cannot run the command successfully, try python3:
 ```sh
 	python3 main.py
 ```
 
 <br />
```

