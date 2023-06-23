# Comparing `tmp/cetto-0.0.5.tar.gz` & `tmp/cetto-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cetto-0.0.5.tar", last modified: Fri Jun 23 22:43:50 2023, max compression
+gzip compressed data, was "cetto-0.0.6.tar", last modified: Fri Jun 23 22:46:41 2023, max compression
```

## Comparing `cetto-0.0.5.tar` & `cetto-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 22:43:50.372075 cetto-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-06-23 15:47:50.000000 cetto-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      801 2023-06-23 22:43:50.372075 cetto-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7083 2023-06-23 22:22:06.000000 cetto-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 22:43:50.345234 cetto-0.0.5/cetto/
--rw-rw-rw-   0        0        0        0 2023-06-23 15:00:01.000000 cetto-0.0.5/cetto/__init__.py
--rw-rw-rw-   0        0        0       56 2023-06-23 16:42:42.000000 cetto-0.0.5/cetto/__main__.py
--rw-rw-rw-   0        0        0     4473 2023-06-23 21:43:14.000000 cetto-0.0.5/cetto/cetto.py
-drwxrwxrwx   0        0        0        0 2023-06-23 22:43:50.368962 cetto-0.0.5/cetto.egg-info/
--rw-rw-rw-   0        0        0      801 2023-06-23 22:43:50.000000 cetto-0.0.5/cetto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-23 22:43:50.000000 cetto-0.0.5/cetto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 22:43:50.000000 cetto-0.0.5/cetto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-23 22:43:50.000000 cetto-0.0.5/cetto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      374 2023-06-23 22:43:50.000000 cetto-0.0.5/cetto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-23 22:43:50.000000 cetto-0.0.5/cetto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-23 22:43:50.372075 cetto-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2171 2023-06-23 22:42:53.000000 cetto-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 22:46:41.222823 cetto-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 15:47:50.000000 cetto-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      801 2023-06-23 22:46:41.225406 cetto-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7083 2023-06-23 22:22:06.000000 cetto-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 22:46:41.181414 cetto-0.0.6/cetto/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:00:01.000000 cetto-0.0.6/cetto/__init__.py
+-rw-rw-rw-   0        0        0       56 2023-06-23 16:42:42.000000 cetto-0.0.6/cetto/__main__.py
+-rw-rw-rw-   0        0        0     4483 2023-06-23 22:46:04.000000 cetto-0.0.6/cetto/cetto.py
+drwxrwxrwx   0        0        0        0 2023-06-23 22:46:41.221120 cetto-0.0.6/cetto.egg-info/
+-rw-rw-rw-   0        0        0      801 2023-06-23 22:46:40.000000 cetto-0.0.6/cetto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-23 22:46:41.000000 cetto-0.0.6/cetto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 22:46:40.000000 cetto-0.0.6/cetto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-23 22:46:41.000000 cetto-0.0.6/cetto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      374 2023-06-23 22:46:41.000000 cetto-0.0.6/cetto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-23 22:46:41.000000 cetto-0.0.6/cetto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-23 22:46:41.226524 cetto-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2171 2023-06-23 22:46:33.000000 cetto-0.0.6/setup.py
```

### Comparing `cetto-0.0.5/LICENSE.txt` & `cetto-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cetto-0.0.5/PKG-INFO` & `cetto-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cetto
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple CLI interface for ChatGPT Based on Langchain. Blazingly fast, easily hackable.
 Home-page: https://github.com/raphael2692/cetto
-Download-URL: https://github.com/user/reponame/archive/v_0_0_5.tar.gz
+Download-URL: https://github.com/user/reponame/archive/v_0_0_6.tar.gz
 Author: Raffaele Spataro
 Author-email: raffaele2692@gmail.com
 License: MIT
 Keywords: CHAT,GPT,CLI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `cetto-0.0.5/README.md` & `cetto-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cetto-0.0.5/cetto/cetto.py` & `cetto-0.0.6/cetto/cetto.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 #     os.path.join(os.path.dirname(os.path.realpath(__file__)), "templates.yaml"), "r"
 # ) as yamlfile:
 #     templates = yaml.safe_load(yamlfile)
 
 
 templates = {
     "default": """
-You are a chatbot having a conversation with a human.
+Your name is Cetto, a chatbot having a conversation with a human.
 If useful, envelop your answer in Markdown.
 
 {chat_history}
 Human: {human_input}
-  Chatbot:
+Chatbot:
 """,
     "python": """
 You are ar a skilled python programmer. Your code is concised and follows best-pratices.
 If useful, envelop your answer in Markdown.
 
 {chat_history}
 Human: {human_input}
```

### Comparing `cetto-0.0.5/cetto.egg-info/PKG-INFO` & `cetto-0.0.6/cetto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cetto
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple CLI interface for ChatGPT Based on Langchain. Blazingly fast, easily hackable.
 Home-page: https://github.com/raphael2692/cetto
-Download-URL: https://github.com/user/reponame/archive/v_0_0_5.tar.gz
+Download-URL: https://github.com/user/reponame/archive/v_0_0_6.tar.gz
 Author: Raffaele Spataro
 Author-email: raffaele2692@gmail.com
 License: MIT
 Keywords: CHAT,GPT,CLI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `cetto-0.0.5/setup.py` & `cetto-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'cetto',         # How you named your package folder (MyLib)
   packages = ['cetto'],   # Chose the same as "name"
-  version = '0.0.5',      # Start with a small number and increase it with every change you make
+  version = '0.0.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Simple CLI interface for ChatGPT Based on Langchain. Blazingly fast, easily hackable.',   # Give a short description about your library
   author = 'Raffaele Spataro',                   # Type in your name
   author_email = 'raffaele2692@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/raphael2692/cetto',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/user/reponame/archive/v_0_0_5.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/user/reponame/archive/v_0_0_6.tar.gz',    # I explain this later on
   keywords = ['CHAT', 'GPT', 'CLI'],   # Keywords that define your package best
   install_requires=
         ['beautifulsoup4', 'aiohttp', 'aiosignal', 'async-timeout', 'attrs', 'certifi', 'charset-normalizer', 'colorama', 'dataclasses-json', 'frozenlist', 'greenlet', 'idna', 'langchain', 'langchainplus-sdk', 'marshmallow', 'marshmallow-enum', 'multidict', 'mypy-extensions', 'numexpr', 'numpy', 'openai', 'openapi-schema-pydantic', 'packaging', 'pydantic', 'pyfiglet', 'PyYAML', 'requests', 'SQLAlchemy', 'tenacity', 'tqdm', 'typing-inspect', 'typing_extensions', 'urllib3', 'yarl'],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
```

