# Comparing `tmp/iam_actions-1.2.20240528.tar.gz` & `tmp/iam_actions-1.2.20240529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240528.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240529.tar", max compression
```

## Comparing `iam_actions-1.2.20240528.tar` & `iam_actions-1.2.20240529.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/README.md
--rw-r--r--   0        0        0      228 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/iam_actions/__init__.py
--rw-r--r--   0        0        0  4851189 2024-05-28 02:25:47.613408 iam_actions-1.2.20240528/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-28 02:24:25.012668 iam_actions-1.2.20240528/iam_actions/generate/services.py
--rw-r--r--   0        0        0   631710 2024-05-28 02:25:47.613408 iam_actions-1.2.20240528/iam_actions/policies.json
--rw-r--r--   0        0        0   209748 2024-05-28 02:25:47.613408 iam_actions-1.2.20240528/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   612689 2024-05-28 02:25:47.613408 iam_actions-1.2.20240528/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-28 02:25:48.305413 iam_actions-1.2.20240528/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240528/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240528/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/README.md
+-rw-r--r--   0        0        0      228 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4854274 2024-05-29 02:28:01.721773 iam_actions-1.2.20240529/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   632109 2024-05-29 02:28:01.721773 iam_actions-1.2.20240529/iam_actions/policies.json
+-rw-r--r--   0        0        0   209748 2024-05-29 02:28:01.721773 iam_actions-1.2.20240529/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   613075 2024-05-29 02:28:01.721773 iam_actions-1.2.20240529/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-29 02:28:02.397773 iam_actions-1.2.20240529/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240529/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240529/PKG-INFO
```

### Comparing `iam_actions-1.2.20240528/LICENSE` & `iam_actions-1.2.20240529/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240528/README.md` & `iam_actions-1.2.20240529/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240528/iam_actions/actions.json` & `iam_actions-1.2.20240529/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999892123774928%*

 * *Differences: {"'glue'": "{'DescribeEntity': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *           "'DescribeEntity'), ('condition_keys', []), ('description', 'Not Documented by AWS'), "*

 * *           "('orphan', False), ('resources', [])]), 'GetDataQualityModelResult': "*

 * *           "OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *           "'GetDataQualityModelResult'), ('condition_keys', []), ('description', 'Not Documented "*

 * *           "by AWS'), ('orphan', False), ('resources', [])]), 'Refr […]*

```diff
@@ -76084,14 +76084,22 @@
             "condition_keys": [],
             "description": "Grants permission to retrieve one or more workflows",
             "orphan": false,
             "resources": [
                 "workflow"
             ]
         },
+        "BatchPutDataQualityStatisticAnnotation": {
+            "access_level": "Undocumented",
+            "action": "BatchPutDataQualityStatisticAnnotation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "BatchStopJobRun": {
             "access_level": "Write",
             "action": "BatchStopJobRun",
             "condition_keys": [],
             "description": "Grants permission to stop one or more job runs for a job",
             "orphan": false,
             "resources": [
@@ -76698,14 +76706,30 @@
             "access_level": "Permissions management",
             "action": "DeregisterDataPreview",
             "condition_keys": [],
             "description": "Grants permission to terminate Glue Studio Notebook session",
             "orphan": false,
             "resources": []
         },
+        "DescribeConnectionType": {
+            "access_level": "Undocumented",
+            "action": "DescribeConnectionType",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeEntity": {
+            "access_level": "Undocumented",
+            "action": "DescribeEntity",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetBlueprint": {
             "access_level": "Read",
             "action": "GetBlueprint",
             "condition_keys": [],
             "description": "Grants permission to retrieve a blueprint",
             "orphan": false,
             "resources": [
@@ -76880,14 +76904,30 @@
             "access_level": "Permissions management",
             "action": "GetDataPreviewStatement",
             "condition_keys": [],
             "description": "Grants permission to get Data Preview Statement",
             "orphan": false,
             "resources": []
         },
+        "GetDataQualityModel": {
+            "access_level": "Undocumented",
+            "action": "GetDataQualityModel",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetDataQualityModelResult": {
+            "access_level": "Undocumented",
+            "action": "GetDataQualityModelResult",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetDataQualityResult": {
             "access_level": "Read",
             "action": "GetDataQualityResult",
             "condition_keys": [],
             "description": "Grants permission to retrieve a Data Quality result",
             "orphan": false,
             "resources": [
@@ -77536,14 +77576,22 @@
             "access_level": "Read",
             "action": "ListColumnStatisticsTaskRuns",
             "condition_keys": [],
             "description": "Grants permission to list all Column Statistics run-ids that have been executed for the account",
             "orphan": false,
             "resources": []
         },
+        "ListConnectionTypes": {
+            "access_level": "Undocumented",
+            "action": "ListConnectionTypes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListCrawlers": {
             "access_level": "List",
             "action": "ListCrawlers",
             "condition_keys": [],
             "description": "Grants permission to retrieve all crawlers",
             "orphan": false,
             "resources": []
@@ -77600,22 +77648,46 @@
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of Data Quality rulesets",
             "orphan": false,
             "resources": [
                 "dataQualityRuleset"
             ]
         },
+        "ListDataQualityStatisticAnnotations": {
+            "access_level": "Undocumented",
+            "action": "ListDataQualityStatisticAnnotations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListDataQualityStatistics": {
+            "access_level": "Undocumented",
+            "action": "ListDataQualityStatistics",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListDevEndpoints": {
             "access_level": "List",
             "action": "ListDevEndpoints",
             "condition_keys": [],
             "description": "Grants permission to retrieve all development endpoints",
             "orphan": false,
             "resources": []
         },
+        "ListEntities": {
+            "access_level": "Undocumented",
+            "action": "ListEntities",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListJobs": {
             "access_level": "List",
             "action": "ListJobs",
             "condition_keys": [],
             "description": "Grants permission to retrieve all current jobs",
             "orphan": false,
             "resources": []
@@ -77741,14 +77813,22 @@
             "condition_keys": [],
             "description": "Grants permission to update catalog encryption settings",
             "orphan": false,
             "resources": [
                 "catalog"
             ]
         },
+        "PutDataQualityProfileAnnotation": {
+            "access_level": "Undocumented",
+            "action": "PutDataQualityProfileAnnotation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "PutResourcePolicy": {
             "access_level": "Permissions management",
             "action": "PutResourcePolicy",
             "condition_keys": [],
             "description": "Grants permission to update a resource policy",
             "orphan": false,
             "resources": [
@@ -77783,14 +77863,22 @@
             "description": "Grants permission to fetch metadata for a schema version",
             "orphan": false,
             "resources": [
                 "registry",
                 "schema"
             ]
         },
+        "RefreshOAuth2Tokens": {
+            "access_level": "Undocumented",
+            "action": "RefreshOAuth2Tokens",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "RegisterSchemaVersion": {
             "access_level": "Write",
             "action": "RegisterSchemaVersion",
             "condition_keys": [],
             "description": "Grants permission to create a new schema version",
             "orphan": false,
             "resources": [
@@ -83601,15 +83689,15 @@
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to import an image",
             "orphan": false,
             "resources": [
-                "image"
+                "imageVersion"
             ]
         },
         "ListComponentBuildVersions": {
             "access_level": "List",
             "action": "ListComponentBuildVersions",
             "condition_keys": [],
             "description": "Grants permission to list the component build versions in your account",
@@ -155479,25 +155567,29 @@
             "resources": [
                 "opsmetadata"
             ]
         },
         "DeleteParameter": {
             "access_level": "Write",
             "action": "DeleteParameter",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to delete a specified SSM parameter",
             "orphan": false,
             "resources": [
                 "parameter"
             ]
         },
         "DeleteParameters": {
             "access_level": "Write",
             "action": "DeleteParameters",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to delete multiple specified SSM parameters",
             "orphan": false,
             "resources": [
                 "parameter"
             ]
         },
         "DeletePatchBaseline": {
@@ -156079,35 +156171,41 @@
             "resources": [
                 "resourcedatasync"
             ]
         },
         "GetParameter": {
             "access_level": "Read",
             "action": "GetParameter",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to view information about a specified parameter",
             "orphan": false,
             "resources": [
                 "parameter"
             ]
         },
         "GetParameterHistory": {
             "access_level": "Read",
             "action": "GetParameterHistory",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to view details and changes for a specified parameter",
             "orphan": false,
             "resources": [
                 "parameter"
             ]
         },
         "GetParameters": {
             "access_level": "Read",
             "action": "GetParameters",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to view information about multiple specified parameters",
             "orphan": false,
             "resources": [
                 "parameter"
             ]
         },
         "GetParametersByPath": {
@@ -156159,15 +156257,17 @@
             "resources": [
                 "servicesetting"
             ]
         },
         "LabelParameterVersion": {
             "access_level": "Write",
             "action": "LabelParameterVersion",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to apply an identifying label to a specified version of a parameter",
             "orphan": false,
             "resources": [
                 "parameter"
             ]
         },
         "ListAssociationVersions": {
@@ -156608,15 +156708,17 @@
             "resources": [
                 "session"
             ]
         },
         "UnlabelParameterVersion": {
             "access_level": "Write",
             "action": "UnlabelParameterVersion",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to remove an identifying label from a specified version of a parameter",
             "orphan": false,
             "resources": [
                 "parameter"
             ]
         },
         "UpdateAssociation": {
@@ -161538,14 +161640,30 @@
             ],
             "description": "Grants permission to return the estimated number of decision tasks in the specified task list",
             "orphan": false,
             "resources": [
                 "domain"
             ]
         },
+        "DeleteActivityType": {
+            "access_level": "Undocumented",
+            "action": "DeleteActivityType",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteWorkflowType": {
+            "access_level": "Undocumented",
+            "action": "DeleteWorkflowType",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeprecateActivityType": {
             "access_level": "Write",
             "action": "DeprecateActivityType",
             "condition_keys": [
                 "swf:activityType.name",
                 "swf:activityType.version"
             ],
```

### Comparing `iam_actions-1.2.20240528/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240529/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240528/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240529/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240528/iam_actions/generate/generate.py` & `iam_actions-1.2.20240529/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240528/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240529/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240528/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240529/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240528/iam_actions/generate/services.py` & `iam_actions-1.2.20240529/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240528/iam_actions/policies.json` & `iam_actions-1.2.20240529/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999991677340263%*

 * *Differences: {"'serviceMap'": "{'AWS Glue': {'Actions': {insert: [(15, "*

 * *                 "'BatchPutDataQualityStatisticAnnotation'), (72, 'DescribeConnectionType'), (73, "*

 * *                 "'DescribeEntity'), (93, 'GetDataQualityModel'), (94, "*

 * *                 "'GetDataQualityModelResult'), (163, 'ListConnectionTypes'), (171, "*

 * *                 "'ListDataQualityStatisticAnnotations'), (172, 'ListDataQualityStatistics'), "*

 * *                 "(174, 'ListEntities'), (189, 'PutDataQualityProfileAnnotation'), (194, "*

 * *       […]*

```diff
@@ -4795,14 +4795,15 @@
                 "BatchGetDevEndpoints",
                 "BatchGetJobs",
                 "BatchGetPartition",
                 "BatchGetStageFiles",
                 "BatchGetTableOptimizer",
                 "BatchGetTriggers",
                 "BatchGetWorkflows",
+                "BatchPutDataQualityStatisticAnnotation",
                 "BatchStopJobRun",
                 "BatchUpdatePartition",
                 "CancelDataQualityRuleRecommendationRun",
                 "CancelDataQualityRulesetEvaluationRun",
                 "CancelMLTaskRun",
                 "CancelStatement",
                 "CheckSchemaVersionValidity",
@@ -4851,14 +4852,16 @@
                 "DeleteTable",
                 "DeleteTableOptimizer",
                 "DeleteTableVersion",
                 "DeleteTrigger",
                 "DeleteUserDefinedFunction",
                 "DeleteWorkflow",
                 "DeregisterDataPreview",
+                "DescribeConnectionType",
+                "DescribeEntity",
                 "GetBlueprint",
                 "GetBlueprintRun",
                 "GetBlueprintRuns",
                 "GetCatalogImportStatus",
                 "GetClassifier",
                 "GetClassifiers",
                 "GetColumnStatisticsForPartition",
@@ -4870,14 +4873,16 @@
                 "GetConnections",
                 "GetCrawler",
                 "GetCrawlerMetrics",
                 "GetCrawlers",
                 "GetCustomEntityType",
                 "GetDataCatalogEncryptionSettings",
                 "GetDataPreviewStatement",
+                "GetDataQualityModel",
+                "GetDataQualityModelResult",
                 "GetDataQualityResult",
                 "GetDataQualityRuleRecommendationRun",
                 "GetDataQualityRuleset",
                 "GetDataQualityRulesetEvaluationRun",
                 "GetDatabase",
                 "GetDatabases",
                 "GetDataflowGraph",
@@ -4938,40 +4943,46 @@
                 "GetWorkflowRunProperties",
                 "GetWorkflowRuns",
                 "GlueNotebookAuthorize",
                 "GlueNotebookRefreshCredentials",
                 "ImportCatalogToGlue",
                 "ListBlueprints",
                 "ListColumnStatisticsTaskRuns",
+                "ListConnectionTypes",
                 "ListCrawlers",
                 "ListCrawls",
                 "ListCustomEntityTypes",
                 "ListDataQualityResults",
                 "ListDataQualityRuleRecommendationRuns",
                 "ListDataQualityRulesetEvaluationRuns",
                 "ListDataQualityRulesets",
+                "ListDataQualityStatisticAnnotations",
+                "ListDataQualityStatistics",
                 "ListDevEndpoints",
+                "ListEntities",
                 "ListJobs",
                 "ListMLTransforms",
                 "ListRegistries",
                 "ListSchemaVersions",
                 "ListSchemas",
                 "ListSessions",
                 "ListStatements",
                 "ListTableOptimizerRuns",
                 "ListTriggers",
                 "ListWorkflows",
                 "NotifyEvent",
                 "PassConnection",
                 "PublishDataQuality",
                 "PutDataCatalogEncryptionSettings",
+                "PutDataQualityProfileAnnotation",
                 "PutResourcePolicy",
                 "PutSchemaVersionMetadata",
                 "PutWorkflowRunProperties",
                 "QuerySchemaVersionMetadata",
+                "RefreshOAuth2Tokens",
                 "RegisterSchemaVersion",
                 "RemoveSchemaVersionMetadata",
                 "RequestLogParsing",
                 "ResetJobBookmark",
                 "ResumeWorkflowRun",
                 "RunDataPreviewStatement",
                 "RunStatement",
@@ -21601,14 +21612,16 @@
                 "CancelWorkflowExecution",
                 "CompleteWorkflowExecution",
                 "ContinueAsNewWorkflowExecution",
                 "CountClosedWorkflowExecutions",
                 "CountOpenWorkflowExecutions",
                 "CountPendingActivityTasks",
                 "CountPendingDecisionTasks",
+                "DeleteActivityType",
+                "DeleteWorkflowType",
                 "DeprecateActivityType",
                 "DeprecateDomain",
                 "DeprecateWorkflowType",
                 "DescribeActivityType",
                 "DescribeDomain",
                 "DescribeWorkflowExecution",
                 "DescribeWorkflowType",
```

### Comparing `iam_actions-1.2.20240528/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240529/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240528/iam_actions/services.json` & `iam_actions-1.2.20240529/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999912770097948%*

 * *Differences: {"'glue'": "{'Actions': {insert: [(15, 'BatchPutDataQualityStatisticAnnotation'), (72, "*

 * *           "'DescribeConnectionType'), (73, 'DescribeEntity'), (93, 'GetDataQualityModel'), (94, "*

 * *           "'GetDataQualityModelResult'), (163, 'ListConnectionTypes'), (171, "*

 * *           "'ListDataQualityStatisticAnnotations'), (172, 'ListDataQualityStatistics'), (174, "*

 * *           "'ListEntities'), (189, 'PutDataQualityProfileAnnotation'), (194, "*

 * *           "'RefreshOAuth2Tokens')]}}",*

 * * "'swf'": "{'Actions': {inser […]*

```diff
@@ -10405,14 +10405,15 @@
             "BatchGetDevEndpoints",
             "BatchGetJobs",
             "BatchGetPartition",
             "BatchGetStageFiles",
             "BatchGetTableOptimizer",
             "BatchGetTriggers",
             "BatchGetWorkflows",
+            "BatchPutDataQualityStatisticAnnotation",
             "BatchStopJobRun",
             "BatchUpdatePartition",
             "CancelDataQualityRuleRecommendationRun",
             "CancelDataQualityRulesetEvaluationRun",
             "CancelMLTaskRun",
             "CancelStatement",
             "CheckSchemaVersionValidity",
@@ -10461,14 +10462,16 @@
             "DeleteTable",
             "DeleteTableOptimizer",
             "DeleteTableVersion",
             "DeleteTrigger",
             "DeleteUserDefinedFunction",
             "DeleteWorkflow",
             "DeregisterDataPreview",
+            "DescribeConnectionType",
+            "DescribeEntity",
             "GetBlueprint",
             "GetBlueprintRun",
             "GetBlueprintRuns",
             "GetCatalogImportStatus",
             "GetClassifier",
             "GetClassifiers",
             "GetColumnStatisticsForPartition",
@@ -10480,14 +10483,16 @@
             "GetConnections",
             "GetCrawler",
             "GetCrawlerMetrics",
             "GetCrawlers",
             "GetCustomEntityType",
             "GetDataCatalogEncryptionSettings",
             "GetDataPreviewStatement",
+            "GetDataQualityModel",
+            "GetDataQualityModelResult",
             "GetDataQualityResult",
             "GetDataQualityRuleRecommendationRun",
             "GetDataQualityRuleset",
             "GetDataQualityRulesetEvaluationRun",
             "GetDatabase",
             "GetDatabases",
             "GetDataflowGraph",
@@ -10548,40 +10553,46 @@
             "GetWorkflowRunProperties",
             "GetWorkflowRuns",
             "GlueNotebookAuthorize",
             "GlueNotebookRefreshCredentials",
             "ImportCatalogToGlue",
             "ListBlueprints",
             "ListColumnStatisticsTaskRuns",
+            "ListConnectionTypes",
             "ListCrawlers",
             "ListCrawls",
             "ListCustomEntityTypes",
             "ListDataQualityResults",
             "ListDataQualityRuleRecommendationRuns",
             "ListDataQualityRulesetEvaluationRuns",
             "ListDataQualityRulesets",
+            "ListDataQualityStatisticAnnotations",
+            "ListDataQualityStatistics",
             "ListDevEndpoints",
+            "ListEntities",
             "ListJobs",
             "ListMLTransforms",
             "ListRegistries",
             "ListSchemaVersions",
             "ListSchemas",
             "ListSessions",
             "ListStatements",
             "ListTableOptimizerRuns",
             "ListTriggers",
             "ListWorkflows",
             "NotifyEvent",
             "PassConnection",
             "PublishDataQuality",
             "PutDataCatalogEncryptionSettings",
+            "PutDataQualityProfileAnnotation",
             "PutResourcePolicy",
             "PutSchemaVersionMetadata",
             "PutWorkflowRunProperties",
             "QuerySchemaVersionMetadata",
+            "RefreshOAuth2Tokens",
             "RegisterSchemaVersion",
             "RemoveSchemaVersionMetadata",
             "RequestLogParsing",
             "ResetJobBookmark",
             "ResumeWorkflowRun",
             "RunDataPreviewStatement",
             "RunStatement",
@@ -22632,14 +22643,16 @@
             "CancelWorkflowExecution",
             "CompleteWorkflowExecution",
             "ContinueAsNewWorkflowExecution",
             "CountClosedWorkflowExecutions",
             "CountOpenWorkflowExecutions",
             "CountPendingActivityTasks",
             "CountPendingDecisionTasks",
+            "DeleteActivityType",
+            "DeleteWorkflowType",
             "DeprecateActivityType",
             "DeprecateDomain",
             "DeprecateWorkflowType",
             "DescribeActivityType",
             "DescribeDomain",
             "DescribeWorkflowExecution",
             "DescribeWorkflowType",
```

### Comparing `iam_actions-1.2.20240528/pyproject.toml` & `iam_actions-1.2.20240529/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240528"
+version = "1.2.20240529"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240528/setup.py` & `iam_actions-1.2.20240529/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240528',
+    'version': '1.2.20240529',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240528/PKG-INFO` & `iam_actions-1.2.20240529/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240528
+Version: 1.2.20240529
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

