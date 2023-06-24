# Comparing `tmp/diot-0.1.8.tar.gz` & `tmp/diot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diot-0.1.8.tar", max compression
+gzip compressed data, was "diot-0.2.0.tar", max compression
```

## Comparing `diot-0.1.8.tar` & `diot-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-06-05 16:01:50.758986 diot-0.1.8/LICENSE
--rw-r--r--   0        0        0     5283 2023-06-05 16:01:50.758986 diot-0.1.8/README.md
--rw-r--r--   0        0        0      195 2023-06-05 16:01:50.758986 diot-0.1.8/diot/__init__.py
--rw-r--r--   0        0        0    27959 2023-06-05 16:01:50.758986 diot-0.1.8/diot/diot.py
--rw-r--r--   0        0        0     3070 2023-06-05 16:01:50.758986 diot-0.1.8/diot/transforms.py
--rw-r--r--   0        0        0     1587 2023-06-05 16:01:50.758986 diot-0.1.8/diot/utils.py
--rw-r--r--   0        0        0     1059 2023-06-05 16:01:50.758986 diot-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 diot-0.1.8/setup.py
--rw-r--r--   0        0        0     5995 1970-01-01 00:00:00.000000 diot-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-24 05:46:06.812260 diot-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5283 2023-06-24 05:46:06.812260 diot-0.2.0/README.md
+-rw-r--r--   0        0        0      195 2023-06-24 05:46:06.812260 diot-0.2.0/diot/__init__.py
+-rw-r--r--   0        0        0    28559 2023-06-24 05:46:06.812260 diot-0.2.0/diot/diot.py
+-rw-r--r--   0        0        0     3070 2023-06-24 05:46:06.812260 diot-0.2.0/diot/transforms.py
+-rw-r--r--   0        0        0     1587 2023-06-24 05:46:06.812260 diot-0.2.0/diot/utils.py
+-rw-r--r--   0        0        0     1059 2023-06-24 05:46:06.816260 diot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 diot-0.2.0/setup.py
+-rw-r--r--   0        0        0     5995 1970-01-01 00:00:00.000000 diot-0.2.0/PKG-INFO
```

### Comparing `diot-0.1.8/LICENSE` & `diot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diot-0.1.8/README.md` & `diot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `diot-0.1.8/diot/diot.py` & `diot-0.2.0/diot/diot.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,26 +287,44 @@
             kwargs: kwargs that can be sent to dict to update the object
 
         Raises:
             DiotFrozenError: when try to update a frozen diot
         """
         if self.__diot__["frozen"]:
             raise DiotFrozenError("Cannot update a frozen diot.")
+
+        dict_to_update = dict(*value, **kwargs)
+        for key, val in dict_to_update.items():
+            self[key] = nest(val, self.__diot__["nest"], type(self), False)
+
+    def update_recursively(self, *value, **kwargs) -> None:
+        """Update the object. Shortcut: `|=`
+
+        Args:
+            args: args that can be sent to dict to update the object
+            kwargs: kwargs that can be sent to dict to update the object
+
+        Raises:
+            DiotFrozenError: when try to update a frozen diot
+        """
+        if self.__diot__["frozen"]:
+            raise DiotFrozenError("Cannot update a frozen diot.")
+
         dict_to_update = dict(*value, **kwargs)
         for key, val in dict_to_update.items():
             if (
                 key not in self
                 or not isinstance(self[key], dict)
                 or not isinstance(val, dict)
             ):
                 self[key] = nest(
                     val,
                     self.__diot__["nest"],
-                    self.__class__,
-                    self.__diot__["frozen"] is True,
+                    type(self),
+                    False,
                 )
             else:
                 self[key].update(val)
 
     def __or__(self, other: Mapping) -> "Diot":
         ret = self.copy()
         ret.update(other)
```

### Comparing `diot-0.1.8/diot/transforms.py` & `diot-0.2.0/diot/transforms.py`

 * *Files identical despite different names*

### Comparing `diot-0.1.8/diot/utils.py` & `diot-0.2.0/diot/utils.py`

 * *Files identical despite different names*

### Comparing `diot-0.1.8/pyproject.toml` & `diot-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "diot"
-version = "0.1.8"
+version = "0.2.0"
 description = "Python dictionary with dot notation."
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/diot"
 repository = "https://github.com/pwwang/diot"
```

### Comparing `diot-0.1.8/setup.py` & `diot-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['inflection>=0.5,<0.6']
 
 setup_kwargs = {
     'name': 'diot',
-    'version': '0.1.8',
+    'version': '0.2.0',
     'description': 'Python dictionary with dot notation.',
     'long_description': '![Logo](https://raw.githubusercontent.com/pwwang/diot/master/logo.png)\n\n[![pypi][1]][2] [![tag][3]][4] [![codacy quality][7]][8] [![coverage][9]][8] ![pyver][10] ![building][6] ![docs][5]\n\nPython dictionary with dot notation (A re-implementation of [python-box](https://github.com/cdgriffith/Box) with some issues fixed and simplified)\n\n```python\nfrom diot import Diot\n\nmovie_data = {\n  "movies": {\n    "Spaceballs": {\n      "imdb stars": 7.1,\n      "rating": "PG",\n      "length": 96,\n      "director": "Mel Brooks",\n      "stars": [{"name": "Mel Brooks", "imdb": "nm0000316", "role": "President Skroob"},\n                {"name": "John Candy","imdb": "nm0001006", "role": "Barf"},\n                {"name": "Rick Moranis", "imdb": "nm0001548", "role": "Dark Helmet"}\n      ]\n    },\n    "Robin Hood: Men in Tights": {\n      "imdb stars": 6.7,\n      "rating": "PG-13",\n      "length": 104,\n      "director": "Mel Brooks",\n      "stars": [\n                {"name": "Cary Elwes", "imdb": "nm0000144", "role": "Robin Hood"},\n                {"name": "Richard Lewis", "imdb": "nm0507659", "role": "Prince John"},\n                {"name": "Roger Rees", "imdb": "nm0715953", "role": "Sheriff of Rottingham"},\n                {"name": "Amy Yasbeck", "imdb": "nm0001865", "role": "Marian"}\n      ]\n    }\n  }\n}\n\n# Box is a conversion_box by default, pass in `conversion_box=False` to disable that behavior\n# Explicitly tell Diot to convert dict/list inside\nmovie_diot = Diot(movie_data)\n\nmovie_diot.movies.Robin_Hood_Men_in_Tights.imdb_stars\n# 6.7\n\nmovie_diot.movies.Spaceballs.stars[0].name\n# \'Mel Brooks\'\n\n# Different as box, you have to use Diot for new data in a list\nmovie_diot.movies.Spaceballs.stars.append(\n\tDiot({"name": "Bill Pullman", "imdb": "nm0000597", "role": "Lone Starr"}))\nmovie_diot.movies.Spaceballs.stars[-1].role\n# \'Lone Starr\'\n```\n\n## Install\n```shell\npip install -U diot\n```\n\n## API\n\nhttps://pwwang.github.io/diot/api/diot/\n\n\n## Usage\n\n### Diot\n\nInstantiated the same ways as `dict`\n```python\nDiot({\'data\': 2, \'count\': 5})\nDiot(data=2, count=5)\nDiot({\'data\': 2, \'count\': 1}, count=5)\nDiot([(\'data\', 2), (\'count\', 5)])\n\n# All will create\n# Diot([(\'data\', 2), (\'count\', 5)], diot_nest = True, diot_transform = \'safe\')\n```\n\nSame as `python-box`, `Diot` is a subclass of dict which overrides some base functionality to make sure everything stored in the dict can be accessed as an attribute or key value.\n\n```python\ndiot = Diot({\'data\': 2, \'count\': 5})\ndiot.data == diot[\'data\'] == getattr(diot, \'data\')\n```\n\nBy default, diot uses a safe transformation to transform keys into safe names that can be accessed by `diot.xxx`\n```python\ndt = Diot({"321 Is a terrible Key!": "yes, really"})\ndt._321_Is_a_terrible_Key_\n# \'yes, really\'\n```\n\nDifferent as `python-box`, duplicate attributes are not allowed.\n```python\ndt = Diot({"!bad!key!": "yes, really", ".bad.key.": "no doubt"})\n# KeyError\n```\n\nUse different transform functions:\n\n```python\ndt = Diot(oneTwo = 12, diot_transform = \'snake_case\')\n# or use alias:\n# dt = SnakeDiot(oneTwo = 12)\ndt.one_two == dt[\'one_two\'] == dt[\'oneTwo\'] == 12\n\ndt = Diot(one_two = 12, diot_transform = \'camel_case\')\n# or use alias:\n# dt = CamelDiot(one_two = 12)\ndt.oneTwo == dt[\'one_two\'] == dt[\'oneTwo\'] == 12\n\ndt = Diot(one_two = 12, diot_transform = \'upper\')\ndt.ONE_TWO == dt[\'one_two\'] == dt[\'ONETWO\'] == 12\n\ndt = Diot(ONE_TWO = 12, diot_transform = \'lower\')\ndt.one_two == dt[\'ONE_TWO\'] == dt[\'one_two\'] == 12\n```\n\nUse your own transform function:\n\n```python\nimport inflection\n\ndt = Diot(post = 10, diot_transform = inflection.pluralize)\ndt.posts == dt[\'posts\'] == dt[\'post\'] == 10\n```\n\n### OrderedDiot\n```python\ndiot_of_order = OrderedDiot()\ndiot_of_order.c = 1\ndiot_of_order.a = 2\ndiot_of_order.d = 3\n\nlist(diot_of_order.keys()) == [\'c\', \'a\', \'d\']\n\n# insertion allowed for OrderedDiot\nod = OrderedDiot()\nod.insert(0, "c", "d")\nod.insert(None, "x", "y")\nod.insert_before(\'c\', "e", "f")\nod.insert_after("a", ("g", "h"))\n\nod2 = OrderedDiot()\nod2.a1 = \'b1\'\nod2.c1 = \'d1\'\nod.insert(-1, od2)\n\nod3 = OrderedDiot()\nod3.a2 = \'b2\'\nod3.c2 = \'d2\'\nod.insert_before(\'c\', od3)\n```\n\n### FrozenDiot\n\n```python\nfd = FrozenDiot(a=1, b=3)\nfd.c = 3 # DiotFrozenError\nwith fd.thaw():\n    fd.c = 3\nfd.c == 3\n```\n\n### Missing key handler\n\n```python\nd = Diot(a=1, b=2, diot_missing=ValueError)\nd[\'c\'] # ValueError\nd.c # AttributeError from ValueError\n\nd = Diot(a=1, b=2, diot_missing=ValueError("Custom message"))\n\nd = Diot(a=1, b=2, diot_missing=None)\n# d.c is None\n\nd = Diot(a=1, b=2, diot_missing=lambda key, diot: diot.a + diot.b)\n# d.c == 3\n```\n\n[1]: https://img.shields.io/pypi/v/diot?style=flat-square\n[2]: https://pypi.org/project/diot/\n[3]: https://img.shields.io/github/tag/pwwang/diot?style=flat-square\n[4]: https://github.com/pwwang/diot\n[5]: https://img.shields.io/github/actions/workflow/status/pwwang/diot/docs.yml?label=docs&style=flat-square\n[6]: https://img.shields.io/github/actions/workflow/status/pwwang/diot/build.yml?style=flat-square\n[7]: https://img.shields.io/codacy/grade/738e49b9cc1745c4ae6a7bb3b198cc3d?style=flat-square\n[8]: https://app.codacy.com/gh/pwwang/diot/dashboard\n[9]: https://img.shields.io/codacy/coverage/738e49b9cc1745c4ae6a7bb3b198cc3d?style=flat-square\n[10]: https://img.shields.io/pypi/pyversions/diot?style=flat-square\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/diot',
```

### Comparing `diot-0.1.8/PKG-INFO` & `diot-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diot
-Version: 0.1.8
+Version: 0.2.0
 Summary: Python dictionary with dot notation.
 Home-page: https://github.com/pwwang/diot
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

