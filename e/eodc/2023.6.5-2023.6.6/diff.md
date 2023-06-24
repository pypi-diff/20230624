# Comparing `tmp/eodc-2023.6.5.tar.gz` & `tmp/eodc-2023.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.6.5.tar", max compression
+gzip compressed data, was "eodc-2023.6.6.tar", max compression
```

## Comparing `eodc-2023.6.5.tar` & `eodc-2023.6.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-06-22 12:02:20.709724 eodc-2023.6.5/README.md
--rw-r--r--   0        0        0      213 2023-06-22 12:02:20.709724 eodc-2023.6.5/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-22 12:02:20.709724 eodc-2023.6.5/eodc/dask.py
--rw-r--r--   0        0        0     9754 2023-06-22 12:02:20.709724 eodc-2023.6.5/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-06-22 12:02:20.709724 eodc-2023.6.5/eodc/settings.py
--rw-r--r--   0        0        0     1204 2023-06-22 12:02:20.709724 eodc-2023.6.5/pyproject.toml
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 eodc-2023.6.5/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-24 09:54:08.666077 eodc-2023.6.6/README.md
+-rw-r--r--   0        0        0      213 2023-06-24 09:54:08.666077 eodc-2023.6.6/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-24 09:54:08.666077 eodc-2023.6.6/eodc/dask.py
+-rw-r--r--   0        0        0    10812 2023-06-24 09:54:08.666077 eodc-2023.6.6/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-06-24 09:54:08.666077 eodc-2023.6.6/eodc/settings.py
+-rw-r--r--   0        0        0     1204 2023-06-24 09:54:08.666077 eodc-2023.6.6/pyproject.toml
+-rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 eodc-2023.6.6/PKG-INFO
```

### Comparing `eodc-2023.6.5/README.md` & `eodc-2023.6.6/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.5/eodc/dask.py` & `eodc-2023.6.6/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.5/eodc/faas.py` & `eodc-2023.6.6/eodc/faas.py`

 * *Files 7% similar despite different names*

```diff
@@ -118,44 +118,47 @@
         workflow_name = created_workflow.metadata.get("name")
 
         logger.info(
             f"Submitted {self.processor_details.name.upper()} workflow: {workflow_name}"
         )
         return workflow_name
 
+    def get_workflow_status(self, workflow_name: str) -> dict:
+        status = self.api_instance_workflows.get_workflow(
+            namespace=settings.NAMESPACE,
+            name=workflow_name,
+            fields="status.phase,status.finishedAt,status.startedAt",
+            _check_return_type=False,
+        ).get("status", {})
+        return status
+
     def wait_for_completion(self, workflow_name: str) -> None:
         """Repeatedly query workflow status until it changes to a completed state"""
 
-        def get_workflow_status(workflow_name: str) -> dict:
-            status = self.api_instance_workflows.get_workflow(
-                namespace=self.namespace,
-                name=workflow_name,
-                fields="status.phase,status.finishedAt,status.startedAt",
-                _check_return_type=False,
-            ).get("status", {})
-            return status
-
-        while (status := get_workflow_status(workflow_name)).get("finishedAt") is None:
+        while (status := self.get_workflow_status(workflow_name)).get(
+            "finishedAt"
+        ) is None:
             logger.info("Workflow still running, sleeping 30 seconds")
             sleep(30)
         logger.info(f"Workflow completed with status {status.get('phase')}.")
 
         if status.get("phase") in ("Failed", "Error"):
             raise ValueError(
                 f"Workflow {workflow_name} ended with status {status.get('phase')}"
             )
 
     def stop_workflow(self, name):
         body = IoArgoprojWorkflowV1alpha1WorkflowStopRequest()
         self.api_instance_workflows.stop_workflow(settings.NAMESPACE, name, body=body)
         logger.info(f"Successfully stopped workflow {name}.")
-        return
 
     def get_logs(self, workflow_name):
-        # This Client method seems semi-broken: https://github.com/argoproj/argo-workflows/issues/7781
+        # The .workflow_logs client method seems semi-broken:
+        # https://github.com/argoproj/argo-workflows/issues/7781
+        # Therefore this workaround is necessary!
         return (
             self.api_instance_workflows.workflow_logs(
                 settings.NAMESPACE,
                 workflow_name,
                 log_options_container="main",
                 #  log_options_follow=True,
                 _check_return_type=False,
@@ -235,24 +238,48 @@
     ):
         return super().submit_workflow(
             openeo_executor_parameters=openeo_parameters.json(),
             openeo_user_id=openeo_user_id,
             openeo_job_id=openeo_job_id,
         )
 
-    def get_output_stac_items(self, openeo_parameters: OpenEOExecutorParameters):
+    def get_output_stac_items(
+        self, openeo_parameters: OpenEOExecutorParameters
+    ) -> list[Item]:
         collection_file = list(openeo_parameters.stac_path.glob("*_collection.json"))[0]
         openeo_output_collection = Collection.from_file(str(collection_file))
         stac_items = [
             Item.from_file(link.get_absolute_href())
             for link in openeo_output_collection.get_item_links()
         ]
 
         return stac_items
 
+    def stop_openeo_job(self, openeo_job_id):
+        associated_workflows = self.api_instance_workflows.list_workflows(
+            namespace=settings.NAMESPACE,
+            list_options_label_selector=f"openeo_job_id={openeo_job_id}",
+        ).items
+        associated_unfinished_workflows = [
+            workflow
+            for workflow in associated_workflows
+            if workflow.status.phase in ("Running", "Pending")
+        ]
+        logger.info(
+            f"Stopping OpenEO job {openeo_job_id} with"
+            f"{len(associated_unfinished_workflows)} unfinished sub-workflows."
+        )
+
+        # Need to stop all sub-jobs too!
+        for workflow in associated_unfinished_workflows:
+            if workflow.status.phase in ("Running", "Pending"):
+                workflow_name = workflow.metadata.name
+                super().stop_workflow(workflow_name)
+        logger.info(f"Successfully stopped OpenEO job {openeo_job_id}.")
+
 
 class Snap(FaasProcessorBase):
     @classmethod
     def get_instance(cls):
         return cls(processor_details=FaasProcessor.Snap.value)
 
     def submit_workflow(
@@ -263,15 +290,15 @@
     ):
         return super().submit_workflow(
             snap_parameters=snap_parameters.json(),
             user_id=user_id,
             job_id=job_id,
         )
 
-    def get_output_stac_items(self, snap_parameters: SnapParameters):
+    def get_output_stac_items(self, snap_parameters: SnapParameters) -> list[Item]:
         collection_file = list(snap_parameters.stac_path.glob("*_collection.json"))[0]
         snap_output_collection = Collection.from_file(str(collection_file))
         stac_items = [
             Item.from_file(link.get_absolute_href())
             for link in snap_output_collection.get_item_links()
         ]
```

### Comparing `eodc-2023.6.5/pyproject.toml` & `eodc-2023.6.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.6.5"
+version = "2023.6.6"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2023.6.5/PKG-INFO` & `eodc-2023.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.6.5
+Version: 2023.6.6
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

