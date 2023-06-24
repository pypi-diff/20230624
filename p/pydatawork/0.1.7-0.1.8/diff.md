# Comparing `tmp/pydatawork-0.1.7.tar.gz` & `tmp/pydatawork-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.1.7.tar", last modified: Sun Jun 18 15:40:36 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.1.8.tar", last modified: Sat Jun 24 10:07:12 2023, max compression
```

## Comparing `pydatawork-0.1.7.tar` & `pydatawork-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:40:36.000000 pydatawork-0.1.7/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3503 2023-06-18 15:40:36.000000 pydatawork-0.1.7/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2291 2023-06-18 15:38:44.000000 pydatawork-0.1.7/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:40:36.000000 pydatawork-0.1.7/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3503 2023-06-18 15:40:36.000000 pydatawork-0.1.7/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 15:40:36.000000 pydatawork-0.1.7/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 15:40:36.000000 pydatawork-0.1.7/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 15:40:36.000000 pydatawork-0.1.7/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    10277 2023-06-18 15:34:02.000000 pydatawork-0.1.7/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 15:40:36.000000 pydatawork-0.1.7/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 15:38:52.000000 pydatawork-0.1.7/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-24 10:07:12.000000 pydatawork-0.1.8/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3707 2023-06-24 10:07:12.000000 pydatawork-0.1.8/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2431 2023-06-24 09:58:59.000000 pydatawork-0.1.8/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-24 10:07:12.000000 pydatawork-0.1.8/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3707 2023-06-24 10:07:12.000000 pydatawork-0.1.8/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-24 10:07:12.000000 pydatawork-0.1.8/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-24 10:07:12.000000 pydatawork-0.1.8/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-24 10:07:12.000000 pydatawork-0.1.8/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    10361 2023-06-24 09:32:45.000000 pydatawork-0.1.8/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-24 10:07:12.000000 pydatawork-0.1.8/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-24 09:59:20.000000 pydatawork-0.1.8/setup.py
```

### Comparing `pydatawork-0.1.7/PKG-INFO` & `pydatawork-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.7
+Version: 0.1.8
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
@@ -26,14 +26,17 @@
         ```python
         def rename_folder_numeric_serialize(path):
             """
             path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
             """
         ```
         
+        来源：原创
+        作者：jk.zhou
+        
         ###### Sun Jun 18 17:10:46 CST 2023
         
         #### get_weibo() 微博图片获取（v 0.1.2）
         
         ```python
         def get_weibo(path,id,weibo_name):
             """
@@ -51,14 +54,19 @@
         path="/home/Desktop/pydatawork"
         id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
         weibo_name="mx"
         
         dw.get_weibo(path,id,weibo_name)
         ```
         
+        来源：非原创
+        原作者：XYJISAW
+        参考链接：https://www.omegaxyz.com/2018/02/13/python_weibo/
+        
+        
         #### pypi维护指令
         
         ```shell
         cd 到pydatawork文件夹
         python3 setup.py sdist bdist_wheel # 打包
         twine check dist/* # 检查
         twine upload dist/* # 上传，需要输入帐号密码
```

### Comparing `pydatawork-0.1.7/README.md` & `pydatawork-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 ```python
 def rename_folder_numeric_serialize(path):
     """
     path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
     """
 ```
 
+来源：原创
+作者：jk.zhou
+
 ###### Sun Jun 18 17:10:46 CST 2023
 
 #### get_weibo() 微博图片获取（v 0.1.2）
 
 ```python
 def get_weibo(path,id,weibo_name):
     """
@@ -43,14 +46,19 @@
 path="/home/Desktop/pydatawork"
 id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
 weibo_name="mx"
 
 dw.get_weibo(path,id,weibo_name)
 ```
 
+来源：非原创
+原作者：XYJISAW
+参考链接：https://www.omegaxyz.com/2018/02/13/python_weibo/
+
+
 #### pypi维护指令
 
 ```shell
 cd 到pydatawork文件夹
 python3 setup.py sdist bdist_wheel # 打包
 twine check dist/* # 检查
 twine upload dist/* # 上传，需要输入帐号密码
```

### Comparing `pydatawork-0.1.7/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.1.8/pydatawork.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.7
+Version: 0.1.8
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
@@ -26,14 +26,17 @@
         ```python
         def rename_folder_numeric_serialize(path):
             """
             path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
             """
         ```
         
+        来源：原创
+        作者：jk.zhou
+        
         ###### Sun Jun 18 17:10:46 CST 2023
         
         #### get_weibo() 微博图片获取（v 0.1.2）
         
         ```python
         def get_weibo(path,id,weibo_name):
             """
@@ -51,14 +54,19 @@
         path="/home/Desktop/pydatawork"
         id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
         weibo_name="mx"
         
         dw.get_weibo(path,id,weibo_name)
         ```
         
+        来源：非原创
+        原作者：XYJISAW
+        参考链接：https://www.omegaxyz.com/2018/02/13/python_weibo/
+        
+        
         #### pypi维护指令
         
         ```shell
         cd 到pydatawork文件夹
         python3 setup.py sdist bdist_wheel # 打包
         twine check dist/* # 检查
         twine upload dist/* # 上传，需要输入帐号密码
```

### Comparing `pydatawork-0.1.7/pydatawork.py` & `pydatawork-0.1.8/pydatawork.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,15 @@
     else:
         os.mkdir(os.path.join(path,weibo_name))
     file = os.path.join(path, weibo_name, weibo_name + ".txt")
 
     get_userInfo(id)
     get_weibo(id, file)
     print("微博数据获取完毕")
+    # 该程序最初来源：http://www.omegaxyz.com/2018/02/13/python_weibo/
 
 
 
 def rename_folder_numeric_serialize(path):
     """
     path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
     """
@@ -218,7 +219,12 @@
     for i, folder in enumerate(subfolders, start=1): # 遍历排序后的子文件夹，从1开始序列化 @ 知识卡片
         new_name = f"{folder}_{i}" # 将序列化的值加在原文件名末尾，以_进行拼接
         os.rename(folder, new_name) # 重命名文件夹 @ 知识卡片
         print(os.path.basename(new_name)) # 打印重命名后的文件夹名字，不包括路径
 
 
 
+
+
+
+
+
```

### Comparing `pydatawork-0.1.7/setup.py` & `pydatawork-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.1.7',
+    version='0.1.8',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

