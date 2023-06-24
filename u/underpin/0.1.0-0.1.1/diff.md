# Comparing `tmp/underpin-0.1.0.tar.gz` & `tmp/underpin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "underpin-0.1.0.tar", max compression
+gzip compressed data, was "underpin-0.1.1.tar", max compression
```

## Comparing `underpin-0.1.0.tar` & `underpin-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     5249 2023-06-23 18:55:48.347419 underpin-0.1.0/README.md
--rw-r--r--   0        0        0      634 2023-06-24 17:38:53.871627 underpin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      188 2023-06-22 02:29:29.669100 underpin-0.1.0/underpin/__init__.py
--rw-r--r--   0        0        0     4807 2023-06-24 00:05:27.998436 underpin-0.1.0/underpin/__main__.py
--rw-r--r--   0        0        0        0 2023-06-19 12:50:03.485800 underpin-0.1.0/underpin/ai/model.py
--rw-r--r--   0        0        0     1328 2023-06-24 03:48:49.474949 underpin-0.1.0/underpin/config.py
--rw-r--r--   0        0        0        0 2023-06-20 22:47:20.939127 underpin-0.1.0/underpin/pipeline/__init__.py
--rw-r--r--   0        0        0     1433 2023-06-23 01:47:02.446887 underpin-0.1.0/underpin/pipeline/default.py
--rw-r--r--   0        0        0      425 2023-06-21 02:44:49.044800 underpin-0.1.0/underpin/schema/ChangeSet.py
--rw-r--r--   0        0        0       32 2023-06-21 11:12:05.687373 underpin-0.1.0/underpin/schema/__init__.py
--rw-r--r--   0        0        0        2 2023-06-21 10:31:27.006880 underpin-0.1.0/underpin/schema/common.py
--rw-r--r--   0        0        0        0 2023-06-19 12:46:41.715073 underpin-0.1.0/underpin/setup.py
--rw-r--r--   0        0        0     5896 2023-06-24 17:30:50.918085 underpin-0.1.0/underpin/templates/UnderpinTemplate.py
--rw-r--r--   0        0        0      212 2023-06-23 01:25:27.413799 underpin-0.1.0/underpin/templates/__init__.py
--rw-r--r--   0        0        0      996 2023-06-23 23:35:03.076115 underpin-0.1.0/underpin/templates/template_containers.py
--rw-r--r--   0        0        0     1927 2023-06-23 23:31:19.123321 underpin-0.1.0/underpin/templates/template_yaml.py
--rw-r--r--   0        0        0       65 2023-06-23 18:39:36.198580 underpin-0.1.0/underpin/utils/__init__.py
--rw-r--r--   0        0        0     1552 2023-06-24 12:27:34.207003 underpin-0.1.0/underpin/utils/funcs.py
--rw-r--r--   0        0        0     5931 2023-06-23 23:47:28.252790 underpin-0.1.0/underpin/utils/git/GitContext.py
--rw-r--r--   0        0        0     6923 2023-06-22 02:29:29.670561 underpin-0.1.0/underpin/utils/git/__init__.py
--rw-r--r--   0        0        0      820 2023-06-23 11:16:03.325554 underpin-0.1.0/underpin/utils/io/__init__.py
--rw-r--r--   0        0        0     5849 1970-01-01 00:00:00.000000 underpin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5249 2023-06-23 18:55:48.347419 underpin-0.1.1/README.md
+-rw-r--r--   0        0        0      634 2023-06-24 18:43:33.407167 underpin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      241 2023-06-24 18:37:51.805665 underpin-0.1.1/underpin/__init__.py
+-rw-r--r--   0        0        0     4903 2023-06-24 18:40:18.954022 underpin-0.1.1/underpin/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:50:03.485800 underpin-0.1.1/underpin/ai/model.py
+-rw-r--r--   0        0        0     1970 2023-06-24 18:42:04.030347 underpin-0.1.1/underpin/config.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:47:20.939127 underpin-0.1.1/underpin/pipeline/__init__.py
+-rw-r--r--   0        0        0     1433 2023-06-23 01:47:02.446887 underpin-0.1.1/underpin/pipeline/default.py
+-rw-r--r--   0        0        0      425 2023-06-21 02:44:49.044800 underpin-0.1.1/underpin/schema/ChangeSet.py
+-rw-r--r--   0        0        0       32 2023-06-21 11:12:05.687373 underpin-0.1.1/underpin/schema/__init__.py
+-rw-r--r--   0        0        0        2 2023-06-21 10:31:27.006880 underpin-0.1.1/underpin/schema/common.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:46:41.715073 underpin-0.1.1/underpin/setup.py
+-rw-r--r--   0        0        0     5896 2023-06-24 17:30:50.918085 underpin-0.1.1/underpin/templates/UnderpinTemplate.py
+-rw-r--r--   0        0        0      212 2023-06-23 01:25:27.413799 underpin-0.1.1/underpin/templates/__init__.py
+-rw-r--r--   0        0        0      996 2023-06-23 23:35:03.076115 underpin-0.1.1/underpin/templates/template_containers.py
+-rw-r--r--   0        0        0     1927 2023-06-23 23:31:19.123321 underpin-0.1.1/underpin/templates/template_yaml.py
+-rw-r--r--   0        0        0       65 2023-06-23 18:39:36.198580 underpin-0.1.1/underpin/utils/__init__.py
+-rw-r--r--   0        0        0     1552 2023-06-24 12:27:34.207003 underpin-0.1.1/underpin/utils/funcs.py
+-rw-r--r--   0        0        0     5931 2023-06-23 23:47:28.252790 underpin-0.1.1/underpin/utils/git/GitContext.py
+-rw-r--r--   0        0        0     6923 2023-06-22 02:29:29.670561 underpin-0.1.1/underpin/utils/git/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-23 11:16:03.325554 underpin-0.1.1/underpin/utils/io/__init__.py
+-rw-r--r--   0        0        0     5849 1970-01-01 00:00:00.000000 underpin-0.1.1/PKG-INFO
```

### Comparing `underpin-0.1.0/README.md` & `underpin-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `underpin-0.1.0/pyproject.toml` & `underpin-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "underpin"
-version = "0.1.0"
+version = "0.1.1"
 description = "tools for sending app modules to k8s infrastructure and managing app versions"
 authors = ["mr-saoirse <amartey@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `underpin-0.1.0/underpin/__main__.py` & `underpin-0.1.1/underpin/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from underpin.config import UnderpinConfig
 from underpin.pipeline.default import DefaultPipeline
 from underpin.utils import io
 from underpin import schema
 from underpin.utils.git import GitContext, app_changes
 from underpin.schema import ChangeSet
-from underpin import logger, UNDERPIN_GIT_ROOT
+from underpin import logger, UNDERPIN_GIT_ROOT, CONFIG_HOME
 from underpin.utils.io import run_command
 from underpin.utils import generate_markdown_table
 
 app = typer.Typer()
 
 template_app = typer.Typer()
 app.add_typer(template_app, name="template")
@@ -25,27 +25,27 @@
 
 
 @build_app.command("containers")
 def build_app_containers(
     config_file: Optional[str] = typer.Option(None, "--config", "-c"),
     dir: Optional[str] = typer.Option(None, "--dir", "-d"),
 ):
-    config = UnderpinConfig(config_file or "config/config.yaml")
+    config = UnderpinConfig(config_file or CONFIG_HOME)
 
     # iterate app actions or use just one app if dir is specified
 
     #
 
 
 @build_app.command("kustomize")
 def build_app_update(
     config_file: Optional[str] = typer.Option(None, "--config", "-c"),
     dir: Optional[str] = typer.Option(None, "--dir", "-d"),
 ):
-    config = UnderpinConfig(config_file or "config/config.yaml")
+    config = UnderpinConfig(config_file or CONFIG_HOME)
 
     target = GitContext(config.target_repo, cwd=UNDERPIN_GIT_ROOT)
     changes = target.get_changes()
     logger.info(changes)
 
     # not sure if we need this - can we tag with the image we are going to build and be done it
     # iterate app actions or use just one app if dir is specified
@@ -59,15 +59,15 @@
     pins: Optional[str] = typer.Option(None, "--pinnings", "-p"),
 ):
     """
     we can provide a config source for how the image tags are to be updated
     run kustomize on all
     and commit the repo
     """
-    config = UnderpinConfig(config_file or "config/config.yaml")
+    config = UnderpinConfig(config_file or CONFIG_HOME)
 
     # templates.update_images(pins)
 
     # get the underpin report which will also be archived somewhere
     app_actions = []
 
     target = GitContext(config.target_repo, cwd=UNDERPIN_GIT_ROOT)
@@ -92,15 +92,19 @@
     """
     underpin generates a target repo away from the current repo to write files into and commit
     the target branch can be auto-generated with a hash in practice
     """
 
     # TODO: if branch exists handle this case properly
 
-    config = UnderpinConfig("config/config.yaml")
+    print(CONFIG_HOME, Path(CONFIG_HOME).is_file())
+    if not Path(CONFIG_HOME).is_file():
+        UnderpinConfig.configure()
+
+    config = UnderpinConfig(CONFIG_HOME)
     target_branch = target_branch or "bot.add_manifests"
     logger.info(config._data)
 
     with GitContext(config.target_repo, cwd=UNDERPIN_GIT_ROOT) as g:
         g.create_branch(target_branch)
         logger.info(f"create target repo to {g}")
         # if we need to do anything to the target we can here
@@ -113,15 +117,15 @@
     config_file: Optional[str] = typer.Option(None, "--config", "-c"),
 ):
     """
     we can get a change set from input or the branch and process all apps
     a config file can be passed in order used from the one in the module
     sha hash is used for the entire build context
     """
-    config = UnderpinConfig(config_file or "config/config.yaml")
+    config = UnderpinConfig(config_file or CONFIG_HOME)
     """
     the default pipeline could be swapped for other pipelines in future 
     but it may be we only need one pipeline and managed templates
     """
     pipeline = DefaultPipeline(config)
 
     target = GitContext(config.target_repo, cwd=UNDERPIN_GIT_ROOT)
```

### Comparing `underpin-0.1.0/underpin/pipeline/default.py` & `underpin-0.1.1/underpin/pipeline/default.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.0/underpin/templates/UnderpinTemplate.py` & `underpin-0.1.1/underpin/templates/UnderpinTemplate.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.0/underpin/templates/template_containers.py` & `underpin-0.1.1/underpin/templates/template_containers.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.0/underpin/templates/template_yaml.py` & `underpin-0.1.1/underpin/templates/template_yaml.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.0/underpin/utils/funcs.py` & `underpin-0.1.1/underpin/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.0/underpin/utils/git/GitContext.py` & `underpin-0.1.1/underpin/utils/git/GitContext.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.0/underpin/utils/git/__init__.py` & `underpin-0.1.1/underpin/utils/git/__init__.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.0/underpin/utils/io/__init__.py` & `underpin-0.1.1/underpin/utils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.0/PKG-INFO` & `underpin-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: underpin
-Version: 0.1.0
+Version: 0.1.1
 Summary: tools for sending app modules to k8s infrastructure and managing app versions
 License: MIT
 Author: mr-saoirse
 Author-email: amartey@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

