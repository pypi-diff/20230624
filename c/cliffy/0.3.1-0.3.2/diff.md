# Comparing `tmp/cliffy-0.3.1.tar.gz` & `tmp/cliffy-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliffy-0.3.1.tar", max compression
+gzip compressed data, was "cliffy-0.3.2.tar", max compression
```

## Comparing `cliffy-0.3.1.tar` & `cliffy-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1060 2023-06-13 02:27:07.090176 cliffy-0.3.1/LICENSE
--rw-r--r--   0        0        0     6810 2023-06-13 02:27:07.090176 cliffy-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/__init__.py
--rw-r--r--   0        0        0       97 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/__main__.py
--rw-r--r--   0        0        0     1859 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/builder.py
--rw-r--r--   0        0        0     8076 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/cli.py
--rw-r--r--   0        0        0        0 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/clis/__init__.py
--rw-r--r--   0        0        0     6461 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/commander.py
--rw-r--r--   0        0        0        0 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/commanders/__init__.py
--rw-r--r--   0        0        0      981 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/commanders/click.py
--rw-r--r--   0        0        0     1976 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/commanders/typer.py
--rw-r--r--   0        0        0     3735 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/helper.py
--rw-r--r--   0        0        0     3036 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/homer.py
--rw-r--r--   0        0        0     1392 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/loader.py
--rw-r--r--   0        0        0      396 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/manifests/__init__.py
--rw-r--r--   0        0        0     7356 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/manifests/v1.py
--rw-r--r--   0        0        0      137 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/merger.py
--rw-r--r--   0        0        0     4663 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/parser.py
--rw-r--r--   0        0        0        0 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/py.typed
--rw-r--r--   0        0        0      972 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/rich.py
--rw-r--r--   0        0        0       47 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/run.py
--rw-r--r--   0        0        0     4108 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/transformer.py
--rw-r--r--   0        0        0      895 2023-06-13 02:27:07.094176 cliffy-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7763 1970-01-01 00:00:00.000000 cliffy-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-24 20:57:23.061909 cliffy-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6810 2023-06-24 20:57:23.061909 cliffy-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/__init__.py
+-rw-r--r--   0        0        0       97 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/__main__.py
+-rw-r--r--   0        0        0     1859 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/builder.py
+-rw-r--r--   0        0        0     8076 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/cli.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/clis/__init__.py
+-rw-r--r--   0        0        0     6380 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/commander.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/commanders/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/commanders/click.py
+-rw-r--r--   0        0        0     1976 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/commanders/typer.py
+-rw-r--r--   0        0        0     3776 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/helper.py
+-rw-r--r--   0        0        0     3000 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/homer.py
+-rw-r--r--   0        0        0     1392 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/loader.py
+-rw-r--r--   0        0        0      396 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/manifests/__init__.py
+-rw-r--r--   0        0        0     7355 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/manifests/v1.py
+-rw-r--r--   0        0        0      137 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/merger.py
+-rw-r--r--   0        0        0     4663 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/parser.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/py.typed
+-rw-r--r--   0        0        0      972 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/rich.py
+-rw-r--r--   0        0        0       47 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/run.py
+-rw-r--r--   0        0        0     3829 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/transformer.py
+-rw-r--r--   0        0        0      895 2023-06-24 20:57:23.065909 cliffy-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7763 1970-01-01 00:00:00.000000 cliffy-0.3.2/PKG-INFO
```

### Comparing `cliffy-0.3.1/LICENSE` & `cliffy-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.1/README.md` & `cliffy-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.1/cliffy/builder.py` & `cliffy-0.3.2/cliffy/builder.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.1/cliffy/cli.py` & `cliffy-0.3.2/cliffy/cli.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.1/cliffy/commander.py` & `cliffy-0.3.2/cliffy/commander.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,39 +118,42 @@
         self.cli += "\n"
 
     def add_command(self, command: Command) -> None:
         if "." in command.name:
             group = command.name.split(".")[:-1][-1]
             self.add_sub_command(command, self.groups[group])
 
+    def add_lazy_command(self, greedy_command: Command, group: str):
+        # make it lazy and interpolate
+        lazy_command_name = greedy_command.name.replace("(*)", group)
+        lazy_command_script = ""
+        if isinstance(greedy_command.script, str):
+            lazy_command_script = greedy_command.script.replace("{(*)}", group)
+        elif isinstance(greedy_command.script, list):
+            lazy_command_script = []
+            for script_block in greedy_command.script:
+                if isinstance(script_block, dict):
+                    lazy_command_script.append(script_block["help"].replace("{(*)}", group))
+                else:
+                    lazy_command_script.append(script_block.replace("{(*)}", group))
+
+        if greedy_command_args := self.manifest.args.get(greedy_command.name):
+            self.manifest.args[lazy_command_name] = greedy_command_args
+
+        # lazy load
+        lazy_command = Command(name=lazy_command_name, script=lazy_command_script)
+        self.commands.append(lazy_command)
+        self.add_command(lazy_command)
+
     def add_greedy_commands(self) -> None:
         """Greedy commands get lazy-loaded. Only supported for group-commands currently"""
         for greedy_command in self.greedy:
             if greedy_command.name.startswith("(*)"):
                 for group in self.groups:
-                    # make it lazy and interpolate
-                    lazy_command_name = greedy_command.name.replace("(*)", group)
-                    lazy_command_script = ""
-                    if isinstance(greedy_command.script, str):
-                        lazy_command_script = greedy_command.script.replace("{(*)}", group)
-                    elif isinstance(greedy_command.script, list):
-                        lazy_command_script = []
-                        for script_block in greedy_command.script:
-                            if isinstance(script_block, dict):
-                                lazy_command_script.append(script_block["help"].replace("{(*)}", group))
-                            else:
-                                lazy_command_script.append(script_block.replace("{(*)}", group))
-
-                    if greedy_command_args := self.manifest.args.get(greedy_command.name):
-                        self.manifest.args[lazy_command_name] = greedy_command_args
-
-                    # lazy load
-                    lazy_command = Command(name=lazy_command_name, script=lazy_command_script)
-                    self.commands.append(lazy_command)
-                    self.add_command(lazy_command)
+                    self.add_lazy_command(greedy_command, group)
 
     def is_greedy(self, val: str) -> bool:
         """Greedy strings must contain (*)- marked to be evaluated lazily."""
         return "(*)" in val
 
     def add_group(self, group: Group) -> None:
         raise NotImplementedError
```

### Comparing `cliffy-0.3.1/cliffy/commanders/click.py` & `cliffy-0.3.2/cliffy/commanders/click.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.1/cliffy/commanders/typer.py` & `cliffy-0.3.2/cliffy/commanders/typer.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.1/cliffy/helper.py` & `cliffy-0.3.2/cliffy/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     for row in rows:
         table.add_row(*row)
 
     console = Console()
     console.print(table)
 
 
-def get_installed_pip_packages() -> dict[str, str]:
+def get_installed_package_versions() -> dict[str, str]:
     reqs = subprocess.check_output([sys.executable, "-m", "pip", "freeze"])
     installed_packages = {}
     for r in reqs.split():
         r_spec = r.decode().split("==")
         if len(r_spec) > 1:
             installed_packages[r_spec[0]] = r_spec[1]
     return installed_packages
@@ -110,18 +110,19 @@
         if op in requirement:
             parts = requirement.replace(" ", "").split(op)
             return RequirementSpec(name=parts[0], operator=op, version=parts[1])
 
     return RequirementSpec(name=requirement.strip(), operator=None, version=None)
 
 
-def compare_versions(version1: str, version2: str, op: str) -> bool:
+def compare_versions(version1: str, version2: str, op: Optional[str] = "=") -> bool:
     v1 = version.parse(version1)
     v2 = version.parse(version2)
-    return OPERATOR_MAP[op](v1, v2)
+
+    return OPERATOR_MAP[op](v1, v2) if op else v1 == v2
 
 
 def out(text: str, **echo_kwargs: Any) -> None:
     secho(text, **echo_kwargs)
 
 
 def out_err(text: str) -> None:
```

### Comparing `cliffy-0.3.1/cliffy/homer.py` & `cliffy-0.3.2/cliffy/homer.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,19 +79,15 @@
     Args:
         cli_name (str): CLI name
 
     Returns:
         Optional[CLIMetadata]: CLI metadata
     """
     cli_path = get_metadata_path(cli_name)
-    if not cli_path:
-        return None
-
-    path = Path(cli_path)
-    return get_metadata_bypath(path)
+    return get_metadata_bypath(Path(cli_path)) if cli_path else None
 
 
 def get_metadata_path(cli_name: str) -> Optional[str]:
     """Fetches CLI metadata path
 
     Args:
         cli_name (str): CLI name
```

### Comparing `cliffy-0.3.1/cliffy/loader.py` & `cliffy-0.3.2/cliffy/loader.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.1/cliffy/manifests/v1.py` & `cliffy-0.3.2/cliffy/manifests/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from datetime import datetime
 from typing import Any, Literal, Union
-
 from pydantic import BaseModel, Field
 
 from ..helper import wrap_as_comment, wrap_as_var
 
 COMMAND_BLOCK = Union[str, list[Union[str, dict[Literal["help"], str]]]]
 
 
@@ -75,19 +74,20 @@
         {},
         description="A mapping for any additional options that can be used to customize the behavior of the CLI.",
     )
 
     @classmethod
     def get_field_description(cls, field_name: str, as_comment: bool = True) -> str:
         field = cls.model_fields.get(field_name)
-        if field and field.description:
-            if as_comment:
-                return wrap_as_comment(field.description, split_on=". ")
-            return field.description
-        return ""
+        if not field or not field.description:
+            return ""
+
+        if as_comment:
+            return wrap_as_comment(field.description, split_on=". ")
+        return field.description
 
     @classmethod
     def get_template(cls, name: str) -> str:
         return f"""# cliffy v1 template
 manifestVersion: v1
 
 {cls.get_field_description('name')}
```

### Comparing `cliffy-0.3.1/cliffy/parser.py` & `cliffy-0.3.2/cliffy/parser.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.1/cliffy/rich.py` & `cliffy-0.3.2/cliffy/rich.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.1/cliffy/transformer.py` & `cliffy-0.3.2/cliffy/transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import yaml
 from jinja2 import BaseLoader, Environment, FileSystemLoader
 from pydantic import ValidationError
 from typing_extensions import Self
 
 from .commander import generate_cli
 from .commanders.typer import TyperCommander
-from .helper import compare_versions, exit_err, get_installed_pip_packages, out, parse_requirement
+from .helper import compare_versions, exit_err, get_installed_package_versions, out, parse_requirement
 from .manifests import IncludeManifest, Manifest, set_manifest_version
 from .merger import cliffy_merger
 
 
 class Transformer:
     """Loads command manifest and transforms it into a CLI"""
 
@@ -23,53 +23,44 @@
         self.command_config = self.load_manifest(manifest_io)
         self.manifest_version = self.command_config.pop("manifestVersion", "v1")
         if self.command_config.get("includes"):
             self.includes_config = self.resolve_includes()
             cliffy_merger.merge(self.command_config, self.includes_config)
 
         set_manifest_version(self.manifest_version)
-        if as_include:
-            try:
-                self.manifest = IncludeManifest(**self.command_config)
-            except ValidationError as e:
-                out(f"{e}")
-                exit_err(f"~ error validating {manifest_io.name}")
-        else:
-            try:
-                self.manifest = Manifest(**self.command_config)
-            except ValidationError as e:
-                out(f"{e}")
-                exit_err(f"~ error validating {manifest_io.name}")
 
-            if validate_requires:
-                self.validate_cli_requires()
+        manifest_cls = IncludeManifest if as_include else Manifest
+        try:
+            self.manifest = manifest_cls(**self.command_config)
+        except ValidationError as e:
+            out(f"{e}")
+            exit_err(f"~ error validating {manifest_io.name}")
+
+        if validate_requires:
+            self.validate_cli_requires()
+
+        if isinstance(self.manifest, Manifest):
             self.cli = generate_cli(self.manifest, commander_cls=TyperCommander)
 
     def validate_cli_requires(self) -> None:
         if not self.manifest.requires:
             return
 
-        installed_pip_packages = get_installed_pip_packages()
+        installed_package_versions = get_installed_package_versions()
         for dep in self.manifest.requires:
             dep_spec = parse_requirement(dep)
-            if dep_spec.name not in installed_pip_packages:
+            if dep_spec.name not in installed_package_versions:
                 exit_err(f"~ missing requirement: `{self.manifest_io.name}` requires `{dep}` to be installed")
 
-            if (
-                dep_spec.version
-                and dep_spec.operator
-                and not compare_versions(
-                    installed_pip_packages[dep_spec.name],
-                    dep_spec.version,
-                    dep_spec.operator,
-                )
+            if dep_spec.version and not compare_versions(
+                installed_package_versions[dep_spec.name], dep_spec.version, dep_spec.operator
             ):
                 exit_err(
                     f"~ missing requirement: `{self.manifest_io.name}` requires `{dep}` to be installed"
-                    f"    found version `{installed_pip_packages[dep_spec.name]}`"
+                    f"    found version `{installed_package_versions[dep_spec.name]}`"
                 )
 
     def resolve_includes(self) -> dict:
         include_transforms = map(self.resolve_include_by_path, set(self.command_config["includes"]))
         merged_config: dict[str, Any] = {}
         for transformed_include in include_transforms:
             cliffy_merger.merge(merged_config, transformed_include.command_config)
```

### Comparing `cliffy-0.3.1/pyproject.toml` & `cliffy-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "cliffy"
-version = "0.3.1"
+version = "0.3.2"
 description = "$ cli load from.yaml"
 authors = ["Jay <jay.github0@gmail.com>"]
 repository = "https://github.com/jaykv/cliffy"
 readme = "README.md"
 packages = [{include = "cliffy"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pybash = "^0.3.3"
+pybash = "^0.3.4"
 pyyaml = "^6.0"
 typer = "^0.9.0"
 pydantic = ">=2.0a4"
 deepmerge = "^1.1.0"
 jinja2 = "^3.1.2"
 packaging = "^23.1"
 rich-click = { version = "^1.6.1", optional = true }
```

### Comparing `cliffy-0.3.1/PKG-INFO` & `cliffy-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cliffy
-Version: 0.3.1
+Version: 0.3.2
 Summary: $ cli load from.yaml
 Home-page: https://github.com/jaykv/cliffy
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: rich
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: packaging (>=23.1,<24.0)
-Requires-Dist: pybash (>=0.3.3,<0.4.0)
+Requires-Dist: pybash (>=0.3.4,<0.4.0)
 Requires-Dist: pydantic (>=2.0a4)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0) ; extra == "rich"
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0) ; extra == "rich"
 Requires-Dist: shiv (>=1.0.3,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/jaykv/cliffy
```

