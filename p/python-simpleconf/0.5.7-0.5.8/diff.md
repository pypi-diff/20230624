# Comparing `tmp/python-simpleconf-0.5.7.tar.gz` & `tmp/python_simpleconf-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-simpleconf-0.5.7.tar", max compression
+gzip compressed data, was "python_simpleconf-0.5.8.tar", max compression
```

## Comparing `python-simpleconf-0.5.7.tar` & `python_simpleconf-0.5.8.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1056 2022-07-12 04:28:46.252553 python-simpleconf-0.5.7/LICENSE
--rw-r--r--   0        0        0     5173 2022-07-12 04:28:46.252553 python-simpleconf-0.5.7/README.md
--rw-r--r--   0        0        0     1209 2022-07-12 04:28:46.252553 python-simpleconf-0.5.7/pyproject.toml
--rw-r--r--   0        0        0       65 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/__init__.py
--rw-r--r--   0        0        0     2319 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/caster.py
--rw-r--r--   0        0        0     7558 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/config.py
--rw-r--r--   0        0        0      172 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/exceptions.py
--rw-r--r--   0        0        0     1164 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/loaders/__init__.py
--rw-r--r--   0        0        0      258 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/loaders/dict.py
--rw-r--r--   0        0        0     1525 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/loaders/env.py
--rw-r--r--   0        0        0     1991 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/loaders/ini.py
--rw-r--r--   0        0        0      401 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/loaders/json.py
--rw-r--r--   0        0        0     1602 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/loaders/osenv.py
--rw-r--r--   0        0        0      593 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/loaders/toml.py
--rw-r--r--   0        0        0      490 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/loaders/yaml.py
--rw-r--r--   0        0        0     1750 2022-07-12 04:28:46.256553 python-simpleconf-0.5.7/simpleconf/utils.py
--rw-r--r--   0        0        0     6533 2022-07-12 04:28:54.680911 python-simpleconf-0.5.7/setup.py
--rw-r--r--   0        0        0     6248 2022-07-12 04:28:54.681322 python-simpleconf-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-24 05:58:42.152358 python_simpleconf-0.5.8/LICENSE
+-rw-r--r--   0        0        0     5173 2023-06-24 05:58:42.152358 python_simpleconf-0.5.8/README.md
+-rw-r--r--   0        0        0     1218 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/__init__.py
+-rw-r--r--   0        0        0     2319 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/caster.py
+-rw-r--r--   0        0        0     7558 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/config.py
+-rw-r--r--   0        0        0      172 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/exceptions.py
+-rw-r--r--   0        0        0     1164 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/__init__.py
+-rw-r--r--   0        0        0      258 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/dict.py
+-rw-r--r--   0        0        0     1525 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/env.py
+-rw-r--r--   0        0        0     1991 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/ini.py
+-rw-r--r--   0        0        0      401 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/json.py
+-rw-r--r--   0        0        0     1602 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/osenv.py
+-rw-r--r--   0        0        0      593 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/toml.py
+-rw-r--r--   0        0        0      490 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/yaml.py
+-rw-r--r--   0        0        0     1750 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/utils.py
+-rw-r--r--   0        0        0     6303 1970-01-01 00:00:00.000000 python_simpleconf-0.5.8/PKG-INFO
```

### Comparing `python-simpleconf-0.5.7/LICENSE` & `python_simpleconf-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-simpleconf-0.5.7/README.md` & `python_simpleconf-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `python-simpleconf-0.5.7/pyproject.toml` & `python_simpleconf-0.5.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "python-simpleconf"
-version = "0.5.7"
+version = "0.5.8"
 description = "Simple configuration management with python."
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/simpleconf"
 repository = "https://github.com/pwwang/simpleconf"
 packages = [
     {include = "simpleconf"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-diot = "^0.1"
-python-dotenv = { version="^0.20", optional = true}
+diot = "^0.2"
+python-dotenv = { version="^0.21", optional = true}
 pyyaml = { version="^6", optional = true}
 rtoml = {version = "^0.8", optional = true}
-iniconfig = {version = "^1.1", optional = true}
+iniconfig = {version = "^2.0", optional = true}
 
 [tool.poetry.extras]
 ini = [ "iniconfig" ]
 env = [ "python-dotenv"]
 yaml = [ "pyyaml"]
 toml = [ "rtoml"]
 all = [ "iniconfig", "python-dotenv", "pyyaml", "rtoml"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
-pytest-cov = "^3"
+pytest-cov = "^4"
 
 [tool.pytest.ini_options]
 addopts = "-vv -p no:asyncio --cov=simpleconf --cov-report xml:cov.xml --cov-report term-missing"
 filterwarnings = [
     "error"
 ]
 console_output_style = "progress"
 junit_family = "xunit1"
 
 [tool.black]
 line-length = 80
-target-version = ['py37', 'py38', 'py39']
+target-version = ['py37', 'py38', 'py39', 'py310']
 include = '\.pyi?$'
```

### Comparing `python-simpleconf-0.5.7/simpleconf/caster.py` & `python_simpleconf-0.5.8/simpleconf/caster.py`

 * *Files identical despite different names*

### Comparing `python-simpleconf-0.5.7/simpleconf/config.py` & `python_simpleconf-0.5.8/simpleconf/config.py`

 * *Files identical despite different names*

### Comparing `python-simpleconf-0.5.7/simpleconf/loaders/__init__.py` & `python_simpleconf-0.5.8/simpleconf/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `python-simpleconf-0.5.7/simpleconf/loaders/env.py` & `python_simpleconf-0.5.8/simpleconf/loaders/env.py`

 * *Files identical despite different names*

### Comparing `python-simpleconf-0.5.7/simpleconf/loaders/ini.py` & `python_simpleconf-0.5.8/simpleconf/loaders/ini.py`

 * *Files identical despite different names*

### Comparing `python-simpleconf-0.5.7/simpleconf/loaders/osenv.py` & `python_simpleconf-0.5.8/simpleconf/loaders/osenv.py`

 * *Files identical despite different names*

### Comparing `python-simpleconf-0.5.7/simpleconf/loaders/toml.py` & `python_simpleconf-0.5.8/simpleconf/loaders/toml.py`

 * *Files identical despite different names*

### Comparing `python-simpleconf-0.5.7/simpleconf/utils.py` & `python_simpleconf-0.5.8/simpleconf/utils.py`

 * *Files identical despite different names*

### Comparing `python-simpleconf-0.5.7/setup.py` & `python_simpleconf-0.5.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,291 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: python-simpleconf
+Version: 0.5.8
+Summary: Simple configuration management with python.
+Home-page: https://github.com/pwwang/simpleconf
+License: MIT
+Author: pwwang
+Author-email: pwwang@pwwang.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: env
+Provides-Extra: ini
+Provides-Extra: toml
+Provides-Extra: yaml
+Requires-Dist: diot (>=0.2,<0.3)
+Requires-Dist: iniconfig (>=2.0,<3.0) ; extra == "ini" or extra == "all"
+Requires-Dist: python-dotenv (>=0.21,<0.22) ; extra == "env" or extra == "all"
+Requires-Dist: pyyaml (>=6,<7) ; extra == "yaml" or extra == "all"
+Requires-Dist: rtoml (>=0.8,<0.9) ; extra == "toml" or extra == "all"
+Project-URL: Repository, https://github.com/pwwang/simpleconf
+Description-Content-Type: text/markdown
 
-packages = \
-['simpleconf', 'simpleconf.loaders']
+# simpleconf
 
-package_data = \
-{'': ['*']}
+Simple configuration management for python
 
-install_requires = \
-['diot>=0.1,<0.2']
-
-extras_require = \
-{'all': ['python-dotenv>=0.20,<0.21',
-         'pyyaml>=6,<7',
-         'rtoml>=0.8,<0.9',
-         'iniconfig>=1.1,<2.0'],
- 'env': ['python-dotenv>=0.20,<0.21'],
- 'ini': ['iniconfig>=1.1,<2.0'],
- 'toml': ['rtoml>=0.8,<0.9'],
- 'yaml': ['pyyaml>=6,<7']}
-
-setup_kwargs = {
-    'name': 'python-simpleconf',
-    'version': '0.5.7',
-    'description': 'Simple configuration management with python.',
-    'long_description': '# simpleconf\n\nSimple configuration management for python\n\n## Installation\n```shell\n# released version\npip install python-simpleconf\n\n# Install support for ini\npip install python-simpleconf[ini]\n\n# Install support for dotenv\npip install python-simpleconf[dotenv]\n\n# Install support for yaml\npip install python-simpleconf[yaml]\n\n# Install support for toml\npip install python-simpleconf[toml]\n\n# Install support for all supported formats\npip install python-simpleconf[all]\n```\n\n## Features\n- Multiple formats supported\n- Type casting\n- Profile support\n- Simple APIs\n\n## Usage\n\n### Loading configurations\n\n```python\nfrom simpleconf import Config\n\n# Load a single file\nconf = Config.load(\'~/xxx.ini\')\n# load multiple files, later files override previous ones\nconf = Config.load(\n   \'~/xxx.ini\', \'~/xxx.env\', \'~/xxx.yaml\', \'~/xxx.toml\',\n   \'~/xxx.json\', \'simpleconf.osenv\', {\'a\': 3}\n)\n\n# Load a single file with a different loader\nconf = Config.load(\'~/xxx.ini\', loader="toml")\n```\n\n### Accessing configuration values\n\n```python\nfrom simpleconf import Config\n\nconf = Config.load({\'a\': 1, \'b\': {\'c\': 2}})\n# conf.a == 1\n# conf.b.c == 2\n```\n\n### Supported formats\n\n- `.ini/.cfg/.config` (parsed by `iniconfig`).\n  - For confiurations without profiles, an ini-like configuration like must have a `default` (case-insensitive) section.\n- `.env` (using `python-dotenv`). A file with environment variables.\n- `.yaml/.yml` (using `pyyaml`). A file with YAML data.\n- `.toml` (using `rtoml`). A file with TOML data.\n- `.json` (using `json`). A file with JSON data.\n- `XXX.osenv`: System environment variables with prefix `XXX_` (case-sensitive) is used.\n  - `XXX_A=1` will be loaded as `conf.A = 1`.\n- python dictionary.\n\n### Profile support\n\n#### Loading configurations\n\n##### Loading dictionaries\n\n```python\nfrom simpleconf import ProfileConfig\n\nconf = ProfileConfig.load({\'default\': {\'a\': 1})\n# conf.a == 1\n```\n\n##### Loading a `.env` file\n\n`config.env`\n```env\n# config.env\ndefault_a=1\n```\n\n```python\nfrom simpleconf import ProfileConfig\n\nconf = ProfileConfig.load(\'config.env\')\n# conf.a == 1\n```\n\n##### Loading ini-like configuration files\n\n```ini\n# config.ini\n[default]\na = 1\n```\n\n```python\nfrom simpleconf import ProfileConfig\n\nconf = ProfileConfig.load(\'config.ini\')\n# conf.a == 1\n```\n\n##### Loading JSON files\n\n`config.json`\n```json\n{\n  "default": {\n    "a": 1\n  }\n}\n```\n\n```python\nfrom simpleconf import ProfileConfig\n\nconf = ProfileConfig.load(\'config.json\')\n# conf.a == 1\n```\n\n##### Loading system environment variables\n\n```python\nfrom os import environ\nfrom simpleconf import ProfileConfig\n\nenviron[\'XXX_DEFAULT_A\'] = \'1\'\n\nconf = ProfileConfig.load(\'XXX.osenv\')\n# conf.a == 1\n```\n\n##### Loading TOML files\n\n```toml\n# config.toml\n[default]\na = 1\n```\n\n```python\nfrom simpleconf import ProfileConfig\n\nconf = ProfileConfig.load(\'config.toml\')\n# conf.a == 1\n```\n\n##### Loading YAML files\n\n```yaml\n# config.yaml\ndefault:\n  a: 1\n```\n\n```python\nfrom simpleconf import ProfileConfig\n\nconf = ProfileConfig.load(\'config.yaml\')\n# conf.a == 1\n```\n\n#### Switching profile\n\n```python\nfrom simpleconf import ProfileConfig\n\nconf = ProfileConfig.load(\n   {\'default\': {\'a\': 1, \'b\': 2}, \'dev\': {\'a\': 3}, \'prod\': {\'a\': 4}}\n)\n# conf.a == 1; conf.b == 2\n# ProfileConfig.profiles(conf) == [\'default\', \'dev\', \'prod\']\n# ProfileConfig.pool(conf) == {\'default\': {\'a\': 1, \'b\': 2}, \'dev\': {\'a\': 3}, \'prod\': {\'a\': 4}}\n# ProfileConfig.current_profile(conf) == \'default\'\n# ProfileConfig.base_profile(conf) == \'default\'\n\nProfileConfig.use_profile(conf, \'dev\')\n# conf.a == 3; conf.b == 2\n# ProfileConfig.current_profile(conf) == \'dev\'\n# ProfileConfig.base_profile(conf) == \'default\'\n\n# use a different base profile\nProfileConfig.use_profile(conf, \'prod\', base=\'dev\')\n# conf.a == 4   # No \'b\' in conf\n# ProfileConfig.current_profile(conf) == \'prod\'\n# ProfileConfig.base_profile(conf) == \'dev\'\n\n# Copy configuration instead of inplace modification\nconf2 = ProfileConfig.use_profile(conf, \'dev\', copy=True)\n# conf2 is not conf\n# conf2.a == 3; conf2.b == 2\n\n# Use a context manager\nwith ProfileConfig.use_profile(conf2, \'default\'):\n    conf2.a == 3\n    conf2.b == 2\n# conf2.a == 3; conf2.b == 2\n```\n\n### Type casting\n\nFor configuration formats with type support, including dictionary, no type casting is done by this library, except that for TOML files.\n\nTOML does not support `None` value in python. We use `rtoml` library to parse TOML files, which dumps `None` as `"null"`. So a `null_caster` is used to cast `"null"` to `None`.\n\nA `none_caster` is also enabled for TOML files, a pure string of `"@none"` is casted to `None`.\n\nFor other formats, following casters are supported:\n\n#### Int caster\n\n```python\nfrom os import environ\nfrom simpleconf import Config\n\nenviron[\'XXX_A\'] = \'@int:1\'\n\nconf = Config.load(\'XXX.osenv\')\n# conf.a == 1 # int\n```\n\n#### Float caster\n\n`@float:1.0` -> `1.0`\n\n### Bool caster\n\n`@bool:true` -> `True`\n`@bool:false` -> `False`\n\n#### Python caster\n\nValues are casted by `ast.literal_eval()`.\n\n```python\n"@python:1" => 1  # or\n"@py:1" => 1\n"@py:1.0` -> `1.0`\n"@py:[1, 2, 3]" => [1, 2, 3]\n```\n\n#### JSON caster\n\n`@json:{"a": 1}` -> `{"a": 1}`\n\n#### TOML caster\n\n`@toml:a = 1` -> `{"a": 1}`\n',
-    'author': 'pwwang',
-    'author_email': 'pwwang@pwwang.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/pwwang/simpleconf',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+## Installation
+```shell
+# released version
+pip install python-simpleconf
+
+# Install support for ini
+pip install python-simpleconf[ini]
+
+# Install support for dotenv
+pip install python-simpleconf[dotenv]
+
+# Install support for yaml
+pip install python-simpleconf[yaml]
+
+# Install support for toml
+pip install python-simpleconf[toml]
+
+# Install support for all supported formats
+pip install python-simpleconf[all]
+```
+
+## Features
+- Multiple formats supported
+- Type casting
+- Profile support
+- Simple APIs
+
+## Usage
+
+### Loading configurations
+
+```python
+from simpleconf import Config
+
+# Load a single file
+conf = Config.load('~/xxx.ini')
+# load multiple files, later files override previous ones
+conf = Config.load(
+   '~/xxx.ini', '~/xxx.env', '~/xxx.yaml', '~/xxx.toml',
+   '~/xxx.json', 'simpleconf.osenv', {'a': 3}
+)
+
+# Load a single file with a different loader
+conf = Config.load('~/xxx.ini', loader="toml")
+```
+
+### Accessing configuration values
+
+```python
+from simpleconf import Config
+
+conf = Config.load({'a': 1, 'b': {'c': 2}})
+# conf.a == 1
+# conf.b.c == 2
+```
+
+### Supported formats
+
+- `.ini/.cfg/.config` (parsed by `iniconfig`).
+  - For confiurations without profiles, an ini-like configuration like must have a `default` (case-insensitive) section.
+- `.env` (using `python-dotenv`). A file with environment variables.
+- `.yaml/.yml` (using `pyyaml`). A file with YAML data.
+- `.toml` (using `rtoml`). A file with TOML data.
+- `.json` (using `json`). A file with JSON data.
+- `XXX.osenv`: System environment variables with prefix `XXX_` (case-sensitive) is used.
+  - `XXX_A=1` will be loaded as `conf.A = 1`.
+- python dictionary.
+
+### Profile support
+
+#### Loading configurations
+
+##### Loading dictionaries
+
+```python
+from simpleconf import ProfileConfig
+
+conf = ProfileConfig.load({'default': {'a': 1})
+# conf.a == 1
+```
+
+##### Loading a `.env` file
+
+`config.env`
+```env
+# config.env
+default_a=1
+```
+
+```python
+from simpleconf import ProfileConfig
+
+conf = ProfileConfig.load('config.env')
+# conf.a == 1
+```
+
+##### Loading ini-like configuration files
+
+```ini
+# config.ini
+[default]
+a = 1
+```
+
+```python
+from simpleconf import ProfileConfig
+
+conf = ProfileConfig.load('config.ini')
+# conf.a == 1
+```
+
+##### Loading JSON files
+
+`config.json`
+```json
+{
+  "default": {
+    "a": 1
+  }
 }
+```
+
+```python
+from simpleconf import ProfileConfig
+
+conf = ProfileConfig.load('config.json')
+# conf.a == 1
+```
+
+##### Loading system environment variables
+
+```python
+from os import environ
+from simpleconf import ProfileConfig
+
+environ['XXX_DEFAULT_A'] = '1'
+
+conf = ProfileConfig.load('XXX.osenv')
+# conf.a == 1
+```
+
+##### Loading TOML files
+
+```toml
+# config.toml
+[default]
+a = 1
+```
+
+```python
+from simpleconf import ProfileConfig
+
+conf = ProfileConfig.load('config.toml')
+# conf.a == 1
+```
+
+##### Loading YAML files
+
+```yaml
+# config.yaml
+default:
+  a: 1
+```
+
+```python
+from simpleconf import ProfileConfig
+
+conf = ProfileConfig.load('config.yaml')
+# conf.a == 1
+```
+
+#### Switching profile
+
+```python
+from simpleconf import ProfileConfig
+
+conf = ProfileConfig.load(
+   {'default': {'a': 1, 'b': 2}, 'dev': {'a': 3}, 'prod': {'a': 4}}
+)
+# conf.a == 1; conf.b == 2
+# ProfileConfig.profiles(conf) == ['default', 'dev', 'prod']
+# ProfileConfig.pool(conf) == {'default': {'a': 1, 'b': 2}, 'dev': {'a': 3}, 'prod': {'a': 4}}
+# ProfileConfig.current_profile(conf) == 'default'
+# ProfileConfig.base_profile(conf) == 'default'
+
+ProfileConfig.use_profile(conf, 'dev')
+# conf.a == 3; conf.b == 2
+# ProfileConfig.current_profile(conf) == 'dev'
+# ProfileConfig.base_profile(conf) == 'default'
+
+# use a different base profile
+ProfileConfig.use_profile(conf, 'prod', base='dev')
+# conf.a == 4   # No 'b' in conf
+# ProfileConfig.current_profile(conf) == 'prod'
+# ProfileConfig.base_profile(conf) == 'dev'
+
+# Copy configuration instead of inplace modification
+conf2 = ProfileConfig.use_profile(conf, 'dev', copy=True)
+# conf2 is not conf
+# conf2.a == 3; conf2.b == 2
+
+# Use a context manager
+with ProfileConfig.use_profile(conf2, 'default'):
+    conf2.a == 3
+    conf2.b == 2
+# conf2.a == 3; conf2.b == 2
+```
+
+### Type casting
+
+For configuration formats with type support, including dictionary, no type casting is done by this library, except that for TOML files.
+
+TOML does not support `None` value in python. We use `rtoml` library to parse TOML files, which dumps `None` as `"null"`. So a `null_caster` is used to cast `"null"` to `None`.
+
+A `none_caster` is also enabled for TOML files, a pure string of `"@none"` is casted to `None`.
+
+For other formats, following casters are supported:
+
+#### Int caster
+
+```python
+from os import environ
+from simpleconf import Config
+
+environ['XXX_A'] = '@int:1'
+
+conf = Config.load('XXX.osenv')
+# conf.a == 1 # int
+```
+
+#### Float caster
+
+`@float:1.0` -> `1.0`
+
+### Bool caster
+
+`@bool:true` -> `True`
+`@bool:false` -> `False`
+
+#### Python caster
+
+Values are casted by `ast.literal_eval()`.
+
+```python
+"@python:1" => 1  # or
+"@py:1" => 1
+"@py:1.0` -> `1.0`
+"@py:[1, 2, 3]" => [1, 2, 3]
+```
+
+#### JSON caster
+
+`@json:{"a": 1}` -> `{"a": 1}`
+
+#### TOML caster
 
+`@toml:a = 1` -> `{"a": 1}`
 
-setup(**setup_kwargs)
```

