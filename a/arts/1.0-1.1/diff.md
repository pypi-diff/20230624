# Comparing `tmp/arts-1.0.tar.gz` & `tmp/arts-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arts-1.0.tar", last modified: Sat Jun 24 13:03:23 2023, max compression
+gzip compressed data, was "arts-1.1.tar", last modified: Sat Jun 24 13:11:34 2023, max compression
```

## Comparing `arts-1.0.tar` & `arts-1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1990 2023-06-24 12:37:19.999502 arts-1.0/.gitignore
--rw-r--r--   0        0        0     1373 2023-06-24 12:43:54.393595 arts-1.0/README.md
--rw-r--r--   0        0        0       35 2023-06-24 05:26:09.197796 arts-1.0/arts/__init__.py
--rw-r--r--   0        0        0      411 2023-06-24 05:26:19.045385 arts-1.0/arts/_core.py
--rw-r--r--   0        0        0     2114 2023-06-24 07:00:51.182588 arts-1.0/arts/万象思考/ChatGPT已经有自我意识了/README.md
--rw-r--r--   0        0        0      772 2023-06-23 06:31:13.738964 arts-1.0/arts/万象思考/万物为什么会遵循着物理定律？/README.md
--rw-r--r--   0        0        0     3693 2023-06-24 08:40:00.061857 arts-1.0/arts/万象思考/人权/人人平等是个伪概念/README.md
--rw-r--r--   0        0        0     5051 2023-06-24 08:20:27.835932 arts-1.0/arts/万象思考/人权/堕胎自由权/README.md
--rw-r--r--   0        0        0     1584 2023-06-23 06:49:51.732869 arts-1.0/arts/万象思考/什么是“迷信科学”？/README.md
--rw-r--r--   0        0        0     3149 2023-06-24 08:34:59.453148 arts-1.0/arts/万象思考/有无相生，难易相成的启发/README.md
--rw-r--r--   0        0        0     1226 2023-06-24 06:51:31.392036 arts-1.0/arts/万象思考/熵增都是坏的，熵减都是好的吗？/README.md
--rw-r--r--   0        0        0     1120 2023-06-24 06:40:41.705204 arts-1.0/arts/其它/现在的‘人工智能’是‘穷举智能’/README.md
--rw-r--r--   0        0        0     2974 2023-06-24 07:25:06.881399 arts-1.0/arts/其它/用均匀抽样作文件指纹的可靠性/README.md
--rw-r--r--   0        0        0     1652 2023-06-23 06:48:35.450766 arts-1.0/arts/原创小说/天使传奇/1、被绑架/README.md
--rw-r--r--   0        0        0     7343 2023-06-23 06:29:16.614903 arts-1.0/arts/原创小说/陆小凤新传/燕山宝藏/第一章/README.md
--rw-r--r--   0        0        0     3353 2023-06-24 07:15:39.665620 arts-1.0/arts/时空瞎想/轮回转世真的存在吗？/README.md
--rw-r--r--   0        0        0     2042 2023-06-24 05:45:38.711787 arts-1.0/arts/编程教程/Python/其它/调用openAI进行连续对话/README.md
--rw-r--r--   0        0        0   254025 2023-06-14 02:25:03.834797 arts-1.0/arts/编程教程/Python/其它/调用openAI进行连续对话/封面.jpg
--rw-r--r--   0        0        0     3395 2023-06-24 07:55:32.849161 arts-1.0/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/README.md
--rw-r--r--   0        0        0   132558 2023-06-24 07:41:37.503743 arts-1.0/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/无颜色版.png
--rw-r--r--   0        0        0   135794 2023-06-24 07:38:22.760800 arts-1.0/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/有颜色版.png
--rw-r--r--   0        0        0    18019 2023-06-24 06:12:43.983353 arts-1.0/arts/编程教程/Python/数据库/操作MongoDB简明教程/README.md
--rw-r--r--   0        0        0    18733 2023-06-24 06:13:20.633561 arts-1.0/arts/编程教程/Python/数据库/操作MySQL简明教程/README.md
--rw-r--r--   0        0        0     8138 2023-06-24 05:44:39.242507 arts-1.0/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md
--rw-r--r--   0        0        0   486729 2023-06-17 08:11:16.639983 arts-1.0/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png
--rw-r--r--   0        0        0     1742 2023-06-24 07:01:54.613165 arts-1.0/arts/论时事/评价在北京工体冲进场的的梅西粉丝/README.md
--rw-r--r--   0        0        0   148143 2023-06-18 06:04:10.170676 arts-1.0/arts/论时事/评价在北京工体冲进场的的梅西粉丝/封面.jpg
--rw-r--r--   0        0        0     7744 2023-06-24 12:52:01.250044 arts-1.0/index.html
--rw-r--r--   0        0        0      322 2023-06-24 12:52:37.161966 arts-1.0/pyproject.toml
--rw-r--r--   0        0        0     1551 1970-01-01 00:00:00.000000 arts-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1990 2023-06-24 12:37:19.999502 arts-1.1/.gitignore
+-rw-r--r--   0        0        0     1526 2023-06-24 13:09:38.900688 arts-1.1/README.md
+-rw-r--r--   0        0        0       35 2023-06-24 05:26:09.197796 arts-1.1/arts/__init__.py
+-rw-r--r--   0        0        0      411 2023-06-24 05:26:19.045385 arts-1.1/arts/_core.py
+-rw-r--r--   0        0        0     2114 2023-06-24 07:00:51.182588 arts-1.1/arts/万象思考/ChatGPT已经有自我意识了/README.md
+-rw-r--r--   0        0        0      772 2023-06-23 06:31:13.738964 arts-1.1/arts/万象思考/万物为什么会遵循着物理定律？/README.md
+-rw-r--r--   0        0        0     3693 2023-06-24 08:40:00.061857 arts-1.1/arts/万象思考/人权/人人平等是个伪概念/README.md
+-rw-r--r--   0        0        0     5051 2023-06-24 08:20:27.835932 arts-1.1/arts/万象思考/人权/堕胎自由权/README.md
+-rw-r--r--   0        0        0     1584 2023-06-23 06:49:51.732869 arts-1.1/arts/万象思考/什么是“迷信科学”？/README.md
+-rw-r--r--   0        0        0     3149 2023-06-24 08:34:59.453148 arts-1.1/arts/万象思考/有无相生，难易相成的启发/README.md
+-rw-r--r--   0        0        0     1226 2023-06-24 06:51:31.392036 arts-1.1/arts/万象思考/熵增都是坏的，熵减都是好的吗？/README.md
+-rw-r--r--   0        0        0     1120 2023-06-24 06:40:41.705204 arts-1.1/arts/其它/现在的‘人工智能’是‘穷举智能’/README.md
+-rw-r--r--   0        0        0     2974 2023-06-24 07:25:06.881399 arts-1.1/arts/其它/用均匀抽样作文件指纹的可靠性/README.md
+-rw-r--r--   0        0        0     1652 2023-06-23 06:48:35.450766 arts-1.1/arts/原创小说/天使传奇/1、被绑架/README.md
+-rw-r--r--   0        0        0     7343 2023-06-23 06:29:16.614903 arts-1.1/arts/原创小说/陆小凤新传/燕山宝藏/第一章/README.md
+-rw-r--r--   0        0        0     3353 2023-06-24 07:15:39.665620 arts-1.1/arts/时空瞎想/轮回转世真的存在吗？/README.md
+-rw-r--r--   0        0        0     2042 2023-06-24 05:45:38.711787 arts-1.1/arts/编程教程/Python/其它/调用openAI进行连续对话/README.md
+-rw-r--r--   0        0        0   254025 2023-06-14 02:25:03.834797 arts-1.1/arts/编程教程/Python/其它/调用openAI进行连续对话/封面.jpg
+-rw-r--r--   0        0        0     3395 2023-06-24 07:55:32.849161 arts-1.1/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/README.md
+-rw-r--r--   0        0        0   132558 2023-06-24 07:41:37.503743 arts-1.1/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/无颜色版.png
+-rw-r--r--   0        0        0   135794 2023-06-24 07:38:22.760800 arts-1.1/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/有颜色版.png
+-rw-r--r--   0        0        0    18019 2023-06-24 06:12:43.983353 arts-1.1/arts/编程教程/Python/数据库/操作MongoDB简明教程/README.md
+-rw-r--r--   0        0        0    18733 2023-06-24 06:13:20.633561 arts-1.1/arts/编程教程/Python/数据库/操作MySQL简明教程/README.md
+-rw-r--r--   0        0        0     8138 2023-06-24 05:44:39.242507 arts-1.1/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md
+-rw-r--r--   0        0        0   486729 2023-06-17 08:11:16.639983 arts-1.1/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png
+-rw-r--r--   0        0        0     1742 2023-06-24 07:01:54.613165 arts-1.1/arts/论时事/评价在北京工体冲进场的的梅西粉丝/README.md
+-rw-r--r--   0        0        0   148143 2023-06-18 06:04:10.170676 arts-1.1/arts/论时事/评价在北京工体冲进场的的梅西粉丝/封面.jpg
+-rw-r--r--   0        0        0     7744 2023-06-24 12:52:01.250044 arts-1.1/index.html
+-rw-r--r--   0        0        0      322 2023-06-24 13:10:01.583676 arts-1.1/pyproject.toml
+-rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 arts-1.1/PKG-INFO
```

### Comparing `arts-1.0/.gitignore` & `arts-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `arts-1.0/README.md` & `arts-1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,26 @@
 [主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)
 
 # 教程
 
 ```python
 from arts import get_readme_files
 
+your_folder_path = '...'
+for x in get_readme_files(your_folder_path):
+    print(x)
+```
+
+返回的文件路径为相对目标文件夹 your_folder_path 的相对路径。
+
+## 示例
+
+```python
+from arts import get_readme_files
+
 for x in get_readme_files('writings/articles'):
     print(x)
 ```
 
 返回：
 
 ```
@@ -38,9 +50,7 @@
 /万象思考/熵增都是坏的，熵减都是好的吗？/README.md
 /原创小说/陆小凤新传/燕山宝藏/第一章/README.md
 /编程教程/Python/其它/调用openAI进行连续对话/README.md
 /编程教程/Python/数据库/操作MongoDB简明教程/README.md
 /编程教程/Python/数据库/操作MySQL简明教程/README.md
 /编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md
 ```
-
-返回的文件路径为相对目标文件夹 'writings/articles' 的相对路径。
```

### Comparing `arts-1.0/arts/万象思考/ChatGPT已经有自我意识了/README.md` & `arts-1.1/arts/万象思考/ChatGPT已经有自我意识了/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/万象思考/万物为什么会遵循着物理定律？/README.md` & `arts-1.1/arts/万象思考/万物为什么会遵循着物理定律？/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/万象思考/人权/人人平等是个伪概念/README.md` & `arts-1.1/arts/万象思考/人权/人人平等是个伪概念/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/万象思考/人权/堕胎自由权/README.md` & `arts-1.1/arts/万象思考/人权/堕胎自由权/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/万象思考/什么是“迷信科学”？/README.md` & `arts-1.1/arts/万象思考/什么是“迷信科学”？/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/万象思考/有无相生，难易相成的启发/README.md` & `arts-1.1/arts/万象思考/有无相生，难易相成的启发/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/万象思考/熵增都是坏的，熵减都是好的吗？/README.md` & `arts-1.1/arts/万象思考/熵增都是坏的，熵减都是好的吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/其它/现在的‘人工智能’是‘穷举智能’/README.md` & `arts-1.1/arts/其它/现在的‘人工智能’是‘穷举智能’/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/其它/用均匀抽样作文件指纹的可靠性/README.md` & `arts-1.1/arts/其它/用均匀抽样作文件指纹的可靠性/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/原创小说/天使传奇/1、被绑架/README.md` & `arts-1.1/arts/原创小说/天使传奇/1、被绑架/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/原创小说/陆小凤新传/燕山宝藏/第一章/README.md` & `arts-1.1/arts/原创小说/陆小凤新传/燕山宝藏/第一章/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/时空瞎想/轮回转世真的存在吗？/README.md` & `arts-1.1/arts/时空瞎想/轮回转世真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/编程教程/Python/其它/调用openAI进行连续对话/README.md` & `arts-1.1/arts/编程教程/Python/其它/调用openAI进行连续对话/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/编程教程/Python/其它/调用openAI进行连续对话/封面.jpg` & `arts-1.1/arts/编程教程/Python/其它/调用openAI进行连续对话/封面.jpg`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/README.md` & `arts-1.1/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/无颜色版.png` & `arts-1.1/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/无颜色版.png`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/有颜色版.png` & `arts-1.1/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/有颜色版.png`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/编程教程/Python/数据库/操作MongoDB简明教程/README.md` & `arts-1.1/arts/编程教程/Python/数据库/操作MongoDB简明教程/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/编程教程/Python/数据库/操作MySQL简明教程/README.md` & `arts-1.1/arts/编程教程/Python/数据库/操作MySQL简明教程/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md` & `arts-1.1/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png` & `arts-1.1/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/论时事/评价在北京工体冲进场的的梅西粉丝/README.md` & `arts-1.1/arts/论时事/评价在北京工体冲进场的的梅西粉丝/README.md`

 * *Files identical despite different names*

### Comparing `arts-1.0/arts/论时事/评价在北京工体冲进场的的梅西粉丝/封面.jpg` & `arts-1.1/arts/论时事/评价在北京工体冲进场的的梅西粉丝/封面.jpg`

 * *Files identical despite different names*

### Comparing `arts-1.0/index.html` & `arts-1.1/index.html`

 * *Files identical despite different names*

### Comparing `arts-1.0/PKG-INFO` & `arts-1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arts
-Version: 1.0
+Version: 1.1
 Summary: GitHub Pages 部署辅助 —— README 文件提取器
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 项目描述
 
@@ -27,14 +27,26 @@
 [主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)
 
 # 教程
 
 ```python
 from arts import get_readme_files
 
+your_folder_path = '...'
+for x in get_readme_files(your_folder_path):
+    print(x)
+```
+
+返回的文件路径为相对目标文件夹 your_folder_path 的相对路径。
+
+## 示例
+
+```python
+from arts import get_readme_files
+
 for x in get_readme_files('writings/articles'):
     print(x)
 ```
 
 返回：
 
 ```
@@ -47,8 +59,7 @@
 /原创小说/陆小凤新传/燕山宝藏/第一章/README.md
 /编程教程/Python/其它/调用openAI进行连续对话/README.md
 /编程教程/Python/数据库/操作MongoDB简明教程/README.md
 /编程教程/Python/数据库/操作MySQL简明教程/README.md
 /编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md
 ```
 
-返回的文件路径为相对目标文件夹 'writings/articles' 的相对路径。
```

