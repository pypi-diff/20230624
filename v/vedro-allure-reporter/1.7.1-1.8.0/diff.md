# Comparing `tmp/vedro-allure-reporter-1.7.1.tar.gz` & `tmp/vedro-allure-reporter-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-allure-reporter-1.7.1.tar", last modified: Tue Jun  6 18:33:21 2023, max compression
+gzip compressed data, was "vedro-allure-reporter-1.8.0.tar", last modified: Sat Jun 24 10:11:28 2023, max compression
```

## Comparing `vedro-allure-reporter-1.7.1.tar` & `vedro-allure-reporter-1.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:21.530949 vedro-allure-reporter-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-06 18:33:21.530949 vedro-allure-reporter-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 18:33:21.530949 vedro-allure-reporter-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:21.526949 vedro-allure-reporter-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/tests/test_allure_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/tests/test_allure_reporter_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:21.530949 vedro-allure-reporter-1.7.1/vedro_allure_reporter/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter/_allure_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter/_allure_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:11.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:21.530949 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-06 18:33:21.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-06 18:33:21.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:33:21.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 18:33:21.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 18:33:21.000000 vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:11:27.995609 vedro-allure-reporter-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 10:11:14.000000 vedro-allure-reporter-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-24 10:11:27.995609 vedro-allure-reporter-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-24 10:11:14.000000 vedro-allure-reporter-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-24 10:11:27.995609 vedro-allure-reporter-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-24 10:11:14.000000 vedro-allure-reporter-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:11:27.991609 vedro-allure-reporter-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-24 10:11:14.000000 vedro-allure-reporter-1.8.0/tests/test_allure_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15558 2023-06-24 10:11:14.000000 vedro-allure-reporter-1.8.0/tests/test_allure_reporter_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:11:27.991609 vedro-allure-reporter-1.8.0/vedro_allure_reporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-24 10:11:14.000000 vedro-allure-reporter-1.8.0/vedro_allure_reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-24 10:11:14.000000 vedro-allure-reporter-1.8.0/vedro_allure_reporter/_allure_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-06-24 10:11:14.000000 vedro-allure-reporter-1.8.0/vedro_allure_reporter/_allure_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:11:14.000000 vedro-allure-reporter-1.8.0/vedro_allure_reporter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:11:27.995609 vedro-allure-reporter-1.8.0/vedro_allure_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-24 10:11:27.000000 vedro-allure-reporter-1.8.0/vedro_allure_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-24 10:11:27.000000 vedro-allure-reporter-1.8.0/vedro_allure_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:11:27.000000 vedro-allure-reporter-1.8.0/vedro_allure_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-24 10:11:27.000000 vedro-allure-reporter-1.8.0/vedro_allure_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 10:11:27.000000 vedro-allure-reporter-1.8.0/vedro_allure_reporter.egg-info/top_level.txt
```

### Comparing `vedro-allure-reporter-1.7.1/LICENSE` & `vedro-allure-reporter-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-allure-reporter-1.7.1/PKG-INFO` & `vedro-allure-reporter-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vedro-allure-reporter
-Version: 1.7.1
+Version: 1.8.0
 Summary: Allure reporter for Vedro testing framework
 Home-page: https://github.com/vedro-universe/vedro-allure-reporter
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
-Project-URL: Docs, https://vedro.io/en/docs/integrations/allure-reporter
+Project-URL: Docs, https://vedro.io/docs/integrations/allure-reporter
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-allure-reporter
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -89,8 +89,8 @@
 $ allure serve ./allure_reports
 ```
 
 This command will serve up the report ([demo](https://allure-framework.github.io/allure-demo/5/)).
 
 ---
 
-Explore more at https://vedro.io/en/docs/integrations/allure-reporter
+Explore more at https://vedro.io/docs/integrations/allure-reporter
```

### Comparing `vedro-allure-reporter-1.7.1/README.md` & `vedro-allure-reporter-1.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 $ allure serve ./allure_reports
 ```
 
 This command will serve up the report ([demo](https://allure-framework.github.io/allure-demo/5/)).
 
 ---
 
-Explore more at https://vedro.io/en/docs/integrations/allure-reporter
+Explore more at https://vedro.io/docs/integrations/allure-reporter
```

### Comparing `vedro-allure-reporter-1.7.1/setup.cfg` & `vedro-allure-reporter-1.8.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.7.1
+current_version = 1.8.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-allure-reporter-1.7.1/setup.py` & `vedro-allure-reporter-1.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-allure-reporter",
-    version="1.7.1",
+    version="1.8.0",
     description="Allure reporter for Vedro testing framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
     url="https://github.com/vedro-universe/vedro-allure-reporter",
     project_urls={
-        "Docs": "https://vedro.io/en/docs/integrations/allure-reporter",
+        "Docs": "https://vedro.io/docs/integrations/allure-reporter",
         "GitHub": "https://github.com/vedro-universe/vedro-allure-reporter",
     },
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"vedro_allure_reporter": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
```

### Comparing `vedro-allure-reporter-1.7.1/tests/test_allure_reporter.py` & `vedro-allure-reporter-1.8.0/tests/test_allure_reporter.py`

 * *Files identical despite different names*

### Comparing `vedro-allure-reporter-1.7.1/tests/test_allure_reporter_integration.py` & `vedro-allure-reporter-1.8.0/tests/test_allure_reporter_integration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from pathlib import Path
 from typing import Callable
 from uuid import uuid4
 
 import pytest
 from allure_commons.logger import AllureMemoryLogger
 from baby_steps import given, then, when
-from vedro.core import Dispatcher, FileArtifact, MemoryArtifact, ScenarioResult
-from vedro.events import ScenarioReportedEvent
+from vedro.core import Dispatcher, FileArtifact, MemoryArtifact
+from vedro.core import MonotonicScenarioScheduler as Scheduler
+from vedro.core import ScenarioResult
+from vedro.events import ArgParsedEvent, ScenarioReportedEvent, StartupEvent
 from vedro.plugins.director import DirectorPlugin
 
 import vedro_allure_reporter
 from vedro_allure_reporter import AllureLabel, AllureReporterPlugin
 
 from ._utils import (
     choose_reporter,
     create_attachment,
     director,
     dispatcher,
     fire_arg_parsed_event,
     logger,
     make_aggregated_result,
+    make_parsed_args,
     make_scenario_result,
     make_step_result,
     make_test_case,
+    make_vscenario,
     patch_uuid,
     patch_uuids,
 )
 
 __all__ = ("dispatcher", "director", "logger",)
 
 
@@ -271,7 +275,139 @@
 
     with then:
         assert logger.test_cases == [
             make_test_case(uuid, scenario_result, labels=scenario_labels)
         ]
         assert logger.test_containers == []
         assert logger.attachments == {}
+
+
+async def test_arg_parsed_event_allure_labels(*, dispatcher: Dispatcher,
+                                              director: DirectorPlugin,
+                                              reporter: AllureReporterPlugin):
+    with given:
+        await choose_reporter(dispatcher, director, reporter)
+
+        labels = "key1=value1,key2=value2"
+        report_dir = "allure_reports"
+        args = make_parsed_args(allure_labels=labels, allure_report_dir=report_dir)
+        event = ArgParsedEvent(args)
+
+    with when:
+        await dispatcher.fire(event)
+
+    with then:
+        assert reporter.allure_labels_to_run == labels
+
+
+async def test_no_allure_labels_to_run(*, dispatcher: Dispatcher,
+                                       director: DirectorPlugin,
+                                       reporter: AllureReporterPlugin,
+                                       logger: AllureMemoryLogger):
+    with given:
+        labels = [
+            (AllureLabel('label1', 'value1'),),
+            (AllureLabel('label2', 'value2'),)
+        ]
+        scenarios = [make_vscenario(labels=labels[0]), make_vscenario(labels=labels[1])]
+        scheduler = Scheduler(scenarios)
+
+        await fire_arg_parsed_event(dispatcher, labels=[])
+
+        startup_event = StartupEvent(scheduler)
+
+    with when:
+        await dispatcher.fire(startup_event)
+
+    with then:
+        assert list(scheduler.scheduled) == scenarios
+
+
+async def test_nonexisting_label_to_run(*, dispatcher: Dispatcher,
+                                        director: DirectorPlugin,
+                                        reporter: AllureReporterPlugin,
+                                        logger: AllureMemoryLogger):
+    with given:
+        labels = [
+            (AllureLabel('label1', 'value1'),),
+            (AllureLabel('label2', 'value2'),),
+        ]
+        scenarios = [make_vscenario(labels=labels[0]), make_vscenario(labels=labels[1])]
+        scheduler = Scheduler(scenarios)
+
+        await fire_arg_parsed_event(dispatcher, labels=['label3=value3'])
+
+        startup_event = StartupEvent(scheduler)
+
+    with when:
+        await dispatcher.fire(startup_event)
+
+    with then:
+        assert list(scheduler.scheduled) == []
+
+
+async def test_multiple_labels(*, dispatcher: Dispatcher,
+                               director: DirectorPlugin,
+                               reporter: AllureReporterPlugin,
+                               logger: AllureMemoryLogger):
+    with given:
+        labels = [
+            (AllureLabel('label1', 'value1'),),
+            (AllureLabel('label2', 'value2'),)
+        ]
+        scenarios = [make_vscenario(labels=labels[0]), make_vscenario(labels=labels[1])]
+        scheduler = Scheduler(scenarios)
+
+        await fire_arg_parsed_event(dispatcher, labels=['label1=value1', 'label2=value2'])
+
+        startup_event = StartupEvent(scheduler)
+
+    with when:
+        await dispatcher.fire(startup_event)
+
+    with then:
+        assert list(scheduler.scheduled) == []
+
+
+async def test_multiple_labels_in_one_test(*, dispatcher: Dispatcher,
+                                           director: DirectorPlugin,
+                                           reporter: AllureReporterPlugin,
+                                           logger: AllureMemoryLogger):
+    with given:
+        labels = [
+            (AllureLabel('label1', 'value1'), AllureLabel('label2', 'value2')),
+            (AllureLabel('label3', 'value3'),)
+        ]
+        scenarios = [make_vscenario(labels=labels[0]), make_vscenario(labels=labels[1])]
+        scheduler = Scheduler(scenarios)
+
+        await fire_arg_parsed_event(dispatcher, labels=['label1=value1'])
+
+        startup_event = StartupEvent(scheduler)
+
+    with when:
+        await dispatcher.fire(startup_event)
+
+    with then:
+        assert list(scheduler.scheduled) == [scenarios[0]]
+
+
+async def test_labels_name_case_insensitive(*, dispatcher: Dispatcher,
+                                            director: DirectorPlugin,
+                                            reporter: AllureReporterPlugin,
+                                            logger: AllureMemoryLogger):
+    with given:
+        labels = [
+            (AllureLabel('lAbEl', 'value'),),
+        ]
+        scenarios = [make_vscenario(labels=labels[0])]
+        scheduler = Scheduler(scenarios)
+
+        await fire_arg_parsed_event(dispatcher, labels=['LaBeL=value'])
+
+        startup_event = StartupEvent(scheduler)
+
+    with when:
+        await dispatcher.fire(startup_event)
+
+    with then:
+        assert list(scheduler.scheduled) == scenarios
```

### Comparing `vedro-allure-reporter-1.7.1/vedro_allure_reporter/_allure_labels.py` & `vedro-allure-reporter-1.8.0/vedro_allure_reporter/_allure_labels.py`

 * *Files identical despite different names*

### Comparing `vedro-allure-reporter-1.7.1/vedro_allure_reporter/_allure_reporter.py` & `vedro-allure-reporter-1.8.0/vedro_allure_reporter/_allure_reporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     MemoryArtifact,
     PluginConfig,
     ScenarioResult,
     StepResult,
     StepStatus,
     VirtualScenario,
 )
-from vedro.events import ArgParsedEvent, ArgParseEvent, ScenarioReportedEvent
+from vedro.events import ArgParsedEvent, ArgParseEvent, ScenarioReportedEvent, StartupEvent
 from vedro.plugins.director import DirectorInitEvent, Reporter
 
 __all__ = ("AllureReporter", "AllureReporterPlugin",)
 
 
 class AllureReporterPlugin(Reporter):
     def __init__(self, config: Type["AllureReporter"], *,
@@ -43,44 +43,74 @@
         self._test_result: Union[TestResult, None] = None
         self._project_name = config.project_name
         self._report_dir = config.report_dir
         self._attach_scope = config.attach_scope
         self._attach_artifacts = config.attach_artifacts
         self._config_labels = config.labels
 
+    async def on_startup(self, event: StartupEvent) -> None:
+        if self._allure_labels is None:
+            return
+
+        labels = set()
+        for label_str in self._allure_labels:
+            name, value = label_str.split("=")
+            label = (name.lower(), value)
+            labels.add(label)
+
+        async for scenario in event.scheduler:
+            scenario_labels = set([(label.name.lower(), label.value)
+                                   for label in self._get_scenario_labels(scenario)])
+            if not labels.issubset(scenario_labels):
+                event.scheduler.ignore(scenario)
+
     def subscribe(self, dispatcher: Dispatcher) -> None:
         super().subscribe(dispatcher)
         dispatcher.listen(DirectorInitEvent, lambda e: e.director.register("allure", self))
+        dispatcher.listen(ArgParseEvent, self.on_subscribe_arg_parse)
+        dispatcher.listen(ArgParsedEvent, self.on_subscribe_arg_parsed)
+        dispatcher.listen(StartupEvent, self.on_startup)
 
     def on_chosen(self) -> None:
         assert isinstance(self._dispatcher, Dispatcher)
-        self._dispatcher.listen(ArgParseEvent, self.on_arg_parse) \
-                        .listen(ArgParsedEvent, self.on_arg_parsed) \
+        self._dispatcher.listen(ArgParseEvent, self.on_choosen_arg_parse) \
+                        .listen(ArgParsedEvent, self.on_choosen_arg_parsed) \
                         .listen(ScenarioReportedEvent, self.on_scenario_reported)
 
-    def on_arg_parse(self, event: ArgParseEvent) -> None:
+    def on_choosen_arg_parse(self, event: ArgParseEvent) -> None:
         group = event.arg_parser.add_argument_group("Allure Reporter")
 
         group.add_argument("--allure-report-dir",
                            default=self._report_dir,
                            type=Path,
                            help="Set directory for Allure reports")
         group.add_argument("--allure-attach-scope",
                            action='store_true',
                            default=self._attach_scope,
                            help="Attach scope to Allure report")
 
-    def on_arg_parsed(self, event: ArgParsedEvent) -> None:
+    def on_subscribe_arg_parse(self, event: ArgParseEvent) -> None:
+        group = event.arg_parser.add_argument_group("Allure Reporter")
+        group.add_argument("--allure-labels",
+                           default=None,
+                           nargs="+",
+                           help="Run tests with specific Allure labels")
+
+    def on_choosen_arg_parsed(self, event: ArgParsedEvent) -> None:
         self._report_dir = event.args.allure_report_dir
         self._attach_scope = event.args.allure_attach_scope
+        self._allure_labels = event.args.allure_labels
 
         self._plugin_manager.register(self)
         self._logger = self._logger_factory(self._report_dir, clean=True)
         self._plugin_manager.register(self._logger)
 
+    def on_subscribe_arg_parsed(self, event: ArgParsedEvent) -> None:
+        self._allure_labels = event.args.allure_labels
+
     def on_scenario_reported(self, event: ScenarioReportedEvent) -> None:
         aggregated_result = event.aggregated_result
         if aggregated_result.is_passed():
             self._report_result(aggregated_result, Status.PASSED)
         elif aggregated_result.is_failed():
             self._report_result(aggregated_result, Status.FAILED)
         elif aggregated_result.is_skipped():
@@ -215,14 +245,18 @@
         test_step_result.stop = self._to_seconds(step_result.ended_at or time())
         if step_result.status == StepStatus.PASSED:
             test_step_result.status = Status.PASSED
         elif step_result.status == StepStatus.FAILED:
             test_step_result.status = Status.FAILED
         return test_step_result
 
+    @property
+    def allure_labels_to_run(self) -> Any:
+        return self._allure_labels
+
 
 class AllureReporter(PluginConfig):
     plugin = AllureReporterPlugin
 
     # Set project name (adds label "project_name" and prefix for testCaseId)
     project_name: str = ""
```

### Comparing `vedro-allure-reporter-1.7.1/vedro_allure_reporter.egg-info/PKG-INFO` & `vedro-allure-reporter-1.8.0/vedro_allure_reporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vedro-allure-reporter
-Version: 1.7.1
+Version: 1.8.0
 Summary: Allure reporter for Vedro testing framework
 Home-page: https://github.com/vedro-universe/vedro-allure-reporter
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
-Project-URL: Docs, https://vedro.io/en/docs/integrations/allure-reporter
+Project-URL: Docs, https://vedro.io/docs/integrations/allure-reporter
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-allure-reporter
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -89,8 +89,8 @@
 $ allure serve ./allure_reports
 ```
 
 This command will serve up the report ([demo](https://allure-framework.github.io/allure-demo/5/)).
 
 ---
 
-Explore more at https://vedro.io/en/docs/integrations/allure-reporter
+Explore more at https://vedro.io/docs/integrations/allure-reporter
```

