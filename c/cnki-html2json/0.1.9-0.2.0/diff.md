# Comparing `tmp/cnki_html2json-0.1.9.tar.gz` & `tmp/cnki-html2json-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.1.9.tar", last modified: Fri May 12 13:46:46 2023, max compression
+gzip compressed data, was "cnki-html2json-0.2.0.tar", last modified: Sat Jun 24 18:48:17 2023, max compression
```

## Comparing `cnki_html2json-0.1.9.tar` & `cnki-html2json-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 13:46:34.000000 cnki_html2json-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-12 13:46:34.000000 cnki_html2json-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 13:46:34.000000 cnki_html2json-0.1.9/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/cnki_html2json/html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/tests/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:48:17.156376 cnki-html2json-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-24 18:48:17.156376 cnki-html2json-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:48:17.152376 cnki-html2json-0.2.0/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:48:17.152376 cnki-html2json-0.2.0/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-24 18:48:17.000000 cnki-html2json-0.2.0/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 18:48:17.000000 cnki-html2json-0.2.0/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 18:48:17.000000 cnki-html2json-0.2.0/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-24 18:48:17.000000 cnki-html2json-0.2.0/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-24 18:48:17.000000 cnki-html2json-0.2.0/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-24 18:48:17.000000 cnki-html2json-0.2.0/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 18:48:17.156376 cnki-html2json-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:48:17.152376 cnki-html2json-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/tests/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-24 18:48:06.000000 cnki-html2json-0.2.0/tests/test_metadata.py
```

### Comparing `cnki_html2json-0.1.9/LICENSE` & `cnki-html2json-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.9/PKG-INFO` & `cnki-html2json-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,130 +1,114 @@
 Metadata-Version: 2.1
-Name: cnki_html2json
-Version: 0.1.9
-Summary: A package to convert cnki html to json
-Home-page: https://github.com/doublessay/cnki-html2json
-Author: WangK2
-Author-email: kw221225@gmail.com
+Name: cnki-html2json
+Version: 0.2.0
+Summary: A package for converting cnki journal papers' html to json
+Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
-Keywords: cnki,text-structure,crawler
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
+Project-URL: Homepage, https://github.com/doublessay/cnki-html2json
+Keywords: cnki,text structure,crawler
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8.0
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
-本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
+本仓库是一个从知网HTML格式的期刊论文中提取结构化文本，然后导出JSON文件的工具，方便对中文期刊论文进行全文分析。
 
 最近更新：  
 - `v0.1.8` 优化爬虫策略，适当提高了爬取速度；
-- `v0.1.5` 对解析论文html的方式进行重构，提高了解析的准确率；
+- `v0.1.5` 对解析论文HTML字符串的方法进行重构，提高了解析的准确率；
 
 核心功能：
-- 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
-- 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
+- 从期刊论文的HTML字符串中解析出包含两级子章节的结构化文本；
+- 实现一个Selenium爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
-  - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
-  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符；
-  - `plain` 导出纯文本，不包含章节标题和参考文献索引；
+  - `structure` 导出结构化文本，包含两级子章节对应的正文和参考文献索引；
+  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符等；
+  - `plain` 导出纯文本，不含章节结构；
   - 以上三种模式都包含参考文献，可以参考 [examples](examples) 文件夹中给出的样例；
 
-<!-- 使用场景：
-- 对中文期刊论文进行全文获取和分析，为下游任务提供支持；
-- 对中文期刊论文进行引文分析； -->
-
 使用限制：
-- 确保你所在的网络环境能正常使用知网；
-- 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试；
+- 确保所在的网络环境能正常使用知网；
+- 仅能提取期刊论文，其他文献类型未做测试；
 - 无法提取文献中的图片、表格等，因此提取的内容可能不完整；
 - 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取；
 
 ## 快速开始
-本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
+本工具使用 Python 开发，请确保电脑上安装了 Python3.8 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如Chrome的驱动为 [ChromeDriver](https://chromedriver.chromium.org/downloads)
 
 ```console
 $ pip install cnki_html2json
 ```
 
 ## 使用方法
-1、调用函数
+1、函数调用，解析单篇文献的HTML字符串
 
 ```python
 from cnki_html2json.html2json import ExtractContent
 with open('paper.html', 'r', encoding='utf-8') as f:
     raw_html = f.read()
 print(ExtractContent(raw_html).extract(mode='raw',export_path=None))
 ```
 `extract` 函数参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `raw` |
-| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为 `json` 文件 |
+| `export_path` | 保存结果的路径，默认为 `None` ，则不保存文件 |
 
 > 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据。
 
-2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
+2、使用命令行工具，启动Selenium爬虫，在弹出的浏览器窗口(默认为Chrome)中完成检索，默认120秒后开始爬取
+
 ```console
-$ 无需设置任何参数，直接运行
+$ 无需设置任何参数，在终端中输入以下指令即可启动爬虫
 $ cnki-crawler
 ```
 ```console
 $ 设置论文提取的起始索引和终止索引，模式设置为structure，记录日志
 $ cnki-crawler -s 1 -e 100 -m structure -l
 $ 或者是
 $ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log
 ```
-```console
-$ 查看可选参数
-$ cnki-crawler --help
-```
 
 命令行工具参数说明：
 |  | 参数 | 说明 |
 | --- | --- | --- |
 | -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
 | -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
 | -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下；  
-> 由于提取的是文献正文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)
-
-```python
-# 也可以在代码中调用爬虫，可选参数参考上方的参数说明
-from cnki_html2json.crawl import start_crawl
-start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
-```
+> 如果未指定保存路径，将下载结果默认保存在当前目录的 `dataset` 文件夹中；  
+由于提取的是文献全文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)；
 
-## json文件字段说明
+## JSON文件字段说明
 | 一级字段 | 二级字段 | 三级字段 | 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  | 论文标题 |
 |  | authors |  | 论文作者 |
 |  | orgs |  | 作者所属机构 |
 |  | abstract |  | 论文摘要 |
 |  | keywords |  | 论文关键词 |
 |  | funds |  | 基金资助 |
 |  | class_num |  | 分类号 |
 |  | source |  | 来源期刊 |
-|  | issue |  | 刊号 |
+|  | issue |  | 期 |
 | body_text | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
 |  | 2.xxx | 2.1xxx |  |
 |  | ...| ... |  |
 | other | 作者贡献声明 |  |  |
 |  | 利益冲突声明 |  |  |
 |  | 参考文献 |  |  |
```

### Comparing `cnki_html2json-0.1.9/README.md` & `cnki-html2json-0.2.0/cnki_html2json.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,114 @@
+Metadata-Version: 2.1
+Name: cnki-html2json
+Version: 0.2.0
+Summary: A package for converting cnki journal papers' html to json
+Author-email: WangK2 <kw221225@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/doublessay/cnki-html2json
+Keywords: cnki,text structure,crawler
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 从知网HTML格式的文献中提取结构化文本
 
-本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
+本仓库是一个从知网HTML格式的期刊论文中提取结构化文本，然后导出JSON文件的工具，方便对中文期刊论文进行全文分析。
 
 最近更新：  
 - `v0.1.8` 优化爬虫策略，适当提高了爬取速度；
-- `v0.1.5` 对解析论文html的方式进行重构，提高了解析的准确率；
+- `v0.1.5` 对解析论文HTML字符串的方法进行重构，提高了解析的准确率；
 
 核心功能：
-- 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
-- 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
+- 从期刊论文的HTML字符串中解析出包含两级子章节的结构化文本；
+- 实现一个Selenium爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
-  - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
-  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符；
-  - `plain` 导出纯文本，不包含章节标题和参考文献索引；
+  - `structure` 导出结构化文本，包含两级子章节对应的正文和参考文献索引；
+  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符等；
+  - `plain` 导出纯文本，不含章节结构；
   - 以上三种模式都包含参考文献，可以参考 [examples](examples) 文件夹中给出的样例；
 
-<!-- 使用场景：
-- 对中文期刊论文进行全文获取和分析，为下游任务提供支持；
-- 对中文期刊论文进行引文分析； -->
-
 使用限制：
-- 确保你所在的网络环境能正常使用知网；
-- 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试；
+- 确保所在的网络环境能正常使用知网；
+- 仅能提取期刊论文，其他文献类型未做测试；
 - 无法提取文献中的图片、表格等，因此提取的内容可能不完整；
 - 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取；
 
 ## 快速开始
-本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
+本工具使用 Python 开发，请确保电脑上安装了 Python3.8 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如Chrome的驱动为 [ChromeDriver](https://chromedriver.chromium.org/downloads)
 
 ```console
 $ pip install cnki_html2json
 ```
 
 ## 使用方法
-1、调用函数
+1、函数调用，解析单篇文献的HTML字符串
 
 ```python
 from cnki_html2json.html2json import ExtractContent
 with open('paper.html', 'r', encoding='utf-8') as f:
     raw_html = f.read()
 print(ExtractContent(raw_html).extract(mode='raw',export_path=None))
 ```
 `extract` 函数参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `raw` |
-| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为 `json` 文件 |
+| `export_path` | 保存结果的路径，默认为 `None` ，则不保存文件 |
 
 > 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据。
 
-2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
+2、使用命令行工具，启动Selenium爬虫，在弹出的浏览器窗口(默认为Chrome)中完成检索，默认120秒后开始爬取
+
 ```console
-$ 无需设置任何参数，直接运行
+$ 无需设置任何参数，在终端中输入以下指令即可启动爬虫
 $ cnki-crawler
 ```
 ```console
 $ 设置论文提取的起始索引和终止索引，模式设置为structure，记录日志
 $ cnki-crawler -s 1 -e 100 -m structure -l
 $ 或者是
 $ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log
 ```
-```console
-$ 查看可选参数
-$ cnki-crawler --help
-```
 
 命令行工具参数说明：
 |  | 参数 | 说明 |
 | --- | --- | --- |
 | -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
 | -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
 | -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下；  
-> 由于提取的是文献正文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)
-
-```python
-# 也可以在代码中调用爬虫，可选参数参考上方的参数说明
-from cnki_html2json.crawl import start_crawl
-start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
-```
+> 如果未指定保存路径，将下载结果默认保存在当前目录的 `dataset` 文件夹中；  
+由于提取的是文献全文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)；
 
-## json文件字段说明
+## JSON文件字段说明
 | 一级字段 | 二级字段 | 三级字段 | 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  | 论文标题 |
 |  | authors |  | 论文作者 |
 |  | orgs |  | 作者所属机构 |
 |  | abstract |  | 论文摘要 |
 |  | keywords |  | 论文关键词 |
 |  | funds |  | 基金资助 |
 |  | class_num |  | 分类号 |
 |  | source |  | 来源期刊 |
-|  | issue |  | 刊号 |
+|  | issue |  | 期 |
 | body_text | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
 |  | 2.xxx | 2.1xxx |  |
 |  | ...| ... |  |
 | other | 作者贡献声明 |  |  |
 |  | 利益冲突声明 |  |  |
 |  | 参考文献 |  |  |
```

### Comparing `cnki_html2json-0.1.9/cnki_html2json/cli.py` & `cnki-html2json-0.2.0/cnki_html2json/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from cnki_html2json.crawl import start_crawl
 
 def main():
-    parser = argparse.ArgumentParser(description='CNKI crawler. Convert the html format of papers to json format.')
+    parser = argparse.ArgumentParser(description="CNKI crawler. Convert cnki journal papers' html to json")
     parser.add_argument('-s','--start_paper_index',type=int,default=1,help='start index, default is 1')
     parser.add_argument('-e','--end_paper_index',type=int,default=None,help='end index, default is None, which means download to the end')
     parser.add_argument('-m','--mode',type=str,default='raw',choices=['raw','structure','plain'])
     parser.add_argument('-b','--browser_type',type=str,default='Chrome',choices=['Chrome','Edge','Firefox'])
     parser.add_argument('-save','--save_path',type=str,default='dataset',help='save path, default is <dataset> folder in the current directory')
     parser.add_argument('-wait','--wait_time',type=int,default=120,help='waiting time for search, default is 120 seconds')
     parser.add_argument('-l','--log',action='store_true',help="whether to save log, specify this parameter to save log, no need to pass value")
```

### Comparing `cnki_html2json-0.1.9/cnki_html2json/crawl.py` & `cnki-html2json-0.2.0/cnki_html2json/crawl.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.9/cnki_html2json/html2json.py` & `cnki-html2json-0.2.0/cnki_html2json/html2json.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.9/cnki_html2json/parse_metadata.py` & `cnki-html2json-0.2.0/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.9/cnki_html2json/recognize_slider_coordinate.py` & `cnki-html2json-0.2.0/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.9/cnki_html2json.egg-info/PKG-INFO` & `cnki-html2json-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,94 @@
-Metadata-Version: 2.1
-Name: cnki-html2json
-Version: 0.1.9
-Summary: A package to convert cnki html to json
-Home-page: https://github.com/doublessay/cnki-html2json
-Author: WangK2
-Author-email: kw221225@gmail.com
-License: MIT
-Keywords: cnki,text-structure,crawler
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 从知网HTML格式的文献中提取结构化文本
 
-本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
+本仓库是一个从知网HTML格式的期刊论文中提取结构化文本，然后导出JSON文件的工具，方便对中文期刊论文进行全文分析。
 
 最近更新：  
 - `v0.1.8` 优化爬虫策略，适当提高了爬取速度；
-- `v0.1.5` 对解析论文html的方式进行重构，提高了解析的准确率；
+- `v0.1.5` 对解析论文HTML字符串的方法进行重构，提高了解析的准确率；
 
 核心功能：
-- 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
-- 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
+- 从期刊论文的HTML字符串中解析出包含两级子章节的结构化文本；
+- 实现一个Selenium爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
-  - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
-  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符；
-  - `plain` 导出纯文本，不包含章节标题和参考文献索引；
+  - `structure` 导出结构化文本，包含两级子章节对应的正文和参考文献索引；
+  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符等；
+  - `plain` 导出纯文本，不含章节结构；
   - 以上三种模式都包含参考文献，可以参考 [examples](examples) 文件夹中给出的样例；
 
-<!-- 使用场景：
-- 对中文期刊论文进行全文获取和分析，为下游任务提供支持；
-- 对中文期刊论文进行引文分析； -->
-
 使用限制：
-- 确保你所在的网络环境能正常使用知网；
-- 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试；
+- 确保所在的网络环境能正常使用知网；
+- 仅能提取期刊论文，其他文献类型未做测试；
 - 无法提取文献中的图片、表格等，因此提取的内容可能不完整；
 - 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取；
 
 ## 快速开始
-本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
+本工具使用 Python 开发，请确保电脑上安装了 Python3.8 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如Chrome的驱动为 [ChromeDriver](https://chromedriver.chromium.org/downloads)
 
 ```console
 $ pip install cnki_html2json
 ```
 
 ## 使用方法
-1、调用函数
+1、函数调用，解析单篇文献的HTML字符串
 
 ```python
 from cnki_html2json.html2json import ExtractContent
 with open('paper.html', 'r', encoding='utf-8') as f:
     raw_html = f.read()
 print(ExtractContent(raw_html).extract(mode='raw',export_path=None))
 ```
 `extract` 函数参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `raw` |
-| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为 `json` 文件 |
+| `export_path` | 保存结果的路径，默认为 `None` ，则不保存文件 |
 
 > 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据。
 
-2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
+2、使用命令行工具，启动Selenium爬虫，在弹出的浏览器窗口(默认为Chrome)中完成检索，默认120秒后开始爬取
+
 ```console
-$ 无需设置任何参数，直接运行
+$ 无需设置任何参数，在终端中输入以下指令即可启动爬虫
 $ cnki-crawler
 ```
 ```console
 $ 设置论文提取的起始索引和终止索引，模式设置为structure，记录日志
 $ cnki-crawler -s 1 -e 100 -m structure -l
 $ 或者是
 $ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log
 ```
-```console
-$ 查看可选参数
-$ cnki-crawler --help
-```
 
 命令行工具参数说明：
 |  | 参数 | 说明 |
 | --- | --- | --- |
 | -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
 | -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
 | -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下；  
-> 由于提取的是文献正文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)
-
-```python
-# 也可以在代码中调用爬虫，可选参数参考上方的参数说明
-from cnki_html2json.crawl import start_crawl
-start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
-```
+> 如果未指定保存路径，将下载结果默认保存在当前目录的 `dataset` 文件夹中；  
+由于提取的是文献全文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)；
 
-## json文件字段说明
+## JSON文件字段说明
 | 一级字段 | 二级字段 | 三级字段 | 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  | 论文标题 |
 |  | authors |  | 论文作者 |
 |  | orgs |  | 作者所属机构 |
 |  | abstract |  | 论文摘要 |
 |  | keywords |  | 论文关键词 |
 |  | funds |  | 基金资助 |
 |  | class_num |  | 分类号 |
 |  | source |  | 来源期刊 |
-|  | issue |  | 刊号 |
+|  | issue |  | 期 |
 | body_text | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
 |  | 2.xxx | 2.1xxx |  |
 |  | ...| ... |  |
 | other | 作者贡献声明 |  |  |
 |  | 利益冲突声明 |  |  |
 |  | 参考文献 |  |  |
```

### Comparing `cnki_html2json-0.1.9/setup.py` & `cnki-html2json-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-from setuptools import setup
+[build-system]
+requires = ["setuptools","wheel"]
+build-backend = "setuptools.build_meta"
 
-setup(
-    name="cnki_html2json",
-    author = "WangK2",
-    author_email = "kw221225@gmail.com",
-    version="0.1.9",
-    description="A package to convert cnki html to json",
-    long_description = open("README.md", "r", encoding="utf-8").read(),
-    long_description_content_type="text/markdown",
-    keywords = ["cnki","text-structure","crawler"],
-    license="MIT",
-    url="https://github.com/doublessay/cnki-html2json",
-    packages=["cnki_html2json"],
-    python_requires=">=3.8.0",
-    install_requires=[
-        "selenium",
-        "lxml",
-        "opencv-python",
-        "numpy",
-        "loguru"],
-    
-    classifiers=[
-        "Intended Audience :: Developers",
-        "Intended Audience :: Education",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
-    entry_points={
-        "console_scripts": [
-            "cnki-crawler = cnki_html2json.cli:main",
-        ]
-    },
+[project]
+name = "cnki-html2json"
+authors = [
+    {name = "WangK2", email = "kw221225@gmail.com"}
+    ]
+description = "A package for converting cnki journal papers' html to json"
+version = "0.2.0"
+readme = "README.md"
+requires-python = ">=3.8"
+keywords = ["cnki","text structure","crawler"]
+license = {text = "MIT"}
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: OS Independent",
+    ]
+dependencies = [
+    "selenium",
+    "lxml",
+    "opencv-python",
+    "numpy",
+    "loguru",]
 
-)
+[project.urls]
+Homepage = "https://github.com/doublessay/cnki-html2json"
+
+[project.scripts]
+histcite = "cnki_html2json.cli:main"
+
+[tool.setuptools]
+packages = ["cnki_html2json"]
```

### Comparing `cnki_html2json-0.1.9/tests/test_html2json.py` & `cnki-html2json-0.2.0/tests/test_html2json.py`

 * *Files identical despite different names*

