# Comparing `tmp/mcresources-1.5.9.tar.gz` & `tmp/mcresources-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcresources-1.5.9.tar", last modified: Sun Jul  3 16:03:25 2022, max compression
+gzip compressed data, was "mcresources-1.6.0.tar", last modified: Sat Jun 24 20:32:39 2023, max compression
```

## Comparing `mcresources-1.5.9.tar` & `mcresources-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 16:03:25.321420 mcresources-1.5.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-07-03 16:03:11.000000 mcresources-1.5.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-07-03 16:03:25.321420 mcresources-1.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-07-03 16:03:11.000000 mcresources-1.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 16:03:25.321420 mcresources-1.5.9/mcresources/
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/advancements.py
--rw-r--r--   0 runner    (1001) docker     (121)    14270 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/block_context.py
--rw-r--r--   0 runner    (1001) docker     (121)    14412 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/block_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/item_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     4260 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/loot_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/recipe_context.py
--rw-r--r--   0 runner    (1001) docker     (121)    28038 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4008 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/surface_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/type_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)    21442 2022-07-03 16:03:11.000000 mcresources-1.5.9/mcresources/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 16:03:25.321420 mcresources-1.5.9/mcresources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-07-03 16:03:25.000000 mcresources-1.5.9/mcresources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-07-03 16:03:25.000000 mcresources-1.5.9/mcresources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-03 16:03:25.000000 mcresources-1.5.9/mcresources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-03 16:03:25.000000 mcresources-1.5.9/mcresources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-07-03 16:03:25.321420 mcresources-1.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-07-03 16:03:11.000000 mcresources-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 20:32:39.845972 mcresources-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-24 20:32:23.000000 mcresources-1.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-24 20:32:39.845972 mcresources-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-24 20:32:23.000000 mcresources-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 20:32:39.845972 mcresources-1.6.0/mcresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/advancements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/atlases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/block_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14412 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/block_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/item_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/loot_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/recipe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29767 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/surface_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/type_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-06-24 20:32:23.000000 mcresources-1.6.0/mcresources/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 20:32:39.845972 mcresources-1.6.0/mcresources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-24 20:32:39.000000 mcresources-1.6.0/mcresources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-24 20:32:39.000000 mcresources-1.6.0/mcresources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 20:32:39.000000 mcresources-1.6.0/mcresources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-24 20:32:39.000000 mcresources-1.6.0/mcresources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 20:32:39.845972 mcresources-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-24 20:32:23.000000 mcresources-1.6.0/setup.py
```

### Comparing `mcresources-1.5.9/LICENSE.txt` & `mcresources-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mcresources-1.5.9/PKG-INFO` & `mcresources-1.6.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: mcresources
-Version: 1.5.9
+Version: 1.6.0
 Summary: A Python Data Generator for Minecraft Modding
 Home-page: https://github.com/alcatrazEscapee/mcresources
 Author: Alex O'Neill
 Author-email: alex@molleroneill.com
 License: MIT
 Keywords: python,minecraft,resources,modding,forge
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Minecraft Resource Generator
 
 This is a python module aimed to enable simple generation of the many json files that are required for Minecraft modding.
 
-### Pack Format
+### Data Format
 
-Updates of this tool will track the latest pack format (`pack_format` in a resource pack) as soon as possible. In order to generate resources compliant with a specific pack format, the latest version can be found below
+Updates of this tool will track the format of the latest version of Minecraft. For each specific Minecraft version, the latest version of `mcresources`, targeting that version, can be found below:
 
-Pack Format | Minimum Minecraft Version | Latest mcresources Version
----|---|---
-8 | 1.18 | Latest
-7 | 1.17 | 1.4.6
-6 | 1.16.2 | 1.4.6
-5 | 1.15 | 1.3.3
-4 | 1.13 | 0.0.2
+| Minecraft Version | Latest mcresources Version |
+|-------------------|----------------------------|
+| 1.20              | Latest                     |
+| 1.18              | 1.5.11                     |
+| 1.17              | 1.4.6                      |
+| 1.16.2            | 1.4.6                      |
+| 1.15              | 1.3.3                      |
+| 1.13              | 0.0.2                      |
 
 ---
 
 ### [Documentation](https://github.com/alcatrazEscapee/mcresources/wiki)
 
 The wiki (link above) is generated from the methods and docstring comments of the library itself using `./docs.py`, and will always be up-to-date with the latest version of the library.
-
```

### Comparing `mcresources-1.5.9/README.md` & `mcresources-1.6.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Minecraft Resource Generator
 
 This is a python module aimed to enable simple generation of the many json files that are required for Minecraft modding.
 
-### Pack Format
+### Data Format
 
-Updates of this tool will track the latest pack format (`pack_format` in a resource pack) as soon as possible. In order to generate resources compliant with a specific pack format, the latest version can be found below
+Updates of this tool will track the format of the latest version of Minecraft. For each specific Minecraft version, the latest version of `mcresources`, targeting that version, can be found below:
 
-Pack Format | Minimum Minecraft Version | Latest mcresources Version
----|---|---
-8 | 1.18 | Latest
-7 | 1.17 | 1.4.6
-6 | 1.16.2 | 1.4.6
-5 | 1.15 | 1.3.3
-4 | 1.13 | 0.0.2
+| Minecraft Version | Latest mcresources Version |
+|-------------------|----------------------------|
+| 1.20              | Latest                     |
+| 1.18              | 1.5.11                     |
+| 1.17              | 1.4.6                      |
+| 1.16.2            | 1.4.6                      |
+| 1.15              | 1.3.3                      |
+| 1.13              | 0.0.2                      |
 
 ---
 
 ### [Documentation](https://github.com/alcatrazEscapee/mcresources/wiki)
 
 The wiki (link above) is generated from the methods and docstring comments of the library itself using `./docs.py`, and will always be up-to-date with the latest version of the library.
```

### Comparing `mcresources-1.5.9/mcresources/advancements.py` & `mcresources-1.6.0/mcresources/advancements.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class AdvancementCategory:
     def __init__(self, rm, category: str, background: str):
         self.rm = rm
         self.category = category
         self.background = background
 
-    def advancement(self, name: str, icon: Json, title: str, description: str, parent: Optional[str], criteria: Json, requirements: Json = None, frame: str = 'task', toast: bool = True, chat: bool = True, hidden: bool = False):
+    def advancement(self, name: str, icon: Json, title: str, description: str, parent: Optional[str], criteria: Json, requirements: Json = None, frame: str = 'task', toast: bool = True, chat: bool = True, hidden: bool = False) -> 'AdvancementContext':
         key = '%s.advancements.%s.%s' % (self.rm.domain, self.category, name)
 
         if parent is not None:
             parent = utils.resource_location(self.rm.domain, self.category + '/' + parent).join()
 
         self.rm.advancement((self.category, name), {
             'icon': utils.item_stack(icon),
@@ -37,14 +37,25 @@
             'show_toast': toast,
             'announce_to_chat': chat,
             'hidden': hidden,
             'background': self.background
         }, parent, criteria, requirements)
         self.rm.lang(key + '.title', title)
         self.rm.lang(key + '.description', description)
+        return AdvancementContext(self, name, parent)
+
+
+class AdvancementContext:
+    def __init__(self, category: AdvancementCategory, name: str, parent: Optional[str]) -> None:
+        self.category = category
+        self.name = name
+        self.parent = parent
+    
+    def add_child(self, name: str, icon: Json, title: str, description: str, criteria: Json, requirements: Json = None, frame: str = 'task', toast: bool = True, chat: bool = True, hidden: bool = False) -> 'AdvancementContext':
+        return self.category.advancement(name, icon, title, description, self.name, criteria, requirements, frame, toast, chat, hidden)
 
 
 def inventory_changed(*item_predicates: Json) -> Json:
     return {
         'trigger': 'minecraft:inventory_changed',
         'conditions': {
             'items': [utils.item_predicate(ip) for ip in item_predicates]
@@ -54,7 +65,29 @@
 def recipe_unlocked(recipe: ResourceIdentifier) -> Json:
     return {
         'trigger': 'minecraft:recipe_unlocked',
         'conditions': {
             'recipe': utils.resource_location(recipe).join()
         }
     }
+
+def enter_biome(biome: ResourceIdentifier) -> Json:
+    return {
+        'trigger': 'minecraft:location',
+        'conditions': {
+            'biome': utils.resource_location(biome).join()
+        }
+    }
+
+def first_tick() -> Json:
+    """
+    Granted when the player begins ticking in the world. Used for 'root' advancements.
+    """
+    return {'trigger': 'minecraft:tick'}
+
+def consume_item(item: str) -> Json:
+    return {
+        'trigger': 'minecraft:consume_item',
+        'conditions': {
+            'item': utils.item_predicate(item)
+        }
+    }
```

### Comparing `mcresources-1.5.9/mcresources/block_context.py` & `mcresources-1.6.0/mcresources/block_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  Part of mcresources by Alex O'Neill
 #  Work under copyright. Licensed under MIT
 #  For more information see the project LICENSE file
 
-from mcresources.type_definitions import Json, JsonObject, ResourceLocation
+from mcresources.type_definitions import Json, JsonObject, ResourceLocation, ResourceIdentifier
 from mcresources import utils, block_states
 
 from typing import Optional, Union, Dict, Sequence
 
 
 class BlockContext:
     """
@@ -69,14 +69,26 @@
         """
         if tag_name_parts is None:
             tag_name_parts = self.res
         tag_res = utils.resource_location(self.rm.domain, tag_name_parts)
         self.rm.block_tag(tag_res, self.res, replace=replace)
         return self
 
+    def with_item_tag(self, tag_name_parts: ResourceIdentifier = None, replace: bool = None) -> 'BlockContext':
+        """
+        Shortcut for {@link ResourceManager#item_tag}. Creates an item tag, assuming this block has an identically named item.
+        :param tag_name_parts: The resource location for the tag.
+        :param replace: If the tag should replace previous values
+        """
+        if tag_name_parts is None:
+            tag_name_parts = self.res
+        tag_res = utils.resource_location(self.rm.domain, tag_name_parts)
+        self.rm.item_tag(tag_res, self.res, replace=replace)
+        return self
+
     def with_lang(self, block_name: str, language: Optional[str] = None) -> 'BlockContext':
         """
         Shortcut for {@link ResourceManager#lang} using the block name
         """
         self.rm.lang(('block.%s.%s' % self.res).replace('/', '.'), block_name, language=language)
         return self
```

### Comparing `mcresources-1.5.9/mcresources/block_states.py` & `mcresources-1.6.0/mcresources/block_states.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.5.9/mcresources/item_context.py` & `mcresources-1.6.0/mcresources/item_context.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.5.9/mcresources/loot_tables.py` & `mcresources-1.6.0/mcresources/loot_tables.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,84 +23,80 @@
         'entries': entries,
         'conditions': conditions,
         'functions': functions,
         'rolls': rolls,
         'bonus_rolls': bonus_rolls
     }
 
-def alternatives(*entries: Json, conditions: Optional[Json] = None, functions: Optional[Json] = None) -> JsonObject:
-    return {
-        'type': 'minecraft:alternatives',
-        'children': entries,
-        'conditions': conditions,
-        'functions': functions
-    }
-
 
 # Loot Conditions
 
-def or_condition(*terms: Json) -> JsonObject:
+def all_of(*terms: Json) -> Json:
+    return {
+        'condition': 'minecraft:any_of',
+        'terms': utils.loot_conditions(terms)
+    }
+
+def any_of(*terms: Json) -> Json:
     return {
-        'condition': 'minecraft:alternative',
+        'condition': 'minecraft:all_of',
         'terms': utils.loot_conditions(terms)
     }
 
-def not_condition(term: Json) -> JsonObject:
+def inverted(term: Json) -> Json:
     condition = utils.loot_conditions(term)
-    assert len(condition) == 1, 'Expected one condition for not_condition() term'
+    assert len(condition) == 1, 'Expected one condition for inverted() term'
     return {
-        'condition': 'minecraft:not',
+        'condition': 'minecraft:inverted',
         'term': condition[0]
     }
 
-def random_chance(chance: float) -> JsonObject:
+def random_chance(chance: float) -> Json:
     return {
         'condition': 'minecraft:random_chance',
         'chance': chance
     }
 
-def block_state_property(data: Json) -> JsonObject:
+def block_state_property(data: Json) -> Json:
     """ Accepts a block like 'minecraft:grass[snowy=true]', or a dictionary with 'Name' and 'Properties' entries """
     block_state = utils.block_state(data)
     assert 'Name' in block_state, 'Missing Name'
     assert 'Properties' in block_state and len(block_state['Properties']) > 0, 'Requires at least one property'
     return {
         'condition': 'minecraft:block_state_property',
         'block': block_state['Name'],
         'properties': block_state['Properties']
     }
 
-def match_tag(tag: str) -> JsonObject:
+def match_tag(tag: str) -> Json:
     return {
         'condition': 'minecraft:match_tool',
         'predicate': {'tag': tag}
     }
 
-def silk_touch() -> JsonObject:
+def silk_touch() -> Json:
     return {
         'condition': 'minecraft:match_tool',
         'predicate': {
             'enchantments': [{
                 'enchantment': 'minecraft:silk_touch',
                 'levels': {'min': 1}
             }]
         }
     }
 
-def fortune_table(chances: Sequence[float]) -> JsonObject:
+def fortune_table(chances: Sequence[float]) -> Json:
     return {
         'condition': 'minecraft:table_bonus',
         'enchantment': 'minecraft:fortune',
         'chances': chances
     }
 
-def survives_explosion() -> JsonObject:
-    return {
-        'condition': 'minecraft:survives_explosion'
-    }
+def survives_explosion() -> Json:
+    return 'minecraft:survives_explosion'
 
 
 # Loot Functions
 
 def set_count(min_inclusive: int = 1, max_inclusive: int = -1) -> JsonObject:
     """ `minecraft:set_count` function """
     if max_inclusive == -1:
```

### Comparing `mcresources-1.5.9/mcresources/recipe_context.py` & `mcresources-1.6.0/mcresources/recipe_context.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.5.9/mcresources/resource_manager.py` & `mcresources-1.6.0/mcresources/resource_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,23 +26,25 @@
     # resource generation here
     rm.flush()  # call flush to finish any tag or lang files, see note below
     ```
 
     <strong>Important:</strong> When generating files such as tags or lang, the `ResourceManager` does not create the files every time `.tag()` or `.lang()` is invoked. Rather, it collects all values from all invocations, until a call to `.flush()` is made, which then writes all tag and lang files together.
     """
 
-    def __init__(self, domain: str = 'minecraft', resource_dir: Sequence[str] = ('src', 'main', 'resources'), indent: int = 2, default_language: str = 'en_us', on_error: Callable[[str, Exception], Any] = None):
+    def __init__(self, domain: str = 'minecraft', resource_dir: Sequence[str] = ('src', 'main', 'resources'), indent: int = 2, ensure_ascii: bool = False, default_language: str = 'en_us', on_error: Callable[[str, Exception], Any] = None):
         """
         Creates a new Resource Manager. This is the supplier for all resource creation calls.
         :param domain: the domain / mod id for current resources.
         :param indent: the indentation level for all generated json files
+        :param ensure_ascii: The ensure_ascii passed to json.dump - if non-ascii characters should be replaced with escape sequences.
         """
         self.resource_dir = utils.str_path(resource_dir)
         self.domain = domain
         self.indent = indent
+        self.ensure_ascii = ensure_ascii
         self.default_language = default_language
         self.on_error = on_error
 
         if self.on_error is None:
             self.on_error = lambda file, err: None  # Ignore errors
 
         # Internal buffers, used for tags and lang entries, which are all written at the same time
@@ -171,28 +173,34 @@
         res = utils.resource_location(self.domain, name_parts)
         self.write((*self.resource_dir, 'assets', res.domain, 'models', 'item', res.path), {
             'loader': utils.resource_location(loader).join(),
             **data
         })
         return ItemContext(self, res)
 
+    def atlas(self, name_parts: ResourceIdentifier, *sources: Json):
+        res = utils.resource_location(self.domain, name_parts)
+        self.write((*self.resource_dir, 'assets', res.domain, 'atlases', res.path), {
+            'sources': [s for s in sources]
+        })
+
     def crafting_shapeless(self, name_parts: ResourceIdentifier, ingredients: Json, result: Json, group: str = None, conditions: Optional[Json] = None) -> RecipeContext:
         """
         Creates a shapeless crafting recipe.
         :param name_parts: The resource location, including path elements.
         :param ingredients: The ingredients.
         :param result: The result of crafting the recipe.
         :param group: The group.
         :param conditions: Any conditions for the recipe to be enabled.
         """
         res = utils.resource_location(self.domain, name_parts)
         self.write((*self.resource_dir, 'data', res.domain, 'recipes', res.path), {
             'type': 'minecraft:crafting_shapeless',
             'group': group,
-            'ingredients': utils.item_stack_list(ingredients),
+            'ingredients': utils.ingredient_list(ingredients),
             'result': utils.item_stack(result),
             'conditions': utils.recipe_condition(conditions)
         })
         return RecipeContext(self, res)
 
     def crafting_shaped(self, name_parts: ResourceIdentifier, pattern: Sequence[str], ingredients: Json, result: Json, group: str = None, conditions: Optional[Json] = None) -> RecipeContext:
         """
@@ -200,14 +208,15 @@
         :param name_parts: The resource location, including path elements.
         :param pattern: The pattern for the recipe.
         :param ingredients: The ingredients, indexed by key in pattern.
         :param result: The result of crafting the recipe.
         :param group: The group.
         :param conditions: Any conditions for the recipe to be enabled.
         """
+        utils.validate_crafting_pattern(pattern)
         res = utils.resource_location(self.domain, name_parts)
         self.write((*self.resource_dir, 'data', res.domain, 'recipes', res.path), {
             'type': 'minecraft:crafting_shaped',
             'group': group,
             'pattern': pattern,
             'key': utils.item_stack_dict(ingredients, ''.join(pattern)[0]),
             'result': utils.item_stack(result),
@@ -247,85 +256,30 @@
     def advancement(self, name_parts: ResourceIdentifier, display: Json = None, parent: str = None, criteria: Dict[str, Dict[str, Json]] = None, requirements: Sequence[Sequence[str]] = None, rewards: Dict[str, Json] = None):
         """
         Creates a generic advancement. Performs basic filling in of data types
         :param name_parts: The resource location, including path elements.
         :param display: The display data. Inserted as is.
         :param parent: The parent advancement registry name
         :param criteria: The criteria for an advancement. Inserted as is.
-        :param requirements: The requirements. If None, will default to a list of all the requirements (OR'd together).
+        :param requirements: The requirements. If None or 'or', the criteria names will in one list. If 'and', the criteria will each get their own sublist, which requires all of them to be achieved.
         :param rewards: The rewards. Inserted as is.
         """
         res = utils.resource_location(self.domain, name_parts)
-        if requirements is None:
+        if requirements is None or requirements == 'or':
             requirements = [[k for k in criteria.keys()]]
+        elif requirements == 'and':
+            requirements = [[k] for k in criteria.keys()]
         self.write((*self.resource_dir, 'data', res.domain, 'advancements', res.path), {
             'parent': parent,
             'criteria': criteria,
             'display': display,
             'requirements': requirements,
             'rewards': rewards
         })
 
-    def tag(self, name_parts: ResourceIdentifier, root_domain: str, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
-        """
-        Creates or appends to a tag entry
-        :param name_parts: The resource location, including path elements.
-        :param root_domain: The root domain of the tag. Should be 'blocks', 'items', 'fluids', or 'entity_types', or a world generation folder.
-        :param values: The resource location values for the tag. Can specify optional tags by suffixing with `?`, i.e. `'minecraft:foo?'`. Can also accept explicit optional tags via a dictionary with `id` and `required`.
-        :param replace: If the tag should replace previous values
-        """
-        res = utils.resource_location(self.domain, name_parts)
-        values = [utils.tag_entry(v, self.domain) for v in values]
-        if res not in self.tags_buffer[root_domain]:
-            if replace is None:
-                replace = False
-            tag = Tag(replace)
-            tag.add_all(values)
-            self.tags_buffer[root_domain][res] = tag
-        else:
-            self.tags_buffer[root_domain][res].add_all(values)
-            if replace is not None:
-                self.tags_buffer[root_domain][res].replace = replace
-
-    def item_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
-        """
-        Creates or appends to an item tag
-        :param name_parts: The resource location, including path elements.
-        :param values:The resource location values for the tag. Can specify optional tags by suffixing with `?`, i.e. `'minecraft:foo?'`. Can also accept explicit optional tags via a dictionary with `id` and `required`.
-        :param replace: If the tag should replace previous values
-        """
-        self.tag(name_parts, 'items', *values, replace=replace)
-
-    def block_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
-        """
-        Creates or appends to a block tag
-        :param name_parts: The resource location, including path elements.
-        :param values: The resource location values for the tag. Can specify optional tags by suffixing with `?`, i.e. `'minecraft:foo?'`. Can also accept explicit optional tags via a dictionary with `id` and `required`.
-        :param replace: If the tag should replace previous values
-        """
-        self.tag(name_parts, 'blocks', *values, replace=replace)
-
-    def entity_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
-        """
-        Creates or appends to an entity tag
-        :param name_parts: The resource location, including path elements.
-        :param values: The resource location values for the tag. Can specify optional tags by suffixing with `?`, i.e. `'minecraft:foo?'`. Can also accept explicit optional tags via a dictionary with `id` and `required`.
-        :param replace: If the tag should replace previous values
-        """
-        self.tag(name_parts, 'entity_types', *values, replace=replace)
-
-    def fluid_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
-        """
-        Creates or appends to a fluid tag
-        :param name_parts: The resource location, including path elements.
-        :param values: The resource location values for the tag. Can specify optional tags by suffixing with `?`, i.e. `'minecraft:foo?'`. Can also accept explicit optional tags via a dictionary with `id` and `required`.
-        :param replace: If the tag should replace previous values
-        """
-        self.tag(name_parts, 'fluids', *values, replace=replace)
-
     def block_loot(self, name_parts: ResourceIdentifier, *loot_pools: Json) -> BlockContext:
         """
         Creates a loot table for a block
         :param name_parts: The resource location, including path elements.
         :param loot_pools: Loot pools. Each argument is interpreted as a single pool. Loot pools may be a single string (which will be expanded to a single default `minecraft:item` entry), or a dictionary, which will be expanded into either a single loot pool, or single loot entry based on context, or a sequence of loot entries, which will be expanded into a `minecraft:alternatives` loot entry, and loot pool.
         """
         res = self.loot(name_parts, *loot_pools, path='blocks', loot_type='minecraft:block')
@@ -486,22 +440,95 @@
             'processors': processors
         })
 
     def template_pool(self, name_parts: ResourceIdentifier, data: Json):
         res = utils.resource_location(self.domain, name_parts)
         self.write((*self.resource_dir, 'data', res.domain, 'worldgen', 'template_pool', res.path), data)
 
+    # === Tags === #
+
+    def item_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization for {@link #tag} for item tags. """
+        self.tag(name_parts, 'items', *values, replace=replace)
+
+    def block_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization for {@link #tag} for block tags. """
+        self.tag(name_parts, 'blocks', *values, replace=replace)
+
+    def block_and_item_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Calls both `.block_tag()` and `.item_tag()` with the same arguments. """
+        self.tag(name_parts, 'items', *values, replace=replace)
+        self.tag(name_parts, 'blocks', *values, replace=replace)
+
+    def entity_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization of {@link #tag} for entity tags. """
+        self.tag(name_parts, 'entity_types', *values, replace=replace)
+
+    def fluid_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization of {@link #tag} for fluid tags """
+        self.tag(name_parts, 'fluids', *values, replace=replace)
+
+    def dimension_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization of {@link #tag} for dimension tags """
+        self.tag(name_parts, 'dimension', *values, replace=replace)
+
+    def dimension_type_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization of {@link #tag} for dimension type tags """
+        self.tag(name_parts, 'dimension_type', *values, replace=replace)
+
+    def configured_carver_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization of {@link #tag} for configured carver tags """
+        self.tag(name_parts, 'worldgen/configured_carver', *values, replace=replace)
+
+    def configured_structure_feature_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization of {@link #tag} for configured structure feature tags """
+        self.tag(name_parts, 'worldgen/configured_structure_feature', *values, replace=replace)
+
+    def configured_feature_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization of {@link #tag} for configured feature tags """
+        self.tag(name_parts, 'worldgen/configured_feature', *values, replace=replace)
+
+    def placed_feature_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization of {@link #tag} for placed feature tags """
+        self.tag(name_parts, 'worldgen/placed_feature', *values, replace=replace)
+
+    def biome_tag(self, name_parts: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """ Specialization of {@link #tag} for biome tags """
+        self.tag(name_parts, 'worldgen/biome', *values, replace=replace)
+
+    def tag(self, name_parts: ResourceIdentifier, root_domain: ResourceIdentifier, *values: Union[ResourceIdentifier, JsonObject], replace: bool = None):
+        """
+        Creates or appends to a tag entry
+        :param name_parts: The resource location, including path elements.
+        :param root_domain: The root domain of the tag. Should be 'blocks', 'items', 'fluids', or 'entity_types', or a world generation folder.
+        :param values: The resource location values for the tag. Can specify optional tags by suffixing with `?`, i.e. `'minecraft:foo?'`. Can also accept explicit optional tags via a dictionary with `id` and `required`.
+        :param replace: If the tag should replace previous values
+        """
+        res = utils.resource_location(self.domain, name_parts)
+        values = [utils.tag_entry(v, self.domain) for v in values]
+        root = '/'.join(utils.str_path(root_domain))
+        if res not in self.tags_buffer[root]:
+            if replace is None:
+                replace = False
+            tag = Tag(replace)
+            tag.add_all(values)
+            self.tags_buffer[root][res] = tag
+        else:
+            self.tags_buffer[root][res].add_all(values)
+            if replace is not None:
+                self.tags_buffer[root][res].replace = replace
+
     def write(self, path_parts: Sequence[str], data: Json):
         """
         Writes data to a file, inserting an autogenerated comment and deletes None entries from the data
         :param path_parts: The path elements of the file
         :param data: The json data to write
         """
         data = utils.del_none({'__comment__': 'This file was automatically created by mcresources', **data})
-        flag = utils.write(path_parts, data, self.indent, self.on_error)
+        flag = utils.write(path_parts, data, self.indent, self.ensure_ascii, self.on_error)
         if flag == utils.WriteFlag.NEW:
             self.new_files += 1
         elif flag == utils.WriteFlag.MODIFIED:
             self.modified_files += 1
         elif flag == utils.WriteFlag.UNCHANGED:
             self.unchanged_files += 1
         elif flag == utils.WriteFlag.ERROR:
```

### Comparing `mcresources-1.5.9/mcresources/surface_rules.py` & `mcresources-1.6.0/mcresources/surface_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     }
 
 # Conditions
 
 def biome_condition(biomes: Sequence[ResourceIdentifier], then: JsonObject) -> JsonObject:
     return condition({
         'type': 'minecraft:biome',
-        'biome_is': [utils.resource_location(r).join() for r in utils.str_list(biomes)]
+        'biome_is': [utils.resource_location(r).join() for r in biomes]
     }, then)
 
 def noise_threshold_condition(noise: ResourceIdentifier, min_value: float, max_value: float, then: JsonObject) -> JsonObject:
     return condition({
         'type': 'minecraft:noise_threshold',
         'noise': utils.resource_location(noise).join(),
         'min_threshold': min_value,
```

### Comparing `mcresources-1.5.9/mcresources/tag.py` & `mcresources-1.6.0/mcresources/tag.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.5.9/mcresources/type_definitions.py` & `mcresources-1.6.0/mcresources/type_definitions.py`

 * *Files identical despite different names*

### Comparing `mcresources-1.5.9/mcresources/utils.py` & `mcresources-1.6.0/mcresources/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,35 +51,36 @@
         return [del_none(p) for p in data_in if p is not None]
     elif data_in is not None:
         return data_in
     else:
         raise ValueError('None passed to `del_none`, should not be possible.')
 
 
-def write(path_parts: Sequence[str], data: Json, indent: int = 2, on_error: Callable[[str, Exception], Any] = None) -> WriteFlag:
+def write(path_parts: Sequence[str], data: Json, indent: int = 2, ensure_ascii: bool = False, on_error: Callable[[str, Exception], Any] = None) -> WriteFlag:
     """
     Writes json to a file.
     :param path_parts: The path elements of the file
     :param data: The data to write
     :param indent: The indent level for the json output
+    :param ensure_ascii: The ensure_ascii passed to json.dump - if non-ascii characters should be replaced with escape sequences.
     :param on_error: A consumer of a file name and error if one occurs
     :return: 0 if the file was new, 1 if the file was modified, 2 if the file was not modified, 3 if an error occurred
     """
     path = os.path.join(*path_parts) + '.json'
     try:
         os.makedirs(os.path.dirname(path), exist_ok=True)
         exists = False
         if os.path.isfile(path):
             with open(path, 'r', encoding='utf-8') as file:
                 old_data = json.load(file)
             if old_data == data:
                 return WriteFlag.UNCHANGED
             exists = True
         with open(path, 'w', encoding='utf-8') as file:
-            json.dump(data, file, indent=indent)
+            json.dump(data, file, indent=indent, ensure_ascii=ensure_ascii)
             return WriteFlag.MODIFIED if exists else WriteFlag.NEW
     except Exception as e:
         on_error(path, e)
         return WriteFlag.ERROR
 
 
 def resource_location(*elements: ResourceIdentifier) -> ResourceLocation:
@@ -115,24 +116,14 @@
         return [s for s in data_in.split('/')]
     elif isinstance(data_in, Sequence):
         return [*flatten_list([str_path(s) for s in data_in])]
     else:
         raise ValueError('Unknown object %s at str_path' % str(data_in))
 
 
-def str_list(data_in: Sequence[str]) -> List[str]:
-    # Converts an iterable or string to a string list
-    if isinstance(data_in, str):
-        return [data_in]
-    elif isinstance(data_in, Sequence):
-        return [*flatten_list(data_in)]
-    else:
-        raise ValueError('Unknown object %s at str_list' % str(data_in))
-
-
 def domain_path_parts(name_parts: Sequence[str], default_domain: str) -> Tuple[str, List[str]]:
     joined = '/'.join(str_path(name_parts))
     if ':' in joined:
         i = joined.index(':')
         return joined[:i], joined[i + 1:].split('/')
     else:
         return default_domain, str_path(joined)
@@ -232,14 +223,23 @@
         if count:
             d['count'] = count
         return d
     else:
         raise ValueError('Unknown object %s at item_stack' % str(data_in))
 
 
+def ingredient_list(data_in: Json) -> List[JsonObject]:
+    if isinstance(data_in, str) or isinstance(data_in, Dict):
+        return [ingredient(data_in)]
+    elif is_sequence(data_in):  # Treat a top-level sequence without flattening
+        return [ingredient(s) for s in data_in]
+    else:
+        raise ValueError('Unknown object %s at ingredient_list' % str(data_in))
+
+
 def item_stack_list(data_in: Json) -> List[JsonObject]:
     if isinstance(data_in, str) or isinstance(data_in, Dict):
         return [item_stack(data_in)]
     elif is_sequence(data_in):
         return [*flatten_list([item_stack(s) for s in data_in])]
     else:
         raise ValueError('Unknown object %s at item_stack_list' % str(data_in))
@@ -566,7 +566,20 @@
         if 'Name' not in data:
             raise ValueError('Missing \'Name\' key in block_state for object %s' % str(data))
         if 'Properties' not in data:
             data['Properties'] = {}
         return data
     else:
         raise ValueError('Unknown object %s at block_state' % str(data))
+    
+def validate_crafting_pattern(pattern: Sequence[str], max_width: int = 3, max_height: int = 3):
+    height = len(pattern)
+    if height > max_height or height == 0:
+        raise ValueError('Pattern must be 1-%s lines long, found %s' % (max_height, height))
+    length = -1
+    for sequence in pattern:
+        if length == -1:
+            length = len(sequence)
+        elif length != len(sequence):
+            raise ValueError('Pattern must be square: %s. Expected: %s, Found: %s' % (pattern, length, len(sequence)))
+        elif length > max_width:
+            raise ValueError('Pattern must be 1-%s characters wide, found %s' % (max_width, length))
```

### Comparing `mcresources-1.5.9/mcresources.egg-info/PKG-INFO` & `mcresources-1.6.0/mcresources.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: mcresources
-Version: 1.5.9
+Version: 1.6.0
 Summary: A Python Data Generator for Minecraft Modding
 Home-page: https://github.com/alcatrazEscapee/mcresources
 Author: Alex O'Neill
 Author-email: alex@molleroneill.com
 License: MIT
 Keywords: python,minecraft,resources,modding,forge
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Minecraft Resource Generator
 
 This is a python module aimed to enable simple generation of the many json files that are required for Minecraft modding.
 
-### Pack Format
+### Data Format
 
-Updates of this tool will track the latest pack format (`pack_format` in a resource pack) as soon as possible. In order to generate resources compliant with a specific pack format, the latest version can be found below
+Updates of this tool will track the format of the latest version of Minecraft. For each specific Minecraft version, the latest version of `mcresources`, targeting that version, can be found below:
 
-Pack Format | Minimum Minecraft Version | Latest mcresources Version
----|---|---
-8 | 1.18 | Latest
-7 | 1.17 | 1.4.6
-6 | 1.16.2 | 1.4.6
-5 | 1.15 | 1.3.3
-4 | 1.13 | 0.0.2
+| Minecraft Version | Latest mcresources Version |
+|-------------------|----------------------------|
+| 1.20              | Latest                     |
+| 1.18              | 1.5.11                     |
+| 1.17              | 1.4.6                      |
+| 1.16.2            | 1.4.6                      |
+| 1.15              | 1.3.3                      |
+| 1.13              | 0.0.2                      |
 
 ---
 
 ### [Documentation](https://github.com/alcatrazEscapee/mcresources/wiki)
 
 The wiki (link above) is generated from the methods and docstring comments of the library itself using `./docs.py`, and will always be up-to-date with the latest version of the library.
-
```

### Comparing `mcresources-1.5.9/setup.py` & `mcresources-1.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alex O\'Neill',
     author_email='alex@molleroneill.com',
     url='https://github.com/alcatrazEscapee/mcresources',
     keywords=['python', 'minecraft', 'resources', 'modding', 'forge'],
     install_requires=[],
+    package_data={"pixelmatch": ["py.typed"]},
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',  # Define that your audience are developers
         'License :: OSI Approved :: MIT License',  # Again, pick a license
         'Programming Language :: Python :: 3.7',
     ],
```

