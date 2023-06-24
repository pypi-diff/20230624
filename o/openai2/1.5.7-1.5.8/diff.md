# Comparing `tmp/openai2-1.5.7.tar.gz` & `tmp/openai2-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.7.tar", last modified: Tue Jun 20 13:41:32 2023, max compression
+gzip compressed data, was "openai2-1.5.8.tar", last modified: Sat Jun 24 14:47:15 2023, max compression
```

## Comparing `openai2-1.5.7.tar` & `openai2-1.5.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.7/LICENSE
--rw-r--r--   0        0        0     3202 2023-06-20 13:40:21.926193 openai2-1.5.7/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.7/openai2/Dependent Packages/openai/LICENSE
--rw-r--r--   0        0        0       23 2023-05-28 06:12:32.856591 openai2-1.5.7/openai2/__init__.py
--rw-r--r--   0        0        0     2576 2023-05-28 05:05:03.581780 openai2-1.5.7/openai2/_core.py
--rw-r--r--   0        0        0      637 2023-06-20 13:40:48.811746 openai2-1.5.7/pyproject.toml
--rw-r--r--   0        0        0     3568 1970-01-01 00:00:00.000000 openai2-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.8/LICENSE
+-rw-r--r--   0        0        0     3090 2023-06-23 03:29:02.608130 openai2-1.5.8/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.8/openai2/Dependent Packages/openai/LICENSE
+-rw-r--r--   0        0        0       23 2023-05-28 06:12:32.856591 openai2-1.5.8/openai2/__init__.py
+-rw-r--r--   0        0        0     2576 2023-05-28 05:05:03.581780 openai2-1.5.8/openai2/_core.py
+-rw-r--r--   0        0        0      637 2023-06-24 14:46:37.857272 openai2-1.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 openai2-1.5.8/PKG-INFO
```

### Comparing `openai2-1.5.7/LICENSE` & `openai2-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.7/README.md` & `openai2-1.5.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -95,18 +95,18 @@
 
 #### 更多方法
 
 openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)、[技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [微信公众号](https://lcctoor.github.io/me/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg)
 
 开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
```

### Comparing `openai2-1.5.7/openai2/Dependent Packages/openai/LICENSE` & `openai2-1.5.8/openai2/Dependent Packages/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.7/openai2/_core.py` & `openai2-1.5.8/openai2/_core.py`

 * *Files identical despite different names*

### Comparing `openai2-1.5.7/pyproject.toml` & `openai2-1.5.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.5.7"
+version = "1.5.8"
 description = "根据 openai 官方接口 ‘openai’ 改造的 ‘openai2’ ，比官方接口更好用一点"
 dependencies = ["openai >=0.27.0"]
 keywords = ["openai2", "openai"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `openai2-1.5.7/PKG-INFO` & `openai2-1.5.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5.7
+Version: 1.5.8
 Summary: 根据 openai 官方接口 ‘openai’ 改造的 ‘openai2’ ，比官方接口更好用一点
 Keywords: openai2,openai
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai >=0.27.0
@@ -107,19 +107,19 @@
 
 #### 更多方法
 
 openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)、[技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [微信公众号](https://lcctoor.github.io/me/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg)
 
 开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
```

