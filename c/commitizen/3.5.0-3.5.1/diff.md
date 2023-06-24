# Comparing `tmp/commitizen-3.5.0.tar.gz` & `tmp/commitizen-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.5.0.tar", max compression
+gzip compressed data, was "commitizen-3.5.1.tar", max compression
```

## Comparing `commitizen-3.5.0.tar` & `commitizen-3.5.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-06-23 09:44:24.137200 commitizen-3.5.0/LICENSE
--rw-r--r--   0        0        0      609 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/__version__.py
--rw-r--r--   0        0        0     4609 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/bump.py
--rw-r--r--   0        0        0    11712 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/changelog.py
--rw-r--r--   0        0        0     3455 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    17750 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-06-23 09:44:24.137200 commitizen-3.5.0/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    14245 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7142 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5075 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/check.py
--rw-r--r--   0        0        0     3435 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/info.py
--rw-r--r--   0        0        0    12966 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/commands/version.py
--rw-r--r--   0        0        0     1235 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/config/__init__.py
--rw-r--r--   0        0        0      898 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1568 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1746 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1431 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1213 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2983 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7070 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      287 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3176 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/defaults.py
--rw-r--r--   0        0        0     4706 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/factory.py
--rw-r--r--   0        0        0     6900 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/out.py
--rw-r--r--   0        0        0     7109 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     9732 2023-06-23 09:44:24.141200 commitizen-3.5.0/commitizen/version_schemes.py
--rw-r--r--   0        0        0     5750 2023-06-23 09:44:24.141200 commitizen-3.5.0/docs/README.md
--rw-r--r--   0        0        0     4200 2023-06-23 09:44:24.153200 commitizen-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-24 07:23:15.343195 commitizen-3.5.1/LICENSE
+-rw-r--r--   0        0        0      609 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/__version__.py
+-rw-r--r--   0        0        0     4609 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/bump.py
+-rw-r--r--   0        0        0    12112 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/changelog.py
+-rw-r--r--   0        0        0     3455 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    17750 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    14245 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7145 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5075 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3435 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12966 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1235 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1568 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1746 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1431 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1213 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2983 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7070 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      287 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3176 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/defaults.py
+-rw-r--r--   0        0        0     4706 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/factory.py
+-rw-r--r--   0        0        0     7295 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/out.py
+-rw-r--r--   0        0        0     7109 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     9732 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/version_schemes.py
+-rw-r--r--   0        0        0     5750 2023-06-24 07:23:15.343195 commitizen-3.5.1/docs/README.md
+-rw-r--r--   0        0        0     4290 2023-06-24 07:23:15.355195 commitizen-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.5.1/PKG-INFO
```

### Comparing `commitizen-3.5.0/LICENSE` & `commitizen-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/__init__.py` & `commitizen-3.5.1/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/bump.py` & `commitizen-3.5.1/commitizen/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/changelog.py` & `commitizen-3.5.1/commitizen/changelog.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,22 +26,28 @@
 """
 from __future__ import annotations
 
 import os
 import re
 from collections import OrderedDict, defaultdict
 from datetime import date
-from typing import TYPE_CHECKING, Callable, Iterable, cast
+from typing import TYPE_CHECKING, Callable, Iterable, Type, cast
 
 from jinja2 import Environment, PackageLoader
 
+from commitizen import out
 from commitizen.bump import normalize_tag
 from commitizen.exceptions import InvalidConfigurationError, NoCommitsFoundError
 from commitizen.git import GitCommit, GitTag
-from commitizen.version_schemes import DEFAULT_SCHEME, Pep440, InvalidVersion
+from commitizen.version_schemes import (
+    DEFAULT_SCHEME,
+    BaseVersion,
+    InvalidVersion,
+    Pep440,
+)
 
 if TYPE_CHECKING:
     from commitizen.version_schemes import VersionScheme
 
 
 def get_commit_tag(commit: GitCommit, tags: list[GitTag]) -> GitTag | None:
     return next((tag for tag in tags if tag.rev == commit.rev), None)
@@ -63,14 +69,27 @@
 
     if merge_prerelease and version.is_prerelease:
         return False
 
     return True
 
 
+def get_version_tags(scheme: Type[BaseVersion], tags: list[GitTag]) -> list[GitTag]:
+    valid_tags: list[GitTag] = []
+    for tag in tags:
+        try:
+            scheme(tag.name)
+        except InvalidVersion:
+            out.warn(f"InvalidVersion {tag}")
+        else:
+            valid_tags.append(tag)
+
+    return valid_tags
+
+
 def generate_tree_from_commits(
     commits: list[GitCommit],
     tags: list[GitTag],
     commit_parser: str,
     changelog_pattern: str,
     unreleased_version: str | None = None,
     change_type_map: dict[str, str] | None = None,
```

### Comparing `commitizen-3.5.0/commitizen/changelog_parser.py` & `commitizen-3.5.1/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/cli.py` & `commitizen-3.5.1/commitizen/cli.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/cmd.py` & `commitizen-3.5.1/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/commands/bump.py` & `commitizen-3.5.1/commitizen/commands/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/commands/changelog.py` & `commitizen-3.5.1/commitizen/commands/changelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,20 +133,17 @@
 
         if self.incremental and self.rev_range:
             raise NotAllowed("--incremental cannot be combined with a rev_range")
 
         # Don't continue if no `file_name` specified.
         assert self.file_name
 
-        tags = git.get_tags()
-        if not tags:
-            tags = []
+        tags = changelog.get_version_tags(self.scheme, git.get_tags()) or []
 
         end_rev = ""
-
         if self.incremental:
             changelog_meta = changelog.get_metadata(self.file_name, self.scheme)
             latest_version = changelog_meta.get("latest_version")
             if latest_version:
                 latest_tag_version: str = bump.normalize_tag(
                     latest_version,
                     tag_format=self.tag_format,
```

### Comparing `commitizen-3.5.0/commitizen/commands/check.py` & `commitizen-3.5.1/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/commands/commit.py` & `commitizen-3.5.1/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/commands/init.py` & `commitizen-3.5.1/commitizen/commands/init.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/commands/version.py` & `commitizen-3.5.1/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/config/__init__.py` & `commitizen-3.5.1/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/config/base_config.py` & `commitizen-3.5.1/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/config/json_config.py` & `commitizen-3.5.1/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/config/toml_config.py` & `commitizen-3.5.1/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/config/yaml_config.py` & `commitizen-3.5.1/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/cz/__init__.py` & `commitizen-3.5.1/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/cz/base.py` & `commitizen-3.5.1/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.5.1/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.5.1/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/cz/customize/customize.py` & `commitizen-3.5.1/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/cz/jira/jira.py` & `commitizen-3.5.1/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/cz/jira/jira_info.txt` & `commitizen-3.5.1/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/defaults.py` & `commitizen-3.5.1/commitizen/defaults.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/exceptions.py` & `commitizen-3.5.1/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/factory.py` & `commitizen-3.5.1/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/git.py` & `commitizen-3.5.1/commitizen/git.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,19 +88,30 @@
         _opt = f"-a {tag} -m"
     if signed:
         _opt = f"-s {tag} -m"
     c = cmd.run(f"git tag {_opt} {tag}")
     return c
 
 
-def commit(message: str, args: str = "") -> cmd.Command:
+def commit(
+    message: str, args: str = "", committer_date: str | None = None
+) -> cmd.Command:
     f = NamedTemporaryFile("wb", delete=False)
     f.write(message.encode("utf-8"))
     f.close()
-    c = cmd.run(f"git commit {args} -F {f.name}")
+
+    command = f"git commit {args} -F {f.name}"
+
+    if committer_date and os.name == "nt":  # pragma: no cover
+        # Using `cmd /v /c "{command}"` sets environment variables only for that command
+        command = f'cmd /v /c "set GIT_COMMITTER_DATE={committer_date}&& {command}"'
+    elif committer_date:
+        command = f"GIT_COMMITTER_DATE={committer_date} {command}"
+
+    c = cmd.run(command)
     os.unlink(f.name)
     return c
 
 
 def get_commits(
     start: str | None = None,
     end: str = "HEAD",
```

### Comparing `commitizen-3.5.0/commitizen/hooks.py` & `commitizen-3.5.1/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/out.py` & `commitizen-3.5.1/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/providers.py` & `commitizen-3.5.1/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/commitizen/version_schemes.py` & `commitizen-3.5.1/commitizen/version_schemes.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/docs/README.md` & `commitizen-3.5.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.0/pyproject.toml` & `commitizen-3.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.5.0"
+version = "3.5.1"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.5.0"
+version = "3.5.1"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
@@ -65,14 +65,17 @@
 pre-commit = "^2.18.0"
 mypy = "^1.4"
 types-PyYAML = "^5.4.3"
 types-termcolor = "^0.1.1"
 # documentation
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.6"
+deprecated = "^1.2.13"
+types-deprecated = "^1.2.9.2"
+types-python-dateutil = "^2.8.19.13"
 
 
 [tool.poetry.scripts]
 cz = "commitizen.cli:main"
 git-cz = "commitizen.cli:main"
 
 [tool.poetry.plugins."commitizen.plugin"]
```

### Comparing `commitizen-3.5.0/PKG-INFO` & `commitizen-3.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.5.0
+Version: 3.5.1
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
```

