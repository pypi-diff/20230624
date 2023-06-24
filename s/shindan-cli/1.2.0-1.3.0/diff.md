# Comparing `tmp/shindan_cli-1.2.0.tar.gz` & `tmp/shindan_cli-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shindan_cli-1.2.0.tar", max compression
+gzip compressed data, was "shindan_cli-1.3.0.tar", max compression
```

## Comparing `shindan_cli-1.2.0.tar` & `shindan_cli-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/LICENSE
--rw-r--r--   0        0        0     3795 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/README.md
--rw-r--r--   0        0        0     2037 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      210 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/shindan_cli/__init__.py
--rw-r--r--   0        0        0     1630 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/shindan_cli/main.py
--rw-r--r--   0        0        0        0 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/shindan_cli/py.typed
--rw-r--r--   0        0        0     2678 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/shindan_cli/shindan.py
--rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 shindan_cli-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3795 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/README.md
+-rw-r--r--   0        0        0     2037 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/shindan_cli/__init__.py
+-rw-r--r--   0        0        0     1832 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/shindan_cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/shindan_cli/py.typed
+-rw-r--r--   0        0        0     2562 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/shindan_cli/shindan.py
+-rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 shindan_cli-1.3.0/PKG-INFO
```

### Comparing `shindan_cli-1.2.0/LICENSE` & `shindan_cli-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shindan_cli-1.2.0/README.md` & `shindan_cli-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shindan_cli-1.2.0/pyproject.toml` & `shindan_cli-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 [tool.mypy]
 pretty = true
 python_version = "3.9"
 show_error_codes = true
 strict = true
 
 [tool.ruff]
-select = ["ALL"]
 ignore = [
   "D203", # 1 blank line required before class docstring
   "D213", # Multi-line docstring summary should start at the second line
 ]
 line-length = 120
+select = ["ALL"]
 
 [tool.ruff.mccabe]
 max-complexity = 18
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = [
   "D",
@@ -43,46 +43,45 @@
   "Development Status :: 3 - Alpha",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3 :: Only"
+  "Programming Language :: Python :: 3 :: Only",
 ]
 description = "ShindanMaker (https://shindanmaker.com) CLI"
 keywords = ["shindanmaker", "cli"]
+license = "MIT"
 name = "shindan_cli"
 packages = [{include = "shindan_cli"}]
-license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/shindan-cli"
-version = "1.2.0"
+version = "1.3.0"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4"
 beautifulsoup4 = "^4.11.2"
 lxml = "^4.9.2"
+python = ">=3.7,<4"
 requests = "^2.28.2"
 
-
 [tool.poetry.group.dev.dependencies]
-mypy = ">=0.991,<1.3"
+lxml-stubs = "^0.4.0"
+mypy = ">=0.991,<1.4"
 pre-commit = "^2.20.0"
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
 taskipy = "^1.10.3"
 types-beautifulsoup4 = "^4.11.6.7"
 types-requests = "^2.28.11.14"
-lxml-stubs = "^0.4.0"
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
 
 [tool.poetry.scripts]
 shindan = "shindan_cli.main:main"
 
 [tool.poetry_bumpversion.file."shindan_cli/__init__.py"]
 
 [tool.taskipy.tasks]
+lint = "pre-commit run -a"
+profile = "python -m cProfile"
 setup = "poetry install && pre-commit install -t pre-commit -t pre-push"
 test = "pytest --cov=shindan_cli --cov-report=term"
 "test:ci" = "task test --cov-report=xml:cov.xml"
-lint = "pre-commit run -a"
-profile = "python -m cProfile"
```

### Comparing `shindan_cli-1.2.0/shindan_cli/main.py` & `shindan_cli-1.3.0/shindan_cli/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Implements Shindan CLI as a main script."""
 
 from __future__ import annotations
 
 import argparse
+from pprint import pprint
 
 from . import __version__, shindan
 
 
 def _check_natural(v: str) -> int:
     if int(v) < 0:
         raise argparse.ArgumentTypeError("%s is an invalid natural int" % v)
@@ -21,23 +22,32 @@
     )
     parser.add_argument("page_id", metavar="ID", type=_check_natural, help="shindan page id")
     parser.add_argument("shindan_name", metavar="NAME", type=str, help="shindan name")
     parser.add_argument("-w", "--wait", action="store_true", help="insert random wait")
     parser.add_argument("-H", "--hashtag", action="store_true", help="add hashtag `#shindanmaker`")
     parser.add_argument("-l", "--link", action="store_true", help="add link to last of output")
     parser.add_argument("-V", "--version", action="version", version=f"%(prog)s {__version__}")
+
+    # secret option!
+    parser.add_argument("--debug", action="store_true", help=argparse.SUPPRESS)
+
     if test is None:
         return parser.parse_args()
     return parser.parse_args(test)
 
 
 def main(*, test: list[str] | None = None) -> None:
     """Run CLI."""
     args = _parse_args(test=test)
     result = shindan(args.page_id, args.shindan_name, wait=args.wait)
+
+    if args.debug:
+        pprint(result)  # noqa: T203
+        return
+
     print("\n".join(result["results"]))  # noqa: T201
     if args.hashtag:
         print(" ".join(result["hashtags"]))  # noqa: T201
     if args.link:
         print(result["shindan_url"])  # noqa: T201
```

### Comparing `shindan_cli-1.2.0/shindan_cli/shindan.py` & `shindan_cli-1.3.0/shindan_cli/shindan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Implements the function to get the shindan result from <https://shindanmaker.com>."""
 
 from __future__ import annotations
 
 import random
 import time
 from typing import TypedDict
-from urllib.parse import parse_qs, unquote, urlparse
 
 import requests
 from bs4 import BeautifulSoup, Tag
 
 
 class ShindanResult(TypedDict):
     """TypedDict Class for result of shindan."""
@@ -61,39 +60,37 @@
     session = requests.session()
     s = session.get(url, headers=headers)
     if s.status_code != requests.codes.ok:
         raise ShindanError(s.status_code)
 
     source = BeautifulSoup(s.text, features="lxml")
 
-    # _token, shindanName, hiddenName=, type=name
-    params = {i["name"]: i["value"] for i in source.find_all("input")[1:4]}
+    # q, _token, shindanName, hiddenName, type, shindan_token, q
+    params = {i["name"]: i["value"] for i in source.find_all("input")[1:5]}
+
+    # overwrite shindanName
     params["shindanName"] = shindan_name
-    params["type"] = "name"
 
     login = session.post(url, data=params, headers=headers)
     if wait:
         time.sleep(random.uniform(2, 5))  # noqa: S311
 
     soup = BeautifulSoup(login.text, features="lxml")
-    result_tag = soup.find(class_="flex-fill")
+    result_tag = soup.find(id="share-copytext-shindanresult-textarea")
 
-    if not isinstance(result_tag, Tag) or not result_tag.has_attr("href"):
+    if not isinstance(result_tag, Tag) or not result_tag.text:
         msg = f"Could not find a tag contains the result, returns: {result_tag}"
         raise ShindanError(msg)
 
-    parsed_url = urlparse(str(result_tag["href"]))
-    *results, hashtag, shindan_url = unquote(
-        parse_qs(parsed_url.query)["text"][0],
-    ).split("\n")
+    *results, hashtag, shindan_url, _ = result_tag.text.split("\n")
 
     if not results[-1]:
         results.pop(-1)
 
     return {
         "results": results,
-        "hashtags": hashtag.split(" "),
+        "hashtags": hashtag.split("\xa0"),
         "shindan_url": shindan_url,
     }
 
 
 __all__ = ("ShindanResult", "shindan")
```

### Comparing `shindan_cli-1.2.0/PKG-INFO` & `shindan_cli-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shindan-cli
-Version: 1.2.0
+Version: 1.3.0
 Summary: ShindanMaker (https://shindanmaker.com) CLI
 Home-page: https://github.com/eggplants/shindan-cli
 License: MIT
 Keywords: shindanmaker,cli
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.7,<4
@@ -12,20 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/eggplants/shindan-cli
 Description-Content-Type: text/markdown
 
 # shindan-cli
```

