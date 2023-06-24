# Comparing `tmp/dronefly_discord-0.1.1.dev2.tar.gz` & `tmp/dronefly_discord-0.1.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_discord-0.1.1.dev2.tar", max compression
+gzip compressed data, was "dronefly_discord-0.1.1.dev3.tar", max compression
```

## Comparing `dronefly_discord-0.1.1.dev2.tar` & `dronefly_discord-0.1.1.dev3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    56697 2023-04-22 11:51:53.202527 dronefly_discord-0.1.1.dev2/LICENSE
--rw-r--r--   0        0        0      916 2023-04-22 11:51:09.749659 dronefly_discord-0.1.1.dev2/README.md
--rw-r--r--   0        0        0        0 2023-04-22 12:15:11.202522 dronefly_discord-0.1.1.dev2/dronefly/discord/__init__.py
--rw-r--r--   0        0        0     3500 2023-06-18 10:38:56.459872 dronefly_discord-0.1.1.dev2/dronefly/discord/embeds.py
--rw-r--r--   0        0        0      722 2023-06-18 12:36:18.677638 dronefly_discord-0.1.1.dev2/pyproject.toml
--rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev2/setup.py
--rw-r--r--   0        0        0     1648 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0    56697 2023-04-22 11:51:53.202527 dronefly_discord-0.1.1.dev3/LICENSE
+-rw-r--r--   0        0        0      916 2023-04-22 11:51:09.749659 dronefly_discord-0.1.1.dev3/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 12:15:11.202522 dronefly_discord-0.1.1.dev3/dronefly/discord/__init__.py
+-rw-r--r--   0        0        0     3500 2023-06-18 10:38:56.459872 dronefly_discord-0.1.1.dev3/dronefly/discord/embeds.py
+-rw-r--r--   0        0        0      728 2023-06-24 10:03:25.599385 dronefly_discord-0.1.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev3/setup.py
+-rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev3/PKG-INFO
```

### Comparing `dronefly_discord-0.1.1.dev2/LICENSE` & `dronefly_discord-0.1.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_discord-0.1.1.dev2/README.md` & `dronefly_discord-0.1.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_discord-0.1.1.dev2/dronefly/discord/embeds.py` & `dronefly_discord-0.1.1.dev3/dronefly/discord/embeds.py`

 * *Files identical despite different names*

### Comparing `dronefly_discord-0.1.1.dev2/pyproject.toml` & `dronefly_discord-0.1.1.dev3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 max-line-length = 100
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.poetry]
 name = "dronefly-discord"
-version = "0.1.1.dev2"
+version = "0.1.1.dev3"
 description = "Dronefly Discord library"
 authors = ["Ben Armstrong <synrg@debian.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
         { include = "dronefly/discord" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 pyinaturalist = ">=0.19.0.dev2,<0.20"
 inflect = "^5.3.0"
-discord-py = "^2.2.3"
-dronefly-core = "^0.3.6.dev2"
+discord-py = "^2.2.0"
+dronefly-core = ">=0.3.6.dev5,<0.4"
 
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
 pytest = "^7.2.1"
 pytest-mock = "^3.10.0"
 pylint = "^2.10.2"
 pytest-asyncio = "^0.20.3"
```

### Comparing `dronefly_discord-0.1.1.dev2/setup.py` & `dronefly_discord-0.1.1.dev3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['discord']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['discord-py>=2.2.3,<3.0.0',
- 'dronefly-core>=0.3.6.dev2,<0.4.0',
+['discord-py>=2.2.0,<3.0.0',
+ 'dronefly-core>=0.3.6.dev5,<0.4',
  'inflect>=5.3.0,<6.0.0',
  'pyinaturalist>=0.19.0.dev2,<0.20']
 
 setup_kwargs = {
     'name': 'dronefly-discord',
-    'version': '0.1.1.dev2',
+    'version': '0.1.1.dev3',
     'description': 'Dronefly Discord library',
     'long_description': "# Dronefly Discord\n\nThis library will support writing Discord cogs based on\n[dronefly-core](https://github.com/dronefly-garden/dronefly-core). It is\nderived from the Discord-specific code extracted from the original\n[Dronefly](https://dronefly.readthedocs.io) bot codebase. We aim to keep\nthe library general enough to work with any bot based on\n[discord.py](https://discordpy.readthedocs.io), as well as on bots using\nthe [Red-DiscordBot](https://docs.discord.red) framework.\n\n# Related packages\n\n## Dronefly core\n\nThe [dronefly-core](https://github.com/dronefly-garden/dronefly-core)\npackage is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io/)\nDiscord bot's core components.\n\n## Dronefly Discord bot\n\nDronefly Discord bot brings [iNaturalist](https://www.inaturalist.org) taxa,\nobservations, and other data from the site into conversations on the\n[Discord](https://discord.com) chat platform.\n",
     'author': 'Ben Armstrong',
     'author_email': 'synrg@debian.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dronefly_discord-0.1.1.dev2/PKG-INFO` & `dronefly_discord-0.1.1.dev3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dronefly-discord
-Version: 0.1.1.dev2
+Version: 0.1.1.dev3
 Summary: Dronefly Discord library
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: discord-py (>=2.2.3,<3.0.0)
-Requires-Dist: dronefly-core (>=0.3.6.dev2,<0.4.0)
+Requires-Dist: discord-py (>=2.2.0,<3.0.0)
+Requires-Dist: dronefly-core (>=0.3.6.dev5,<0.4)
 Requires-Dist: inflect (>=5.3.0,<6.0.0)
 Requires-Dist: pyinaturalist (>=0.19.0.dev2,<0.20)
 Description-Content-Type: text/markdown
 
 # Dronefly Discord
 
 This library will support writing Discord cogs based on
```

