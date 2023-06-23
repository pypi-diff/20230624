# Comparing `tmp/yunxiao-0.3.2.tar.gz` & `tmp/yunxiao-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.3.2.tar", last modified: Fri Jun 23 20:56:53 2023, max compression
+gzip compressed data, was "yunxiao-0.3.3.tar", last modified: Fri Jun 23 23:25:53 2023, max compression
```

## Comparing `yunxiao-0.3.2.tar` & `yunxiao-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 20:56:53.436468 yunxiao-0.3.2/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     6351 2023-06-23 20:56:53.435459 yunxiao-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.2/README.md
--rw-rw-rw-   0        0        0     1378 2023-06-23 20:56:27.000000 yunxiao-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 20:56:53.436468 yunxiao-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 20:56:53.411895 yunxiao-0.3.2/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.2/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-23 20:56:53.414926 yunxiao-0.3.2/yunxiao/
--rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.2/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    40861 2023-06-23 20:55:47.000000 yunxiao-0.3.2/yunxiao/v2.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.2/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-23 20:56:53.434452 yunxiao-0.3.2/yunxiao.egg-info/
--rw-rw-rw-   0        0        0     6351 2023-06-23 20:56:53.000000 yunxiao-0.3.2/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-23 20:56:53.000000 yunxiao-0.3.2/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 20:56:53.000000 yunxiao-0.3.2/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 20:56:53.000000 yunxiao-0.3.2/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-23 20:56:53.000000 yunxiao-0.3.2/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 23:25:53.560052 yunxiao-0.3.3/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     6351 2023-06-23 23:25:53.559544 yunxiao-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.3/README.md
+-rw-rw-rw-   0        0        0     1443 2023-06-23 23:25:37.000000 yunxiao-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 23:25:53.560052 yunxiao-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 23:25:53.548396 yunxiao-0.3.3/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.3/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-23 23:25:53.552469 yunxiao-0.3.3/yunxiao/
+-rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.3/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    40861 2023-06-23 23:25:37.000000 yunxiao-0.3.3/yunxiao/v2.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.3/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-23 23:25:53.557517 yunxiao-0.3.3/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0     6351 2023-06-23 23:25:53.000000 yunxiao-0.3.3/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-23 23:25:53.000000 yunxiao-0.3.3/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 23:25:53.000000 yunxiao-0.3.3/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 23:25:53.000000 yunxiao-0.3.3/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 23:25:53.000000 yunxiao-0.3.3/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.3.2/LICENSE` & `yunxiao-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.2/PKG-INFO` & `yunxiao-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.3.2
+Version: 0.3.3
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.3.2/README.md` & `yunxiao-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.2/pyproject.toml` & `yunxiao-0.3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.3.2"
+version = "0.3.3"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
@@ -22,14 +22,15 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.3.3" = "修复BUG：班级查询根据名称检索失效。"
 "0.3.2" = "更新参数，修复BUG，新增意向管理API"
 "0.3.1" = "修复整合"
 "0.2.9" = "删除其他，只使用V2"
 "0.2.6" = "V2 中更多使用分片读取。"
 "0.2.5" = "修复 V2 中的 API端点错误。新增 loop 装饰器便于分片提取大量数据。"
 "0.2.4" = "修复 v2 中一个API端点错误及鉴权更新错误"
 "0.2.2" = "新增 v2, 更清晰的函数命名，简洁快速的拉取全部数据。"
```

### Comparing `yunxiao-0.3.2/yunxiao/v2.py` & `yunxiao-0.3.3/yunxiao/v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,15 +620,15 @@
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-edu/classInfo/page",
             json={
                 "_t_": UsedTime.stamp,
                 "orgTag": 1,
                 "classStatus": classStatus,
                 "campusIds": self.campus,
-                "classname": classname,
+                "className": classname,
                 "teacherIds": list(teacherids),
                 "page": {"pageNum": page, "pageSize": size}
             }
         )
 
     # 查询班级信息
     def class_query_info(self, classid: int = None) -> dict:
```

### Comparing `yunxiao-0.3.2/yunxiao/yunxiao.py` & `yunxiao-0.3.3/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.2/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.3.3/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.3.2
+Version: 0.3.3
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

