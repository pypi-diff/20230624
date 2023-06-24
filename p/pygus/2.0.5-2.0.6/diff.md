# Comparing `tmp/pygus-2.0.5.tar.gz` & `tmp/pygus-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygus-2.0.5.tar", max compression
+gzip compressed data, was "pygus-2.0.6.tar", max compression
```

## Comparing `pygus-2.0.5.tar` & `pygus-2.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2022-10-24 14:24:35.788368 pygus-2.0.5/LICENSE
--rw-r--r--   0        0        0     1541 2023-04-19 16:37:11.282155 pygus-2.0.5/README-pypi.md
--rw-r--r--   0        0        0      185 2023-06-20 14:39:46.120957 pygus-2.0.5/pygus/__init__.py
--rw-r--r--   0        0        0      217 2023-06-20 14:39:46.121591 pygus-2.0.5/pygus/gus/__init__.py
--rw-r--r--   0        0        0    27333 2023-06-21 15:20:21.033607 pygus-2.0.5/pygus/gus/agents.py
--rw-r--r--   0        0        0     7484 2023-06-07 17:14:01.718672 pygus-2.0.5/pygus/gus/allometrics.py
--rw-r--r--   0        0        0     3069 2023-04-26 08:20:10.279558 pygus-2.0.5/pygus/gus/inputs/allometrics.json
--rw-r--r--   0        0        0    39187 2023-05-23 14:51:09.274748 pygus-2.0.5/pygus/gus/inputs/amsterdam_all_trees_1000.csv
--rw-r--r--   0        0        0  9874219 2023-05-30 13:48:12.428717 pygus-2.0.5/pygus/gus/inputs/amsterdam_all_trees_100000.csv
--rw-r--r--   0        0        0     7679 2023-05-29 16:04:17.254756 pygus-2.0.5/pygus/gus/inputs/amsterdam_all_trees_200.csv
--rw-r--r--   0        0        0   793770 2023-05-30 13:23:28.448382 pygus-2.0.5/pygus/gus/inputs/amsterdam_all_trees_20000.csv
--rw-r--r--   0        0        0  9874219 2023-05-23 13:42:14.779205 pygus-2.0.5/pygus/gus/inputs/amsterdam_all_trees_cleaned.csv
--rw-r--r--   0        0        0       95 2023-05-22 14:31:01.986378 pygus-2.0.5/pygus/gus/inputs/scenario.json
--rw-r--r--   0        0        0      264 2023-04-26 08:20:10.279976 pygus-2.0.5/pygus/gus/inputs/site.json
--rw-r--r--   0        0        0     5932 2023-04-26 08:20:10.280228 pygus-2.0.5/pygus/gus/inputs/trees.csv
--rw-r--r--   0        0        0    16419 2023-06-20 16:53:01.989214 pygus-2.0.5/pygus/gus/models.py
--rw-r--r--   0        0        0  1566870 2023-04-26 08:20:10.288567 pygus-2.0.5/pygus/gus/outputs/trees_yearly.json
--rw-r--r--   0        0        0     4959 2023-06-20 14:39:46.124655 pygus-2.0.5/pygus/gus/utilities.py
--rw-r--r--   0        0        0     1701 2023-04-26 08:20:10.289503 pygus-2.0.5/pygus/gus/weather.py
--rw-r--r--   0        0        0       58 2023-04-26 08:20:10.290114 pygus-2.0.5/pygus/impacts/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-26 08:20:10.290632 pygus-2.0.5/pygus/impacts/carbon.py
--rw-r--r--   0        0        0    32960 2023-04-26 08:20:10.291410 pygus-2.0.5/pygus/impacts/water.py
--rw-r--r--   0        0        0     1523 2023-06-21 15:21:33.623497 pygus-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 pygus-2.0.5/setup.py
--rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 pygus-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-24 14:24:35.788368 pygus-2.0.6/LICENSE
+-rw-r--r--   0        0        0     1541 2023-04-19 16:37:11.282155 pygus-2.0.6/README-pypi.md
+-rw-r--r--   0        0        0      185 2023-06-20 14:39:46.120957 pygus-2.0.6/pygus/__init__.py
+-rw-r--r--   0        0        0      217 2023-06-20 14:39:46.121591 pygus-2.0.6/pygus/gus/__init__.py
+-rw-r--r--   0        0        0    27333 2023-06-24 16:00:43.525451 pygus-2.0.6/pygus/gus/agents.py
+-rw-r--r--   0        0        0     7484 2023-06-07 17:14:01.718672 pygus-2.0.6/pygus/gus/allometrics.py
+-rw-r--r--   0        0        0     3069 2023-04-26 08:20:10.279558 pygus-2.0.6/pygus/gus/inputs/allometrics.json
+-rw-r--r--   0        0        0    39187 2023-05-23 14:51:09.274748 pygus-2.0.6/pygus/gus/inputs/amsterdam_all_trees_1000.csv
+-rw-r--r--   0        0        0  9874219 2023-05-30 13:48:12.428717 pygus-2.0.6/pygus/gus/inputs/amsterdam_all_trees_100000.csv
+-rw-r--r--   0        0        0     7679 2023-05-29 16:04:17.254756 pygus-2.0.6/pygus/gus/inputs/amsterdam_all_trees_200.csv
+-rw-r--r--   0        0        0   793770 2023-05-30 13:23:28.448382 pygus-2.0.6/pygus/gus/inputs/amsterdam_all_trees_20000.csv
+-rw-r--r--   0        0        0  9874219 2023-05-23 13:42:14.779205 pygus-2.0.6/pygus/gus/inputs/amsterdam_all_trees_cleaned.csv
+-rw-r--r--   0        0        0       95 2023-05-22 14:31:01.986378 pygus-2.0.6/pygus/gus/inputs/scenario.json
+-rw-r--r--   0        0        0      264 2023-04-26 08:20:10.279976 pygus-2.0.6/pygus/gus/inputs/site.json
+-rw-r--r--   0        0        0     5932 2023-04-26 08:20:10.280228 pygus-2.0.6/pygus/gus/inputs/trees.csv
+-rw-r--r--   0        0        0    16419 2023-06-20 16:53:01.989214 pygus-2.0.6/pygus/gus/models.py
+-rw-r--r--   0        0        0  1566870 2023-04-26 08:20:10.288567 pygus-2.0.6/pygus/gus/outputs/trees_yearly.json
+-rw-r--r--   0        0        0     4959 2023-06-20 14:39:46.124655 pygus-2.0.6/pygus/gus/utilities.py
+-rw-r--r--   0        0        0     1701 2023-04-26 08:20:10.289503 pygus-2.0.6/pygus/gus/weather.py
+-rw-r--r--   0        0        0       58 2023-04-26 08:20:10.290114 pygus-2.0.6/pygus/impacts/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-26 08:20:10.290632 pygus-2.0.6/pygus/impacts/carbon.py
+-rw-r--r--   0        0        0    32960 2023-04-26 08:20:10.291410 pygus-2.0.6/pygus/impacts/water.py
+-rw-r--r--   0        0        0     1523 2023-06-24 16:01:05.411437 pygus-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 pygus-2.0.6/setup.py
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 pygus-2.0.6/PKG-INFO
```

### Comparing `pygus-2.0.5/LICENSE` & `pygus-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/README-pypi.md` & `pygus-2.0.6/README-pypi.md`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/agents.py` & `pygus-2.0.6/pygus/gus/agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         self.decomposing_trunk = 0
         self.immediate_release = 0
         self.death_acc = False
 
         if self.model.maintenance_scope == 0:
             self.expected_care = 0
         elif self.model.maintenance_scope == 1:
-            self.expected_care = 0.3
+            self.expected_care = 0.5
         else:
             self.expected_care = 1.0
 
     def step(self):
         """State transitions of a given Tree agent.
 
         Args:
```

### Comparing `pygus-2.0.5/pygus/gus/allometrics.py` & `pygus-2.0.6/pygus/gus/allometrics.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/inputs/allometrics.json` & `pygus-2.0.6/pygus/gus/inputs/allometrics.json`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/inputs/amsterdam_all_trees_1000.csv` & `pygus-2.0.6/pygus/gus/inputs/amsterdam_all_trees_1000.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/inputs/amsterdam_all_trees_100000.csv` & `pygus-2.0.6/pygus/gus/inputs/amsterdam_all_trees_100000.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/inputs/amsterdam_all_trees_200.csv` & `pygus-2.0.6/pygus/gus/inputs/amsterdam_all_trees_200.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/inputs/amsterdam_all_trees_20000.csv` & `pygus-2.0.6/pygus/gus/inputs/amsterdam_all_trees_20000.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/inputs/amsterdam_all_trees_cleaned.csv` & `pygus-2.0.6/pygus/gus/inputs/amsterdam_all_trees_cleaned.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/inputs/trees.csv` & `pygus-2.0.6/pygus/gus/inputs/trees.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/models.py` & `pygus-2.0.6/pygus/gus/models.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/outputs/trees_yearly.json` & `pygus-2.0.6/pygus/gus/outputs/trees_yearly.json`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/utilities.py` & `pygus-2.0.6/pygus/gus/utilities.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/gus/weather.py` & `pygus-2.0.6/pygus/gus/weather.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/impacts/carbon.py` & `pygus-2.0.6/pygus/impacts/carbon.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pygus/impacts/water.py` & `pygus-2.0.6/pygus/impacts/water.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.5/pyproject.toml` & `pygus-2.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyGUS"
-version = "2.0.5"
+version = "2.0.6"
 description = "Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis."
 authors = ["Bulent Ozel <bulent@lucidminds.ai>"] 
 maintainers = [
     "Oguzhan Yayla <oguzhan@lucidminds.ai>", 
     "Marko Petrovic <marko@lucidminds.ai>", 
     "Axel Nilsson <axel@darkmatterlabs.org>"
 ]
```

### Comparing `pygus-2.0.5/setup.py` & `pygus-2.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'pytest>=7.1.2,<8.0.0',
  'seaborn>=0.11.2,<0.12.0',
  'termcolor>=2.1.1,<3.0.0',
  'utm>=0.7.0,<0.8.0']
 
 setup_kwargs = {
     'name': 'pygus',
-    'version': '2.0.5',
+    'version': '2.0.6',
     'description': 'Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.',
     'long_description': '[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Versions](https://img.shields.io/pypi/pyversions/pygus)]()\n\n\n\n# gus\n![GUS-IMAGE](https://miro.medium.com/max/1400/1*fMM7rnq1RJCh-nFBGLUvyA.png)\n\nGreen Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.\n\n## Getting Started\nVisit the GUS [website documentation](https://lucidmindsai.github.io/gus/) for help with installing GUS, code documentation, and a [basic tutorial](https://github.com/lucidmindsai/gus/blob/main/notebooks/Tutorial.ipynb) to get you started. \n\n## Install from PyPi\nWe publish GUS as `pyGus` package in PyPi. Dependencies can be found in the .toml file on the GUS GitHub page. Even though installation with Poetry is possible, the most stable installation can be done via pip.\n\n```\n$ pip install pygus\n```\n\nFor further instructions and code documentation, visit [GUS Code Documentation](https://lucidmindsai.github.io/gus/)\n\n### Who maintains GUS?\nThe GUS is currently developed and maintained by [Lucidminds](https://lucidminds.ai/) and [Dark Matter Labs](https://darkmatterlabs.org/) members as part of their joint project [TreesAI](https://treesasinfrastructure.com/#/).\n\n### Notes\n* The GUS is open for PRs.\n* PRs will be reviewed by the current maintainers of the project.\n* Extensive development guidelines will be provided soon.\n* To report bugs, fixes, and questions, please use the [GitHub issues](https://github.com/lucidmindsai/gus/issues).',
     'author': 'Bulent Ozel',
     'author_email': 'bulent@lucidminds.ai',
     'maintainer': 'Oguzhan Yayla',
     'maintainer_email': 'oguzhan@lucidminds.ai',
     'url': 'https://github.com/lucidmindsai/gus',
```

### Comparing `pygus-2.0.5/PKG-INFO` & `pygus-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygus
-Version: 2.0.5
+Version: 2.0.6
 Summary: Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.
 Home-page: https://github.com/lucidmindsai/gus
 License: Apache-2.0
 Author: Bulent Ozel
 Author-email: bulent@lucidminds.ai
 Maintainer: Oguzhan Yayla
 Maintainer-email: oguzhan@lucidminds.ai
```

