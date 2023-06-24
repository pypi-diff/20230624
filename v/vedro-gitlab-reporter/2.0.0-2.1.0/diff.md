# Comparing `tmp/vedro-gitlab-reporter-2.0.0.tar.gz` & `tmp/vedro-gitlab-reporter-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-gitlab-reporter-2.0.0.tar", last modified: Sun Sep  4 20:29:17 2022, max compression
+gzip compressed data, was "vedro-gitlab-reporter-2.1.0.tar", last modified: Sat Jun 24 08:57:32 2023, max compression
```

## Comparing `vedro-gitlab-reporter-2.0.0.tar` & `vedro-gitlab-reporter-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 20:29:17.773090 vedro-gitlab-reporter-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-04 20:29:08.000000 vedro-gitlab-reporter-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-09-04 20:29:17.773090 vedro-gitlab-reporter-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-09-04 20:29:08.000000 vedro-gitlab-reporter-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-09-04 20:29:17.773090 vedro-gitlab-reporter-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-09-04 20:29:08.000000 vedro-gitlab-reporter-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 20:29:17.773090 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter/
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-09-04 20:29:08.000000 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-09-04 20:29:08.000000 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter/_collapsable_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)    11319 2022-09-04 20:29:08.000000 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter/_gitlab_reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-04 20:29:08.000000 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 20:29:17.773090 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-09-04 20:29:17.000000 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-09-04 20:29:17.000000 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 20:29:17.000000 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-04 20:29:17.000000 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-04 20:29:17.000000 vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:57:32.671075 vedro-gitlab-reporter-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-24 08:57:32.671075 vedro-gitlab-reporter-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-24 08:57:32.671075 vedro-gitlab-reporter-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:57:32.667075 vedro-gitlab-reporter-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/tests/test_collapsable_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/tests/test_gitlab_collapsable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/tests/test_gitlab_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:57:32.671075 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/_collapsable_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/_gitlab_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:57:32.671075 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-24 08:57:32.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-24 08:57:32.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:57:32.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-24 08:57:32.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 08:57:32.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/top_level.txt
```

### Comparing `vedro-gitlab-reporter-2.0.0/LICENSE` & `vedro-gitlab-reporter-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-gitlab-reporter-2.0.0/PKG-INFO` & `vedro-gitlab-reporter-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,80 @@
 Metadata-Version: 2.1
 Name: vedro-gitlab-reporter
-Version: 2.0.0
+Version: 2.1.0
 Summary: GitLab reporter with collapsable sections for Vedro framework
-Home-page: https://github.com/nikitanovosibirsk/vedro-gitlab-reporter
+Home-page: https://github.com/vedro-universe/vedro-gitlab-reporter
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vedro GitLab Reporter
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-gitlab-reporter/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-gitlab-reporter)
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-gitlab-reporter/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-gitlab-reporter)
 [![PyPI](https://img.shields.io/pypi/v/vedro-gitlab-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-gitlab-reporter/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-gitlab-reporter?style=flat-square)](https://pypi.python.org/pypi/vedro-gitlab-reporter/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-gitlab-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-gitlab-reporter/)
 
-GitLab (>=12.0) reporter with [collapsable sections](https://docs.gitlab.com/ee/ci/jobs/#custom-collapsible-sections) for [Vedro](https://github.com/nikitanovosibirsk/vedro) framework
+GitLab (>=12.0) reporter with [collapsable sections](https://docs.gitlab.com/ee/ci/jobs/#custom-collapsible-sections) for [Vedro](https://vedro.io/) framework
 
 ## Installation
 
-### 1. Install package
+<details open>
+<summary>Quick</summary>
+<p>
+
+For a quick installation, you can use a plugin manager as follows:
+
+```shell
+$ vedro plugin install vedro-gitlab-reporter
+```
+
+</p>
+</details>
+
+<details>
+<summary>Manual</summary>
+<p>
+
+To install manually, follow these steps:
+
+1. Install the package using pip:
 
 ```shell
 $ pip3 install vedro-gitlab-reporter
 ```
 
-### 2. Enable plugin
+2. Next, activate the plugin in your `vedro.cfg.py` configuration file:
 
 ```python
 # ./vedro.cfg.py
 import vedro
-import vedro_gitlab_reporter as gitlab_reporter
+import vedro_gitlab_reporter
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
-        class GitlabReporter(gitlab_reporter.GitlabReporter):
+        class GitlabReporter(vedro_gitlab_reporter.GitlabReporter):
             enabled = True
 ```
 
+</p>
+</details>
+
 ## Usage
 
 ### Run tests
 
 ```shell
 $ vedro run -r gitlab --gitlab-collapsable steps
 ```
```

### Comparing `vedro-gitlab-reporter-2.0.0/setup.cfg` & `vedro-gitlab-reporter-2.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.0.0
+current_version = 2.1.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-gitlab-reporter-2.0.0/setup.py` & `vedro-gitlab-reporter-2.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-gitlab-reporter",
-    version="2.0.0",
+    version="2.1.0",
     description="GitLab reporter with collapsable sections for Vedro framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
+    author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
-    url="https://github.com/nikitanovosibirsk/vedro-gitlab-reporter",
+    url="https://github.com/vedro-universe/vedro-gitlab-reporter",
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"vedro_gitlab_reporter": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
 )
```

### Comparing `vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter/_gitlab_reporter.py` & `vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/_gitlab_reporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import operator
 import uuid
 from functools import reduce
-from typing import Callable, Dict, Set, Type, Union
+from typing import Callable, Dict, List, Set, Type, Union
 
 from vedro.core import Dispatcher, PluginConfig, ScenarioResult
 from vedro.events import (
     ArgParsedEvent,
     ArgParseEvent,
     CleanupEvent,
     ScenarioReportedEvent,
@@ -31,15 +31,15 @@
         self._tb_show_internal_calls = config.tb_show_internal_calls
         self._tb_show_locals = config.tb_show_locals
         self._tb_max_frames = config.tb_max_frames
         self._collapsable_mode: Union[GitlabCollapsableMode, None] = None
 
         self._namespace: Union[str, None] = None
         self._scenario_result: Union[ScenarioResult, None] = None
-        self._scenario_steps: Dict[str, Set[str]] = {}
+        self._scenario_steps: List[Dict[str, Set[str]]] = []
 
     def subscribe(self, dispatcher: Dispatcher) -> None:
         super().subscribe(dispatcher)
         dispatcher.listen(DirectorInitEvent, lambda e: e.director.register("gitlab", self))
 
     def on_chosen(self) -> None:
         assert isinstance(self._dispatcher, Dispatcher)
@@ -78,50 +78,57 @@
 
     def on_scenario_run(self, event: ScenarioRunEvent) -> None:
         namespace = event.scenario_result.scenario.namespace
         if namespace != self._namespace:
             self._namespace = namespace
             self._printer.print_namespace(namespace)
 
+        unique_id = event.scenario_result.scenario.unique_id
+        if self._scenario_result is None or self._scenario_result.scenario.unique_id != unique_id:
+            self._scenario_steps = []
+        self._scenario_steps.append({})
         self._scenario_result = event.scenario_result
-        self._scenario_steps = {}
 
     def on_step_end(self, event: Union[StepPassedEvent, StepFailedEvent]) -> None:
         assert isinstance(self._scenario_result, ScenarioResult)
 
+        scenario_steps = self._scenario_steps[-1]
         step_scope: Set[str] = set(self._scenario_result.scope.keys())
-        prev_scope: Set[str] = reduce(operator.or_, self._scenario_steps.values(), set())
-        self._scenario_steps[event.step_result.step_name] = step_scope - prev_scope
+        prev_scope: Set[str] = reduce(operator.or_, scenario_steps.values(), set())
+        scenario_steps[event.step_result.step_name] = step_scope - prev_scope
 
-    def _print_scenario_result(self, scenario_result: ScenarioResult, *, prefix: str = "") -> None:
+    def _print_scenario_result(self, scenario_result: ScenarioResult, *,
+                               index: int = 0, prefix: str = "") -> None:
         if scenario_result.is_passed():
-            self._print_scenario_passed(scenario_result, prefix=prefix)
+            self._print_scenario_passed(scenario_result, index=index, prefix=prefix)
         elif scenario_result.is_failed():
-            self._print_scenario_failed(scenario_result, prefix=prefix)
+            self._print_scenario_failed(scenario_result, index=index, prefix=prefix)
 
-    def _print_scenario_passed(self, scenario_result: ScenarioResult, *, prefix: str = "") -> None:
+    def _print_scenario_passed(self, scenario_result: ScenarioResult, *,
+                               index: int = 0, prefix: str = "") -> None:
         self._printer.print_scenario_subject(scenario_result.scenario.subject,
                                              scenario_result.status,
                                              elapsed=scenario_result.elapsed,
                                              prefix=prefix)
 
-    def _print_scenario_failed(self, scenario_result: ScenarioResult, *, prefix: str = "") -> None:
+    def _print_scenario_failed(self, scenario_result: ScenarioResult, *,
+                               index: int = 0, prefix: str = "") -> None:
         self._printer.print_scenario_subject(scenario_result.scenario.subject,
                                              scenario_result.status,
                                              elapsed=scenario_result.elapsed,
                                              prefix=prefix)
 
         if self._collapsable_mode == GitlabCollapsableMode.STEPS:
             prefix = self._prefix_to_indent(prefix, indent=2)
-            self._print_collapsable_steps(scenario_result, prefix=prefix)
+            self._print_collapsable_steps(scenario_result, index=index, prefix=prefix)
             self._print_exceptions(scenario_result)
 
         elif self._collapsable_mode == GitlabCollapsableMode.VARS:
             prefix = self._prefix_to_indent(prefix, indent=2)
-            self._print_steps_with_collapsable_vars(scenario_result, prefix=prefix)
+            self._print_steps_with_collapsable_vars(scenario_result, index=index, prefix=prefix)
             self._print_exceptions(scenario_result)
 
         elif self._collapsable_mode == GitlabCollapsableMode.SCOPE:
             prefix = self._prefix_to_indent(prefix, indent=2)
             self._print_steps(scenario_result, prefix=prefix)
             self._print_exceptions(scenario_result)
             self._print_collapsable_scope(scenario_result)
@@ -131,17 +138,17 @@
         rescheduled = len(aggregated_result.scenario_results)
         if rescheduled == 1:
             self._print_scenario_result(aggregated_result, prefix=" ")
             return
 
         self._printer.print_scenario_subject(aggregated_result.scenario.subject,
                                              aggregated_result.status, elapsed=None, prefix=" ")
-        for index, scenario_result in enumerate(aggregated_result.scenario_results, start=1):
-            prefix = f" │\n ├─[{index}/{rescheduled}] "
-            self._print_scenario_result(scenario_result, prefix=prefix)
+        for index, scenario_result in enumerate(aggregated_result.scenario_results):
+            prefix = f" │\n ├─[{index+1}/{rescheduled}] "
+            self._print_scenario_result(scenario_result, index=index, prefix=prefix)
 
         self._printer.print_empty_line()
 
     def on_cleanup(self, event: CleanupEvent) -> None:
         self._printer.print_empty_line()
         self._printer.print_report_summary(event.report.summary)
         self._printer.print_report_stats(total=event.report.total,
@@ -166,40 +173,42 @@
 
     def _print_steps(self, scenario_result: ScenarioResult, *, prefix: str = "") -> None:
         for step_result in scenario_result.step_results:
             self._printer.print_step_name(step_result.step_name, step_result.status,
                                           elapsed=step_result.elapsed, prefix=prefix)
 
     def _print_collapsable_steps(self, scenario_result: ScenarioResult, *,
-                                 prefix: str = "") -> None:
+                                 index: int = 0, prefix: str = "") -> None:
         for step_result in scenario_result.step_results:
             section_name = str(uuid.uuid4())
             started_at = int(step_result.started_at) if step_result.started_at else 0
             self._print_section_start(section_name, started_at)
 
             self._printer.print_step_name(step_result.step_name, step_result.status,
                                           elapsed=step_result.elapsed, prefix=prefix)
 
+            scenario_steps = self._scenario_steps[index]
             for key, val in scenario_result.scope.items():
-                if key not in self._scenario_steps[step_result.step_name]:
+                if key not in scenario_steps[step_result.step_name]:
                     continue
                 self._printer.print_scope_key(key, indent=len(prefix) + 2, line_break=True)
                 self._printer.print_scope_val(self._printer.pretty_format(val))
 
             ended_at = int(step_result.ended_at) if step_result.ended_at else 0
             self._print_section_end(section_name, ended_at)
 
     def _print_steps_with_collapsable_vars(self, scenario_result: ScenarioResult, *,
-                                           prefix: str = "") -> None:
+                                           index: int = 0, prefix: str = "") -> None:
         for step_result in scenario_result.step_results:
             self._printer.print_step_name(step_result.step_name, step_result.status,
                                           elapsed=step_result.elapsed, prefix=prefix)
 
+            scenario_steps = self._scenario_steps[index]
             for key, val in scenario_result.scope.items():
-                if key not in self._scenario_steps[step_result.step_name]:
+                if key not in scenario_steps[step_result.step_name]:
                     continue
                 section_name = str(uuid.uuid4())
                 self._print_section_start(section_name)
 
                 self._printer.print_scope_key(key, indent=len(prefix) + 2, line_break=True)
                 self._printer.print_scope_val(self._printer.pretty_format(val))
```

### Comparing `vedro-gitlab-reporter-2.0.0/vedro_gitlab_reporter.egg-info/PKG-INFO` & `vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,80 @@
 Metadata-Version: 2.1
 Name: vedro-gitlab-reporter
-Version: 2.0.0
+Version: 2.1.0
 Summary: GitLab reporter with collapsable sections for Vedro framework
-Home-page: https://github.com/nikitanovosibirsk/vedro-gitlab-reporter
+Home-page: https://github.com/vedro-universe/vedro-gitlab-reporter
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vedro GitLab Reporter
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-gitlab-reporter/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-gitlab-reporter)
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-gitlab-reporter/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-gitlab-reporter)
 [![PyPI](https://img.shields.io/pypi/v/vedro-gitlab-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-gitlab-reporter/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-gitlab-reporter?style=flat-square)](https://pypi.python.org/pypi/vedro-gitlab-reporter/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-gitlab-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-gitlab-reporter/)
 
-GitLab (>=12.0) reporter with [collapsable sections](https://docs.gitlab.com/ee/ci/jobs/#custom-collapsible-sections) for [Vedro](https://github.com/nikitanovosibirsk/vedro) framework
+GitLab (>=12.0) reporter with [collapsable sections](https://docs.gitlab.com/ee/ci/jobs/#custom-collapsible-sections) for [Vedro](https://vedro.io/) framework
 
 ## Installation
 
-### 1. Install package
+<details open>
+<summary>Quick</summary>
+<p>
+
+For a quick installation, you can use a plugin manager as follows:
+
+```shell
+$ vedro plugin install vedro-gitlab-reporter
+```
+
+</p>
+</details>
+
+<details>
+<summary>Manual</summary>
+<p>
+
+To install manually, follow these steps:
+
+1. Install the package using pip:
 
 ```shell
 $ pip3 install vedro-gitlab-reporter
 ```
 
-### 2. Enable plugin
+2. Next, activate the plugin in your `vedro.cfg.py` configuration file:
 
 ```python
 # ./vedro.cfg.py
 import vedro
-import vedro_gitlab_reporter as gitlab_reporter
+import vedro_gitlab_reporter
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
-        class GitlabReporter(gitlab_reporter.GitlabReporter):
+        class GitlabReporter(vedro_gitlab_reporter.GitlabReporter):
             enabled = True
 ```
 
+</p>
+</details>
+
 ## Usage
 
 ### Run tests
 
 ```shell
 $ vedro run -r gitlab --gitlab-collapsable steps
 ```
```

