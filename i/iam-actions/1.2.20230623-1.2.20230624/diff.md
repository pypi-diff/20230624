# Comparing `tmp/iam_actions-1.2.20230623.tar.gz` & `tmp/iam_actions-1.2.20230624.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230623.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230624.tar", max compression
```

## Comparing `iam_actions-1.2.20230623.tar` & `iam_actions-1.2.20230624.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/README.md
--rw-r--r--   0        0        0      228 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/__init__.py
--rw-r--r--   0        0        0  4341498 2023-06-23 02:54:44.404923 iam_actions-1.2.20230623/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/services.py
--rw-r--r--   0        0        0   558388 2023-06-23 02:54:44.404923 iam_actions-1.2.20230623/iam_actions/policies.json
--rw-r--r--   0        0        0   196684 2023-06-23 02:54:44.404923 iam_actions-1.2.20230623/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   541563 2023-06-23 02:54:44.404923 iam_actions-1.2.20230623/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-23 02:54:45.396926 iam_actions-1.2.20230623/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230623/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230623/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/README.md
+-rw-r--r--   0        0        0      228 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4345395 2023-06-24 02:54:20.015354 iam_actions-1.2.20230624/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-24 02:52:54.750103 iam_actions-1.2.20230624/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   558814 2023-06-24 02:54:20.015354 iam_actions-1.2.20230624/iam_actions/policies.json
+-rw-r--r--   0        0        0   196908 2023-06-24 02:54:20.015354 iam_actions-1.2.20230624/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   541974 2023-06-24 02:54:20.015354 iam_actions-1.2.20230624/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-24 02:54:20.847365 iam_actions-1.2.20230624/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230624/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230624/PKG-INFO
```

### Comparing `iam_actions-1.2.20230623/LICENSE` & `iam_actions-1.2.20230624/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230623/README.md` & `iam_actions-1.2.20230624/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230623/iam_actions/actions.json` & `iam_actions-1.2.20230624/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997644285759739%*

 * *Differences: {"'discovery'": "{'DeleteTags': {'condition_keys': ['aws:TagKeys']}, 'DescribeAgents': "*

 * *                "{'description': 'Grants permission to DescribeAgents API. DescribeAgents lists "*

 * *                'agents or the Connector by ID or lists all agents/Connectors associated with your '*

 * *                "user if you did not specify an ID'}, 'DescribeContinuousExports': {'description': "*

 * *                "'Grants permission to DescribeContinuousExports API. DescribeContinuousExports "*

 * *                'lists ex […]*

```diff
@@ -38529,24 +38529,26 @@
             "description": "Grants permission to DeleteApplications API. DeleteApplications deletes a list of applications and their associations with configuration items",
             "orphan": false,
             "resources": []
         },
         "DeleteTags": {
             "access_level": "Tagging",
             "action": "DeleteTags",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to DeleteTags API. DeleteTags deletes the association between configuration items and one or more tags. This API accepts a list of multiple configuration items",
             "orphan": false,
             "resources": []
         },
         "DescribeAgents": {
             "access_level": "Read",
             "action": "DescribeAgents",
             "condition_keys": [],
-            "description": "Grants permission to DescribeAgents API. DescribeAgents lists agents or the Connector by ID or lists all agents/Connectors associated with your user account if you did not specify an ID",
+            "description": "Grants permission to DescribeAgents API. DescribeAgents lists agents or the Connector by ID or lists all agents/Connectors associated with your user if you did not specify an ID",
             "orphan": false,
             "resources": []
         },
         "DescribeConfigurations": {
             "access_level": "Read",
             "action": "DescribeConfigurations",
             "condition_keys": [],
@@ -38554,15 +38556,15 @@
             "orphan": false,
             "resources": []
         },
         "DescribeContinuousExports": {
             "access_level": "Read",
             "action": "DescribeContinuousExports",
             "condition_keys": [],
-            "description": "Grants permission to DescribeContinuousExports API. DescribeContinuousExports lists exports as specified by ID. All continuous exports associated with your user account can be listed if you call DescribeContinuousExports as is without passing any parameters",
+            "description": "Grants permission to DescribeContinuousExports API. DescribeContinuousExports lists exports as specified by ID. All continuous exports associated with your user can be listed if you call DescribeContinuousExports as is without passing any parameters",
             "orphan": false,
             "resources": []
         },
         "DescribeExportConfigurations": {
             "access_level": "Read",
             "action": "DescribeExportConfigurations",
             "condition_keys": [],
@@ -38578,15 +38580,15 @@
             "orphan": false,
             "resources": []
         },
         "DescribeImportTasks": {
             "access_level": "List",
             "action": "DescribeImportTasks",
             "condition_keys": [],
-            "description": "Grants permission to DescribeImportTasks API. DescribeImportTasks returns an array of import tasks for your account, including status information, times, IDs, the Amazon S3 Object URL for the import file, and more",
+            "description": "Grants permission to DescribeImportTasks API. DescribeImportTasks returns an array of import tasks for your user, including status information, times, IDs, the Amazon S3 Object URL for the import file, and more",
             "orphan": false,
             "resources": []
         },
         "DescribeTags": {
             "access_level": "Read",
             "action": "DescribeTags",
             "condition_keys": [],
@@ -84520,20 +84522,22 @@
             "description": "Grants permission to query documents and faqs",
             "orphan": false,
             "resources": [
                 "index"
             ]
         },
         "Retrieve": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "Retrieve",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve relevant content from an index",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "index"
+            ]
         },
         "StartDataSourceSyncJob": {
             "access_level": "Write",
             "action": "StartDataSourceSyncJob",
             "condition_keys": [],
             "description": "Grants permission to start Data Source sync job",
             "orphan": false,
@@ -87900,14 +87904,30 @@
             "description": "Creates a new version based on the $LATEST version of the specified slot type",
             "orphan": false,
             "resources": [
                 "slottype",
                 "version"
             ]
         },
+        "CreateTestSet": {
+            "access_level": "Undocumented",
+            "action": "CreateTestSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateTestSetDiscrepancyReport": {
+            "access_level": "Undocumented",
+            "action": "CreateTestSetDiscrepancyReport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateUploadUrl": {
             "access_level": "Write",
             "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Grants permission to create an upload url for import file",
             "orphan": false,
             "resources": []
@@ -88074,14 +88094,22 @@
             "description": "Deletes a specific version of a slot type",
             "orphan": false,
             "resources": [
                 "slottype",
                 "version"
             ]
         },
+        "DeleteTestSet": {
+            "access_level": "Undocumented",
+            "action": "DeleteTestSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteUtterances": {
             "access_level": "Write",
             "action": "DeleteUtterances",
             "condition_keys": [],
             "description": "Grants permission to delete utterance data for a bot",
             "orphan": false,
             "resources": [
@@ -88226,14 +88254,46 @@
             "condition_keys": [],
             "description": "Grants permission to retrieve an existing slot type",
             "orphan": false,
             "resources": [
                 "bot"
             ]
         },
+        "DescribeTestExecution": {
+            "access_level": "Undocumented",
+            "action": "DescribeTestExecution",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeTestSet": {
+            "access_level": "Undocumented",
+            "action": "DescribeTestSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeTestSetDiscrepancyReport": {
+            "access_level": "Undocumented",
+            "action": "DescribeTestSetDiscrepancyReport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeTestSetGeneration": {
+            "access_level": "Undocumented",
+            "action": "DescribeTestSetGeneration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetBot": {
             "access_level": "Read",
             "action": "GetBot",
             "condition_keys": [],
             "description": "Returns information for a specific bot. In addition to the bot name, the bot version or alias is required",
             "orphan": false,
             "resources": [
@@ -88426,14 +88486,22 @@
             "access_level": "List",
             "action": "GetSlotTypes",
             "condition_keys": [],
             "description": "Returns information for the $LATEST version of all slot types, subject to filters provided by the client",
             "orphan": false,
             "resources": []
         },
+        "GetTestExecutionArtifactsUrl": {
+            "access_level": "Undocumented",
+            "action": "GetTestExecutionArtifactsUrl",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetUtterancesView": {
             "access_level": "List",
             "action": "GetUtterancesView",
             "condition_keys": [],
             "description": "Returns a view of aggregate utterance data for versions of a bot for a recent time period",
             "orphan": false,
             "resources": [
@@ -88598,14 +88666,46 @@
             "description": "Grants permission to lists tags for a Lex resource",
             "orphan": false,
             "resources": [
                 "alias",
                 "bot"
             ]
         },
+        "ListTestExecutionResultItems": {
+            "access_level": "Undocumented",
+            "action": "ListTestExecutionResultItems",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTestExecutions": {
+            "access_level": "Undocumented",
+            "action": "ListTestExecutions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTestSetRecords": {
+            "access_level": "Undocumented",
+            "action": "ListTestSetRecords",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTestSets": {
+            "access_level": "Undocumented",
+            "action": "ListTestSets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "PostContent": {
             "access_level": "Write",
             "action": "PostContent",
             "condition_keys": [],
             "description": "Sends user input (text or speech) to Amazon Lex",
             "orphan": false,
             "resources": [
@@ -88761,14 +88861,30 @@
             "description": "Grants permission to migrate a bot from Amazon Lex v1 to Amazon Lex v2",
             "orphan": false,
             "resources": [
                 "bot",
                 "version"
             ]
         },
+        "StartTestExecution": {
+            "access_level": "Undocumented",
+            "action": "StartTestExecution",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartTestSetGeneration": {
+            "access_level": "Undocumented",
+            "action": "StartTestSetGeneration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StopBotRecommendation": {
             "access_level": "Write",
             "action": "StopBotRecommendation",
             "condition_keys": [],
             "description": "Grants permission to stop a bot recommendation for an existing bot locale",
             "orphan": false,
             "resources": [
@@ -88900,14 +89016,22 @@
             "action": "UpdateSlotType",
             "condition_keys": [],
             "description": "Grants permission to update an existing slot type",
             "orphan": false,
             "resources": [
                 "bot"
             ]
+        },
+        "UpdateTestSet": {
+            "access_level": "Undocumented",
+            "action": "UpdateTestSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "license-manager": {
         "AcceptGrant": {
             "access_level": "Write",
             "action": "AcceptGrant",
             "condition_keys": [],
@@ -142223,20 +142347,24 @@
             "description": "Grants permission to create a state machine",
             "orphan": false,
             "resources": [
                 "statemachine"
             ]
         },
         "CreateStateMachineAlias": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateStateMachineAlias",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "states:StateMachineQualifier"
+            ],
+            "description": "Grants permission to create a state machine alias",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "statemachine"
+            ]
         },
         "DeleteActivity": {
             "access_level": "Write",
             "action": "DeleteActivity",
             "condition_keys": [],
             "description": "Grants permission to delete an activity",
             "orphan": false,
@@ -142251,28 +142379,36 @@
             "description": "Grants permission to delete a state machine",
             "orphan": false,
             "resources": [
                 "statemachine"
             ]
         },
         "DeleteStateMachineAlias": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteStateMachineAlias",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "states:StateMachineQualifier"
+            ],
+            "description": "Grants permission to delete a state machine alias",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "statemachine"
+            ]
         },
         "DeleteStateMachineVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteStateMachineVersion",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "states:StateMachineQualifier"
+            ],
+            "description": "Grants permission to delete a state machine version",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "statemachine"
+            ]
         },
         "DescribeActivity": {
             "access_level": "Read",
             "action": "DescribeActivity",
             "condition_keys": [],
             "description": "Grants permission to describe an activity",
             "orphan": false,
@@ -142300,28 +142436,34 @@
             "resources": [
                 "maprun"
             ]
         },
         "DescribeStateMachine": {
             "access_level": "Read",
             "action": "DescribeStateMachine",
-            "condition_keys": [],
+            "condition_keys": [
+                "states:StateMachineQualifier"
+            ],
             "description": "Grants permission to describe a state machine",
             "orphan": false,
             "resources": [
                 "statemachine"
             ]
         },
         "DescribeStateMachineAlias": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeStateMachineAlias",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "states:StateMachineQualifier"
+            ],
+            "description": "Grants permission to describe a state machine alias",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "statemachine"
+            ]
         },
         "DescribeStateMachineForExecution": {
             "access_level": "Read",
             "action": "DescribeStateMachineForExecution",
             "condition_keys": [],
             "description": "Grants permission to describe the state machine for an execution",
             "orphan": false,
@@ -142354,17 +142496,19 @@
             "action": "ListActivities",
             "condition_keys": [],
             "description": "Grants permission to list the existing activities",
             "orphan": false,
             "resources": []
         },
         "ListExecutions": {
-            "access_level": "Read",
+            "access_level": "List",
             "action": "ListExecutions",
-            "condition_keys": [],
+            "condition_keys": [
+                "states:StateMachineQualifier"
+            ],
             "description": "Grants permission to list the executions of a state machine",
             "orphan": false,
             "resources": [
                 "maprun",
                 "statemachine"
             ]
         },
@@ -142375,55 +142519,63 @@
             "description": "Grants permission to list the map runs of an execution",
             "orphan": false,
             "resources": [
                 "execution"
             ]
         },
         "ListStateMachineAliases": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListStateMachineAliases",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "states:StateMachineQualifier"
+            ],
+            "description": "Grants permission to list the aliases of a state machine",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "statemachine"
+            ]
         },
         "ListStateMachineVersions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListStateMachineVersions",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list the versions of a state machine",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "statemachine"
+            ]
         },
         "ListStateMachines": {
             "access_level": "List",
             "action": "ListStateMachines",
             "condition_keys": [],
             "description": "Grants permission to lists the existing state machines",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
-            "access_level": "Read",
+            "access_level": "List",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags for an AWS Step Functions resource",
             "orphan": false,
             "resources": [
                 "activity",
                 "statemachine"
             ]
         },
         "PublishStateMachineVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PublishStateMachineVersion",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to publish a state machine version",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "statemachine"
+            ]
         },
         "SendTaskFailure": {
             "access_level": "Write",
             "action": "SendTaskFailure",
             "condition_keys": [],
             "description": "Grants permission to report that the task identified by the taskToken failed",
             "orphan": false,
@@ -142444,25 +142596,29 @@
             "description": "Grants permission to report that the task identified by the taskToken completed successfully",
             "orphan": false,
             "resources": []
         },
         "StartExecution": {
             "access_level": "Write",
             "action": "StartExecution",
-            "condition_keys": [],
+            "condition_keys": [
+                "states:StateMachineQualifier"
+            ],
             "description": "Grants permission to start a state machine execution",
             "orphan": false,
             "resources": [
                 "statemachine"
             ]
         },
         "StartSyncExecution": {
             "access_level": "Write",
             "action": "StartSyncExecution",
-            "condition_keys": [],
+            "condition_keys": [
+                "states:StateMachineQualifier"
+            ],
             "description": "Grants permission to start a Synchronous Express state machine execution",
             "orphan": false,
             "resources": [
                 "statemachine"
             ]
         },
         "StopExecution": {
@@ -142522,20 +142678,24 @@
             "description": "Grants permission to update a state machine",
             "orphan": false,
             "resources": [
                 "statemachine"
             ]
         },
         "UpdateStateMachineAlias": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateStateMachineAlias",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "states:StateMachineQualifier"
+            ],
+            "description": "Grants permission to update a state machine alias",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "statemachine"
+            ]
         }
     },
     "storagegateway": {
         "ActivateGateway": {
             "access_level": "Write",
             "action": "ActivateGateway",
             "condition_keys": [
@@ -143116,37 +143276,31 @@
         },
         "ListAutomaticTapeCreationPolicies": {
             "access_level": "List",
             "action": "ListAutomaticTapeCreationPolicies",
             "condition_keys": [],
             "description": "Grants permission to list the automatic tape creation policies configured on the specified gateway-VTL or all gateway-VTLs owned by your account",
             "orphan": false,
-            "resources": [
-                "gateway"
-            ]
+            "resources": []
         },
         "ListFileShares": {
             "access_level": "List",
             "action": "ListFileShares",
             "condition_keys": [],
             "description": "Grants permission to get a list of the file shares for a specific file gateway, or the list of file shares that belong to the calling user account",
             "orphan": false,
-            "resources": [
-                "gateway"
-            ]
+            "resources": []
         },
         "ListFileSystemAssociations": {
             "access_level": "List",
             "action": "ListFileSystemAssociations",
             "condition_keys": [],
             "description": "Grants permission to get a list of the file system associations for the specified gateway",
             "orphan": false,
-            "resources": [
-                "gateway"
-            ]
+            "resources": []
         },
         "ListGateways": {
             "access_level": "List",
             "action": "ListGateways",
             "condition_keys": [],
             "description": "Grants permission to list gateways owned by an AWS account in a region specified in the request. The returned list is ordered by gateway Amazon Resource Name (ARN)",
             "orphan": false,
@@ -143177,27 +143331,23 @@
         },
         "ListTapePools": {
             "access_level": "List",
             "action": "ListTapePools",
             "condition_keys": [],
             "description": "Grants permission to list tape pools owned by your AWS account",
             "orphan": false,
-            "resources": [
-                "tapepool"
-            ]
+            "resources": []
         },
         "ListTapes": {
             "access_level": "List",
             "action": "ListTapes",
             "condition_keys": [],
             "description": "Grants permission to list virtual tapes in your virtual tape library (VTL) and your virtual tape shelf (VTS)",
             "orphan": false,
-            "resources": [
-                "tape"
-            ]
+            "resources": []
         },
         "ListVolumeInitiators": {
             "access_level": "List",
             "action": "ListVolumeInitiators",
             "condition_keys": [],
             "description": "Grants permission to list iSCSI initiators that are connected to a volume",
             "orphan": false,
@@ -143217,17 +143367,15 @@
         },
         "ListVolumes": {
             "access_level": "List",
             "action": "ListVolumes",
             "condition_keys": [],
             "description": "Grants permission to list the iSCSI stored volumes of a gateway",
             "orphan": false,
-            "resources": [
-                "gateway"
-            ]
+            "resources": []
         },
         "NotifyWhenUploaded": {
             "access_level": "Write",
             "action": "NotifyWhenUploaded",
             "condition_keys": [],
             "description": "Grants permission to send you a notification through CloudWatch Events when all files written to your NFS file share have been uploaded to Amazon S3",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230623/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230624/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230623/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230624/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230623/iam_actions/generate/generate.py` & `iam_actions-1.2.20230624/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230623/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230624/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230623/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230624/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230623/iam_actions/generate/services.py` & `iam_actions-1.2.20230624/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230623/iam_actions/policies.json` & `iam_actions-1.2.20230624/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999982999211163%*

 * *Differences: {"'serviceMap'": "{'Amazon Lex V2': {'Actions': {insert: [(15, 'CreateTestSet'), (16, "*

 * *                 "'CreateTestSetDiscrepancyReport'), (31, 'DeleteTestSet'), (47, "*

 * *                 "'DescribeTestExecution'), (48, 'DescribeTestSet'), (49, "*

 * *                 "'DescribeTestSetDiscrepancyReport'), (50, 'DescribeTestSetGeneration'), (52, "*

 * *                 "'GetTestExecutionArtifactsUrl'), (70, 'ListTestExecutionResultItems'), (71, "*

 * *                 "'ListTestExecutions'), (72, 'ListTestSetRecords'), (73 […]*

```diff
@@ -15186,28 +15186,31 @@
                 "CreateBotVersion",
                 "CreateCustomVocabulary",
                 "CreateExport",
                 "CreateIntent",
                 "CreateResourcePolicy",
                 "CreateSlot",
                 "CreateSlotType",
+                "CreateTestSet",
+                "CreateTestSetDiscrepancyReport",
                 "CreateUploadUrl",
                 "DeleteBot",
                 "DeleteBotAlias",
                 "DeleteBotChannel",
                 "DeleteBotLocale",
                 "DeleteBotVersion",
                 "DeleteCustomVocabulary",
                 "DeleteExport",
                 "DeleteImport",
                 "DeleteIntent",
                 "DeleteResourcePolicy",
                 "DeleteSession",
                 "DeleteSlot",
                 "DeleteSlotType",
+                "DeleteTestSet",
                 "DeleteUtterances",
                 "DescribeBot",
                 "DescribeBotAlias",
                 "DescribeBotChannel",
                 "DescribeBotLocale",
                 "DescribeBotRecommendation",
                 "DescribeBotVersion",
@@ -15215,15 +15218,20 @@
                 "DescribeCustomVocabularyMetadata",
                 "DescribeExport",
                 "DescribeImport",
                 "DescribeIntent",
                 "DescribeResourcePolicy",
                 "DescribeSlot",
                 "DescribeSlotType",
+                "DescribeTestExecution",
+                "DescribeTestSet",
+                "DescribeTestSetDiscrepancyReport",
+                "DescribeTestSetGeneration",
                 "GetSession",
+                "GetTestExecutionArtifactsUrl",
                 "ListAggregatedUtterances",
                 "ListBotAliases",
                 "ListBotChannels",
                 "ListBotLocales",
                 "ListBotRecommendations",
                 "ListBotVersions",
                 "ListBots",
@@ -15233,34 +15241,41 @@
                 "ListExports",
                 "ListImports",
                 "ListIntents",
                 "ListRecommendedIntents",
                 "ListSlotTypes",
                 "ListSlots",
                 "ListTagsForResource",
+                "ListTestExecutionResultItems",
+                "ListTestExecutions",
+                "ListTestSetRecords",
+                "ListTestSets",
                 "PutSession",
                 "RecognizeText",
                 "RecognizeUtterance",
                 "SearchAssociatedTranscripts",
                 "StartBotRecommendation",
                 "StartConversation",
                 "StartImport",
+                "StartTestExecution",
+                "StartTestSetGeneration",
                 "StopBotRecommendation",
                 "TagResource",
                 "UntagResource",
                 "UpdateBot",
                 "UpdateBotAlias",
                 "UpdateBotLocale",
                 "UpdateBotRecommendation",
                 "UpdateCustomVocabulary",
                 "UpdateExport",
                 "UpdateIntent",
                 "UpdateResourcePolicy",
                 "UpdateSlot",
-                "UpdateSlotType"
+                "UpdateSlotType",
+                "UpdateTestSet"
             ],
             "HasResource": true,
             "StringPrefix": "lex",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
```

### Comparing `iam_actions-1.2.20230623/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230624/iam_actions/resourcetypes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996053670086819%*

 * *Differences: {"'states'": "{'statemachineversion': OrderedDict([('arn_pattern', "*

 * *             "'arn:*:states:*:*:stateMachine:*:*'), ('condition_keys', None)]), "*

 * *             "'statemachinealias': OrderedDict([('arn_pattern', "*

 * *             "'arn:*:states:*:*:stateMachine:*:*'), ('condition_keys', None)])}"}*

```diff
@@ -6176,14 +6176,22 @@
         "maprun": {
             "arn_pattern": "arn:*:states:*:*:mapRun:*/*:*",
             "condition_keys": null
         },
         "statemachine": {
             "arn_pattern": "arn:*:states:*:*:stateMachine:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "statemachinealias": {
+            "arn_pattern": "arn:*:states:*:*:stateMachine:*:*",
+            "condition_keys": null
+        },
+        "statemachineversion": {
+            "arn_pattern": "arn:*:states:*:*:stateMachine:*:*",
+            "condition_keys": null
         }
     },
     "storagegateway": {
         "device": {
             "arn_pattern": "arn:*:storagegateway:*:*:gateway/*/device/*",
             "condition_keys": null
         },
```

### Comparing `iam_actions-1.2.20230623/iam_actions/services.json` & `iam_actions-1.2.20230624/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999986719082023%*

 * *Differences: {"'lex'": "{'Actions': {insert: [(17, 'CreateTestSet'), (18, 'CreateTestSetDiscrepancyReport'), "*

 * *          "(36, 'DeleteTestSet'), (52, 'DescribeTestExecution'), (53, 'DescribeTestSet'), (54, "*

 * *          "'DescribeTestSetDiscrepancyReport'), (55, 'DescribeTestSetGeneration'), (77, "*

 * *          "'GetTestExecutionArtifactsUrl'), (96, 'ListTestExecutionResultItems'), (97, "*

 * *          "'ListTestExecutions'), (98, 'ListTestSetRecords'), (99, 'ListTestSets'), (114, "*

 * *          "'StartTestExecution'), (115, 'Start […]*

```diff
@@ -12226,14 +12226,16 @@
             "CreateExport",
             "CreateIntent",
             "CreateIntentVersion",
             "CreateResourcePolicy",
             "CreateSlot",
             "CreateSlotType",
             "CreateSlotTypeVersion",
+            "CreateTestSet",
+            "CreateTestSetDiscrepancyReport",
             "CreateUploadUrl",
             "DeleteBot",
             "DeleteBotAlias",
             "DeleteBotChannel",
             "DeleteBotChannelAssociation",
             "DeleteBotLocale",
             "DeleteBotVersion",
@@ -12243,14 +12245,15 @@
             "DeleteIntent",
             "DeleteIntentVersion",
             "DeleteResourcePolicy",
             "DeleteSession",
             "DeleteSlot",
             "DeleteSlotType",
             "DeleteSlotTypeVersion",
+            "DeleteTestSet",
             "DeleteUtterances",
             "DescribeBot",
             "DescribeBotAlias",
             "DescribeBotChannel",
             "DescribeBotLocale",
             "DescribeBotRecommendation",
             "DescribeBotVersion",
@@ -12258,14 +12261,18 @@
             "DescribeCustomVocabularyMetadata",
             "DescribeExport",
             "DescribeImport",
             "DescribeIntent",
             "DescribeResourcePolicy",
             "DescribeSlot",
             "DescribeSlotType",
+            "DescribeTestExecution",
+            "DescribeTestSet",
+            "DescribeTestSetDiscrepancyReport",
+            "DescribeTestSetGeneration",
             "GetBot",
             "GetBotAlias",
             "GetBotAliases",
             "GetBotChannelAssociation",
             "GetBotChannelAssociations",
             "GetBotVersions",
             "GetBots",
@@ -12279,14 +12286,15 @@
             "GetIntents",
             "GetMigration",
             "GetMigrations",
             "GetSession",
             "GetSlotType",
             "GetSlotTypeVersions",
             "GetSlotTypes",
+            "GetTestExecutionArtifactsUrl",
             "GetUtterancesView",
             "ListAggregatedUtterances",
             "ListBotAliases",
             "ListBotChannels",
             "ListBotLocales",
             "ListBotRecommendations",
             "ListBotVersions",
@@ -12297,41 +12305,48 @@
             "ListExports",
             "ListImports",
             "ListIntents",
             "ListRecommendedIntents",
             "ListSlotTypes",
             "ListSlots",
             "ListTagsForResource",
+            "ListTestExecutionResultItems",
+            "ListTestExecutions",
+            "ListTestSetRecords",
+            "ListTestSets",
             "PostContent",
             "PostText",
             "PutBot",
             "PutBotAlias",
             "PutIntent",
             "PutSession",
             "PutSlotType",
             "RecognizeText",
             "RecognizeUtterance",
             "SearchAssociatedTranscripts",
             "StartBotRecommendation",
             "StartConversation",
             "StartImport",
             "StartMigration",
+            "StartTestExecution",
+            "StartTestSetGeneration",
             "StopBotRecommendation",
             "TagResource",
             "UntagResource",
             "UpdateBot",
             "UpdateBotAlias",
             "UpdateBotLocale",
             "UpdateBotRecommendation",
             "UpdateCustomVocabulary",
             "UpdateExport",
             "UpdateIntent",
             "UpdateResourcePolicy",
             "UpdateSlot",
-            "UpdateSlotType"
+            "UpdateSlotType",
+            "UpdateTestSet"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
             "lex:associatedIntents",
             "lex:associatedSlotTypes",
```

### Comparing `iam_actions-1.2.20230623/pyproject.toml` & `iam_actions-1.2.20230624/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230623"
+version = "1.2.20230624"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230623/setup.py` & `iam_actions-1.2.20230624/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230623',
+    'version': '1.2.20230624',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230623/PKG-INFO` & `iam_actions-1.2.20230624/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230623
+Version: 1.2.20230624
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

