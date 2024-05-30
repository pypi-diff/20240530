# Comparing `tmp/mypy-boto3-connect-1.34.82.tar.gz` & `tmp/mypy_boto3_connect-1.34.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connect-1.34.82.tar", last modified: Wed Apr 10 19:19:35 2024, max compression
+gzip compressed data, was "mypy_boto3_connect-1.34.98.tar", last modified: Fri May  3 19:32:41 2024, max compression
```

## Comparing `mypy-boto3-connect-1.34.82.tar` & `mypy_boto3_connect-1.34.98.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:35.321250 mypy-boto3-connect-1.34.82/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20551 2024-04-10 19:19:35.321250 mypy-boto3-connect-1.34.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18996 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:35.321250 mypy-boto3-connect-1.34.82/mypy_boto3_connect/
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   187084 2024-04-10 19:19:10.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   187081 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    30510 2024-04-10 19:19:10.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    30510 2024-04-10 19:19:10.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    65203 2024-04-10 19:19:10.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    65148 2024-04-10 19:19:10.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   221361 2024-04-10 19:19:14.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   221361 2024-04-10 19:19:13.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:35.321250 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20551 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:19:35.321250 mypy-boto3-connect-1.34.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-10 19:19:07.000000 mypy-boto3-connect-1.34.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:41.645281 mypy_boto3_connect-1.34.98/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 19:31:50.000000 mypy_boto3_connect-1.34.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20551 2024-05-03 19:32:41.645281 mypy_boto3_connect-1.34.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18996 2024-05-03 19:31:50.000000 mypy_boto3_connect-1.34.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:41.641281 mypy_boto3_connect-1.34.98/mypy_boto3_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-05-03 19:31:50.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-05-03 19:31:50.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-03 19:31:50.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190601 2024-05-03 19:31:52.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190598 2024-05-03 19:31:51.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-05-03 19:31:53.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-05-03 19:31:53.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    65167 2024-05-03 19:31:53.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65112 2024-05-03 19:31:53.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:31:50.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   234677 2024-05-03 19:31:57.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   234677 2024-05-03 19:31:56.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 19:31:50.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:41.645281 mypy_boto3_connect-1.34.98/mypy_boto3_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20551 2024-05-03 19:32:41.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-03 19:32:41.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:41.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:41.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 19:32:41.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 19:32:41.000000 mypy_boto3_connect-1.34.98/mypy_boto3_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:32:41.645281 mypy_boto3_connect-1.34.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-03 19:31:50.000000 mypy_boto3_connect-1.34.98/setup.py
```

### Comparing `mypy-boto3-connect-1.34.82/LICENSE` & `mypy_boto3_connect-1.34.98/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.82/PKG-INFO` & `mypy_boto3_connect-1.34.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.34.82
-Summary: Type annotations for boto3.Connect 1.34.82 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.98
+Summary: Type annotations for boto3.Connect 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connect)](https://pepy.tech/project/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connect-1.34.82/README.md` & `mypy_boto3_connect-1.34.98/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connect)](https://pepy.tech/project/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/__init__.py` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/__init__.pyi` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/__main__.py` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Connect 1.34.82\n"
-        "Version:         1.34.82\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.Connect 1.34.98\n"
+        "Version:         1.34.98\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.82")
+    print("1.34.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/client.py` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,33 +107,35 @@
     SearchRoutingProfilesPaginator,
     SearchSecurityProfilesPaginator,
     SearchUsersPaginator,
     SearchVocabulariesPaginator,
 )
 from .type_defs import (
     ActivateEvaluationFormResponseTypeDef,
-    AgentConfigTypeDef,
+    AgentConfigUnionTypeDef,
     AllowedCapabilitiesTypeDef,
     AnswerMachineDetectionConfigTypeDef,
-    ApplicationTypeDef,
+    ApplicationUnionTypeDef,
     AssociateAnalyticsDataSetResponseTypeDef,
     AssociateInstanceStorageConfigResponseTypeDef,
     AssociateSecurityKeyResponseTypeDef,
     BatchAssociateAnalyticsDataSetResponseTypeDef,
     BatchDisassociateAnalyticsDataSetResponseTypeDef,
+    BatchGetAttachedFileMetadataResponseTypeDef,
     BatchGetFlowAssociationResponseTypeDef,
     BatchPutContactResponseTypeDef,
     ChatEventTypeDef,
     ChatMessageTypeDef,
     ChatStreamingConfigurationTypeDef,
     ClaimPhoneNumberResponseTypeDef,
     ContactDataRequestTypeDef,
     CreateAgentStatusResponseTypeDef,
     CreateContactFlowModuleResponseTypeDef,
     CreateContactFlowResponseTypeDef,
+    CreatedByInfoTypeDef,
     CreateEvaluationFormResponseTypeDef,
     CreateHoursOfOperationResponseTypeDef,
     CreateInstanceResponseTypeDef,
     CreateIntegrationAssociationResponseTypeDef,
     CreateParticipantResponseTypeDef,
     CreatePersistentContactAssociationResponseTypeDef,
     CreatePromptResponseTypeDef,
@@ -177,19 +179,20 @@
     DescribeUserHierarchyStructureResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeViewResponseTypeDef,
     DescribeVocabularyResponseTypeDef,
     DisconnectReasonTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationAnswerInputTypeDef,
-    EvaluationFormItemTypeDef,
+    EvaluationFormItemUnionTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationNoteTypeDef,
     FiltersTypeDef,
     FilterV2TypeDef,
+    GetAttachedFileResponseTypeDef,
     GetContactAttributesResponseTypeDef,
     GetCurrentMetricDataResponseTypeDef,
     GetCurrentUserDataResponseTypeDef,
     GetFederationTokenResponseTypeDef,
     GetFlowAssociationResponseTypeDef,
     GetMetricDataResponseTypeDef,
     GetMetricDataV2ResponseTypeDef,
@@ -247,38 +250,38 @@
     ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsResponseTypeDef,
     ListUserProficienciesResponseTypeDef,
     ListUsersResponseTypeDef,
     ListViewsResponseTypeDef,
     ListViewVersionsResponseTypeDef,
     MediaConcurrencyTypeDef,
-    MetricV2TypeDef,
+    MetricV2UnionTypeDef,
     MonitorContactResponseTypeDef,
     NewSessionDetailsTypeDef,
     OutboundCallerConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     PersistentChatTypeDef,
     PredefinedAttributeSearchCriteriaTypeDef,
-    PredefinedAttributeValuesTypeDef,
+    PredefinedAttributeValuesUnionTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectConfigTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
     ReferenceTypeDef,
     ReplicateInstanceResponseTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    RuleActionTypeDef,
+    RuleActionUnionTypeDef,
     RuleTriggerEventSourceTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SearchContactsResponseTypeDef,
     SearchContactsTimeRangeTypeDef,
     SearchCriteriaTypeDef,
     SearchHoursOfOperationsResponseTypeDef,
     SearchPredefinedAttributesResponseTypeDef,
@@ -290,27 +293,28 @@
     SearchSecurityProfilesResponseTypeDef,
     SearchUsersResponseTypeDef,
     SearchVocabulariesResponseTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     SecurityProfilesSearchFilterTypeDef,
     SegmentAttributeValueTypeDef,
     SendChatIntegrationEventResponseTypeDef,
-    SignInConfigTypeDef,
+    SignInConfigUnionTypeDef,
     SortTypeDef,
+    StartAttachedFileUploadResponseTypeDef,
     StartChatContactResponseTypeDef,
     StartContactEvaluationResponseTypeDef,
     StartContactStreamingResponseTypeDef,
     StartOutboundVoiceContactResponseTypeDef,
     StartTaskContactResponseTypeDef,
     StartWebRTCContactResponseTypeDef,
     SubmitContactEvaluationResponseTypeDef,
-    TaskTemplateConstraintsTypeDef,
-    TaskTemplateDefaultsTypeDef,
-    TaskTemplateFieldTypeDef,
-    TelephonyConfigTypeDef,
+    TaskTemplateConstraintsUnionTypeDef,
+    TaskTemplateDefaultsUnionTypeDef,
+    TaskTemplateFieldUnionTypeDef,
+    TelephonyConfigUnionTypeDef,
     TimestampTypeDef,
     TransferContactResponseTypeDef,
     UpdateContactEvaluationResponseTypeDef,
     UpdateEvaluationFormResponseTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     UpdatePromptResponseTypeDef,
@@ -568,14 +572,25 @@
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.batch_disassociate_analytics_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#batch_disassociate_analytics_data_set)
         """
 
+    def batch_get_attached_file_metadata(
+        self, *, FileIds: Sequence[str], InstanceId: str, AssociatedResourceArn: str
+    ) -> BatchGetAttachedFileMetadataResponseTypeDef:
+        """
+        Allows you to retrieve metadata about multiple attached files on an associated
+        resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.batch_get_attached_file_metadata)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#batch_get_attached_file_metadata)
+        """
+
     def batch_get_flow_association(
         self,
         *,
         InstanceId: str,
         ResourceIds: Sequence[str],
         ResourceType: Literal["VOICE_PHONE_NUMBER"] = ...,
     ) -> BatchGetFlowAssociationResponseTypeDef:
@@ -631,14 +646,26 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#close)
         """
 
+    def complete_attached_file_upload(
+        self, *, InstanceId: str, FileId: str, AssociatedResourceArn: str
+    ) -> Dict[str, Any]:
+        """
+        Allows you to confirm that the attached file has been uploaded using the
+        pre-signed URL provided in the StartAttachedFileUpload
+        API.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.complete_attached_file_upload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#complete_attached_file_upload)
+        """
+
     def create_agent_status(
         self,
         *,
         InstanceId: str,
         Name: str,
         State: AgentStatusStateType,
         Description: str = ...,
@@ -687,15 +714,15 @@
         """
 
     def create_evaluation_form(
         self,
         *,
         InstanceId: str,
         Title: str,
-        Items: Sequence["EvaluationFormItemTypeDef"],
+        Items: Sequence[EvaluationFormItemUnionTypeDef],
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
         ClientToken: str = ...,
     ) -> CreateEvaluationFormResponseTypeDef:
         """
         Creates an evaluation form in the specified Amazon Connect instance.
 
@@ -785,15 +812,15 @@
         Enables rehydration of chats for the lifespan of a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_persistent_contact_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_persistent_contact_association)
         """
 
     def create_predefined_attribute(
-        self, *, InstanceId: str, Name: str, Values: PredefinedAttributeValuesTypeDef
+        self, *, InstanceId: str, Name: str, Values: PredefinedAttributeValuesUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new predefined attribute for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_predefined_attribute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_predefined_attribute)
         """
@@ -871,15 +898,15 @@
     def create_rule(
         self,
         *,
         InstanceId: str,
         Name: str,
         TriggerEventSource: RuleTriggerEventSourceTypeDef,
         Function: str,
-        Actions: Sequence[RuleActionTypeDef],
+        Actions: Sequence[RuleActionUnionTypeDef],
         PublishStatus: RulePublishStatusType,
         ClientToken: str = ...,
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)
@@ -892,15 +919,15 @@
         SecurityProfileName: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...,
-        Applications: Sequence[ApplicationTypeDef] = ...,
+        Applications: Sequence[ApplicationUnionTypeDef] = ...,
         HierarchyRestrictedResources: Sequence[str] = ...,
         AllowedAccessControlHierarchyGroupId: str = ...,
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_security_profile)
@@ -908,19 +935,19 @@
         """
 
     def create_task_template(
         self,
         *,
         InstanceId: str,
         Name: str,
-        Fields: Sequence[TaskTemplateFieldTypeDef],
+        Fields: Sequence[TaskTemplateFieldUnionTypeDef],
         Description: str = ...,
         ContactFlowId: str = ...,
-        Constraints: TaskTemplateConstraintsTypeDef = ...,
-        Defaults: TaskTemplateDefaultsTypeDef = ...,
+        Constraints: TaskTemplateConstraintsUnionTypeDef = ...,
+        Defaults: TaskTemplateDefaultsUnionTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
         ClientToken: str = ...,
     ) -> CreateTaskTemplateResponseTypeDef:
         """
         Creates a new task template in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)
@@ -1047,14 +1074,24 @@
         """
         Deactivates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.deactivate_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#deactivate_evaluation_form)
         """
 
+    def delete_attached_file(
+        self, *, InstanceId: str, FileId: str, AssociatedResourceArn: str
+    ) -> Dict[str, Any]:
+        """
+        Deletes an attached file along with the underlying S3 Object.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_attached_file)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_attached_file)
+        """
+
     def delete_contact_evaluation(
         self, *, InstanceId: str, EvaluationId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_contact_evaluation)
@@ -1352,15 +1389,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_storage_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance_storage_config)
         """
 
     def describe_phone_number(self, *, PhoneNumberId: str) -> DescribePhoneNumberResponseTypeDef:
         """
-        Gets details and status of a phone number that’s claimed to your Amazon Connect
+        Gets details and status of a phone number that's claimed to your Amazon Connect
         instance or traffic distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_phone_number)
         """
 
@@ -1624,15 +1661,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#disassociate_user_proficiencies)
         """
 
     def dismiss_user_contact(
         self, *, UserId: str, InstanceId: str, ContactId: str
     ) -> Dict[str, Any]:
         """
-        Dismisses contacts from an agent’s CCP and returns the agent to an available
+        Dismisses contacts from an agent's CCP and returns the agent to an available
         state, which allows the agent to receive a new routed
         contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.dismiss_user_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#dismiss_user_contact)
         """
 
@@ -1646,14 +1683,29 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#generate_presigned_url)
         """
 
+    def get_attached_file(
+        self,
+        *,
+        InstanceId: str,
+        FileId: str,
+        AssociatedResourceArn: str,
+        UrlExpiryInSeconds: int = ...,
+    ) -> GetAttachedFileResponseTypeDef:
+        """
+        Provides a pre-signed URL for download of an approved attached file.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_attached_file)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_attached_file)
+        """
+
     def get_contact_attributes(
         self, *, InstanceId: str, InitialContactId: str
     ) -> GetContactAttributesResponseTypeDef:
         """
         Retrieves the contact attributes for the specified contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_contact_attributes)
@@ -1733,15 +1785,15 @@
     def get_metric_data_v2(
         self,
         *,
         ResourceArn: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Filters: Sequence[FilterV2TypeDef],
-        Metrics: Sequence[MetricV2TypeDef],
+        Metrics: Sequence[MetricV2UnionTypeDef],
         Interval: IntervalDetailsTypeDef = ...,
         Groupings: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
     ) -> GetMetricDataV2ResponseTypeDef:
         """
         Gets metric data from the specified Amazon Connect instance.
@@ -2662,14 +2714,34 @@
         integrations to Amazon
         Connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.send_chat_integration_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#send_chat_integration_event)
         """
 
+    def start_attached_file_upload(
+        self,
+        *,
+        InstanceId: str,
+        FileName: str,
+        FileSizeInBytes: int,
+        FileUseCaseType: Literal["ATTACHMENT"],
+        AssociatedResourceArn: str,
+        ClientToken: str = ...,
+        UrlExpiryInSeconds: int = ...,
+        CreatedBy: CreatedByInfoTypeDef = ...,
+        Tags: Mapping[str, str] = ...,
+    ) -> StartAttachedFileUploadResponseTypeDef:
+        """
+        Provides a pre-signed Amazon S3 URL in response for uploading your content.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_attached_file_upload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_attached_file_upload)
+        """
+
     def start_chat_contact(
         self,
         *,
         InstanceId: str,
         ContactFlowId: str,
         ParticipantDetails: ParticipantDetailsTypeDef,
         Attributes: Mapping[str, str] = ...,
@@ -3070,15 +3142,15 @@
     def update_evaluation_form(
         self,
         *,
         InstanceId: str,
         EvaluationFormId: str,
         EvaluationFormVersion: int,
         Title: str,
-        Items: Sequence["EvaluationFormItemTypeDef"],
+        Items: Sequence[EvaluationFormItemUnionTypeDef],
         CreateNewVersion: bool = ...,
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
         ClientToken: str = ...,
     ) -> UpdateEvaluationFormResponseTypeDef:
         """
         Updates details about a specific evaluation form version in the specified
@@ -3165,22 +3237,22 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_phone_number)
         """
 
     def update_phone_number_metadata(
         self, *, PhoneNumberId: str, PhoneNumberDescription: str = ..., ClientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Updates a phone number’s metadata.
+        Updates a phone number's metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_phone_number_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_phone_number_metadata)
         """
 
     def update_predefined_attribute(
-        self, *, InstanceId: str, Name: str, Values: PredefinedAttributeValuesTypeDef = ...
+        self, *, InstanceId: str, Name: str, Values: PredefinedAttributeValuesUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a predefined attribute for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_predefined_attribute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_predefined_attribute)
         """
@@ -3340,15 +3412,15 @@
     def update_rule(
         self,
         *,
         RuleId: str,
         InstanceId: str,
         Name: str,
         Function: str,
-        Actions: Sequence[RuleActionTypeDef],
+        Actions: Sequence[RuleActionUnionTypeDef],
         PublishStatus: RulePublishStatusType,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_rule)
@@ -3359,15 +3431,15 @@
         *,
         SecurityProfileId: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...,
-        Applications: Sequence[ApplicationTypeDef] = ...,
+        Applications: Sequence[ApplicationUnionTypeDef] = ...,
         HierarchyRestrictedResources: Sequence[str] = ...,
         AllowedAccessControlHierarchyGroupId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_security_profile)
@@ -3378,34 +3450,34 @@
         self,
         *,
         TaskTemplateId: str,
         InstanceId: str,
         Name: str = ...,
         Description: str = ...,
         ContactFlowId: str = ...,
-        Constraints: TaskTemplateConstraintsTypeDef = ...,
-        Defaults: TaskTemplateDefaultsTypeDef = ...,
+        Constraints: TaskTemplateConstraintsUnionTypeDef = ...,
+        Defaults: TaskTemplateDefaultsUnionTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
-        Fields: Sequence[TaskTemplateFieldTypeDef] = ...,
+        Fields: Sequence[TaskTemplateFieldUnionTypeDef] = ...,
     ) -> UpdateTaskTemplateResponseTypeDef:
         """
         Updates details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_task_template)
         """
 
     def update_traffic_distribution(
         self,
         *,
         Id: str,
-        TelephonyConfig: TelephonyConfigTypeDef = ...,
-        SignInConfig: SignInConfigTypeDef = ...,
-        AgentConfig: AgentConfigTypeDef = ...,
+        TelephonyConfig: TelephonyConfigUnionTypeDef = ...,
+        SignInConfig: SignInConfigUnionTypeDef = ...,
+        AgentConfig: AgentConfigUnionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the traffic distribution for a given traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_traffic_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_traffic_distribution)
         """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/client.pyi` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -107,33 +107,35 @@
     SearchRoutingProfilesPaginator,
     SearchSecurityProfilesPaginator,
     SearchUsersPaginator,
     SearchVocabulariesPaginator,
 )
 from .type_defs import (
     ActivateEvaluationFormResponseTypeDef,
-    AgentConfigTypeDef,
+    AgentConfigUnionTypeDef,
     AllowedCapabilitiesTypeDef,
     AnswerMachineDetectionConfigTypeDef,
-    ApplicationTypeDef,
+    ApplicationUnionTypeDef,
     AssociateAnalyticsDataSetResponseTypeDef,
     AssociateInstanceStorageConfigResponseTypeDef,
     AssociateSecurityKeyResponseTypeDef,
     BatchAssociateAnalyticsDataSetResponseTypeDef,
     BatchDisassociateAnalyticsDataSetResponseTypeDef,
+    BatchGetAttachedFileMetadataResponseTypeDef,
     BatchGetFlowAssociationResponseTypeDef,
     BatchPutContactResponseTypeDef,
     ChatEventTypeDef,
     ChatMessageTypeDef,
     ChatStreamingConfigurationTypeDef,
     ClaimPhoneNumberResponseTypeDef,
     ContactDataRequestTypeDef,
     CreateAgentStatusResponseTypeDef,
     CreateContactFlowModuleResponseTypeDef,
     CreateContactFlowResponseTypeDef,
+    CreatedByInfoTypeDef,
     CreateEvaluationFormResponseTypeDef,
     CreateHoursOfOperationResponseTypeDef,
     CreateInstanceResponseTypeDef,
     CreateIntegrationAssociationResponseTypeDef,
     CreateParticipantResponseTypeDef,
     CreatePersistentContactAssociationResponseTypeDef,
     CreatePromptResponseTypeDef,
@@ -177,19 +179,20 @@
     DescribeUserHierarchyStructureResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeViewResponseTypeDef,
     DescribeVocabularyResponseTypeDef,
     DisconnectReasonTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationAnswerInputTypeDef,
-    EvaluationFormItemTypeDef,
+    EvaluationFormItemUnionTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationNoteTypeDef,
     FiltersTypeDef,
     FilterV2TypeDef,
+    GetAttachedFileResponseTypeDef,
     GetContactAttributesResponseTypeDef,
     GetCurrentMetricDataResponseTypeDef,
     GetCurrentUserDataResponseTypeDef,
     GetFederationTokenResponseTypeDef,
     GetFlowAssociationResponseTypeDef,
     GetMetricDataResponseTypeDef,
     GetMetricDataV2ResponseTypeDef,
@@ -247,38 +250,38 @@
     ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsResponseTypeDef,
     ListUserProficienciesResponseTypeDef,
     ListUsersResponseTypeDef,
     ListViewsResponseTypeDef,
     ListViewVersionsResponseTypeDef,
     MediaConcurrencyTypeDef,
-    MetricV2TypeDef,
+    MetricV2UnionTypeDef,
     MonitorContactResponseTypeDef,
     NewSessionDetailsTypeDef,
     OutboundCallerConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     PersistentChatTypeDef,
     PredefinedAttributeSearchCriteriaTypeDef,
-    PredefinedAttributeValuesTypeDef,
+    PredefinedAttributeValuesUnionTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectConfigTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
     ReferenceTypeDef,
     ReplicateInstanceResponseTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    RuleActionTypeDef,
+    RuleActionUnionTypeDef,
     RuleTriggerEventSourceTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SearchContactsResponseTypeDef,
     SearchContactsTimeRangeTypeDef,
     SearchCriteriaTypeDef,
     SearchHoursOfOperationsResponseTypeDef,
     SearchPredefinedAttributesResponseTypeDef,
@@ -290,27 +293,28 @@
     SearchSecurityProfilesResponseTypeDef,
     SearchUsersResponseTypeDef,
     SearchVocabulariesResponseTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     SecurityProfilesSearchFilterTypeDef,
     SegmentAttributeValueTypeDef,
     SendChatIntegrationEventResponseTypeDef,
-    SignInConfigTypeDef,
+    SignInConfigUnionTypeDef,
     SortTypeDef,
+    StartAttachedFileUploadResponseTypeDef,
     StartChatContactResponseTypeDef,
     StartContactEvaluationResponseTypeDef,
     StartContactStreamingResponseTypeDef,
     StartOutboundVoiceContactResponseTypeDef,
     StartTaskContactResponseTypeDef,
     StartWebRTCContactResponseTypeDef,
     SubmitContactEvaluationResponseTypeDef,
-    TaskTemplateConstraintsTypeDef,
-    TaskTemplateDefaultsTypeDef,
-    TaskTemplateFieldTypeDef,
-    TelephonyConfigTypeDef,
+    TaskTemplateConstraintsUnionTypeDef,
+    TaskTemplateDefaultsUnionTypeDef,
+    TaskTemplateFieldUnionTypeDef,
+    TelephonyConfigUnionTypeDef,
     TimestampTypeDef,
     TransferContactResponseTypeDef,
     UpdateContactEvaluationResponseTypeDef,
     UpdateEvaluationFormResponseTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     UpdatePromptResponseTypeDef,
@@ -565,14 +569,25 @@
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.batch_disassociate_analytics_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#batch_disassociate_analytics_data_set)
         """
 
+    def batch_get_attached_file_metadata(
+        self, *, FileIds: Sequence[str], InstanceId: str, AssociatedResourceArn: str
+    ) -> BatchGetAttachedFileMetadataResponseTypeDef:
+        """
+        Allows you to retrieve metadata about multiple attached files on an associated
+        resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.batch_get_attached_file_metadata)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#batch_get_attached_file_metadata)
+        """
+
     def batch_get_flow_association(
         self,
         *,
         InstanceId: str,
         ResourceIds: Sequence[str],
         ResourceType: Literal["VOICE_PHONE_NUMBER"] = ...,
     ) -> BatchGetFlowAssociationResponseTypeDef:
@@ -628,14 +643,26 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#close)
         """
 
+    def complete_attached_file_upload(
+        self, *, InstanceId: str, FileId: str, AssociatedResourceArn: str
+    ) -> Dict[str, Any]:
+        """
+        Allows you to confirm that the attached file has been uploaded using the
+        pre-signed URL provided in the StartAttachedFileUpload
+        API.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.complete_attached_file_upload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#complete_attached_file_upload)
+        """
+
     def create_agent_status(
         self,
         *,
         InstanceId: str,
         Name: str,
         State: AgentStatusStateType,
         Description: str = ...,
@@ -684,15 +711,15 @@
         """
 
     def create_evaluation_form(
         self,
         *,
         InstanceId: str,
         Title: str,
-        Items: Sequence["EvaluationFormItemTypeDef"],
+        Items: Sequence[EvaluationFormItemUnionTypeDef],
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
         ClientToken: str = ...,
     ) -> CreateEvaluationFormResponseTypeDef:
         """
         Creates an evaluation form in the specified Amazon Connect instance.
 
@@ -782,15 +809,15 @@
         Enables rehydration of chats for the lifespan of a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_persistent_contact_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_persistent_contact_association)
         """
 
     def create_predefined_attribute(
-        self, *, InstanceId: str, Name: str, Values: PredefinedAttributeValuesTypeDef
+        self, *, InstanceId: str, Name: str, Values: PredefinedAttributeValuesUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new predefined attribute for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_predefined_attribute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_predefined_attribute)
         """
@@ -868,15 +895,15 @@
     def create_rule(
         self,
         *,
         InstanceId: str,
         Name: str,
         TriggerEventSource: RuleTriggerEventSourceTypeDef,
         Function: str,
-        Actions: Sequence[RuleActionTypeDef],
+        Actions: Sequence[RuleActionUnionTypeDef],
         PublishStatus: RulePublishStatusType,
         ClientToken: str = ...,
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)
@@ -889,15 +916,15 @@
         SecurityProfileName: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...,
-        Applications: Sequence[ApplicationTypeDef] = ...,
+        Applications: Sequence[ApplicationUnionTypeDef] = ...,
         HierarchyRestrictedResources: Sequence[str] = ...,
         AllowedAccessControlHierarchyGroupId: str = ...,
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_security_profile)
@@ -905,19 +932,19 @@
         """
 
     def create_task_template(
         self,
         *,
         InstanceId: str,
         Name: str,
-        Fields: Sequence[TaskTemplateFieldTypeDef],
+        Fields: Sequence[TaskTemplateFieldUnionTypeDef],
         Description: str = ...,
         ContactFlowId: str = ...,
-        Constraints: TaskTemplateConstraintsTypeDef = ...,
-        Defaults: TaskTemplateDefaultsTypeDef = ...,
+        Constraints: TaskTemplateConstraintsUnionTypeDef = ...,
+        Defaults: TaskTemplateDefaultsUnionTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
         ClientToken: str = ...,
     ) -> CreateTaskTemplateResponseTypeDef:
         """
         Creates a new task template in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)
@@ -1044,14 +1071,24 @@
         """
         Deactivates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.deactivate_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#deactivate_evaluation_form)
         """
 
+    def delete_attached_file(
+        self, *, InstanceId: str, FileId: str, AssociatedResourceArn: str
+    ) -> Dict[str, Any]:
+        """
+        Deletes an attached file along with the underlying S3 Object.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_attached_file)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_attached_file)
+        """
+
     def delete_contact_evaluation(
         self, *, InstanceId: str, EvaluationId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_contact_evaluation)
@@ -1349,15 +1386,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_storage_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance_storage_config)
         """
 
     def describe_phone_number(self, *, PhoneNumberId: str) -> DescribePhoneNumberResponseTypeDef:
         """
-        Gets details and status of a phone number that’s claimed to your Amazon Connect
+        Gets details and status of a phone number that's claimed to your Amazon Connect
         instance or traffic distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_phone_number)
         """
 
@@ -1621,15 +1658,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#disassociate_user_proficiencies)
         """
 
     def dismiss_user_contact(
         self, *, UserId: str, InstanceId: str, ContactId: str
     ) -> Dict[str, Any]:
         """
-        Dismisses contacts from an agent’s CCP and returns the agent to an available
+        Dismisses contacts from an agent's CCP and returns the agent to an available
         state, which allows the agent to receive a new routed
         contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.dismiss_user_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#dismiss_user_contact)
         """
 
@@ -1643,14 +1680,29 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#generate_presigned_url)
         """
 
+    def get_attached_file(
+        self,
+        *,
+        InstanceId: str,
+        FileId: str,
+        AssociatedResourceArn: str,
+        UrlExpiryInSeconds: int = ...,
+    ) -> GetAttachedFileResponseTypeDef:
+        """
+        Provides a pre-signed URL for download of an approved attached file.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_attached_file)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_attached_file)
+        """
+
     def get_contact_attributes(
         self, *, InstanceId: str, InitialContactId: str
     ) -> GetContactAttributesResponseTypeDef:
         """
         Retrieves the contact attributes for the specified contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_contact_attributes)
@@ -1730,15 +1782,15 @@
     def get_metric_data_v2(
         self,
         *,
         ResourceArn: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Filters: Sequence[FilterV2TypeDef],
-        Metrics: Sequence[MetricV2TypeDef],
+        Metrics: Sequence[MetricV2UnionTypeDef],
         Interval: IntervalDetailsTypeDef = ...,
         Groupings: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
     ) -> GetMetricDataV2ResponseTypeDef:
         """
         Gets metric data from the specified Amazon Connect instance.
@@ -2659,14 +2711,34 @@
         integrations to Amazon
         Connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.send_chat_integration_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#send_chat_integration_event)
         """
 
+    def start_attached_file_upload(
+        self,
+        *,
+        InstanceId: str,
+        FileName: str,
+        FileSizeInBytes: int,
+        FileUseCaseType: Literal["ATTACHMENT"],
+        AssociatedResourceArn: str,
+        ClientToken: str = ...,
+        UrlExpiryInSeconds: int = ...,
+        CreatedBy: CreatedByInfoTypeDef = ...,
+        Tags: Mapping[str, str] = ...,
+    ) -> StartAttachedFileUploadResponseTypeDef:
+        """
+        Provides a pre-signed Amazon S3 URL in response for uploading your content.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_attached_file_upload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_attached_file_upload)
+        """
+
     def start_chat_contact(
         self,
         *,
         InstanceId: str,
         ContactFlowId: str,
         ParticipantDetails: ParticipantDetailsTypeDef,
         Attributes: Mapping[str, str] = ...,
@@ -3067,15 +3139,15 @@
     def update_evaluation_form(
         self,
         *,
         InstanceId: str,
         EvaluationFormId: str,
         EvaluationFormVersion: int,
         Title: str,
-        Items: Sequence["EvaluationFormItemTypeDef"],
+        Items: Sequence[EvaluationFormItemUnionTypeDef],
         CreateNewVersion: bool = ...,
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
         ClientToken: str = ...,
     ) -> UpdateEvaluationFormResponseTypeDef:
         """
         Updates details about a specific evaluation form version in the specified
@@ -3162,22 +3234,22 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_phone_number)
         """
 
     def update_phone_number_metadata(
         self, *, PhoneNumberId: str, PhoneNumberDescription: str = ..., ClientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Updates a phone number’s metadata.
+        Updates a phone number's metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_phone_number_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_phone_number_metadata)
         """
 
     def update_predefined_attribute(
-        self, *, InstanceId: str, Name: str, Values: PredefinedAttributeValuesTypeDef = ...
+        self, *, InstanceId: str, Name: str, Values: PredefinedAttributeValuesUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a predefined attribute for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_predefined_attribute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_predefined_attribute)
         """
@@ -3337,15 +3409,15 @@
     def update_rule(
         self,
         *,
         RuleId: str,
         InstanceId: str,
         Name: str,
         Function: str,
-        Actions: Sequence[RuleActionTypeDef],
+        Actions: Sequence[RuleActionUnionTypeDef],
         PublishStatus: RulePublishStatusType,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_rule)
@@ -3356,15 +3428,15 @@
         *,
         SecurityProfileId: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...,
-        Applications: Sequence[ApplicationTypeDef] = ...,
+        Applications: Sequence[ApplicationUnionTypeDef] = ...,
         HierarchyRestrictedResources: Sequence[str] = ...,
         AllowedAccessControlHierarchyGroupId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a security profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_security_profile)
@@ -3375,34 +3447,34 @@
         self,
         *,
         TaskTemplateId: str,
         InstanceId: str,
         Name: str = ...,
         Description: str = ...,
         ContactFlowId: str = ...,
-        Constraints: TaskTemplateConstraintsTypeDef = ...,
-        Defaults: TaskTemplateDefaultsTypeDef = ...,
+        Constraints: TaskTemplateConstraintsUnionTypeDef = ...,
+        Defaults: TaskTemplateDefaultsUnionTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
-        Fields: Sequence[TaskTemplateFieldTypeDef] = ...,
+        Fields: Sequence[TaskTemplateFieldUnionTypeDef] = ...,
     ) -> UpdateTaskTemplateResponseTypeDef:
         """
         Updates details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_task_template)
         """
 
     def update_traffic_distribution(
         self,
         *,
         Id: str,
-        TelephonyConfig: TelephonyConfigTypeDef = ...,
-        SignInConfig: SignInConfigTypeDef = ...,
-        AgentConfig: AgentConfigTypeDef = ...,
+        TelephonyConfig: TelephonyConfigUnionTypeDef = ...,
+        SignInConfig: SignInConfigUnionTypeDef = ...,
+        AgentConfig: AgentConfigUnionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the traffic distribution for a given traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_traffic_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_traffic_distribution)
         """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/literals.py` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     "EvaluationFormScoringModeType",
     "EvaluationFormScoringStatusType",
     "EvaluationFormSingleSelectQuestionDisplayModeType",
     "EvaluationFormVersionStatusType",
     "EvaluationStatusType",
     "EventSourceNameType",
     "FailureReasonCodeType",
+    "FileStatusTypeType",
+    "FileUseCaseTypeType",
     "FlowAssociationResourceTypeType",
     "GetMetricDataPaginatorName",
     "GroupingType",
     "HierarchyGroupMatchTypeType",
     "HistoricalMetricNameType",
     "HoursOfOperationDaysType",
     "InstanceAttributeTypeType",
@@ -266,14 +268,16 @@
     "INVALID_QUEUE",
     "INVALID_SYSTEM_ENDPOINT",
     "MISSING_CAMPAIGN",
     "MISSING_CUSTOMER_ENDPOINT",
     "MISSING_QUEUE_ID_AND_SYSTEM_ENDPOINT",
     "REQUEST_THROTTLED",
 ]
+FileStatusTypeType = Literal["APPROVED", "FAILED", "PROCESSING", "REJECTED"]
+FileUseCaseTypeType = Literal["ATTACHMENT"]
 FlowAssociationResourceTypeType = Literal["SMS_PHONE_NUMBER"]
 GetMetricDataPaginatorName = Literal["get_metric_data"]
 GroupingType = Literal["CHANNEL", "QUEUE", "ROUTING_PROFILE", "ROUTING_STEP_EXPRESSION"]
 HierarchyGroupMatchTypeType = Literal["EXACT", "WITH_CHILD_GROUPS"]
 HistoricalMetricNameType = Literal[
     "ABANDON_TIME",
     "AFTER_CONTACT_WORK_TIME",
@@ -1060,14 +1064,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/literals.pyi` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     "EvaluationFormScoringModeType",
     "EvaluationFormScoringStatusType",
     "EvaluationFormSingleSelectQuestionDisplayModeType",
     "EvaluationFormVersionStatusType",
     "EvaluationStatusType",
     "EventSourceNameType",
     "FailureReasonCodeType",
+    "FileStatusTypeType",
+    "FileUseCaseTypeType",
     "FlowAssociationResourceTypeType",
     "GetMetricDataPaginatorName",
     "GroupingType",
     "HierarchyGroupMatchTypeType",
     "HistoricalMetricNameType",
     "HoursOfOperationDaysType",
     "InstanceAttributeTypeType",
@@ -266,14 +268,16 @@
     "INVALID_QUEUE",
     "INVALID_SYSTEM_ENDPOINT",
     "MISSING_CAMPAIGN",
     "MISSING_CUSTOMER_ENDPOINT",
     "MISSING_QUEUE_ID_AND_SYSTEM_ENDPOINT",
     "REQUEST_THROTTLED",
 ]
+FileStatusTypeType = Literal["APPROVED", "FAILED", "PROCESSING", "REJECTED"]
+FileUseCaseTypeType = Literal["ATTACHMENT"]
 FlowAssociationResourceTypeType = Literal["SMS_PHONE_NUMBER"]
 GetMetricDataPaginatorName = Literal["get_metric_data"]
 GroupingType = Literal["CHANNEL", "QUEUE", "ROUTING_PROFILE", "ROUTING_STEP_EXPRESSION"]
 HierarchyGroupMatchTypeType = Literal["EXACT", "WITH_CHILD_GROUPS"]
 HistoricalMetricNameType = Literal[
     "ABANDON_TIME",
     "AFTER_CONTACT_WORK_TIME",
@@ -1060,14 +1064,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/paginator.py` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     ListQueueQuickConnectsResponseTypeDef,
     ListQueuesResponseTypeDef,
     ListQuickConnectsResponseTypeDef,
     ListRoutingProfileQueuesResponseTypeDef,
     ListRoutingProfilesResponseTypeDef,
     ListRulesResponseTypeDef,
     ListSecurityKeysResponseTypeDef,
-    ListSecurityProfileApplicationsResponsePaginatorTypeDef,
+    ListSecurityProfileApplicationsResponseTypeDef,
     ListSecurityProfilePermissionsResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsResponseTypeDef,
     ListTrafficDistributionGroupUsersResponseTypeDef,
     ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsResponseTypeDef,
@@ -210,15 +210,15 @@
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SearchContactsResponseTypeDef,
     SearchContactsTimeRangeTypeDef,
     SearchCriteriaTypeDef,
     SearchHoursOfOperationsResponseTypeDef,
-    SearchPredefinedAttributesResponsePaginatorTypeDef,
+    SearchPredefinedAttributesResponseTypeDef,
     SearchPromptsResponseTypeDef,
     SearchQueuesResponseTypeDef,
     SearchQuickConnectsResponseTypeDef,
     SearchResourceTagsResponseTypeDef,
     SearchRoutingProfilesResponseTypeDef,
     SearchSecurityProfilesResponseTypeDef,
     SearchUsersResponseTypeDef,
@@ -840,15 +840,15 @@
 
     def paginate(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListSecurityProfileApplicationsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListSecurityProfileApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfileApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofileapplicationspaginator)
         """
 
 
 class ListSecurityProfilePermissionsPaginator(Paginator):
@@ -1104,15 +1104,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchCriteria: PredefinedAttributeSearchCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[SearchPredefinedAttributesResponsePaginatorTypeDef]:
+    ) -> _PageIterator[SearchPredefinedAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchPredefinedAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchpredefinedattributespaginator)
         """
 
 
 class SearchPromptsPaginator(Paginator):
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/paginator.pyi` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     ListQueueQuickConnectsResponseTypeDef,
     ListQueuesResponseTypeDef,
     ListQuickConnectsResponseTypeDef,
     ListRoutingProfileQueuesResponseTypeDef,
     ListRoutingProfilesResponseTypeDef,
     ListRulesResponseTypeDef,
     ListSecurityKeysResponseTypeDef,
-    ListSecurityProfileApplicationsResponsePaginatorTypeDef,
+    ListSecurityProfileApplicationsResponseTypeDef,
     ListSecurityProfilePermissionsResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsResponseTypeDef,
     ListTrafficDistributionGroupUsersResponseTypeDef,
     ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsResponseTypeDef,
@@ -210,15 +210,15 @@
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SearchContactsResponseTypeDef,
     SearchContactsTimeRangeTypeDef,
     SearchCriteriaTypeDef,
     SearchHoursOfOperationsResponseTypeDef,
-    SearchPredefinedAttributesResponsePaginatorTypeDef,
+    SearchPredefinedAttributesResponseTypeDef,
     SearchPromptsResponseTypeDef,
     SearchQueuesResponseTypeDef,
     SearchQuickConnectsResponseTypeDef,
     SearchResourceTagsResponseTypeDef,
     SearchRoutingProfilesResponseTypeDef,
     SearchSecurityProfilesResponseTypeDef,
     SearchUsersResponseTypeDef,
@@ -808,15 +808,15 @@
 
     def paginate(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListSecurityProfileApplicationsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListSecurityProfileApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfileApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofileapplicationspaginator)
         """
 
 class ListSecurityProfilePermissionsPaginator(Paginator):
     """
@@ -1057,15 +1057,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchCriteria: PredefinedAttributeSearchCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[SearchPredefinedAttributesResponsePaginatorTypeDef]:
+    ) -> _PageIterator[SearchPredefinedAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchPredefinedAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchpredefinedattributespaginator)
         """
 
 class SearchPromptsPaginator(Paginator):
     """
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/type_defs.py` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     EvaluationFormScoringModeType,
     EvaluationFormScoringStatusType,
     EvaluationFormSingleSelectQuestionDisplayModeType,
     EvaluationFormVersionStatusType,
     EvaluationStatusType,
     EventSourceNameType,
     FailureReasonCodeType,
+    FileStatusTypeType,
     GroupingType,
     HierarchyGroupMatchTypeType,
     HistoricalMetricNameType,
     HoursOfOperationDaysType,
     InstanceAttributeTypeType,
     InstanceStatusType,
     InstanceStorageResourceTypeType,
@@ -119,61 +120,67 @@
     "AgentInfoTypeDef",
     "AgentStatusReferenceTypeDef",
     "AgentStatusSummaryTypeDef",
     "AgentStatusTypeDef",
     "ParticipantCapabilitiesTypeDef",
     "AnalyticsDataAssociationResultTypeDef",
     "AnswerMachineDetectionConfigTypeDef",
-    "ApplicationPaginatorTypeDef",
+    "ApplicationExtraOutputTypeDef",
+    "ApplicationOutputTypeDef",
     "ApplicationTypeDef",
     "AssociateAnalyticsDataSetRequestRequestTypeDef",
     "AssociateApprovedOriginRequestRequestTypeDef",
     "LexBotTypeDef",
     "LexV2BotTypeDef",
     "AssociateDefaultVocabularyRequestRequestTypeDef",
     "AssociateFlowRequestRequestTypeDef",
     "AssociateLambdaFunctionRequestRequestTypeDef",
     "AssociatePhoneNumberContactFlowRequestRequestTypeDef",
     "AssociateQueueQuickConnectsRequestRequestTypeDef",
     "AssociateSecurityKeyRequestRequestTypeDef",
     "AssociateTrafficDistributionGroupUserRequestRequestTypeDef",
     "UserProficiencyTypeDef",
+    "AttachedFileErrorTypeDef",
+    "CreatedByInfoTypeDef",
     "AttachmentReferenceTypeDef",
     "AttendeeTypeDef",
     "HierarchyGroupConditionTypeDef",
     "TagConditionTypeDef",
     "AttributeTypeDef",
     "AudioFeaturesTypeDef",
     "AvailableNumberSummaryTypeDef",
     "BatchAssociateAnalyticsDataSetRequestRequestTypeDef",
     "ErrorResultTypeDef",
     "BatchDisassociateAnalyticsDataSetRequestRequestTypeDef",
+    "BatchGetAttachedFileMetadataRequestRequestTypeDef",
     "BatchGetFlowAssociationRequestRequestTypeDef",
     "FlowAssociationSummaryTypeDef",
     "FailedRequestTypeDef",
     "SuccessfulRequestTypeDef",
     "CampaignTypeDef",
     "ChatEventTypeDef",
     "ChatMessageTypeDef",
     "ChatStreamingConfigurationTypeDef",
     "ClaimPhoneNumberRequestRequestTypeDef",
     "PhoneNumberStatusTypeDef",
+    "CompleteAttachedFileUploadRequestRequestTypeDef",
     "EndpointTypeDef",
     "ContactFilterTypeDef",
     "ContactFlowModuleSummaryTypeDef",
     "ContactFlowModuleTypeDef",
     "ContactFlowSummaryTypeDef",
     "ContactFlowTypeDef",
     "ContactSearchSummaryAgentInfoTypeDef",
     "ContactSearchSummaryQueueInfoTypeDef",
     "QueueInfoTypeDef",
     "WisdomInfoTypeDef",
     "CreateAgentStatusRequestRequestTypeDef",
     "CreateContactFlowModuleRequestRequestTypeDef",
     "CreateContactFlowRequestRequestTypeDef",
+    "EvaluationFormItemUnionTypeDef",
     "EvaluationFormScoringStrategyTypeDef",
     "CreateInstanceRequestRequestTypeDef",
     "CreateIntegrationAssociationRequestRequestTypeDef",
     "ParticipantDetailsToAddTypeDef",
     "ParticipantTokenCredentialsTypeDef",
     "CreatePersistentContactAssociationRequestRequestTypeDef",
     "PredefinedAttributeValuesTypeDef",
@@ -191,14 +198,15 @@
     "CredentialsTypeDef",
     "CrossChannelBehaviorTypeDef",
     "CurrentMetricTypeDef",
     "CurrentMetricSortCriteriaTypeDef",
     "DateReferenceTypeDef",
     "DeactivateEvaluationFormRequestRequestTypeDef",
     "DefaultVocabularyTypeDef",
+    "DeleteAttachedFileRequestRequestTypeDef",
     "DeleteContactEvaluationRequestRequestTypeDef",
     "DeleteContactFlowModuleRequestRequestTypeDef",
     "DeleteContactFlowRequestRequestTypeDef",
     "DeleteEvaluationFormRequestRequestTypeDef",
     "DeleteHoursOfOperationRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteIntegrationAssociationRequestRequestTypeDef",
@@ -256,30 +264,34 @@
     "DisassociateQueueQuickConnectsRequestRequestTypeDef",
     "RoutingProfileQueueReferenceTypeDef",
     "DisassociateSecurityKeyRequestRequestTypeDef",
     "DisassociateTrafficDistributionGroupUserRequestRequestTypeDef",
     "UserProficiencyDisassociateTypeDef",
     "DisconnectReasonTypeDef",
     "DismissUserContactRequestRequestTypeDef",
+    "DownloadUrlMetadataTypeDef",
     "EmailReferenceTypeDef",
     "EncryptionConfigTypeDef",
     "EvaluationAnswerDataTypeDef",
     "NumericQuestionPropertyValueAutomationTypeDef",
     "EvaluationFormNumericQuestionOptionTypeDef",
+    "EvaluationFormSectionOutputTypeDef",
     "EvaluationFormSectionTypeDef",
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     "EvaluationFormSingleSelectQuestionOptionTypeDef",
     "EvaluationFormSummaryTypeDef",
     "EvaluationFormVersionSummaryTypeDef",
     "EvaluationScoreTypeDef",
     "EvaluationNoteTypeDef",
     "EventBridgeActionDefinitionTypeDef",
+    "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
     "FilterV2TypeDef",
     "FiltersTypeDef",
+    "GetAttachedFileRequestRequestTypeDef",
     "GetContactAttributesRequestRequestTypeDef",
     "GetFederationTokenRequestRequestTypeDef",
     "GetFlowAssociationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "IntervalDetailsTypeDef",
     "GetPromptFileRequestRequestTypeDef",
@@ -358,26 +370,29 @@
     "ListUsersRequestRequestTypeDef",
     "UserSummaryTypeDef",
     "ListViewVersionsRequestRequestTypeDef",
     "ViewVersionSummaryTypeDef",
     "ListViewsRequestRequestTypeDef",
     "ViewSummaryTypeDef",
     "MediaPlacementTypeDef",
+    "MetricFilterV2OutputTypeDef",
     "MetricFilterV2TypeDef",
     "MetricIntervalTypeDef",
     "ThresholdV2TypeDef",
     "MonitorContactRequestRequestTypeDef",
     "ParticipantDetailsTypeDef",
+    "NotificationRecipientTypeOutputTypeDef",
     "NotificationRecipientTypeTypeDef",
     "NumberReferenceTypeDef",
     "ParticipantTimerValueTypeDef",
     "PauseContactRequestRequestTypeDef",
     "PersistentChatTypeDef",
     "PhoneNumberQuickConnectConfigTypeDef",
-    "PredefinedAttributeValuesPaginatorTypeDef",
+    "PredefinedAttributeValuesOutputTypeDef",
+    "PredefinedAttributeValuesExtraOutputTypeDef",
     "PutUserStatusRequestRequestTypeDef",
     "QueueQuickConnectConfigTypeDef",
     "UserQuickConnectConfigTypeDef",
     "RealTimeContactAnalysisAttachmentTypeDef",
     "RealTimeContactAnalysisCharacterIntervalTypeDef",
     "RealTimeContactAnalysisTimeDataTypeDef",
     "StringReferenceTypeDef",
@@ -395,14 +410,15 @@
     "TagSetTypeDef",
     "SecurityProfileSearchSummaryTypeDef",
     "SearchVocabulariesRequestRequestTypeDef",
     "VocabularySummaryTypeDef",
     "SearchableContactAttributesCriteriaTypeDef",
     "SegmentAttributeValueTypeDef",
     "SignInDistributionTypeDef",
+    "UploadUrlMetadataTypeDef",
     "StartContactEvaluationRequestRequestTypeDef",
     "VoiceRecordingConfigurationTypeDef",
     "StopContactRecordingRequestRequestTypeDef",
     "StopContactStreamingRequestRequestTypeDef",
     "SuspendContactRecordingRequestRequestTypeDef",
     "TagContactRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -485,33 +501,35 @@
     "StartTaskContactResponseTypeDef",
     "SubmitContactEvaluationResponseTypeDef",
     "TransferContactResponseTypeDef",
     "UpdateContactEvaluationResponseTypeDef",
     "UpdateEvaluationFormResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
     "UpdatePromptResponseTypeDef",
+    "AgentConfigOutputTypeDef",
     "AgentConfigTypeDef",
+    "TelephonyConfigOutputTypeDef",
     "TelephonyConfigTypeDef",
     "AgentContactReferenceTypeDef",
     "ListAgentStatusResponseTypeDef",
     "DescribeAgentStatusResponseTypeDef",
     "AllowedCapabilitiesTypeDef",
     "ListAnalyticsDataAssociationsResponseTypeDef",
-    "ListSecurityProfileApplicationsResponsePaginatorTypeDef",
-    "CreateSecurityProfileRequestRequestTypeDef",
     "ListSecurityProfileApplicationsResponseTypeDef",
-    "UpdateSecurityProfileRequestRequestTypeDef",
+    "ApplicationUnionTypeDef",
     "AssociateLexBotRequestRequestTypeDef",
     "ListLexBotsResponseTypeDef",
     "AssociateBotRequestRequestTypeDef",
     "DisassociateBotRequestRequestTypeDef",
     "LexBotConfigTypeDef",
     "AssociateUserProficienciesRequestRequestTypeDef",
     "ListUserProficienciesResponseTypeDef",
     "UpdateUserProficienciesRequestRequestTypeDef",
+    "AttachedFileTypeDef",
+    "StartAttachedFileUploadRequestRequestTypeDef",
     "AttributeAndConditionTypeDef",
     "ControlPlaneTagFilterTypeDef",
     "DescribeInstanceAttributeResponseTypeDef",
     "ListInstanceAttributesResponseTypeDef",
     "MeetingFeaturesConfigurationTypeDef",
     "SearchAvailablePhoneNumbersResponseTypeDef",
     "BatchAssociateAnalyticsDataSetResponseTypeDef",
@@ -532,15 +550,14 @@
     "CreateEvaluationFormRequestRequestTypeDef",
     "EvaluationFormContentTypeDef",
     "EvaluationFormTypeDef",
     "UpdateEvaluationFormRequestRequestTypeDef",
     "CreateParticipantRequestRequestTypeDef",
     "CreateParticipantResponseTypeDef",
     "CreatePredefinedAttributeRequestRequestTypeDef",
-    "PredefinedAttributeTypeDef",
     "UpdatePredefinedAttributeRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "QueueTypeDef",
     "UpdateQueueOutboundCallerConfigRequestRequestTypeDef",
     "UpdateUserIdentityInfoRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserPhoneConfigRequestRequestTypeDef",
@@ -557,24 +574,26 @@
     "DescribeTrafficDistributionGroupResponseTypeDef",
     "DescribeVocabularyResponseTypeDef",
     "DimensionsTypeDef",
     "DisassociateRoutingProfileQueuesRequestRequestTypeDef",
     "RoutingProfileQueueConfigTypeDef",
     "DisassociateUserProficienciesRequestRequestTypeDef",
     "StopContactRequestRequestTypeDef",
+    "GetAttachedFileResponseTypeDef",
     "KinesisVideoStreamConfigTypeDef",
     "S3ConfigTypeDef",
     "EvaluationAnswerInputTypeDef",
     "EvaluationAnswerOutputTypeDef",
     "EvaluationFormNumericQuestionAutomationTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationOptionTypeDef",
     "ListEvaluationFormsResponseTypeDef",
     "ListEvaluationFormVersionsResponseTypeDef",
     "EvaluationMetadataTypeDef",
     "EvaluationSummaryTypeDef",
+    "FieldValueOutputTypeDef",
     "FieldValueTypeDef",
     "GetCurrentMetricDataRequestRequestTypeDef",
     "ListAgentStatusRequestListAgentStatusesPaginateTypeDef",
     "ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     "ListBotsRequestListBotsPaginateTypeDef",
     "ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     "ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
@@ -637,14 +656,15 @@
     "InstanceTypeDef",
     "ListInstancesResponseTypeDef",
     "ListIntegrationAssociationsResponseTypeDef",
     "InvisibleFieldInfoTypeDef",
     "ReadOnlyFieldInfoTypeDef",
     "RequiredFieldInfoTypeDef",
     "TaskTemplateDefaultFieldValueTypeDef",
+    "TaskTemplateFieldOutputTypeDef",
     "TaskTemplateFieldTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "ListPhoneNumbersV2ResponseTypeDef",
     "ListPredefinedAttributesResponseTypeDef",
     "ListPromptsResponseTypeDef",
     "ListQueueQuickConnectsResponseTypeDef",
     "ListQuickConnectsResponseTypeDef",
@@ -656,107 +676,125 @@
     "ListTaskTemplatesResponseTypeDef",
     "ListTrafficDistributionGroupUsersResponseTypeDef",
     "ListTrafficDistributionGroupsResponseTypeDef",
     "ListUseCasesResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ListViewVersionsResponseTypeDef",
     "ListViewsResponseTypeDef",
+    "MetricV2OutputTypeDef",
     "MetricV2TypeDef",
     "NewSessionDetailsTypeDef",
+    "SendNotificationActionDefinitionOutputTypeDef",
     "SendNotificationActionDefinitionTypeDef",
     "ParticipantTimerConfigurationTypeDef",
-    "PredefinedAttributePaginatorTypeDef",
+    "PredefinedAttributeTypeDef",
+    "PredefinedAttributeValuesUnionTypeDef",
     "QuickConnectConfigTypeDef",
     "RealTimeContactAnalysisTranscriptItemRedactionTypeDef",
     "RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef",
     "RealTimeContactAnalysisTranscriptItemWithContentTypeDef",
     "RealTimeContactAnalysisSegmentAttachmentsTypeDef",
     "RealTimeContactAnalysisSegmentEventTypeDef",
     "ReferenceSummaryTypeDef",
     "StartOutboundVoiceContactRequestRequestTypeDef",
     "StartTaskContactRequestRequestTypeDef",
+    "TaskActionDefinitionOutputTypeDef",
     "TaskActionDefinitionTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ResourceTagsSearchCriteriaTypeDef",
     "SearchResourceTagsResponseTypeDef",
     "SearchSecurityProfilesResponseTypeDef",
     "SearchVocabulariesResponseTypeDef",
     "SearchableContactAttributesTypeDef",
     "StartChatContactRequestRequestTypeDef",
+    "SignInConfigOutputTypeDef",
     "SignInConfigTypeDef",
+    "StartAttachedFileUploadResponseTypeDef",
     "StartContactRecordingRequestRequestTypeDef",
     "TranscriptTypeDef",
     "UserSearchSummaryTypeDef",
     "ViewTypeDef",
     "ListRulesResponseTypeDef",
+    "AgentConfigUnionTypeDef",
+    "TelephonyConfigUnionTypeDef",
     "StartWebRTCContactRequestRequestTypeDef",
+    "CreateSecurityProfileRequestRequestTypeDef",
+    "UpdateSecurityProfileRequestRequestTypeDef",
     "ListBotsResponseTypeDef",
+    "BatchGetAttachedFileMetadataResponseTypeDef",
     "ControlPlaneUserAttributeFilterTypeDef",
     "HoursOfOperationSearchFilterTypeDef",
     "PromptSearchFilterTypeDef",
     "QueueSearchFilterTypeDef",
     "QuickConnectSearchFilterTypeDef",
     "RoutingProfileSearchFilterTypeDef",
     "SecurityProfilesSearchFilterTypeDef",
     "MeetingTypeDef",
     "DescribePhoneNumberResponseTypeDef",
     "BatchPutContactRequestRequestTypeDef",
     "GetCurrentUserDataRequestRequestTypeDef",
     "SearchContactsResponseTypeDef",
     "DescribeContactResponseTypeDef",
     "DescribeEvaluationFormResponseTypeDef",
-    "DescribePredefinedAttributeResponseTypeDef",
-    "SearchPredefinedAttributesResponseTypeDef",
     "DescribeQueueResponseTypeDef",
     "SearchQueuesResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "RoutingProfileTypeDef",
     "UpdateRoutingProfileConcurrencyRequestRequestTypeDef",
     "CurrentMetricResultTypeDef",
     "AssociateRoutingProfileQueuesRequestRequestTypeDef",
     "CreateRoutingProfileRequestRequestTypeDef",
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     "InstanceStorageConfigTypeDef",
     "SubmitContactEvaluationRequestRequestTypeDef",
     "UpdateContactEvaluationRequestRequestTypeDef",
+    "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
     "EvaluationFormNumericQuestionPropertiesTypeDef",
+    "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationTypeDef",
     "EvaluationTypeDef",
     "ListContactEvaluationsResponseTypeDef",
+    "CreateCaseActionDefinitionOutputTypeDef",
+    "UpdateCaseActionDefinitionOutputTypeDef",
     "CreateCaseActionDefinitionTypeDef",
     "UpdateCaseActionDefinitionTypeDef",
     "UserDataTypeDef",
     "HierarchyGroupTypeDef",
     "DescribeUserHierarchyStructureResponseTypeDef",
     "UpdateUserHierarchyStructureRequestRequestTypeDef",
     "GetMetricDataRequestGetMetricDataPaginateTypeDef",
     "GetMetricDataRequestRequestTypeDef",
     "HistoricalMetricDataTypeDef",
     "CreateHoursOfOperationRequestRequestTypeDef",
     "HoursOfOperationTypeDef",
     "UpdateHoursOfOperationRequestRequestTypeDef",
     "SearchPredefinedAttributesRequestSearchPredefinedAttributesPaginateTypeDef",
     "DescribeInstanceResponseTypeDef",
+    "TaskTemplateConstraintsOutputTypeDef",
     "TaskTemplateConstraintsTypeDef",
+    "TaskTemplateDefaultsOutputTypeDef",
     "TaskTemplateDefaultsTypeDef",
-    "GetMetricDataV2RequestRequestTypeDef",
+    "TaskTemplateFieldUnionTypeDef",
     "MetricDataV2TypeDef",
+    "MetricV2UnionTypeDef",
     "SendChatIntegrationEventRequestRequestTypeDef",
     "ChatParticipantRoleConfigTypeDef",
-    "SearchPredefinedAttributesResponsePaginatorTypeDef",
+    "DescribePredefinedAttributeResponseTypeDef",
+    "SearchPredefinedAttributesResponseTypeDef",
     "CreateQuickConnectRequestRequestTypeDef",
     "QuickConnectTypeDef",
     "UpdateQuickConnectConfigRequestRequestTypeDef",
     "RealTimeContactAnalysisSegmentTranscriptTypeDef",
     "RealTimeContactAnalysisPointOfInterestTypeDef",
     "RealTimeContactAnalysisIssueDetectedTypeDef",
     "ListContactReferencesResponseTypeDef",
     "SearchResourceTagsRequestRequestTypeDef",
     "SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
     "GetTrafficDistributionResponseTypeDef",
+    "SignInConfigUnionTypeDef",
     "UpdateTrafficDistributionRequestRequestTypeDef",
     "ContactAnalysisTypeDef",
     "SearchUsersResponseTypeDef",
     "CreateViewResponseTypeDef",
     "CreateViewVersionResponseTypeDef",
     "DescribeViewResponseTypeDef",
     "UpdateViewContentResponseTypeDef",
@@ -777,49 +815,58 @@
     "DescribeRoutingProfileResponseTypeDef",
     "SearchRoutingProfilesResponseTypeDef",
     "GetCurrentMetricDataResponseTypeDef",
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
     "DescribeInstanceStorageConfigResponseTypeDef",
     "ListInstanceStorageConfigsResponseTypeDef",
     "UpdateInstanceStorageConfigRequestRequestTypeDef",
+    "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
     "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
     "DescribeContactEvaluationResponseTypeDef",
+    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
     "GetCurrentUserDataResponseTypeDef",
     "DescribeUserHierarchyGroupResponseTypeDef",
     "HistoricalMetricResultTypeDef",
     "DescribeHoursOfOperationResponseTypeDef",
     "SearchHoursOfOperationsResponseTypeDef",
-    "CreateTaskTemplateRequestRequestTypeDef",
+    "TaskTemplateConstraintsUnionTypeDef",
     "GetTaskTemplateResponseTypeDef",
-    "UpdateTaskTemplateRequestRequestTypeDef",
     "UpdateTaskTemplateResponseTypeDef",
+    "TaskTemplateDefaultsUnionTypeDef",
+    "CreateTaskTemplateRequestRequestTypeDef",
+    "UpdateTaskTemplateRequestRequestTypeDef",
     "MetricResultV2TypeDef",
+    "GetMetricDataV2RequestRequestTypeDef",
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     "DescribeQuickConnectResponseTypeDef",
     "SearchQuickConnectsResponseTypeDef",
     "RealTimeContactAnalysisCategoryDetailsTypeDef",
     "RealTimeContactAnalysisSegmentIssuesTypeDef",
     "SearchCriteriaTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchUsersRequestSearchUsersPaginateTypeDef",
     "StartWebRTCContactResponseTypeDef",
+    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
     "EvaluationFormQuestionTypePropertiesTypeDef",
-    "CreateRuleRequestRequestTypeDef",
     "RuleTypeDef",
-    "UpdateRuleRequestRequestTypeDef",
+    "RuleActionUnionTypeDef",
     "GetMetricDataResponseTypeDef",
     "GetMetricDataV2ResponseTypeDef",
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     "RealTimeContactAnalysisSegmentCategoriesTypeDef",
     "SearchContactsRequestRequestTypeDef",
     "SearchContactsRequestSearchContactsPaginateTypeDef",
+    "EvaluationFormQuestionOutputTypeDef",
     "EvaluationFormQuestionTypeDef",
     "DescribeRuleResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
+    "UpdateRuleRequestRequestTypeDef",
     "RealtimeContactAnalysisSegmentTypeDef",
+    "EvaluationFormItemOutputTypeDef",
     "EvaluationFormItemTypeDef",
     "ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef",
 )
 
 ActionSummaryTypeDef = TypedDict(
     "ActionSummaryTypeDef",
     {
@@ -928,16 +975,23 @@
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "EnableAnswerMachineDetection": NotRequired[bool],
         "AwaitAnswerMachinePrompt": NotRequired[bool],
     },
 )
-ApplicationPaginatorTypeDef = TypedDict(
-    "ApplicationPaginatorTypeDef",
+ApplicationExtraOutputTypeDef = TypedDict(
+    "ApplicationExtraOutputTypeDef",
+    {
+        "Namespace": NotRequired[str],
+        "ApplicationPermissions": NotRequired[List[str]],
+    },
+)
+ApplicationOutputTypeDef = TypedDict(
+    "ApplicationOutputTypeDef",
     {
         "Namespace": NotRequired[str],
         "ApplicationPermissions": NotRequired[List[str]],
     },
 )
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
@@ -1033,14 +1087,29 @@
     "UserProficiencyTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
         "Level": float,
     },
 )
+AttachedFileErrorTypeDef = TypedDict(
+    "AttachedFileErrorTypeDef",
+    {
+        "ErrorCode": NotRequired[str],
+        "ErrorMessage": NotRequired[str],
+        "FileId": NotRequired[str],
+    },
+)
+CreatedByInfoTypeDef = TypedDict(
+    "CreatedByInfoTypeDef",
+    {
+        "ConnectUserArn": NotRequired[str],
+        "AWSIdentityArn": NotRequired[str],
+    },
+)
 AttachmentReferenceTypeDef = TypedDict(
     "AttachmentReferenceTypeDef",
     {
         "Name": NotRequired[str],
         "Value": NotRequired[str],
         "Status": NotRequired[ReferenceStatusType],
     },
@@ -1106,14 +1175,22 @@
     "BatchDisassociateAnalyticsDataSetRequestRequestTypeDef",
     {
         "InstanceId": str,
         "DataSetIds": Sequence[str],
         "TargetAccountId": NotRequired[str],
     },
 )
+BatchGetAttachedFileMetadataRequestRequestTypeDef = TypedDict(
+    "BatchGetAttachedFileMetadataRequestRequestTypeDef",
+    {
+        "FileIds": Sequence[str],
+        "InstanceId": str,
+        "AssociatedResourceArn": str,
+    },
+)
 BatchGetFlowAssociationRequestRequestTypeDef = TypedDict(
     "BatchGetFlowAssociationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceIds": Sequence[str],
         "ResourceType": NotRequired[Literal["VOICE_PHONE_NUMBER"]],
     },
@@ -1182,14 +1259,22 @@
 PhoneNumberStatusTypeDef = TypedDict(
     "PhoneNumberStatusTypeDef",
     {
         "Status": NotRequired[PhoneNumberWorkflowStatusType],
         "Message": NotRequired[str],
     },
 )
+CompleteAttachedFileUploadRequestRequestTypeDef = TypedDict(
+    "CompleteAttachedFileUploadRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "FileId": str,
+        "AssociatedResourceArn": str,
+    },
+)
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Type": NotRequired[EndpointTypeType],
         "Address": NotRequired[str],
     },
 )
@@ -1300,14 +1385,17 @@
         "Name": str,
         "Type": ContactFlowTypeType,
         "Content": str,
         "Description": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
+EvaluationFormItemUnionTypeDef = Union[
+    "EvaluationFormItemTypeDef", "EvaluationFormItemOutputTypeDef"
+]
 EvaluationFormScoringStrategyTypeDef = TypedDict(
     "EvaluationFormScoringStrategyTypeDef",
     {
         "Mode": EvaluationFormScoringModeType,
         "Status": EvaluationFormScoringStatusType,
     },
 )
@@ -1513,14 +1601,22 @@
     {
         "InstanceId": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "VocabularyId": str,
         "VocabularyName": str,
     },
 )
+DeleteAttachedFileRequestRequestTypeDef = TypedDict(
+    "DeleteAttachedFileRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "FileId": str,
+        "AssociatedResourceArn": str,
+    },
+)
 DeleteContactEvaluationRequestRequestTypeDef = TypedDict(
     "DeleteContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
     },
 )
@@ -2001,14 +2097,21 @@
     "DismissUserContactRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
         "ContactId": str,
     },
 )
+DownloadUrlMetadataTypeDef = TypedDict(
+    "DownloadUrlMetadataTypeDef",
+    {
+        "Url": NotRequired[str],
+        "UrlExpiry": NotRequired[str],
+    },
+)
 EmailReferenceTypeDef = TypedDict(
     "EmailReferenceTypeDef",
     {
         "Name": NotRequired[str],
         "Value": NotRequired[str],
     },
 )
@@ -2038,14 +2141,24 @@
     {
         "MinValue": int,
         "MaxValue": int,
         "Score": NotRequired[int],
         "AutomaticFail": NotRequired[bool],
     },
 )
+EvaluationFormSectionOutputTypeDef = TypedDict(
+    "EvaluationFormSectionOutputTypeDef",
+    {
+        "Title": str,
+        "RefId": str,
+        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "Instructions": NotRequired[str],
+        "Weight": NotRequired[float],
+    },
+)
 EvaluationFormSectionTypeDef = TypedDict(
     "EvaluationFormSectionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "Items": Sequence["EvaluationFormItemTypeDef"],
         "Instructions": NotRequired[str],
@@ -2115,14 +2228,23 @@
 )
 EventBridgeActionDefinitionTypeDef = TypedDict(
     "EventBridgeActionDefinitionTypeDef",
     {
         "Name": str,
     },
 )
+FieldValueUnionOutputTypeDef = TypedDict(
+    "FieldValueUnionOutputTypeDef",
+    {
+        "BooleanValue": NotRequired[bool],
+        "DoubleValue": NotRequired[float],
+        "EmptyValue": NotRequired[Dict[str, Any]],
+        "StringValue": NotRequired[str],
+    },
+)
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "BooleanValue": NotRequired[bool],
         "DoubleValue": NotRequired[float],
         "EmptyValue": NotRequired[Mapping[str, Any]],
         "StringValue": NotRequired[str],
@@ -2140,14 +2262,23 @@
     {
         "Queues": NotRequired[Sequence[str]],
         "Channels": NotRequired[Sequence[ChannelType]],
         "RoutingProfiles": NotRequired[Sequence[str]],
         "RoutingStepExpressions": NotRequired[Sequence[str]],
     },
 )
+GetAttachedFileRequestRequestTypeDef = TypedDict(
+    "GetAttachedFileRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "FileId": str,
+        "AssociatedResourceArn": str,
+        "UrlExpiryInSeconds": NotRequired[int],
+    },
+)
 GetContactAttributesRequestRequestTypeDef = TypedDict(
     "GetContactAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "InitialContactId": str,
     },
 )
@@ -2892,14 +3023,22 @@
         "AudioHostUrl": NotRequired[str],
         "AudioFallbackUrl": NotRequired[str],
         "SignalingUrl": NotRequired[str],
         "TurnControlUrl": NotRequired[str],
         "EventIngestionUrl": NotRequired[str],
     },
 )
+MetricFilterV2OutputTypeDef = TypedDict(
+    "MetricFilterV2OutputTypeDef",
+    {
+        "MetricFilterKey": NotRequired[str],
+        "MetricFilterValues": NotRequired[List[str]],
+        "Negate": NotRequired[bool],
+    },
+)
 MetricFilterV2TypeDef = TypedDict(
     "MetricFilterV2TypeDef",
     {
         "MetricFilterKey": NotRequired[str],
         "MetricFilterValues": NotRequired[Sequence[str]],
         "Negate": NotRequired[bool],
     },
@@ -2931,14 +3070,21 @@
 )
 ParticipantDetailsTypeDef = TypedDict(
     "ParticipantDetailsTypeDef",
     {
         "DisplayName": str,
     },
 )
+NotificationRecipientTypeOutputTypeDef = TypedDict(
+    "NotificationRecipientTypeOutputTypeDef",
+    {
+        "UserTags": NotRequired[Dict[str, str]],
+        "UserIds": NotRequired[List[str]],
+    },
+)
 NotificationRecipientTypeTypeDef = TypedDict(
     "NotificationRecipientTypeTypeDef",
     {
         "UserTags": NotRequired[Mapping[str, str]],
         "UserIds": NotRequired[Sequence[str]],
     },
 )
@@ -2973,16 +3119,22 @@
 )
 PhoneNumberQuickConnectConfigTypeDef = TypedDict(
     "PhoneNumberQuickConnectConfigTypeDef",
     {
         "PhoneNumber": str,
     },
 )
-PredefinedAttributeValuesPaginatorTypeDef = TypedDict(
-    "PredefinedAttributeValuesPaginatorTypeDef",
+PredefinedAttributeValuesOutputTypeDef = TypedDict(
+    "PredefinedAttributeValuesOutputTypeDef",
+    {
+        "StringList": NotRequired[List[str]],
+    },
+)
+PredefinedAttributeValuesExtraOutputTypeDef = TypedDict(
+    "PredefinedAttributeValuesExtraOutputTypeDef",
     {
         "StringList": NotRequired[List[str]],
     },
 )
 PutUserStatusRequestRequestTypeDef = TypedDict(
     "PutUserStatusRequestRequestTypeDef",
     {
@@ -3180,14 +3332,22 @@
 SignInDistributionTypeDef = TypedDict(
     "SignInDistributionTypeDef",
     {
         "Region": str,
         "Enabled": bool,
     },
 )
+UploadUrlMetadataTypeDef = TypedDict(
+    "UploadUrlMetadataTypeDef",
+    {
+        "Url": NotRequired[str],
+        "UrlExpiry": NotRequired[str],
+        "HeadersToInclude": NotRequired[Dict[str, str]],
+    },
+)
 StartContactEvaluationRequestRequestTypeDef = TypedDict(
     "StartContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "EvaluationFormId": str,
         "ClientToken": NotRequired[str],
@@ -3782,34 +3942,34 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListApprovedOriginsResponseTypeDef = TypedDict(
     "ListApprovedOriginsResponseTypeDef",
     {
         "Origins": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListLambdaFunctionsResponseTypeDef = TypedDict(
     "ListLambdaFunctionsResponseTypeDef",
     {
         "LambdaFunctions": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSecurityProfilePermissionsResponseTypeDef = TypedDict(
     "ListSecurityProfilePermissionsResponseTypeDef",
     {
         "Permissions": List[str],
-        "NextToken": str,
         "LastModifiedTime": datetime,
         "LastModifiedRegion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3923,24 +4083,36 @@
     "UpdatePromptResponseTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AgentConfigOutputTypeDef = TypedDict(
+    "AgentConfigOutputTypeDef",
+    {
+        "Distributions": List[DistributionTypeDef],
+    },
+)
 AgentConfigTypeDef = TypedDict(
     "AgentConfigTypeDef",
     {
+        "Distributions": Sequence[DistributionTypeDef],
+    },
+)
+TelephonyConfigOutputTypeDef = TypedDict(
+    "TelephonyConfigOutputTypeDef",
+    {
         "Distributions": List[DistributionTypeDef],
     },
 )
 TelephonyConfigTypeDef = TypedDict(
     "TelephonyConfigTypeDef",
     {
-        "Distributions": List[DistributionTypeDef],
+        "Distributions": Sequence[DistributionTypeDef],
     },
 )
 AgentContactReferenceTypeDef = TypedDict(
     "AgentContactReferenceTypeDef",
     {
         "ContactId": NotRequired[str],
         "Channel": NotRequired[ChannelType],
@@ -3950,17 +4122,17 @@
         "ConnectedToAgentTimestamp": NotRequired[datetime],
         "Queue": NotRequired[QueueReferenceTypeDef],
     },
 )
 ListAgentStatusResponseTypeDef = TypedDict(
     "ListAgentStatusResponseTypeDef",
     {
-        "NextToken": str,
         "AgentStatusSummaryList": List[AgentStatusSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeAgentStatusResponseTypeDef = TypedDict(
     "DescribeAgentStatusResponseTypeDef",
     {
         "AgentStatus": AgentStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3973,80 +4145,42 @@
         "Agent": NotRequired[ParticipantCapabilitiesTypeDef],
     },
 )
 ListAnalyticsDataAssociationsResponseTypeDef = TypedDict(
     "ListAnalyticsDataAssociationsResponseTypeDef",
     {
         "Results": List[AnalyticsDataAssociationResultTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ListSecurityProfileApplicationsResponsePaginatorTypeDef = TypedDict(
-    "ListSecurityProfileApplicationsResponsePaginatorTypeDef",
-    {
-        "Applications": List[ApplicationPaginatorTypeDef],
-        "NextToken": str,
-        "LastModifiedTime": datetime,
-        "LastModifiedRegion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "CreateSecurityProfileRequestRequestTypeDef",
-    {
-        "SecurityProfileName": str,
-        "InstanceId": str,
-        "Description": NotRequired[str],
-        "Permissions": NotRequired[Sequence[str]],
-        "Tags": NotRequired[Mapping[str, str]],
-        "AllowedAccessControlTags": NotRequired[Mapping[str, str]],
-        "TagRestrictedResources": NotRequired[Sequence[str]],
-        "Applications": NotRequired[Sequence[ApplicationTypeDef]],
-        "HierarchyRestrictedResources": NotRequired[Sequence[str]],
-        "AllowedAccessControlHierarchyGroupId": NotRequired[str],
+        "NextToken": NotRequired[str],
     },
 )
 ListSecurityProfileApplicationsResponseTypeDef = TypedDict(
     "ListSecurityProfileApplicationsResponseTypeDef",
     {
-        "Applications": List[ApplicationTypeDef],
-        "NextToken": str,
+        "Applications": List[ApplicationExtraOutputTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedRegion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-UpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "SecurityProfileId": str,
-        "InstanceId": str,
-        "Description": NotRequired[str],
-        "Permissions": NotRequired[Sequence[str]],
-        "AllowedAccessControlTags": NotRequired[Mapping[str, str]],
-        "TagRestrictedResources": NotRequired[Sequence[str]],
-        "Applications": NotRequired[Sequence[ApplicationTypeDef]],
-        "HierarchyRestrictedResources": NotRequired[Sequence[str]],
-        "AllowedAccessControlHierarchyGroupId": NotRequired[str],
-    },
-)
+ApplicationUnionTypeDef = Union[ApplicationTypeDef, ApplicationExtraOutputTypeDef]
 AssociateLexBotRequestRequestTypeDef = TypedDict(
     "AssociateLexBotRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LexBot": LexBotTypeDef,
     },
 )
 ListLexBotsResponseTypeDef = TypedDict(
     "ListLexBotsResponseTypeDef",
     {
         "LexBots": List[LexBotTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateBotRequestRequestTypeDef = TypedDict(
     "AssociateBotRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LexBot": NotRequired[LexBotTypeDef],
@@ -4075,29 +4209,58 @@
         "UserId": str,
         "UserProficiencies": Sequence[UserProficiencyTypeDef],
     },
 )
 ListUserProficienciesResponseTypeDef = TypedDict(
     "ListUserProficienciesResponseTypeDef",
     {
-        "NextToken": str,
         "UserProficiencyList": List[UserProficiencyTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedRegion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateUserProficienciesRequestRequestTypeDef = TypedDict(
     "UpdateUserProficienciesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "UserId": str,
         "UserProficiencies": Sequence[UserProficiencyTypeDef],
     },
 )
+AttachedFileTypeDef = TypedDict(
+    "AttachedFileTypeDef",
+    {
+        "CreationTime": str,
+        "FileArn": str,
+        "FileId": str,
+        "FileName": str,
+        "FileSizeInBytes": int,
+        "FileStatus": FileStatusTypeType,
+        "CreatedBy": NotRequired[CreatedByInfoTypeDef],
+        "FileUseCaseType": NotRequired[Literal["ATTACHMENT"]],
+        "AssociatedResourceArn": NotRequired[str],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
+StartAttachedFileUploadRequestRequestTypeDef = TypedDict(
+    "StartAttachedFileUploadRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "FileName": str,
+        "FileSizeInBytes": int,
+        "FileUseCaseType": Literal["ATTACHMENT"],
+        "AssociatedResourceArn": str,
+        "ClientToken": NotRequired[str],
+        "UrlExpiryInSeconds": NotRequired[int],
+        "CreatedBy": NotRequired[CreatedByInfoTypeDef],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
 AttributeAndConditionTypeDef = TypedDict(
     "AttributeAndConditionTypeDef",
     {
         "TagConditions": NotRequired[Sequence[TagConditionTypeDef]],
         "HierarchyGroupCondition": NotRequired[HierarchyGroupConditionTypeDef],
     },
 )
@@ -4116,30 +4279,30 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInstanceAttributesResponseTypeDef = TypedDict(
     "ListInstanceAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 MeetingFeaturesConfigurationTypeDef = TypedDict(
     "MeetingFeaturesConfigurationTypeDef",
     {
         "Audio": NotRequired[AudioFeaturesTypeDef],
     },
 )
 SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
     "SearchAvailablePhoneNumbersResponseTypeDef",
     {
-        "NextToken": str,
         "AvailableNumbersList": List[AvailableNumberSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchAssociateAnalyticsDataSetResponseTypeDef = TypedDict(
     "BatchAssociateAnalyticsDataSetResponseTypeDef",
     {
         "Created": List[AnalyticsDataAssociationResultTypeDef],
         "Errors": List[ErrorResultTypeDef],
@@ -4161,16 +4324,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListFlowAssociationsResponseTypeDef = TypedDict(
     "ListFlowAssociationsResponseTypeDef",
     {
         "FlowAssociationSummaryList": List[FlowAssociationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchPutContactResponseTypeDef = TypedDict(
     "BatchPutContactResponseTypeDef",
     {
         "SuccessfulRequestList": List[SuccessfulRequestTypeDef],
         "FailedRequestList": List[FailedRequestTypeDef],
@@ -4223,31 +4386,31 @@
         "UserHierarchyGroups": NotRequired[Sequence[str]],
     },
 )
 ListContactFlowModulesResponseTypeDef = TypedDict(
     "ListContactFlowModulesResponseTypeDef",
     {
         "ContactFlowModulesSummaryList": List[ContactFlowModuleSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeContactFlowModuleResponseTypeDef = TypedDict(
     "DescribeContactFlowModuleResponseTypeDef",
     {
         "ContactFlowModule": ContactFlowModuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListContactFlowsResponseTypeDef = TypedDict(
     "ListContactFlowsResponseTypeDef",
     {
         "ContactFlowSummaryList": List[ContactFlowSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeContactFlowResponseTypeDef = TypedDict(
     "DescribeContactFlowResponseTypeDef",
     {
         "ContactFlow": ContactFlowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4298,42 +4461,42 @@
     },
 )
 CreateEvaluationFormRequestRequestTypeDef = TypedDict(
     "CreateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Title": str,
-        "Items": Sequence["EvaluationFormItemTypeDef"],
+        "Items": Sequence[EvaluationFormItemUnionTypeDef],
         "Description": NotRequired[str],
         "ScoringStrategy": NotRequired[EvaluationFormScoringStrategyTypeDef],
         "ClientToken": NotRequired[str],
     },
 )
 EvaluationFormContentTypeDef = TypedDict(
     "EvaluationFormContentTypeDef",
     {
         "EvaluationFormVersion": int,
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
-        "Items": List["EvaluationFormItemTypeDef"],
+        "Items": List["EvaluationFormItemOutputTypeDef"],
         "Description": NotRequired[str],
         "ScoringStrategy": NotRequired[EvaluationFormScoringStrategyTypeDef],
     },
 )
 EvaluationFormTypeDef = TypedDict(
     "EvaluationFormTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
         "EvaluationFormArn": str,
         "Title": str,
         "Status": EvaluationFormVersionStatusType,
-        "Items": List["EvaluationFormItemTypeDef"],
+        "Items": List["EvaluationFormItemOutputTypeDef"],
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
         "Description": NotRequired[str],
         "ScoringStrategy": NotRequired[EvaluationFormScoringStrategyTypeDef],
         "Tags": NotRequired[Dict[str, str]],
@@ -4342,15 +4505,15 @@
 UpdateEvaluationFormRequestRequestTypeDef = TypedDict(
     "UpdateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Title": str,
-        "Items": Sequence["EvaluationFormItemTypeDef"],
+        "Items": Sequence[EvaluationFormItemUnionTypeDef],
         "CreateNewVersion": NotRequired[bool],
         "Description": NotRequired[str],
         "ScoringStrategy": NotRequired[EvaluationFormScoringStrategyTypeDef],
         "ClientToken": NotRequired[str],
     },
 )
 CreateParticipantRequestRequestTypeDef = TypedDict(
@@ -4374,23 +4537,14 @@
     "CreatePredefinedAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
         "Values": PredefinedAttributeValuesTypeDef,
     },
 )
-PredefinedAttributeTypeDef = TypedDict(
-    "PredefinedAttributeTypeDef",
-    {
-        "Name": NotRequired[str],
-        "Values": NotRequired[PredefinedAttributeValuesTypeDef],
-        "LastModifiedTime": NotRequired[datetime],
-        "LastModifiedRegion": NotRequired[str],
-    },
-)
 UpdatePredefinedAttributeRequestRequestTypeDef = TypedDict(
     "UpdatePredefinedAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
         "Values": NotRequired[PredefinedAttributeValuesTypeDef],
     },
@@ -4526,32 +4680,32 @@
         "Value": NotRequired[float],
     },
 )
 ListDefaultVocabulariesResponseTypeDef = TypedDict(
     "ListDefaultVocabulariesResponseTypeDef",
     {
         "DefaultVocabularyList": List[DefaultVocabularyTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribePromptResponseTypeDef = TypedDict(
     "DescribePromptResponseTypeDef",
     {
         "Prompt": PromptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchPromptsResponseTypeDef = TypedDict(
     "SearchPromptsResponseTypeDef",
     {
         "Prompts": List[PromptTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSecurityProfileResponseTypeDef = TypedDict(
     "DescribeSecurityProfileResponseTypeDef",
     {
         "SecurityProfile": SecurityProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4608,14 +4762,31 @@
     "StopContactRequestRequestTypeDef",
     {
         "ContactId": str,
         "InstanceId": str,
         "DisconnectReason": NotRequired[DisconnectReasonTypeDef],
     },
 )
+GetAttachedFileResponseTypeDef = TypedDict(
+    "GetAttachedFileResponseTypeDef",
+    {
+        "FileArn": str,
+        "FileId": str,
+        "CreationTime": str,
+        "FileStatus": FileStatusTypeType,
+        "FileName": str,
+        "FileSizeInBytes": int,
+        "AssociatedResourceArn": str,
+        "FileUseCaseType": Literal["ATTACHMENT"],
+        "CreatedBy": CreatedByInfoTypeDef,
+        "DownloadUrlMetadata": DownloadUrlMetadataTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 KinesisVideoStreamConfigTypeDef = TypedDict(
     "KinesisVideoStreamConfigTypeDef",
     {
         "Prefix": str,
         "RetentionPeriodHours": int,
         "EncryptionConfig": EncryptionConfigTypeDef,
     },
@@ -4653,24 +4824,24 @@
         "RuleCategory": NotRequired[SingleSelectQuestionRuleCategoryAutomationTypeDef],
     },
 )
 ListEvaluationFormsResponseTypeDef = TypedDict(
     "ListEvaluationFormsResponseTypeDef",
     {
         "EvaluationFormSummaryList": List[EvaluationFormSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListEvaluationFormVersionsResponseTypeDef = TypedDict(
     "ListEvaluationFormVersionsResponseTypeDef",
     {
         "EvaluationFormVersionSummaryList": List[EvaluationFormVersionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 EvaluationMetadataTypeDef = TypedDict(
     "EvaluationMetadataTypeDef",
     {
         "ContactId": str,
         "EvaluatorArn": str,
@@ -4688,14 +4859,21 @@
         "Status": EvaluationStatusType,
         "EvaluatorArn": str,
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
         "Score": NotRequired[EvaluationScoreTypeDef],
     },
 )
+FieldValueOutputTypeDef = TypedDict(
+    "FieldValueOutputTypeDef",
+    {
+        "Id": str,
+        "Value": FieldValueUnionOutputTypeDef,
+    },
+)
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "Id": str,
         "Value": FieldValueUnionTypeDef,
     },
 )
@@ -5089,16 +5267,16 @@
         "LevelFive": NotRequired[HierarchyGroupSummaryTypeDef],
     },
 )
 ListUserHierarchyGroupsResponseTypeDef = TypedDict(
     "ListUserHierarchyGroupsResponseTypeDef",
     {
         "UserHierarchyGroupSummaryList": List[HierarchyGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 HierarchyStructureTypeDef = TypedDict(
     "HierarchyStructureTypeDef",
     {
         "LevelOne": NotRequired[HierarchyLevelTypeDef],
         "LevelTwo": NotRequired[HierarchyLevelTypeDef],
@@ -5200,16 +5378,16 @@
         "HierarchyGroupCondition": NotRequired[HierarchyGroupConditionTypeDef],
     },
 )
 ListHoursOfOperationsResponseTypeDef = TypedDict(
     "ListHoursOfOperationsResponseTypeDef",
     {
         "HoursOfOperationSummaryList": List[HoursOfOperationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "Id": NotRequired[str],
         "Arn": NotRequired[str],
@@ -5225,24 +5403,24 @@
         "Tags": NotRequired[Dict[str, str]],
     },
 )
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "InstanceSummaryList": List[InstanceSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListIntegrationAssociationsResponseTypeDef",
     {
         "IntegrationAssociationSummaryList": List[IntegrationAssociationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InvisibleFieldInfoTypeDef = TypedDict(
     "InvisibleFieldInfoTypeDef",
     {
         "Id": NotRequired[TaskTemplateFieldIdentifierTypeDef],
     },
@@ -5262,169 +5440,186 @@
 TaskTemplateDefaultFieldValueTypeDef = TypedDict(
     "TaskTemplateDefaultFieldValueTypeDef",
     {
         "Id": NotRequired[TaskTemplateFieldIdentifierTypeDef],
         "DefaultValue": NotRequired[str],
     },
 )
+TaskTemplateFieldOutputTypeDef = TypedDict(
+    "TaskTemplateFieldOutputTypeDef",
+    {
+        "Id": TaskTemplateFieldIdentifierTypeDef,
+        "Description": NotRequired[str],
+        "Type": NotRequired[TaskTemplateFieldTypeType],
+        "SingleSelectOptions": NotRequired[List[str]],
+    },
+)
 TaskTemplateFieldTypeDef = TypedDict(
     "TaskTemplateFieldTypeDef",
     {
         "Id": TaskTemplateFieldIdentifierTypeDef,
         "Description": NotRequired[str],
         "Type": NotRequired[TaskTemplateFieldTypeType],
         "SingleSelectOptions": NotRequired[Sequence[str]],
     },
 )
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumberSummaryList": List[PhoneNumberSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPhoneNumbersV2ResponseTypeDef = TypedDict(
     "ListPhoneNumbersV2ResponseTypeDef",
     {
-        "NextToken": str,
         "ListPhoneNumbersSummaryList": List[ListPhoneNumbersSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPredefinedAttributesResponseTypeDef = TypedDict(
     "ListPredefinedAttributesResponseTypeDef",
     {
-        "NextToken": str,
         "PredefinedAttributeSummaryList": List[PredefinedAttributeSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPromptsResponseTypeDef = TypedDict(
     "ListPromptsResponseTypeDef",
     {
         "PromptSummaryList": List[PromptSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListQueueQuickConnectsResponseTypeDef = TypedDict(
     "ListQueueQuickConnectsResponseTypeDef",
     {
-        "NextToken": str,
         "QuickConnectSummaryList": List[QuickConnectSummaryTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedRegion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListQuickConnectsResponseTypeDef = TypedDict(
     "ListQuickConnectsResponseTypeDef",
     {
         "QuickConnectSummaryList": List[QuickConnectSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListQueuesResponseTypeDef = TypedDict(
     "ListQueuesResponseTypeDef",
     {
         "QueueSummaryList": List[QueueSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListRoutingProfileQueuesResponseTypeDef = TypedDict(
     "ListRoutingProfileQueuesResponseTypeDef",
     {
-        "NextToken": str,
         "RoutingProfileQueueConfigSummaryList": List[RoutingProfileQueueConfigSummaryTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedRegion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListRoutingProfilesResponseTypeDef = TypedDict(
     "ListRoutingProfilesResponseTypeDef",
     {
         "RoutingProfileSummaryList": List[RoutingProfileSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSecurityKeysResponseTypeDef = TypedDict(
     "ListSecurityKeysResponseTypeDef",
     {
         "SecurityKeys": List[SecurityKeyTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSecurityProfilesResponseTypeDef = TypedDict(
     "ListSecurityProfilesResponseTypeDef",
     {
         "SecurityProfileSummaryList": List[SecurityProfileSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTaskTemplatesResponseTypeDef = TypedDict(
     "ListTaskTemplatesResponseTypeDef",
     {
         "TaskTemplates": List[TaskTemplateMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTrafficDistributionGroupUsersResponseTypeDef = TypedDict(
     "ListTrafficDistributionGroupUsersResponseTypeDef",
     {
-        "NextToken": str,
         "TrafficDistributionGroupUserSummaryList": List[TrafficDistributionGroupUserSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTrafficDistributionGroupsResponseTypeDef = TypedDict(
     "ListTrafficDistributionGroupsResponseTypeDef",
     {
-        "NextToken": str,
         "TrafficDistributionGroupSummaryList": List[TrafficDistributionGroupSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUseCasesResponseTypeDef = TypedDict(
     "ListUseCasesResponseTypeDef",
     {
         "UseCaseSummaryList": List[UseCaseTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "UserSummaryList": List[UserSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListViewVersionsResponseTypeDef = TypedDict(
     "ListViewVersionsResponseTypeDef",
     {
         "ViewVersionSummaryList": List[ViewVersionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListViewsResponseTypeDef = TypedDict(
     "ListViewsResponseTypeDef",
     {
         "ViewsSummaryList": List[ViewSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+MetricV2OutputTypeDef = TypedDict(
+    "MetricV2OutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Threshold": NotRequired[List[ThresholdV2TypeDef]],
+        "MetricFilters": NotRequired[List[MetricFilterV2OutputTypeDef]],
     },
 )
 MetricV2TypeDef = TypedDict(
     "MetricV2TypeDef",
     {
         "Name": NotRequired[str],
         "Threshold": NotRequired[Sequence[ThresholdV2TypeDef]],
@@ -5436,14 +5631,24 @@
     {
         "SupportedMessagingContentTypes": NotRequired[Sequence[str]],
         "ParticipantDetails": NotRequired[ParticipantDetailsTypeDef],
         "Attributes": NotRequired[Mapping[str, str]],
         "StreamingConfiguration": NotRequired[ChatStreamingConfigurationTypeDef],
     },
 )
+SendNotificationActionDefinitionOutputTypeDef = TypedDict(
+    "SendNotificationActionDefinitionOutputTypeDef",
+    {
+        "DeliveryMethod": Literal["EMAIL"],
+        "Content": str,
+        "ContentType": Literal["PLAIN_TEXT"],
+        "Recipient": NotificationRecipientTypeOutputTypeDef,
+        "Subject": NotRequired[str],
+    },
+)
 SendNotificationActionDefinitionTypeDef = TypedDict(
     "SendNotificationActionDefinitionTypeDef",
     {
         "DeliveryMethod": Literal["EMAIL"],
         "Content": str,
         "ContentType": Literal["PLAIN_TEXT"],
         "Recipient": NotificationRecipientTypeTypeDef,
@@ -5454,23 +5659,26 @@
     "ParticipantTimerConfigurationTypeDef",
     {
         "ParticipantRole": TimerEligibleParticipantRolesType,
         "TimerType": ParticipantTimerTypeType,
         "TimerValue": ParticipantTimerValueTypeDef,
     },
 )
-PredefinedAttributePaginatorTypeDef = TypedDict(
-    "PredefinedAttributePaginatorTypeDef",
+PredefinedAttributeTypeDef = TypedDict(
+    "PredefinedAttributeTypeDef",
     {
         "Name": NotRequired[str],
-        "Values": NotRequired[PredefinedAttributeValuesPaginatorTypeDef],
+        "Values": NotRequired[PredefinedAttributeValuesOutputTypeDef],
         "LastModifiedTime": NotRequired[datetime],
         "LastModifiedRegion": NotRequired[str],
     },
 )
+PredefinedAttributeValuesUnionTypeDef = Union[
+    PredefinedAttributeValuesTypeDef, PredefinedAttributeValuesExtraOutputTypeDef
+]
 QuickConnectConfigTypeDef = TypedDict(
     "QuickConnectConfigTypeDef",
     {
         "QuickConnectType": QuickConnectTypeType,
         "UserConfig": NotRequired[UserQuickConnectConfigTypeDef],
         "QueueConfig": NotRequired[QueueQuickConnectConfigTypeDef],
         "PhoneConfig": NotRequired[PhoneNumberQuickConnectConfigTypeDef],
@@ -5562,14 +5770,23 @@
         "ClientToken": NotRequired[str],
         "ScheduledTime": NotRequired[TimestampTypeDef],
         "TaskTemplateId": NotRequired[str],
         "QuickConnectId": NotRequired[str],
         "RelatedContactId": NotRequired[str],
     },
 )
+TaskActionDefinitionOutputTypeDef = TypedDict(
+    "TaskActionDefinitionOutputTypeDef",
+    {
+        "Name": str,
+        "ContactFlowId": str,
+        "Description": NotRequired[str],
+        "References": NotRequired[Dict[str, ReferenceTypeDef]],
+    },
+)
 TaskActionDefinitionTypeDef = TypedDict(
     "TaskActionDefinitionTypeDef",
     {
         "Name": str,
         "ContactFlowId": str,
         "Description": NotRequired[str],
         "References": NotRequired[Mapping[str, ReferenceTypeDef]],
@@ -5591,33 +5808,33 @@
         "TagSearchCondition": NotRequired[TagSearchConditionTypeDef],
     },
 )
 SearchResourceTagsResponseTypeDef = TypedDict(
     "SearchResourceTagsResponseTypeDef",
     {
         "Tags": List[TagSetTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchSecurityProfilesResponseTypeDef = TypedDict(
     "SearchSecurityProfilesResponseTypeDef",
     {
         "SecurityProfiles": List[SecurityProfileSearchSummaryTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchVocabulariesResponseTypeDef = TypedDict(
     "SearchVocabulariesResponseTypeDef",
     {
         "VocabularySummaryList": List[VocabularySummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchableContactAttributesTypeDef = TypedDict(
     "SearchableContactAttributesTypeDef",
     {
         "Criteria": Sequence[SearchableContactAttributesCriteriaTypeDef],
         "MatchType": NotRequired[SearchContactsMatchTypeType],
@@ -5635,18 +5852,36 @@
         "ChatDurationInMinutes": NotRequired[int],
         "SupportedMessagingContentTypes": NotRequired[Sequence[str]],
         "PersistentChat": NotRequired[PersistentChatTypeDef],
         "RelatedContactId": NotRequired[str],
         "SegmentAttributes": NotRequired[Mapping[str, SegmentAttributeValueTypeDef]],
     },
 )
+SignInConfigOutputTypeDef = TypedDict(
+    "SignInConfigOutputTypeDef",
+    {
+        "Distributions": List[SignInDistributionTypeDef],
+    },
+)
 SignInConfigTypeDef = TypedDict(
     "SignInConfigTypeDef",
     {
-        "Distributions": List[SignInDistributionTypeDef],
+        "Distributions": Sequence[SignInDistributionTypeDef],
+    },
+)
+StartAttachedFileUploadResponseTypeDef = TypedDict(
+    "StartAttachedFileUploadResponseTypeDef",
+    {
+        "FileArn": str,
+        "FileId": str,
+        "CreationTime": str,
+        "FileStatus": FileStatusTypeType,
+        "CreatedBy": CreatedByInfoTypeDef,
+        "UploadUrlMetadata": UploadUrlMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StartContactRecordingRequestRequestTypeDef = TypedDict(
     "StartContactRecordingRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
@@ -5694,37 +5929,76 @@
         "ViewContentSha256": NotRequired[str],
     },
 )
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "RuleSummaryList": List[RuleSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
+AgentConfigUnionTypeDef = Union[AgentConfigTypeDef, AgentConfigOutputTypeDef]
+TelephonyConfigUnionTypeDef = Union[TelephonyConfigTypeDef, TelephonyConfigOutputTypeDef]
 StartWebRTCContactRequestRequestTypeDef = TypedDict(
     "StartWebRTCContactRequestRequestTypeDef",
     {
         "ContactFlowId": str,
         "InstanceId": str,
         "ParticipantDetails": ParticipantDetailsTypeDef,
         "Attributes": NotRequired[Mapping[str, str]],
         "ClientToken": NotRequired[str],
         "AllowedCapabilities": NotRequired[AllowedCapabilitiesTypeDef],
         "RelatedContactId": NotRequired[str],
         "References": NotRequired[Mapping[str, ReferenceTypeDef]],
         "Description": NotRequired[str],
     },
 )
+CreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "CreateSecurityProfileRequestRequestTypeDef",
+    {
+        "SecurityProfileName": str,
+        "InstanceId": str,
+        "Description": NotRequired[str],
+        "Permissions": NotRequired[Sequence[str]],
+        "Tags": NotRequired[Mapping[str, str]],
+        "AllowedAccessControlTags": NotRequired[Mapping[str, str]],
+        "TagRestrictedResources": NotRequired[Sequence[str]],
+        "Applications": NotRequired[Sequence[ApplicationUnionTypeDef]],
+        "HierarchyRestrictedResources": NotRequired[Sequence[str]],
+        "AllowedAccessControlHierarchyGroupId": NotRequired[str],
+    },
+)
+UpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "SecurityProfileId": str,
+        "InstanceId": str,
+        "Description": NotRequired[str],
+        "Permissions": NotRequired[Sequence[str]],
+        "AllowedAccessControlTags": NotRequired[Mapping[str, str]],
+        "TagRestrictedResources": NotRequired[Sequence[str]],
+        "Applications": NotRequired[Sequence[ApplicationUnionTypeDef]],
+        "HierarchyRestrictedResources": NotRequired[Sequence[str]],
+        "AllowedAccessControlHierarchyGroupId": NotRequired[str],
+    },
+)
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "LexBots": List[LexBotConfigTypeDef],
-        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+BatchGetAttachedFileMetadataResponseTypeDef = TypedDict(
+    "BatchGetAttachedFileMetadataResponseTypeDef",
+    {
+        "Files": List[AttachedFileTypeDef],
+        "Errors": List[AttachedFileErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ControlPlaneUserAttributeFilterTypeDef = TypedDict(
     "ControlPlaneUserAttributeFilterTypeDef",
     {
         "OrConditions": NotRequired[Sequence[AttributeAndConditionTypeDef]],
@@ -5802,17 +6076,17 @@
         "MaxResults": NotRequired[int],
     },
 )
 SearchContactsResponseTypeDef = TypedDict(
     "SearchContactsResponseTypeDef",
     {
         "Contacts": List[ContactSearchSummaryTypeDef],
-        "NextToken": str,
         "TotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeContactResponseTypeDef = TypedDict(
     "DescribeContactResponseTypeDef",
     {
         "Contact": ContactTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5821,44 +6095,28 @@
 DescribeEvaluationFormResponseTypeDef = TypedDict(
     "DescribeEvaluationFormResponseTypeDef",
     {
         "EvaluationForm": EvaluationFormTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribePredefinedAttributeResponseTypeDef = TypedDict(
-    "DescribePredefinedAttributeResponseTypeDef",
-    {
-        "PredefinedAttribute": PredefinedAttributeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-SearchPredefinedAttributesResponseTypeDef = TypedDict(
-    "SearchPredefinedAttributesResponseTypeDef",
-    {
-        "PredefinedAttributes": List[PredefinedAttributeTypeDef],
-        "NextToken": str,
-        "ApproximateTotalCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeQueueResponseTypeDef = TypedDict(
     "DescribeQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchQueuesResponseTypeDef = TypedDict(
     "SearchQueuesResponseTypeDef",
     {
         "Queues": List[QueueTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5952,23 +6210,39 @@
     {
         "InstanceId": str,
         "EvaluationId": str,
         "Answers": NotRequired[Mapping[str, EvaluationAnswerInputTypeDef]],
         "Notes": NotRequired[Mapping[str, EvaluationNoteTypeDef]],
     },
 )
+EvaluationFormNumericQuestionPropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
+    {
+        "MinValue": int,
+        "MaxValue": int,
+        "Options": NotRequired[List[EvaluationFormNumericQuestionOptionTypeDef]],
+        "Automation": NotRequired[EvaluationFormNumericQuestionAutomationTypeDef],
+    },
+)
 EvaluationFormNumericQuestionPropertiesTypeDef = TypedDict(
     "EvaluationFormNumericQuestionPropertiesTypeDef",
     {
         "MinValue": int,
         "MaxValue": int,
         "Options": NotRequired[Sequence[EvaluationFormNumericQuestionOptionTypeDef]],
         "Automation": NotRequired[EvaluationFormNumericQuestionAutomationTypeDef],
     },
 )
+EvaluationFormSingleSelectQuestionAutomationOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
+    {
+        "Options": List[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],
+        "DefaultOptionRefId": NotRequired[str],
+    },
+)
 EvaluationFormSingleSelectQuestionAutomationTypeDef = TypedDict(
     "EvaluationFormSingleSelectQuestionAutomationTypeDef",
     {
         "Options": Sequence[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],
         "DefaultOptionRefId": NotRequired[str],
     },
 )
@@ -5987,16 +6261,29 @@
         "Tags": NotRequired[Dict[str, str]],
     },
 )
 ListContactEvaluationsResponseTypeDef = TypedDict(
     "ListContactEvaluationsResponseTypeDef",
     {
         "EvaluationSummaryList": List[EvaluationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+CreateCaseActionDefinitionOutputTypeDef = TypedDict(
+    "CreateCaseActionDefinitionOutputTypeDef",
+    {
+        "Fields": List[FieldValueOutputTypeDef],
+        "TemplateId": str,
+    },
+)
+UpdateCaseActionDefinitionOutputTypeDef = TypedDict(
+    "UpdateCaseActionDefinitionOutputTypeDef",
+    {
+        "Fields": List[FieldValueOutputTypeDef],
     },
 )
 CreateCaseActionDefinitionTypeDef = TypedDict(
     "CreateCaseActionDefinitionTypeDef",
     {
         "Fields": Sequence[FieldValueTypeDef],
         "TemplateId": str,
@@ -6128,49 +6415,51 @@
 DescribeInstanceResponseTypeDef = TypedDict(
     "DescribeInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+TaskTemplateConstraintsOutputTypeDef = TypedDict(
+    "TaskTemplateConstraintsOutputTypeDef",
+    {
+        "RequiredFields": NotRequired[List[RequiredFieldInfoTypeDef]],
+        "ReadOnlyFields": NotRequired[List[ReadOnlyFieldInfoTypeDef]],
+        "InvisibleFields": NotRequired[List[InvisibleFieldInfoTypeDef]],
+    },
+)
 TaskTemplateConstraintsTypeDef = TypedDict(
     "TaskTemplateConstraintsTypeDef",
     {
         "RequiredFields": NotRequired[Sequence[RequiredFieldInfoTypeDef]],
         "ReadOnlyFields": NotRequired[Sequence[ReadOnlyFieldInfoTypeDef]],
         "InvisibleFields": NotRequired[Sequence[InvisibleFieldInfoTypeDef]],
     },
 )
-TaskTemplateDefaultsTypeDef = TypedDict(
-    "TaskTemplateDefaultsTypeDef",
+TaskTemplateDefaultsOutputTypeDef = TypedDict(
+    "TaskTemplateDefaultsOutputTypeDef",
     {
-        "DefaultFieldValues": NotRequired[Sequence[TaskTemplateDefaultFieldValueTypeDef]],
+        "DefaultFieldValues": NotRequired[List[TaskTemplateDefaultFieldValueTypeDef]],
     },
 )
-GetMetricDataV2RequestRequestTypeDef = TypedDict(
-    "GetMetricDataV2RequestRequestTypeDef",
+TaskTemplateDefaultsTypeDef = TypedDict(
+    "TaskTemplateDefaultsTypeDef",
     {
-        "ResourceArn": str,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-        "Filters": Sequence[FilterV2TypeDef],
-        "Metrics": Sequence[MetricV2TypeDef],
-        "Interval": NotRequired[IntervalDetailsTypeDef],
-        "Groupings": NotRequired[Sequence[str]],
-        "NextToken": NotRequired[str],
-        "MaxResults": NotRequired[int],
+        "DefaultFieldValues": NotRequired[Sequence[TaskTemplateDefaultFieldValueTypeDef]],
     },
 )
+TaskTemplateFieldUnionTypeDef = Union[TaskTemplateFieldTypeDef, TaskTemplateFieldOutputTypeDef]
 MetricDataV2TypeDef = TypedDict(
     "MetricDataV2TypeDef",
     {
-        "Metric": NotRequired[MetricV2TypeDef],
+        "Metric": NotRequired[MetricV2OutputTypeDef],
         "Value": NotRequired[float],
     },
 )
+MetricV2UnionTypeDef = Union[MetricV2TypeDef, MetricV2OutputTypeDef]
 SendChatIntegrationEventRequestRequestTypeDef = TypedDict(
     "SendChatIntegrationEventRequestRequestTypeDef",
     {
         "SourceId": str,
         "DestinationId": str,
         "Event": ChatEventTypeDef,
         "Subtype": NotRequired[str],
@@ -6179,21 +6468,28 @@
 )
 ChatParticipantRoleConfigTypeDef = TypedDict(
     "ChatParticipantRoleConfigTypeDef",
     {
         "ParticipantTimerConfigList": Sequence[ParticipantTimerConfigurationTypeDef],
     },
 )
-SearchPredefinedAttributesResponsePaginatorTypeDef = TypedDict(
-    "SearchPredefinedAttributesResponsePaginatorTypeDef",
+DescribePredefinedAttributeResponseTypeDef = TypedDict(
+    "DescribePredefinedAttributeResponseTypeDef",
+    {
+        "PredefinedAttribute": PredefinedAttributeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+SearchPredefinedAttributesResponseTypeDef = TypedDict(
+    "SearchPredefinedAttributesResponseTypeDef",
     {
-        "PredefinedAttributes": List[PredefinedAttributePaginatorTypeDef],
-        "NextToken": str,
+        "PredefinedAttributes": List[PredefinedAttributeTypeDef],
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateQuickConnectRequestRequestTypeDef = TypedDict(
     "CreateQuickConnectRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
@@ -6251,16 +6547,16 @@
         "TranscriptItems": List[RealTimeContactAnalysisTranscriptItemWithContentTypeDef],
     },
 )
 ListContactReferencesResponseTypeDef = TypedDict(
     "ListContactReferencesResponseTypeDef",
     {
         "ReferenceSummaryList": List[ReferenceSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchResourceTagsRequestRequestTypeDef = TypedDict(
     "SearchResourceTagsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceTypes": NotRequired[Sequence[str]],
@@ -6277,22 +6573,23 @@
         "SearchCriteria": NotRequired[ResourceTagsSearchCriteriaTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 GetTrafficDistributionResponseTypeDef = TypedDict(
     "GetTrafficDistributionResponseTypeDef",
     {
-        "TelephonyConfig": TelephonyConfigTypeDef,
+        "TelephonyConfig": TelephonyConfigOutputTypeDef,
         "Id": str,
         "Arn": str,
-        "SignInConfig": SignInConfigTypeDef,
-        "AgentConfig": AgentConfigTypeDef,
+        "SignInConfig": SignInConfigOutputTypeDef,
+        "AgentConfig": AgentConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SignInConfigUnionTypeDef = Union[SignInConfigTypeDef, SignInConfigOutputTypeDef]
 UpdateTrafficDistributionRequestRequestTypeDef = TypedDict(
     "UpdateTrafficDistributionRequestRequestTypeDef",
     {
         "Id": str,
         "TelephonyConfig": NotRequired[TelephonyConfigTypeDef],
         "SignInConfig": NotRequired[SignInConfigTypeDef],
         "AgentConfig": NotRequired[AgentConfigTypeDef],
@@ -6304,17 +6601,17 @@
         "Transcript": NotRequired[TranscriptTypeDef],
     },
 )
 SearchUsersResponseTypeDef = TypedDict(
     "SearchUsersResponseTypeDef",
     {
         "Users": List[UserSearchSummaryTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateViewResponseTypeDef = TypedDict(
     "CreateViewResponseTypeDef",
     {
         "View": ViewTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6476,27 +6773,27 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchRoutingProfilesResponseTypeDef = TypedDict(
     "SearchRoutingProfilesResponseTypeDef",
     {
         "RoutingProfiles": List[RoutingProfileTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetCurrentMetricDataResponseTypeDef = TypedDict(
     "GetCurrentMetricDataResponseTypeDef",
     {
-        "NextToken": str,
         "MetricResults": List[CurrentMetricResultTypeDef],
         "DataSnapshotTime": datetime,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
@@ -6510,27 +6807,35 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInstanceStorageConfigsResponseTypeDef = TypedDict(
     "ListInstanceStorageConfigsResponseTypeDef",
     {
         "StorageConfigs": List[InstanceStorageConfigTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "UpdateInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AssociationId": str,
         "ResourceType": InstanceStorageResourceTypeType,
         "StorageConfig": InstanceStorageConfigTypeDef,
     },
 )
+EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
+    {
+        "Options": List[EvaluationFormSingleSelectQuestionOptionTypeDef],
+        "DisplayAs": NotRequired[EvaluationFormSingleSelectQuestionDisplayModeType],
+        "Automation": NotRequired[EvaluationFormSingleSelectQuestionAutomationOutputTypeDef],
+    },
+)
 EvaluationFormSingleSelectQuestionPropertiesTypeDef = TypedDict(
     "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
     {
         "Options": Sequence[EvaluationFormSingleSelectQuestionOptionTypeDef],
         "DisplayAs": NotRequired[EvaluationFormSingleSelectQuestionDisplayModeType],
         "Automation": NotRequired[EvaluationFormSingleSelectQuestionAutomationTypeDef],
     },
@@ -6539,14 +6844,28 @@
     "DescribeContactEvaluationResponseTypeDef",
     {
         "Evaluation": EvaluationTypeDef,
         "EvaluationForm": EvaluationFormContentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "ActionType": ActionTypeType,
+        "TaskAction": NotRequired[TaskActionDefinitionOutputTypeDef],
+        "EventBridgeAction": NotRequired[EventBridgeActionDefinitionTypeDef],
+        "AssignContactCategoryAction": NotRequired[Dict[str, Any]],
+        "SendNotificationAction": NotRequired[SendNotificationActionDefinitionOutputTypeDef],
+        "CreateCaseAction": NotRequired[CreateCaseActionDefinitionOutputTypeDef],
+        "UpdateCaseAction": NotRequired[UpdateCaseActionDefinitionOutputTypeDef],
+        "EndAssociatedTasksAction": NotRequired[Dict[str, Any]],
+        "SubmitAutoEvaluationAction": NotRequired[SubmitAutoEvaluationActionDefinitionTypeDef],
+    },
+)
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "ActionType": ActionTypeType,
         "TaskAction": NotRequired[TaskActionDefinitionTypeDef],
         "EventBridgeAction": NotRequired[EventBridgeActionDefinitionTypeDef],
         "AssignContactCategoryAction": NotRequired[Mapping[str, Any]],
@@ -6556,18 +6875,18 @@
         "EndAssociatedTasksAction": NotRequired[Mapping[str, Any]],
         "SubmitAutoEvaluationAction": NotRequired[SubmitAutoEvaluationActionDefinitionTypeDef],
     },
 )
 GetCurrentUserDataResponseTypeDef = TypedDict(
     "GetCurrentUserDataResponseTypeDef",
     {
-        "NextToken": str,
         "UserDataList": List[UserDataTypeDef],
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeUserHierarchyGroupResponseTypeDef = TypedDict(
     "DescribeUserHierarchyGroupResponseTypeDef",
     {
         "HierarchyGroup": HierarchyGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6587,92 +6906,112 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchHoursOfOperationsResponseTypeDef = TypedDict(
     "SearchHoursOfOperationsResponseTypeDef",
     {
         "HoursOfOperations": List[HoursOfOperationTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-CreateTaskTemplateRequestRequestTypeDef = TypedDict(
-    "CreateTaskTemplateRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-        "Fields": Sequence[TaskTemplateFieldTypeDef],
-        "Description": NotRequired[str],
-        "ContactFlowId": NotRequired[str],
-        "Constraints": NotRequired[TaskTemplateConstraintsTypeDef],
-        "Defaults": NotRequired[TaskTemplateDefaultsTypeDef],
-        "Status": NotRequired[TaskTemplateStatusType],
-        "ClientToken": NotRequired[str],
-    },
-)
+TaskTemplateConstraintsUnionTypeDef = Union[
+    TaskTemplateConstraintsTypeDef, TaskTemplateConstraintsOutputTypeDef
+]
 GetTaskTemplateResponseTypeDef = TypedDict(
     "GetTaskTemplateResponseTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
-        "Constraints": TaskTemplateConstraintsTypeDef,
-        "Defaults": TaskTemplateDefaultsTypeDef,
-        "Fields": List[TaskTemplateFieldTypeDef],
+        "Constraints": TaskTemplateConstraintsOutputTypeDef,
+        "Defaults": TaskTemplateDefaultsOutputTypeDef,
+        "Fields": List[TaskTemplateFieldOutputTypeDef],
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateTaskTemplateRequestRequestTypeDef = TypedDict(
-    "UpdateTaskTemplateRequestRequestTypeDef",
-    {
-        "TaskTemplateId": str,
-        "InstanceId": str,
-        "Name": NotRequired[str],
-        "Description": NotRequired[str],
-        "ContactFlowId": NotRequired[str],
-        "Constraints": NotRequired[TaskTemplateConstraintsTypeDef],
-        "Defaults": NotRequired[TaskTemplateDefaultsTypeDef],
-        "Status": NotRequired[TaskTemplateStatusType],
-        "Fields": NotRequired[Sequence[TaskTemplateFieldTypeDef]],
-    },
-)
 UpdateTaskTemplateResponseTypeDef = TypedDict(
     "UpdateTaskTemplateResponseTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
-        "Constraints": TaskTemplateConstraintsTypeDef,
-        "Defaults": TaskTemplateDefaultsTypeDef,
-        "Fields": List[TaskTemplateFieldTypeDef],
+        "Constraints": TaskTemplateConstraintsOutputTypeDef,
+        "Defaults": TaskTemplateDefaultsOutputTypeDef,
+        "Fields": List[TaskTemplateFieldOutputTypeDef],
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+TaskTemplateDefaultsUnionTypeDef = Union[
+    TaskTemplateDefaultsTypeDef, TaskTemplateDefaultsOutputTypeDef
+]
+CreateTaskTemplateRequestRequestTypeDef = TypedDict(
+    "CreateTaskTemplateRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "Fields": Sequence[TaskTemplateFieldUnionTypeDef],
+        "Description": NotRequired[str],
+        "ContactFlowId": NotRequired[str],
+        "Constraints": NotRequired[TaskTemplateConstraintsTypeDef],
+        "Defaults": NotRequired[TaskTemplateDefaultsTypeDef],
+        "Status": NotRequired[TaskTemplateStatusType],
+        "ClientToken": NotRequired[str],
+    },
+)
+UpdateTaskTemplateRequestRequestTypeDef = TypedDict(
+    "UpdateTaskTemplateRequestRequestTypeDef",
+    {
+        "TaskTemplateId": str,
+        "InstanceId": str,
+        "Name": NotRequired[str],
+        "Description": NotRequired[str],
+        "ContactFlowId": NotRequired[str],
+        "Constraints": NotRequired[TaskTemplateConstraintsTypeDef],
+        "Defaults": NotRequired[TaskTemplateDefaultsTypeDef],
+        "Status": NotRequired[TaskTemplateStatusType],
+        "Fields": NotRequired[Sequence[TaskTemplateFieldUnionTypeDef]],
+    },
+)
 MetricResultV2TypeDef = TypedDict(
     "MetricResultV2TypeDef",
     {
         "Dimensions": NotRequired[Dict[str, str]],
         "MetricInterval": NotRequired[MetricIntervalTypeDef],
         "Collections": NotRequired[List[MetricDataV2TypeDef]],
     },
 )
+GetMetricDataV2RequestRequestTypeDef = TypedDict(
+    "GetMetricDataV2RequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Filters": Sequence[FilterV2TypeDef],
+        "Metrics": Sequence[MetricV2UnionTypeDef],
+        "Interval": NotRequired[IntervalDetailsTypeDef],
+        "Groupings": NotRequired[Sequence[str]],
+        "NextToken": NotRequired[str],
+        "MaxResults": NotRequired[int],
+    },
+)
 UpdateParticipantRoleConfigChannelInfoTypeDef = TypedDict(
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     {
         "Chat": NotRequired[ChatParticipantRoleConfigTypeDef],
     },
 )
 DescribeQuickConnectResponseTypeDef = TypedDict(
@@ -6682,17 +7021,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchQuickConnectsResponseTypeDef = TypedDict(
     "SearchQuickConnectsResponseTypeDef",
     {
         "QuickConnects": List[QuickConnectTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RealTimeContactAnalysisCategoryDetailsTypeDef = TypedDict(
     "RealTimeContactAnalysisCategoryDetailsTypeDef",
     {
         "PointsOfInterest": List[RealTimeContactAnalysisPointOfInterestTypeDef],
     },
@@ -6740,74 +7079,59 @@
         "ConnectionData": ConnectionDataTypeDef,
         "ContactId": str,
         "ParticipantId": str,
         "ParticipantToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+EvaluationFormQuestionTypePropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
+    {
+        "Numeric": NotRequired[EvaluationFormNumericQuestionPropertiesOutputTypeDef],
+        "SingleSelect": NotRequired[EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef],
+    },
+)
 EvaluationFormQuestionTypePropertiesTypeDef = TypedDict(
     "EvaluationFormQuestionTypePropertiesTypeDef",
     {
         "Numeric": NotRequired[EvaluationFormNumericQuestionPropertiesTypeDef],
         "SingleSelect": NotRequired[EvaluationFormSingleSelectQuestionPropertiesTypeDef],
     },
 )
-CreateRuleRequestRequestTypeDef = TypedDict(
-    "CreateRuleRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-        "TriggerEventSource": RuleTriggerEventSourceTypeDef,
-        "Function": str,
-        "Actions": Sequence[RuleActionTypeDef],
-        "PublishStatus": RulePublishStatusType,
-        "ClientToken": NotRequired[str],
-    },
-)
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "Name": str,
         "RuleId": str,
         "RuleArn": str,
         "TriggerEventSource": RuleTriggerEventSourceTypeDef,
         "Function": str,
-        "Actions": List[RuleActionTypeDef],
+        "Actions": List[RuleActionOutputTypeDef],
         "PublishStatus": RulePublishStatusType,
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "LastUpdatedBy": str,
         "Tags": NotRequired[Dict[str, str]],
     },
 )
-UpdateRuleRequestRequestTypeDef = TypedDict(
-    "UpdateRuleRequestRequestTypeDef",
-    {
-        "RuleId": str,
-        "InstanceId": str,
-        "Name": str,
-        "Function": str,
-        "Actions": Sequence[RuleActionTypeDef],
-        "PublishStatus": RulePublishStatusType,
-    },
-)
+RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
 GetMetricDataResponseTypeDef = TypedDict(
     "GetMetricDataResponseTypeDef",
     {
-        "NextToken": str,
         "MetricResults": List[HistoricalMetricResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetMetricDataV2ResponseTypeDef = TypedDict(
     "GetMetricDataV2ResponseTypeDef",
     {
-        "NextToken": str,
         "MetricResults": List[MetricResultV2TypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateParticipantRoleConfigRequestRequestTypeDef = TypedDict(
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
@@ -6837,14 +7161,26 @@
         "InstanceId": str,
         "TimeRange": SearchContactsTimeRangeTypeDef,
         "SearchCriteria": NotRequired[SearchCriteriaTypeDef],
         "Sort": NotRequired[SortTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+EvaluationFormQuestionOutputTypeDef = TypedDict(
+    "EvaluationFormQuestionOutputTypeDef",
+    {
+        "Title": str,
+        "RefId": str,
+        "QuestionType": EvaluationFormQuestionTypeType,
+        "Instructions": NotRequired[str],
+        "NotApplicableEnabled": NotRequired[bool],
+        "QuestionTypeProperties": NotRequired[EvaluationFormQuestionTypePropertiesOutputTypeDef],
+        "Weight": NotRequired[float],
+    },
+)
 EvaluationFormQuestionTypeDef = TypedDict(
     "EvaluationFormQuestionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "QuestionType": EvaluationFormQuestionTypeType,
         "Instructions": NotRequired[str],
@@ -6856,34 +7192,64 @@
 DescribeRuleResponseTypeDef = TypedDict(
     "DescribeRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateRuleRequestRequestTypeDef = TypedDict(
+    "CreateRuleRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "TriggerEventSource": RuleTriggerEventSourceTypeDef,
+        "Function": str,
+        "Actions": Sequence[RuleActionUnionTypeDef],
+        "PublishStatus": RulePublishStatusType,
+        "ClientToken": NotRequired[str],
+    },
+)
+UpdateRuleRequestRequestTypeDef = TypedDict(
+    "UpdateRuleRequestRequestTypeDef",
+    {
+        "RuleId": str,
+        "InstanceId": str,
+        "Name": str,
+        "Function": str,
+        "Actions": Sequence[RuleActionUnionTypeDef],
+        "PublishStatus": RulePublishStatusType,
+    },
+)
 RealtimeContactAnalysisSegmentTypeDef = TypedDict(
     "RealtimeContactAnalysisSegmentTypeDef",
     {
         "Transcript": NotRequired[RealTimeContactAnalysisSegmentTranscriptTypeDef],
         "Categories": NotRequired[RealTimeContactAnalysisSegmentCategoriesTypeDef],
         "Issues": NotRequired[RealTimeContactAnalysisSegmentIssuesTypeDef],
         "Event": NotRequired[RealTimeContactAnalysisSegmentEventTypeDef],
         "Attachments": NotRequired[RealTimeContactAnalysisSegmentAttachmentsTypeDef],
     },
 )
+EvaluationFormItemOutputTypeDef = TypedDict(
+    "EvaluationFormItemOutputTypeDef",
+    {
+        "Section": NotRequired[Dict[str, Any]],
+        "Question": NotRequired[EvaluationFormQuestionOutputTypeDef],
+    },
+)
 EvaluationFormItemTypeDef = TypedDict(
     "EvaluationFormItemTypeDef",
     {
         "Section": NotRequired[Dict[str, Any]],
         "Question": NotRequired[EvaluationFormQuestionTypeDef],
     },
 )
 ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef = TypedDict(
     "ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef",
     {
         "Channel": RealTimeContactAnalysisSupportedChannelType,
         "Status": RealTimeContactAnalysisStatusType,
         "Segments": List[RealtimeContactAnalysisSegmentTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect/type_defs.pyi` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     EvaluationFormScoringModeType,
     EvaluationFormScoringStatusType,
     EvaluationFormSingleSelectQuestionDisplayModeType,
     EvaluationFormVersionStatusType,
     EvaluationStatusType,
     EventSourceNameType,
     FailureReasonCodeType,
+    FileStatusTypeType,
     GroupingType,
     HierarchyGroupMatchTypeType,
     HistoricalMetricNameType,
     HoursOfOperationDaysType,
     InstanceAttributeTypeType,
     InstanceStatusType,
     InstanceStorageResourceTypeType,
@@ -119,61 +120,67 @@
     "AgentInfoTypeDef",
     "AgentStatusReferenceTypeDef",
     "AgentStatusSummaryTypeDef",
     "AgentStatusTypeDef",
     "ParticipantCapabilitiesTypeDef",
     "AnalyticsDataAssociationResultTypeDef",
     "AnswerMachineDetectionConfigTypeDef",
-    "ApplicationPaginatorTypeDef",
+    "ApplicationExtraOutputTypeDef",
+    "ApplicationOutputTypeDef",
     "ApplicationTypeDef",
     "AssociateAnalyticsDataSetRequestRequestTypeDef",
     "AssociateApprovedOriginRequestRequestTypeDef",
     "LexBotTypeDef",
     "LexV2BotTypeDef",
     "AssociateDefaultVocabularyRequestRequestTypeDef",
     "AssociateFlowRequestRequestTypeDef",
     "AssociateLambdaFunctionRequestRequestTypeDef",
     "AssociatePhoneNumberContactFlowRequestRequestTypeDef",
     "AssociateQueueQuickConnectsRequestRequestTypeDef",
     "AssociateSecurityKeyRequestRequestTypeDef",
     "AssociateTrafficDistributionGroupUserRequestRequestTypeDef",
     "UserProficiencyTypeDef",
+    "AttachedFileErrorTypeDef",
+    "CreatedByInfoTypeDef",
     "AttachmentReferenceTypeDef",
     "AttendeeTypeDef",
     "HierarchyGroupConditionTypeDef",
     "TagConditionTypeDef",
     "AttributeTypeDef",
     "AudioFeaturesTypeDef",
     "AvailableNumberSummaryTypeDef",
     "BatchAssociateAnalyticsDataSetRequestRequestTypeDef",
     "ErrorResultTypeDef",
     "BatchDisassociateAnalyticsDataSetRequestRequestTypeDef",
+    "BatchGetAttachedFileMetadataRequestRequestTypeDef",
     "BatchGetFlowAssociationRequestRequestTypeDef",
     "FlowAssociationSummaryTypeDef",
     "FailedRequestTypeDef",
     "SuccessfulRequestTypeDef",
     "CampaignTypeDef",
     "ChatEventTypeDef",
     "ChatMessageTypeDef",
     "ChatStreamingConfigurationTypeDef",
     "ClaimPhoneNumberRequestRequestTypeDef",
     "PhoneNumberStatusTypeDef",
+    "CompleteAttachedFileUploadRequestRequestTypeDef",
     "EndpointTypeDef",
     "ContactFilterTypeDef",
     "ContactFlowModuleSummaryTypeDef",
     "ContactFlowModuleTypeDef",
     "ContactFlowSummaryTypeDef",
     "ContactFlowTypeDef",
     "ContactSearchSummaryAgentInfoTypeDef",
     "ContactSearchSummaryQueueInfoTypeDef",
     "QueueInfoTypeDef",
     "WisdomInfoTypeDef",
     "CreateAgentStatusRequestRequestTypeDef",
     "CreateContactFlowModuleRequestRequestTypeDef",
     "CreateContactFlowRequestRequestTypeDef",
+    "EvaluationFormItemUnionTypeDef",
     "EvaluationFormScoringStrategyTypeDef",
     "CreateInstanceRequestRequestTypeDef",
     "CreateIntegrationAssociationRequestRequestTypeDef",
     "ParticipantDetailsToAddTypeDef",
     "ParticipantTokenCredentialsTypeDef",
     "CreatePersistentContactAssociationRequestRequestTypeDef",
     "PredefinedAttributeValuesTypeDef",
@@ -191,14 +198,15 @@
     "CredentialsTypeDef",
     "CrossChannelBehaviorTypeDef",
     "CurrentMetricTypeDef",
     "CurrentMetricSortCriteriaTypeDef",
     "DateReferenceTypeDef",
     "DeactivateEvaluationFormRequestRequestTypeDef",
     "DefaultVocabularyTypeDef",
+    "DeleteAttachedFileRequestRequestTypeDef",
     "DeleteContactEvaluationRequestRequestTypeDef",
     "DeleteContactFlowModuleRequestRequestTypeDef",
     "DeleteContactFlowRequestRequestTypeDef",
     "DeleteEvaluationFormRequestRequestTypeDef",
     "DeleteHoursOfOperationRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteIntegrationAssociationRequestRequestTypeDef",
@@ -256,30 +264,34 @@
     "DisassociateQueueQuickConnectsRequestRequestTypeDef",
     "RoutingProfileQueueReferenceTypeDef",
     "DisassociateSecurityKeyRequestRequestTypeDef",
     "DisassociateTrafficDistributionGroupUserRequestRequestTypeDef",
     "UserProficiencyDisassociateTypeDef",
     "DisconnectReasonTypeDef",
     "DismissUserContactRequestRequestTypeDef",
+    "DownloadUrlMetadataTypeDef",
     "EmailReferenceTypeDef",
     "EncryptionConfigTypeDef",
     "EvaluationAnswerDataTypeDef",
     "NumericQuestionPropertyValueAutomationTypeDef",
     "EvaluationFormNumericQuestionOptionTypeDef",
+    "EvaluationFormSectionOutputTypeDef",
     "EvaluationFormSectionTypeDef",
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     "EvaluationFormSingleSelectQuestionOptionTypeDef",
     "EvaluationFormSummaryTypeDef",
     "EvaluationFormVersionSummaryTypeDef",
     "EvaluationScoreTypeDef",
     "EvaluationNoteTypeDef",
     "EventBridgeActionDefinitionTypeDef",
+    "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
     "FilterV2TypeDef",
     "FiltersTypeDef",
+    "GetAttachedFileRequestRequestTypeDef",
     "GetContactAttributesRequestRequestTypeDef",
     "GetFederationTokenRequestRequestTypeDef",
     "GetFlowAssociationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "IntervalDetailsTypeDef",
     "GetPromptFileRequestRequestTypeDef",
@@ -358,26 +370,29 @@
     "ListUsersRequestRequestTypeDef",
     "UserSummaryTypeDef",
     "ListViewVersionsRequestRequestTypeDef",
     "ViewVersionSummaryTypeDef",
     "ListViewsRequestRequestTypeDef",
     "ViewSummaryTypeDef",
     "MediaPlacementTypeDef",
+    "MetricFilterV2OutputTypeDef",
     "MetricFilterV2TypeDef",
     "MetricIntervalTypeDef",
     "ThresholdV2TypeDef",
     "MonitorContactRequestRequestTypeDef",
     "ParticipantDetailsTypeDef",
+    "NotificationRecipientTypeOutputTypeDef",
     "NotificationRecipientTypeTypeDef",
     "NumberReferenceTypeDef",
     "ParticipantTimerValueTypeDef",
     "PauseContactRequestRequestTypeDef",
     "PersistentChatTypeDef",
     "PhoneNumberQuickConnectConfigTypeDef",
-    "PredefinedAttributeValuesPaginatorTypeDef",
+    "PredefinedAttributeValuesOutputTypeDef",
+    "PredefinedAttributeValuesExtraOutputTypeDef",
     "PutUserStatusRequestRequestTypeDef",
     "QueueQuickConnectConfigTypeDef",
     "UserQuickConnectConfigTypeDef",
     "RealTimeContactAnalysisAttachmentTypeDef",
     "RealTimeContactAnalysisCharacterIntervalTypeDef",
     "RealTimeContactAnalysisTimeDataTypeDef",
     "StringReferenceTypeDef",
@@ -395,14 +410,15 @@
     "TagSetTypeDef",
     "SecurityProfileSearchSummaryTypeDef",
     "SearchVocabulariesRequestRequestTypeDef",
     "VocabularySummaryTypeDef",
     "SearchableContactAttributesCriteriaTypeDef",
     "SegmentAttributeValueTypeDef",
     "SignInDistributionTypeDef",
+    "UploadUrlMetadataTypeDef",
     "StartContactEvaluationRequestRequestTypeDef",
     "VoiceRecordingConfigurationTypeDef",
     "StopContactRecordingRequestRequestTypeDef",
     "StopContactStreamingRequestRequestTypeDef",
     "SuspendContactRecordingRequestRequestTypeDef",
     "TagContactRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -485,33 +501,35 @@
     "StartTaskContactResponseTypeDef",
     "SubmitContactEvaluationResponseTypeDef",
     "TransferContactResponseTypeDef",
     "UpdateContactEvaluationResponseTypeDef",
     "UpdateEvaluationFormResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
     "UpdatePromptResponseTypeDef",
+    "AgentConfigOutputTypeDef",
     "AgentConfigTypeDef",
+    "TelephonyConfigOutputTypeDef",
     "TelephonyConfigTypeDef",
     "AgentContactReferenceTypeDef",
     "ListAgentStatusResponseTypeDef",
     "DescribeAgentStatusResponseTypeDef",
     "AllowedCapabilitiesTypeDef",
     "ListAnalyticsDataAssociationsResponseTypeDef",
-    "ListSecurityProfileApplicationsResponsePaginatorTypeDef",
-    "CreateSecurityProfileRequestRequestTypeDef",
     "ListSecurityProfileApplicationsResponseTypeDef",
-    "UpdateSecurityProfileRequestRequestTypeDef",
+    "ApplicationUnionTypeDef",
     "AssociateLexBotRequestRequestTypeDef",
     "ListLexBotsResponseTypeDef",
     "AssociateBotRequestRequestTypeDef",
     "DisassociateBotRequestRequestTypeDef",
     "LexBotConfigTypeDef",
     "AssociateUserProficienciesRequestRequestTypeDef",
     "ListUserProficienciesResponseTypeDef",
     "UpdateUserProficienciesRequestRequestTypeDef",
+    "AttachedFileTypeDef",
+    "StartAttachedFileUploadRequestRequestTypeDef",
     "AttributeAndConditionTypeDef",
     "ControlPlaneTagFilterTypeDef",
     "DescribeInstanceAttributeResponseTypeDef",
     "ListInstanceAttributesResponseTypeDef",
     "MeetingFeaturesConfigurationTypeDef",
     "SearchAvailablePhoneNumbersResponseTypeDef",
     "BatchAssociateAnalyticsDataSetResponseTypeDef",
@@ -532,15 +550,14 @@
     "CreateEvaluationFormRequestRequestTypeDef",
     "EvaluationFormContentTypeDef",
     "EvaluationFormTypeDef",
     "UpdateEvaluationFormRequestRequestTypeDef",
     "CreateParticipantRequestRequestTypeDef",
     "CreateParticipantResponseTypeDef",
     "CreatePredefinedAttributeRequestRequestTypeDef",
-    "PredefinedAttributeTypeDef",
     "UpdatePredefinedAttributeRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "QueueTypeDef",
     "UpdateQueueOutboundCallerConfigRequestRequestTypeDef",
     "UpdateUserIdentityInfoRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserPhoneConfigRequestRequestTypeDef",
@@ -557,24 +574,26 @@
     "DescribeTrafficDistributionGroupResponseTypeDef",
     "DescribeVocabularyResponseTypeDef",
     "DimensionsTypeDef",
     "DisassociateRoutingProfileQueuesRequestRequestTypeDef",
     "RoutingProfileQueueConfigTypeDef",
     "DisassociateUserProficienciesRequestRequestTypeDef",
     "StopContactRequestRequestTypeDef",
+    "GetAttachedFileResponseTypeDef",
     "KinesisVideoStreamConfigTypeDef",
     "S3ConfigTypeDef",
     "EvaluationAnswerInputTypeDef",
     "EvaluationAnswerOutputTypeDef",
     "EvaluationFormNumericQuestionAutomationTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationOptionTypeDef",
     "ListEvaluationFormsResponseTypeDef",
     "ListEvaluationFormVersionsResponseTypeDef",
     "EvaluationMetadataTypeDef",
     "EvaluationSummaryTypeDef",
+    "FieldValueOutputTypeDef",
     "FieldValueTypeDef",
     "GetCurrentMetricDataRequestRequestTypeDef",
     "ListAgentStatusRequestListAgentStatusesPaginateTypeDef",
     "ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     "ListBotsRequestListBotsPaginateTypeDef",
     "ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     "ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
@@ -637,14 +656,15 @@
     "InstanceTypeDef",
     "ListInstancesResponseTypeDef",
     "ListIntegrationAssociationsResponseTypeDef",
     "InvisibleFieldInfoTypeDef",
     "ReadOnlyFieldInfoTypeDef",
     "RequiredFieldInfoTypeDef",
     "TaskTemplateDefaultFieldValueTypeDef",
+    "TaskTemplateFieldOutputTypeDef",
     "TaskTemplateFieldTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "ListPhoneNumbersV2ResponseTypeDef",
     "ListPredefinedAttributesResponseTypeDef",
     "ListPromptsResponseTypeDef",
     "ListQueueQuickConnectsResponseTypeDef",
     "ListQuickConnectsResponseTypeDef",
@@ -656,107 +676,125 @@
     "ListTaskTemplatesResponseTypeDef",
     "ListTrafficDistributionGroupUsersResponseTypeDef",
     "ListTrafficDistributionGroupsResponseTypeDef",
     "ListUseCasesResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ListViewVersionsResponseTypeDef",
     "ListViewsResponseTypeDef",
+    "MetricV2OutputTypeDef",
     "MetricV2TypeDef",
     "NewSessionDetailsTypeDef",
+    "SendNotificationActionDefinitionOutputTypeDef",
     "SendNotificationActionDefinitionTypeDef",
     "ParticipantTimerConfigurationTypeDef",
-    "PredefinedAttributePaginatorTypeDef",
+    "PredefinedAttributeTypeDef",
+    "PredefinedAttributeValuesUnionTypeDef",
     "QuickConnectConfigTypeDef",
     "RealTimeContactAnalysisTranscriptItemRedactionTypeDef",
     "RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef",
     "RealTimeContactAnalysisTranscriptItemWithContentTypeDef",
     "RealTimeContactAnalysisSegmentAttachmentsTypeDef",
     "RealTimeContactAnalysisSegmentEventTypeDef",
     "ReferenceSummaryTypeDef",
     "StartOutboundVoiceContactRequestRequestTypeDef",
     "StartTaskContactRequestRequestTypeDef",
+    "TaskActionDefinitionOutputTypeDef",
     "TaskActionDefinitionTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ResourceTagsSearchCriteriaTypeDef",
     "SearchResourceTagsResponseTypeDef",
     "SearchSecurityProfilesResponseTypeDef",
     "SearchVocabulariesResponseTypeDef",
     "SearchableContactAttributesTypeDef",
     "StartChatContactRequestRequestTypeDef",
+    "SignInConfigOutputTypeDef",
     "SignInConfigTypeDef",
+    "StartAttachedFileUploadResponseTypeDef",
     "StartContactRecordingRequestRequestTypeDef",
     "TranscriptTypeDef",
     "UserSearchSummaryTypeDef",
     "ViewTypeDef",
     "ListRulesResponseTypeDef",
+    "AgentConfigUnionTypeDef",
+    "TelephonyConfigUnionTypeDef",
     "StartWebRTCContactRequestRequestTypeDef",
+    "CreateSecurityProfileRequestRequestTypeDef",
+    "UpdateSecurityProfileRequestRequestTypeDef",
     "ListBotsResponseTypeDef",
+    "BatchGetAttachedFileMetadataResponseTypeDef",
     "ControlPlaneUserAttributeFilterTypeDef",
     "HoursOfOperationSearchFilterTypeDef",
     "PromptSearchFilterTypeDef",
     "QueueSearchFilterTypeDef",
     "QuickConnectSearchFilterTypeDef",
     "RoutingProfileSearchFilterTypeDef",
     "SecurityProfilesSearchFilterTypeDef",
     "MeetingTypeDef",
     "DescribePhoneNumberResponseTypeDef",
     "BatchPutContactRequestRequestTypeDef",
     "GetCurrentUserDataRequestRequestTypeDef",
     "SearchContactsResponseTypeDef",
     "DescribeContactResponseTypeDef",
     "DescribeEvaluationFormResponseTypeDef",
-    "DescribePredefinedAttributeResponseTypeDef",
-    "SearchPredefinedAttributesResponseTypeDef",
     "DescribeQueueResponseTypeDef",
     "SearchQueuesResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "RoutingProfileTypeDef",
     "UpdateRoutingProfileConcurrencyRequestRequestTypeDef",
     "CurrentMetricResultTypeDef",
     "AssociateRoutingProfileQueuesRequestRequestTypeDef",
     "CreateRoutingProfileRequestRequestTypeDef",
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     "InstanceStorageConfigTypeDef",
     "SubmitContactEvaluationRequestRequestTypeDef",
     "UpdateContactEvaluationRequestRequestTypeDef",
+    "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
     "EvaluationFormNumericQuestionPropertiesTypeDef",
+    "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationTypeDef",
     "EvaluationTypeDef",
     "ListContactEvaluationsResponseTypeDef",
+    "CreateCaseActionDefinitionOutputTypeDef",
+    "UpdateCaseActionDefinitionOutputTypeDef",
     "CreateCaseActionDefinitionTypeDef",
     "UpdateCaseActionDefinitionTypeDef",
     "UserDataTypeDef",
     "HierarchyGroupTypeDef",
     "DescribeUserHierarchyStructureResponseTypeDef",
     "UpdateUserHierarchyStructureRequestRequestTypeDef",
     "GetMetricDataRequestGetMetricDataPaginateTypeDef",
     "GetMetricDataRequestRequestTypeDef",
     "HistoricalMetricDataTypeDef",
     "CreateHoursOfOperationRequestRequestTypeDef",
     "HoursOfOperationTypeDef",
     "UpdateHoursOfOperationRequestRequestTypeDef",
     "SearchPredefinedAttributesRequestSearchPredefinedAttributesPaginateTypeDef",
     "DescribeInstanceResponseTypeDef",
+    "TaskTemplateConstraintsOutputTypeDef",
     "TaskTemplateConstraintsTypeDef",
+    "TaskTemplateDefaultsOutputTypeDef",
     "TaskTemplateDefaultsTypeDef",
-    "GetMetricDataV2RequestRequestTypeDef",
+    "TaskTemplateFieldUnionTypeDef",
     "MetricDataV2TypeDef",
+    "MetricV2UnionTypeDef",
     "SendChatIntegrationEventRequestRequestTypeDef",
     "ChatParticipantRoleConfigTypeDef",
-    "SearchPredefinedAttributesResponsePaginatorTypeDef",
+    "DescribePredefinedAttributeResponseTypeDef",
+    "SearchPredefinedAttributesResponseTypeDef",
     "CreateQuickConnectRequestRequestTypeDef",
     "QuickConnectTypeDef",
     "UpdateQuickConnectConfigRequestRequestTypeDef",
     "RealTimeContactAnalysisSegmentTranscriptTypeDef",
     "RealTimeContactAnalysisPointOfInterestTypeDef",
     "RealTimeContactAnalysisIssueDetectedTypeDef",
     "ListContactReferencesResponseTypeDef",
     "SearchResourceTagsRequestRequestTypeDef",
     "SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
     "GetTrafficDistributionResponseTypeDef",
+    "SignInConfigUnionTypeDef",
     "UpdateTrafficDistributionRequestRequestTypeDef",
     "ContactAnalysisTypeDef",
     "SearchUsersResponseTypeDef",
     "CreateViewResponseTypeDef",
     "CreateViewVersionResponseTypeDef",
     "DescribeViewResponseTypeDef",
     "UpdateViewContentResponseTypeDef",
@@ -777,49 +815,58 @@
     "DescribeRoutingProfileResponseTypeDef",
     "SearchRoutingProfilesResponseTypeDef",
     "GetCurrentMetricDataResponseTypeDef",
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
     "DescribeInstanceStorageConfigResponseTypeDef",
     "ListInstanceStorageConfigsResponseTypeDef",
     "UpdateInstanceStorageConfigRequestRequestTypeDef",
+    "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
     "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
     "DescribeContactEvaluationResponseTypeDef",
+    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
     "GetCurrentUserDataResponseTypeDef",
     "DescribeUserHierarchyGroupResponseTypeDef",
     "HistoricalMetricResultTypeDef",
     "DescribeHoursOfOperationResponseTypeDef",
     "SearchHoursOfOperationsResponseTypeDef",
-    "CreateTaskTemplateRequestRequestTypeDef",
+    "TaskTemplateConstraintsUnionTypeDef",
     "GetTaskTemplateResponseTypeDef",
-    "UpdateTaskTemplateRequestRequestTypeDef",
     "UpdateTaskTemplateResponseTypeDef",
+    "TaskTemplateDefaultsUnionTypeDef",
+    "CreateTaskTemplateRequestRequestTypeDef",
+    "UpdateTaskTemplateRequestRequestTypeDef",
     "MetricResultV2TypeDef",
+    "GetMetricDataV2RequestRequestTypeDef",
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     "DescribeQuickConnectResponseTypeDef",
     "SearchQuickConnectsResponseTypeDef",
     "RealTimeContactAnalysisCategoryDetailsTypeDef",
     "RealTimeContactAnalysisSegmentIssuesTypeDef",
     "SearchCriteriaTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchUsersRequestSearchUsersPaginateTypeDef",
     "StartWebRTCContactResponseTypeDef",
+    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
     "EvaluationFormQuestionTypePropertiesTypeDef",
-    "CreateRuleRequestRequestTypeDef",
     "RuleTypeDef",
-    "UpdateRuleRequestRequestTypeDef",
+    "RuleActionUnionTypeDef",
     "GetMetricDataResponseTypeDef",
     "GetMetricDataV2ResponseTypeDef",
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     "RealTimeContactAnalysisSegmentCategoriesTypeDef",
     "SearchContactsRequestRequestTypeDef",
     "SearchContactsRequestSearchContactsPaginateTypeDef",
+    "EvaluationFormQuestionOutputTypeDef",
     "EvaluationFormQuestionTypeDef",
     "DescribeRuleResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
+    "UpdateRuleRequestRequestTypeDef",
     "RealtimeContactAnalysisSegmentTypeDef",
+    "EvaluationFormItemOutputTypeDef",
     "EvaluationFormItemTypeDef",
     "ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef",
 )
 
 ActionSummaryTypeDef = TypedDict(
     "ActionSummaryTypeDef",
     {
@@ -928,16 +975,23 @@
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "EnableAnswerMachineDetection": NotRequired[bool],
         "AwaitAnswerMachinePrompt": NotRequired[bool],
     },
 )
-ApplicationPaginatorTypeDef = TypedDict(
-    "ApplicationPaginatorTypeDef",
+ApplicationExtraOutputTypeDef = TypedDict(
+    "ApplicationExtraOutputTypeDef",
+    {
+        "Namespace": NotRequired[str],
+        "ApplicationPermissions": NotRequired[List[str]],
+    },
+)
+ApplicationOutputTypeDef = TypedDict(
+    "ApplicationOutputTypeDef",
     {
         "Namespace": NotRequired[str],
         "ApplicationPermissions": NotRequired[List[str]],
     },
 )
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
@@ -1033,14 +1087,29 @@
     "UserProficiencyTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
         "Level": float,
     },
 )
+AttachedFileErrorTypeDef = TypedDict(
+    "AttachedFileErrorTypeDef",
+    {
+        "ErrorCode": NotRequired[str],
+        "ErrorMessage": NotRequired[str],
+        "FileId": NotRequired[str],
+    },
+)
+CreatedByInfoTypeDef = TypedDict(
+    "CreatedByInfoTypeDef",
+    {
+        "ConnectUserArn": NotRequired[str],
+        "AWSIdentityArn": NotRequired[str],
+    },
+)
 AttachmentReferenceTypeDef = TypedDict(
     "AttachmentReferenceTypeDef",
     {
         "Name": NotRequired[str],
         "Value": NotRequired[str],
         "Status": NotRequired[ReferenceStatusType],
     },
@@ -1106,14 +1175,22 @@
     "BatchDisassociateAnalyticsDataSetRequestRequestTypeDef",
     {
         "InstanceId": str,
         "DataSetIds": Sequence[str],
         "TargetAccountId": NotRequired[str],
     },
 )
+BatchGetAttachedFileMetadataRequestRequestTypeDef = TypedDict(
+    "BatchGetAttachedFileMetadataRequestRequestTypeDef",
+    {
+        "FileIds": Sequence[str],
+        "InstanceId": str,
+        "AssociatedResourceArn": str,
+    },
+)
 BatchGetFlowAssociationRequestRequestTypeDef = TypedDict(
     "BatchGetFlowAssociationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceIds": Sequence[str],
         "ResourceType": NotRequired[Literal["VOICE_PHONE_NUMBER"]],
     },
@@ -1182,14 +1259,22 @@
 PhoneNumberStatusTypeDef = TypedDict(
     "PhoneNumberStatusTypeDef",
     {
         "Status": NotRequired[PhoneNumberWorkflowStatusType],
         "Message": NotRequired[str],
     },
 )
+CompleteAttachedFileUploadRequestRequestTypeDef = TypedDict(
+    "CompleteAttachedFileUploadRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "FileId": str,
+        "AssociatedResourceArn": str,
+    },
+)
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Type": NotRequired[EndpointTypeType],
         "Address": NotRequired[str],
     },
 )
@@ -1300,14 +1385,17 @@
         "Name": str,
         "Type": ContactFlowTypeType,
         "Content": str,
         "Description": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
+EvaluationFormItemUnionTypeDef = Union[
+    "EvaluationFormItemTypeDef", "EvaluationFormItemOutputTypeDef"
+]
 EvaluationFormScoringStrategyTypeDef = TypedDict(
     "EvaluationFormScoringStrategyTypeDef",
     {
         "Mode": EvaluationFormScoringModeType,
         "Status": EvaluationFormScoringStatusType,
     },
 )
@@ -1513,14 +1601,22 @@
     {
         "InstanceId": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "VocabularyId": str,
         "VocabularyName": str,
     },
 )
+DeleteAttachedFileRequestRequestTypeDef = TypedDict(
+    "DeleteAttachedFileRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "FileId": str,
+        "AssociatedResourceArn": str,
+    },
+)
 DeleteContactEvaluationRequestRequestTypeDef = TypedDict(
     "DeleteContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
     },
 )
@@ -2001,14 +2097,21 @@
     "DismissUserContactRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
         "ContactId": str,
     },
 )
+DownloadUrlMetadataTypeDef = TypedDict(
+    "DownloadUrlMetadataTypeDef",
+    {
+        "Url": NotRequired[str],
+        "UrlExpiry": NotRequired[str],
+    },
+)
 EmailReferenceTypeDef = TypedDict(
     "EmailReferenceTypeDef",
     {
         "Name": NotRequired[str],
         "Value": NotRequired[str],
     },
 )
@@ -2038,14 +2141,24 @@
     {
         "MinValue": int,
         "MaxValue": int,
         "Score": NotRequired[int],
         "AutomaticFail": NotRequired[bool],
     },
 )
+EvaluationFormSectionOutputTypeDef = TypedDict(
+    "EvaluationFormSectionOutputTypeDef",
+    {
+        "Title": str,
+        "RefId": str,
+        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "Instructions": NotRequired[str],
+        "Weight": NotRequired[float],
+    },
+)
 EvaluationFormSectionTypeDef = TypedDict(
     "EvaluationFormSectionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "Items": Sequence["EvaluationFormItemTypeDef"],
         "Instructions": NotRequired[str],
@@ -2115,14 +2228,23 @@
 )
 EventBridgeActionDefinitionTypeDef = TypedDict(
     "EventBridgeActionDefinitionTypeDef",
     {
         "Name": str,
     },
 )
+FieldValueUnionOutputTypeDef = TypedDict(
+    "FieldValueUnionOutputTypeDef",
+    {
+        "BooleanValue": NotRequired[bool],
+        "DoubleValue": NotRequired[float],
+        "EmptyValue": NotRequired[Dict[str, Any]],
+        "StringValue": NotRequired[str],
+    },
+)
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "BooleanValue": NotRequired[bool],
         "DoubleValue": NotRequired[float],
         "EmptyValue": NotRequired[Mapping[str, Any]],
         "StringValue": NotRequired[str],
@@ -2140,14 +2262,23 @@
     {
         "Queues": NotRequired[Sequence[str]],
         "Channels": NotRequired[Sequence[ChannelType]],
         "RoutingProfiles": NotRequired[Sequence[str]],
         "RoutingStepExpressions": NotRequired[Sequence[str]],
     },
 )
+GetAttachedFileRequestRequestTypeDef = TypedDict(
+    "GetAttachedFileRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "FileId": str,
+        "AssociatedResourceArn": str,
+        "UrlExpiryInSeconds": NotRequired[int],
+    },
+)
 GetContactAttributesRequestRequestTypeDef = TypedDict(
     "GetContactAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "InitialContactId": str,
     },
 )
@@ -2892,14 +3023,22 @@
         "AudioHostUrl": NotRequired[str],
         "AudioFallbackUrl": NotRequired[str],
         "SignalingUrl": NotRequired[str],
         "TurnControlUrl": NotRequired[str],
         "EventIngestionUrl": NotRequired[str],
     },
 )
+MetricFilterV2OutputTypeDef = TypedDict(
+    "MetricFilterV2OutputTypeDef",
+    {
+        "MetricFilterKey": NotRequired[str],
+        "MetricFilterValues": NotRequired[List[str]],
+        "Negate": NotRequired[bool],
+    },
+)
 MetricFilterV2TypeDef = TypedDict(
     "MetricFilterV2TypeDef",
     {
         "MetricFilterKey": NotRequired[str],
         "MetricFilterValues": NotRequired[Sequence[str]],
         "Negate": NotRequired[bool],
     },
@@ -2931,14 +3070,21 @@
 )
 ParticipantDetailsTypeDef = TypedDict(
     "ParticipantDetailsTypeDef",
     {
         "DisplayName": str,
     },
 )
+NotificationRecipientTypeOutputTypeDef = TypedDict(
+    "NotificationRecipientTypeOutputTypeDef",
+    {
+        "UserTags": NotRequired[Dict[str, str]],
+        "UserIds": NotRequired[List[str]],
+    },
+)
 NotificationRecipientTypeTypeDef = TypedDict(
     "NotificationRecipientTypeTypeDef",
     {
         "UserTags": NotRequired[Mapping[str, str]],
         "UserIds": NotRequired[Sequence[str]],
     },
 )
@@ -2973,16 +3119,22 @@
 )
 PhoneNumberQuickConnectConfigTypeDef = TypedDict(
     "PhoneNumberQuickConnectConfigTypeDef",
     {
         "PhoneNumber": str,
     },
 )
-PredefinedAttributeValuesPaginatorTypeDef = TypedDict(
-    "PredefinedAttributeValuesPaginatorTypeDef",
+PredefinedAttributeValuesOutputTypeDef = TypedDict(
+    "PredefinedAttributeValuesOutputTypeDef",
+    {
+        "StringList": NotRequired[List[str]],
+    },
+)
+PredefinedAttributeValuesExtraOutputTypeDef = TypedDict(
+    "PredefinedAttributeValuesExtraOutputTypeDef",
     {
         "StringList": NotRequired[List[str]],
     },
 )
 PutUserStatusRequestRequestTypeDef = TypedDict(
     "PutUserStatusRequestRequestTypeDef",
     {
@@ -3180,14 +3332,22 @@
 SignInDistributionTypeDef = TypedDict(
     "SignInDistributionTypeDef",
     {
         "Region": str,
         "Enabled": bool,
     },
 )
+UploadUrlMetadataTypeDef = TypedDict(
+    "UploadUrlMetadataTypeDef",
+    {
+        "Url": NotRequired[str],
+        "UrlExpiry": NotRequired[str],
+        "HeadersToInclude": NotRequired[Dict[str, str]],
+    },
+)
 StartContactEvaluationRequestRequestTypeDef = TypedDict(
     "StartContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "EvaluationFormId": str,
         "ClientToken": NotRequired[str],
@@ -3782,34 +3942,34 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListApprovedOriginsResponseTypeDef = TypedDict(
     "ListApprovedOriginsResponseTypeDef",
     {
         "Origins": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListLambdaFunctionsResponseTypeDef = TypedDict(
     "ListLambdaFunctionsResponseTypeDef",
     {
         "LambdaFunctions": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSecurityProfilePermissionsResponseTypeDef = TypedDict(
     "ListSecurityProfilePermissionsResponseTypeDef",
     {
         "Permissions": List[str],
-        "NextToken": str,
         "LastModifiedTime": datetime,
         "LastModifiedRegion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3923,24 +4083,36 @@
     "UpdatePromptResponseTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AgentConfigOutputTypeDef = TypedDict(
+    "AgentConfigOutputTypeDef",
+    {
+        "Distributions": List[DistributionTypeDef],
+    },
+)
 AgentConfigTypeDef = TypedDict(
     "AgentConfigTypeDef",
     {
+        "Distributions": Sequence[DistributionTypeDef],
+    },
+)
+TelephonyConfigOutputTypeDef = TypedDict(
+    "TelephonyConfigOutputTypeDef",
+    {
         "Distributions": List[DistributionTypeDef],
     },
 )
 TelephonyConfigTypeDef = TypedDict(
     "TelephonyConfigTypeDef",
     {
-        "Distributions": List[DistributionTypeDef],
+        "Distributions": Sequence[DistributionTypeDef],
     },
 )
 AgentContactReferenceTypeDef = TypedDict(
     "AgentContactReferenceTypeDef",
     {
         "ContactId": NotRequired[str],
         "Channel": NotRequired[ChannelType],
@@ -3950,17 +4122,17 @@
         "ConnectedToAgentTimestamp": NotRequired[datetime],
         "Queue": NotRequired[QueueReferenceTypeDef],
     },
 )
 ListAgentStatusResponseTypeDef = TypedDict(
     "ListAgentStatusResponseTypeDef",
     {
-        "NextToken": str,
         "AgentStatusSummaryList": List[AgentStatusSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeAgentStatusResponseTypeDef = TypedDict(
     "DescribeAgentStatusResponseTypeDef",
     {
         "AgentStatus": AgentStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3973,80 +4145,42 @@
         "Agent": NotRequired[ParticipantCapabilitiesTypeDef],
     },
 )
 ListAnalyticsDataAssociationsResponseTypeDef = TypedDict(
     "ListAnalyticsDataAssociationsResponseTypeDef",
     {
         "Results": List[AnalyticsDataAssociationResultTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ListSecurityProfileApplicationsResponsePaginatorTypeDef = TypedDict(
-    "ListSecurityProfileApplicationsResponsePaginatorTypeDef",
-    {
-        "Applications": List[ApplicationPaginatorTypeDef],
-        "NextToken": str,
-        "LastModifiedTime": datetime,
-        "LastModifiedRegion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "CreateSecurityProfileRequestRequestTypeDef",
-    {
-        "SecurityProfileName": str,
-        "InstanceId": str,
-        "Description": NotRequired[str],
-        "Permissions": NotRequired[Sequence[str]],
-        "Tags": NotRequired[Mapping[str, str]],
-        "AllowedAccessControlTags": NotRequired[Mapping[str, str]],
-        "TagRestrictedResources": NotRequired[Sequence[str]],
-        "Applications": NotRequired[Sequence[ApplicationTypeDef]],
-        "HierarchyRestrictedResources": NotRequired[Sequence[str]],
-        "AllowedAccessControlHierarchyGroupId": NotRequired[str],
+        "NextToken": NotRequired[str],
     },
 )
 ListSecurityProfileApplicationsResponseTypeDef = TypedDict(
     "ListSecurityProfileApplicationsResponseTypeDef",
     {
-        "Applications": List[ApplicationTypeDef],
-        "NextToken": str,
+        "Applications": List[ApplicationExtraOutputTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedRegion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-UpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "SecurityProfileId": str,
-        "InstanceId": str,
-        "Description": NotRequired[str],
-        "Permissions": NotRequired[Sequence[str]],
-        "AllowedAccessControlTags": NotRequired[Mapping[str, str]],
-        "TagRestrictedResources": NotRequired[Sequence[str]],
-        "Applications": NotRequired[Sequence[ApplicationTypeDef]],
-        "HierarchyRestrictedResources": NotRequired[Sequence[str]],
-        "AllowedAccessControlHierarchyGroupId": NotRequired[str],
-    },
-)
+ApplicationUnionTypeDef = Union[ApplicationTypeDef, ApplicationExtraOutputTypeDef]
 AssociateLexBotRequestRequestTypeDef = TypedDict(
     "AssociateLexBotRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LexBot": LexBotTypeDef,
     },
 )
 ListLexBotsResponseTypeDef = TypedDict(
     "ListLexBotsResponseTypeDef",
     {
         "LexBots": List[LexBotTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateBotRequestRequestTypeDef = TypedDict(
     "AssociateBotRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LexBot": NotRequired[LexBotTypeDef],
@@ -4075,29 +4209,58 @@
         "UserId": str,
         "UserProficiencies": Sequence[UserProficiencyTypeDef],
     },
 )
 ListUserProficienciesResponseTypeDef = TypedDict(
     "ListUserProficienciesResponseTypeDef",
     {
-        "NextToken": str,
         "UserProficiencyList": List[UserProficiencyTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedRegion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateUserProficienciesRequestRequestTypeDef = TypedDict(
     "UpdateUserProficienciesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "UserId": str,
         "UserProficiencies": Sequence[UserProficiencyTypeDef],
     },
 )
+AttachedFileTypeDef = TypedDict(
+    "AttachedFileTypeDef",
+    {
+        "CreationTime": str,
+        "FileArn": str,
+        "FileId": str,
+        "FileName": str,
+        "FileSizeInBytes": int,
+        "FileStatus": FileStatusTypeType,
+        "CreatedBy": NotRequired[CreatedByInfoTypeDef],
+        "FileUseCaseType": NotRequired[Literal["ATTACHMENT"]],
+        "AssociatedResourceArn": NotRequired[str],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
+StartAttachedFileUploadRequestRequestTypeDef = TypedDict(
+    "StartAttachedFileUploadRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "FileName": str,
+        "FileSizeInBytes": int,
+        "FileUseCaseType": Literal["ATTACHMENT"],
+        "AssociatedResourceArn": str,
+        "ClientToken": NotRequired[str],
+        "UrlExpiryInSeconds": NotRequired[int],
+        "CreatedBy": NotRequired[CreatedByInfoTypeDef],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
 AttributeAndConditionTypeDef = TypedDict(
     "AttributeAndConditionTypeDef",
     {
         "TagConditions": NotRequired[Sequence[TagConditionTypeDef]],
         "HierarchyGroupCondition": NotRequired[HierarchyGroupConditionTypeDef],
     },
 )
@@ -4116,30 +4279,30 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInstanceAttributesResponseTypeDef = TypedDict(
     "ListInstanceAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 MeetingFeaturesConfigurationTypeDef = TypedDict(
     "MeetingFeaturesConfigurationTypeDef",
     {
         "Audio": NotRequired[AudioFeaturesTypeDef],
     },
 )
 SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
     "SearchAvailablePhoneNumbersResponseTypeDef",
     {
-        "NextToken": str,
         "AvailableNumbersList": List[AvailableNumberSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchAssociateAnalyticsDataSetResponseTypeDef = TypedDict(
     "BatchAssociateAnalyticsDataSetResponseTypeDef",
     {
         "Created": List[AnalyticsDataAssociationResultTypeDef],
         "Errors": List[ErrorResultTypeDef],
@@ -4161,16 +4324,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListFlowAssociationsResponseTypeDef = TypedDict(
     "ListFlowAssociationsResponseTypeDef",
     {
         "FlowAssociationSummaryList": List[FlowAssociationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchPutContactResponseTypeDef = TypedDict(
     "BatchPutContactResponseTypeDef",
     {
         "SuccessfulRequestList": List[SuccessfulRequestTypeDef],
         "FailedRequestList": List[FailedRequestTypeDef],
@@ -4223,31 +4386,31 @@
         "UserHierarchyGroups": NotRequired[Sequence[str]],
     },
 )
 ListContactFlowModulesResponseTypeDef = TypedDict(
     "ListContactFlowModulesResponseTypeDef",
     {
         "ContactFlowModulesSummaryList": List[ContactFlowModuleSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeContactFlowModuleResponseTypeDef = TypedDict(
     "DescribeContactFlowModuleResponseTypeDef",
     {
         "ContactFlowModule": ContactFlowModuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListContactFlowsResponseTypeDef = TypedDict(
     "ListContactFlowsResponseTypeDef",
     {
         "ContactFlowSummaryList": List[ContactFlowSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeContactFlowResponseTypeDef = TypedDict(
     "DescribeContactFlowResponseTypeDef",
     {
         "ContactFlow": ContactFlowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4298,42 +4461,42 @@
     },
 )
 CreateEvaluationFormRequestRequestTypeDef = TypedDict(
     "CreateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Title": str,
-        "Items": Sequence["EvaluationFormItemTypeDef"],
+        "Items": Sequence[EvaluationFormItemUnionTypeDef],
         "Description": NotRequired[str],
         "ScoringStrategy": NotRequired[EvaluationFormScoringStrategyTypeDef],
         "ClientToken": NotRequired[str],
     },
 )
 EvaluationFormContentTypeDef = TypedDict(
     "EvaluationFormContentTypeDef",
     {
         "EvaluationFormVersion": int,
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
-        "Items": List["EvaluationFormItemTypeDef"],
+        "Items": List["EvaluationFormItemOutputTypeDef"],
         "Description": NotRequired[str],
         "ScoringStrategy": NotRequired[EvaluationFormScoringStrategyTypeDef],
     },
 )
 EvaluationFormTypeDef = TypedDict(
     "EvaluationFormTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
         "EvaluationFormArn": str,
         "Title": str,
         "Status": EvaluationFormVersionStatusType,
-        "Items": List["EvaluationFormItemTypeDef"],
+        "Items": List["EvaluationFormItemOutputTypeDef"],
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
         "Description": NotRequired[str],
         "ScoringStrategy": NotRequired[EvaluationFormScoringStrategyTypeDef],
         "Tags": NotRequired[Dict[str, str]],
@@ -4342,15 +4505,15 @@
 UpdateEvaluationFormRequestRequestTypeDef = TypedDict(
     "UpdateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Title": str,
-        "Items": Sequence["EvaluationFormItemTypeDef"],
+        "Items": Sequence[EvaluationFormItemUnionTypeDef],
         "CreateNewVersion": NotRequired[bool],
         "Description": NotRequired[str],
         "ScoringStrategy": NotRequired[EvaluationFormScoringStrategyTypeDef],
         "ClientToken": NotRequired[str],
     },
 )
 CreateParticipantRequestRequestTypeDef = TypedDict(
@@ -4374,23 +4537,14 @@
     "CreatePredefinedAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
         "Values": PredefinedAttributeValuesTypeDef,
     },
 )
-PredefinedAttributeTypeDef = TypedDict(
-    "PredefinedAttributeTypeDef",
-    {
-        "Name": NotRequired[str],
-        "Values": NotRequired[PredefinedAttributeValuesTypeDef],
-        "LastModifiedTime": NotRequired[datetime],
-        "LastModifiedRegion": NotRequired[str],
-    },
-)
 UpdatePredefinedAttributeRequestRequestTypeDef = TypedDict(
     "UpdatePredefinedAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
         "Values": NotRequired[PredefinedAttributeValuesTypeDef],
     },
@@ -4526,32 +4680,32 @@
         "Value": NotRequired[float],
     },
 )
 ListDefaultVocabulariesResponseTypeDef = TypedDict(
     "ListDefaultVocabulariesResponseTypeDef",
     {
         "DefaultVocabularyList": List[DefaultVocabularyTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribePromptResponseTypeDef = TypedDict(
     "DescribePromptResponseTypeDef",
     {
         "Prompt": PromptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchPromptsResponseTypeDef = TypedDict(
     "SearchPromptsResponseTypeDef",
     {
         "Prompts": List[PromptTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSecurityProfileResponseTypeDef = TypedDict(
     "DescribeSecurityProfileResponseTypeDef",
     {
         "SecurityProfile": SecurityProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4608,14 +4762,31 @@
     "StopContactRequestRequestTypeDef",
     {
         "ContactId": str,
         "InstanceId": str,
         "DisconnectReason": NotRequired[DisconnectReasonTypeDef],
     },
 )
+GetAttachedFileResponseTypeDef = TypedDict(
+    "GetAttachedFileResponseTypeDef",
+    {
+        "FileArn": str,
+        "FileId": str,
+        "CreationTime": str,
+        "FileStatus": FileStatusTypeType,
+        "FileName": str,
+        "FileSizeInBytes": int,
+        "AssociatedResourceArn": str,
+        "FileUseCaseType": Literal["ATTACHMENT"],
+        "CreatedBy": CreatedByInfoTypeDef,
+        "DownloadUrlMetadata": DownloadUrlMetadataTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 KinesisVideoStreamConfigTypeDef = TypedDict(
     "KinesisVideoStreamConfigTypeDef",
     {
         "Prefix": str,
         "RetentionPeriodHours": int,
         "EncryptionConfig": EncryptionConfigTypeDef,
     },
@@ -4653,24 +4824,24 @@
         "RuleCategory": NotRequired[SingleSelectQuestionRuleCategoryAutomationTypeDef],
     },
 )
 ListEvaluationFormsResponseTypeDef = TypedDict(
     "ListEvaluationFormsResponseTypeDef",
     {
         "EvaluationFormSummaryList": List[EvaluationFormSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListEvaluationFormVersionsResponseTypeDef = TypedDict(
     "ListEvaluationFormVersionsResponseTypeDef",
     {
         "EvaluationFormVersionSummaryList": List[EvaluationFormVersionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 EvaluationMetadataTypeDef = TypedDict(
     "EvaluationMetadataTypeDef",
     {
         "ContactId": str,
         "EvaluatorArn": str,
@@ -4688,14 +4859,21 @@
         "Status": EvaluationStatusType,
         "EvaluatorArn": str,
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
         "Score": NotRequired[EvaluationScoreTypeDef],
     },
 )
+FieldValueOutputTypeDef = TypedDict(
+    "FieldValueOutputTypeDef",
+    {
+        "Id": str,
+        "Value": FieldValueUnionOutputTypeDef,
+    },
+)
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "Id": str,
         "Value": FieldValueUnionTypeDef,
     },
 )
@@ -5089,16 +5267,16 @@
         "LevelFive": NotRequired[HierarchyGroupSummaryTypeDef],
     },
 )
 ListUserHierarchyGroupsResponseTypeDef = TypedDict(
     "ListUserHierarchyGroupsResponseTypeDef",
     {
         "UserHierarchyGroupSummaryList": List[HierarchyGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 HierarchyStructureTypeDef = TypedDict(
     "HierarchyStructureTypeDef",
     {
         "LevelOne": NotRequired[HierarchyLevelTypeDef],
         "LevelTwo": NotRequired[HierarchyLevelTypeDef],
@@ -5200,16 +5378,16 @@
         "HierarchyGroupCondition": NotRequired[HierarchyGroupConditionTypeDef],
     },
 )
 ListHoursOfOperationsResponseTypeDef = TypedDict(
     "ListHoursOfOperationsResponseTypeDef",
     {
         "HoursOfOperationSummaryList": List[HoursOfOperationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "Id": NotRequired[str],
         "Arn": NotRequired[str],
@@ -5225,24 +5403,24 @@
         "Tags": NotRequired[Dict[str, str]],
     },
 )
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "InstanceSummaryList": List[InstanceSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListIntegrationAssociationsResponseTypeDef",
     {
         "IntegrationAssociationSummaryList": List[IntegrationAssociationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InvisibleFieldInfoTypeDef = TypedDict(
     "InvisibleFieldInfoTypeDef",
     {
         "Id": NotRequired[TaskTemplateFieldIdentifierTypeDef],
     },
@@ -5262,169 +5440,186 @@
 TaskTemplateDefaultFieldValueTypeDef = TypedDict(
     "TaskTemplateDefaultFieldValueTypeDef",
     {
         "Id": NotRequired[TaskTemplateFieldIdentifierTypeDef],
         "DefaultValue": NotRequired[str],
     },
 )
+TaskTemplateFieldOutputTypeDef = TypedDict(
+    "TaskTemplateFieldOutputTypeDef",
+    {
+        "Id": TaskTemplateFieldIdentifierTypeDef,
+        "Description": NotRequired[str],
+        "Type": NotRequired[TaskTemplateFieldTypeType],
+        "SingleSelectOptions": NotRequired[List[str]],
+    },
+)
 TaskTemplateFieldTypeDef = TypedDict(
     "TaskTemplateFieldTypeDef",
     {
         "Id": TaskTemplateFieldIdentifierTypeDef,
         "Description": NotRequired[str],
         "Type": NotRequired[TaskTemplateFieldTypeType],
         "SingleSelectOptions": NotRequired[Sequence[str]],
     },
 )
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumberSummaryList": List[PhoneNumberSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPhoneNumbersV2ResponseTypeDef = TypedDict(
     "ListPhoneNumbersV2ResponseTypeDef",
     {
-        "NextToken": str,
         "ListPhoneNumbersSummaryList": List[ListPhoneNumbersSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPredefinedAttributesResponseTypeDef = TypedDict(
     "ListPredefinedAttributesResponseTypeDef",
     {
-        "NextToken": str,
         "PredefinedAttributeSummaryList": List[PredefinedAttributeSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPromptsResponseTypeDef = TypedDict(
     "ListPromptsResponseTypeDef",
     {
         "PromptSummaryList": List[PromptSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListQueueQuickConnectsResponseTypeDef = TypedDict(
     "ListQueueQuickConnectsResponseTypeDef",
     {
-        "NextToken": str,
         "QuickConnectSummaryList": List[QuickConnectSummaryTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedRegion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListQuickConnectsResponseTypeDef = TypedDict(
     "ListQuickConnectsResponseTypeDef",
     {
         "QuickConnectSummaryList": List[QuickConnectSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListQueuesResponseTypeDef = TypedDict(
     "ListQueuesResponseTypeDef",
     {
         "QueueSummaryList": List[QueueSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListRoutingProfileQueuesResponseTypeDef = TypedDict(
     "ListRoutingProfileQueuesResponseTypeDef",
     {
-        "NextToken": str,
         "RoutingProfileQueueConfigSummaryList": List[RoutingProfileQueueConfigSummaryTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedRegion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListRoutingProfilesResponseTypeDef = TypedDict(
     "ListRoutingProfilesResponseTypeDef",
     {
         "RoutingProfileSummaryList": List[RoutingProfileSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSecurityKeysResponseTypeDef = TypedDict(
     "ListSecurityKeysResponseTypeDef",
     {
         "SecurityKeys": List[SecurityKeyTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSecurityProfilesResponseTypeDef = TypedDict(
     "ListSecurityProfilesResponseTypeDef",
     {
         "SecurityProfileSummaryList": List[SecurityProfileSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTaskTemplatesResponseTypeDef = TypedDict(
     "ListTaskTemplatesResponseTypeDef",
     {
         "TaskTemplates": List[TaskTemplateMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTrafficDistributionGroupUsersResponseTypeDef = TypedDict(
     "ListTrafficDistributionGroupUsersResponseTypeDef",
     {
-        "NextToken": str,
         "TrafficDistributionGroupUserSummaryList": List[TrafficDistributionGroupUserSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTrafficDistributionGroupsResponseTypeDef = TypedDict(
     "ListTrafficDistributionGroupsResponseTypeDef",
     {
-        "NextToken": str,
         "TrafficDistributionGroupSummaryList": List[TrafficDistributionGroupSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUseCasesResponseTypeDef = TypedDict(
     "ListUseCasesResponseTypeDef",
     {
         "UseCaseSummaryList": List[UseCaseTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "UserSummaryList": List[UserSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListViewVersionsResponseTypeDef = TypedDict(
     "ListViewVersionsResponseTypeDef",
     {
         "ViewVersionSummaryList": List[ViewVersionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListViewsResponseTypeDef = TypedDict(
     "ListViewsResponseTypeDef",
     {
         "ViewsSummaryList": List[ViewSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+MetricV2OutputTypeDef = TypedDict(
+    "MetricV2OutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Threshold": NotRequired[List[ThresholdV2TypeDef]],
+        "MetricFilters": NotRequired[List[MetricFilterV2OutputTypeDef]],
     },
 )
 MetricV2TypeDef = TypedDict(
     "MetricV2TypeDef",
     {
         "Name": NotRequired[str],
         "Threshold": NotRequired[Sequence[ThresholdV2TypeDef]],
@@ -5436,14 +5631,24 @@
     {
         "SupportedMessagingContentTypes": NotRequired[Sequence[str]],
         "ParticipantDetails": NotRequired[ParticipantDetailsTypeDef],
         "Attributes": NotRequired[Mapping[str, str]],
         "StreamingConfiguration": NotRequired[ChatStreamingConfigurationTypeDef],
     },
 )
+SendNotificationActionDefinitionOutputTypeDef = TypedDict(
+    "SendNotificationActionDefinitionOutputTypeDef",
+    {
+        "DeliveryMethod": Literal["EMAIL"],
+        "Content": str,
+        "ContentType": Literal["PLAIN_TEXT"],
+        "Recipient": NotificationRecipientTypeOutputTypeDef,
+        "Subject": NotRequired[str],
+    },
+)
 SendNotificationActionDefinitionTypeDef = TypedDict(
     "SendNotificationActionDefinitionTypeDef",
     {
         "DeliveryMethod": Literal["EMAIL"],
         "Content": str,
         "ContentType": Literal["PLAIN_TEXT"],
         "Recipient": NotificationRecipientTypeTypeDef,
@@ -5454,23 +5659,26 @@
     "ParticipantTimerConfigurationTypeDef",
     {
         "ParticipantRole": TimerEligibleParticipantRolesType,
         "TimerType": ParticipantTimerTypeType,
         "TimerValue": ParticipantTimerValueTypeDef,
     },
 )
-PredefinedAttributePaginatorTypeDef = TypedDict(
-    "PredefinedAttributePaginatorTypeDef",
+PredefinedAttributeTypeDef = TypedDict(
+    "PredefinedAttributeTypeDef",
     {
         "Name": NotRequired[str],
-        "Values": NotRequired[PredefinedAttributeValuesPaginatorTypeDef],
+        "Values": NotRequired[PredefinedAttributeValuesOutputTypeDef],
         "LastModifiedTime": NotRequired[datetime],
         "LastModifiedRegion": NotRequired[str],
     },
 )
+PredefinedAttributeValuesUnionTypeDef = Union[
+    PredefinedAttributeValuesTypeDef, PredefinedAttributeValuesExtraOutputTypeDef
+]
 QuickConnectConfigTypeDef = TypedDict(
     "QuickConnectConfigTypeDef",
     {
         "QuickConnectType": QuickConnectTypeType,
         "UserConfig": NotRequired[UserQuickConnectConfigTypeDef],
         "QueueConfig": NotRequired[QueueQuickConnectConfigTypeDef],
         "PhoneConfig": NotRequired[PhoneNumberQuickConnectConfigTypeDef],
@@ -5562,14 +5770,23 @@
         "ClientToken": NotRequired[str],
         "ScheduledTime": NotRequired[TimestampTypeDef],
         "TaskTemplateId": NotRequired[str],
         "QuickConnectId": NotRequired[str],
         "RelatedContactId": NotRequired[str],
     },
 )
+TaskActionDefinitionOutputTypeDef = TypedDict(
+    "TaskActionDefinitionOutputTypeDef",
+    {
+        "Name": str,
+        "ContactFlowId": str,
+        "Description": NotRequired[str],
+        "References": NotRequired[Dict[str, ReferenceTypeDef]],
+    },
+)
 TaskActionDefinitionTypeDef = TypedDict(
     "TaskActionDefinitionTypeDef",
     {
         "Name": str,
         "ContactFlowId": str,
         "Description": NotRequired[str],
         "References": NotRequired[Mapping[str, ReferenceTypeDef]],
@@ -5591,33 +5808,33 @@
         "TagSearchCondition": NotRequired[TagSearchConditionTypeDef],
     },
 )
 SearchResourceTagsResponseTypeDef = TypedDict(
     "SearchResourceTagsResponseTypeDef",
     {
         "Tags": List[TagSetTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchSecurityProfilesResponseTypeDef = TypedDict(
     "SearchSecurityProfilesResponseTypeDef",
     {
         "SecurityProfiles": List[SecurityProfileSearchSummaryTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchVocabulariesResponseTypeDef = TypedDict(
     "SearchVocabulariesResponseTypeDef",
     {
         "VocabularySummaryList": List[VocabularySummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchableContactAttributesTypeDef = TypedDict(
     "SearchableContactAttributesTypeDef",
     {
         "Criteria": Sequence[SearchableContactAttributesCriteriaTypeDef],
         "MatchType": NotRequired[SearchContactsMatchTypeType],
@@ -5635,18 +5852,36 @@
         "ChatDurationInMinutes": NotRequired[int],
         "SupportedMessagingContentTypes": NotRequired[Sequence[str]],
         "PersistentChat": NotRequired[PersistentChatTypeDef],
         "RelatedContactId": NotRequired[str],
         "SegmentAttributes": NotRequired[Mapping[str, SegmentAttributeValueTypeDef]],
     },
 )
+SignInConfigOutputTypeDef = TypedDict(
+    "SignInConfigOutputTypeDef",
+    {
+        "Distributions": List[SignInDistributionTypeDef],
+    },
+)
 SignInConfigTypeDef = TypedDict(
     "SignInConfigTypeDef",
     {
-        "Distributions": List[SignInDistributionTypeDef],
+        "Distributions": Sequence[SignInDistributionTypeDef],
+    },
+)
+StartAttachedFileUploadResponseTypeDef = TypedDict(
+    "StartAttachedFileUploadResponseTypeDef",
+    {
+        "FileArn": str,
+        "FileId": str,
+        "CreationTime": str,
+        "FileStatus": FileStatusTypeType,
+        "CreatedBy": CreatedByInfoTypeDef,
+        "UploadUrlMetadata": UploadUrlMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StartContactRecordingRequestRequestTypeDef = TypedDict(
     "StartContactRecordingRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
@@ -5694,37 +5929,76 @@
         "ViewContentSha256": NotRequired[str],
     },
 )
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "RuleSummaryList": List[RuleSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
+AgentConfigUnionTypeDef = Union[AgentConfigTypeDef, AgentConfigOutputTypeDef]
+TelephonyConfigUnionTypeDef = Union[TelephonyConfigTypeDef, TelephonyConfigOutputTypeDef]
 StartWebRTCContactRequestRequestTypeDef = TypedDict(
     "StartWebRTCContactRequestRequestTypeDef",
     {
         "ContactFlowId": str,
         "InstanceId": str,
         "ParticipantDetails": ParticipantDetailsTypeDef,
         "Attributes": NotRequired[Mapping[str, str]],
         "ClientToken": NotRequired[str],
         "AllowedCapabilities": NotRequired[AllowedCapabilitiesTypeDef],
         "RelatedContactId": NotRequired[str],
         "References": NotRequired[Mapping[str, ReferenceTypeDef]],
         "Description": NotRequired[str],
     },
 )
+CreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "CreateSecurityProfileRequestRequestTypeDef",
+    {
+        "SecurityProfileName": str,
+        "InstanceId": str,
+        "Description": NotRequired[str],
+        "Permissions": NotRequired[Sequence[str]],
+        "Tags": NotRequired[Mapping[str, str]],
+        "AllowedAccessControlTags": NotRequired[Mapping[str, str]],
+        "TagRestrictedResources": NotRequired[Sequence[str]],
+        "Applications": NotRequired[Sequence[ApplicationUnionTypeDef]],
+        "HierarchyRestrictedResources": NotRequired[Sequence[str]],
+        "AllowedAccessControlHierarchyGroupId": NotRequired[str],
+    },
+)
+UpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "SecurityProfileId": str,
+        "InstanceId": str,
+        "Description": NotRequired[str],
+        "Permissions": NotRequired[Sequence[str]],
+        "AllowedAccessControlTags": NotRequired[Mapping[str, str]],
+        "TagRestrictedResources": NotRequired[Sequence[str]],
+        "Applications": NotRequired[Sequence[ApplicationUnionTypeDef]],
+        "HierarchyRestrictedResources": NotRequired[Sequence[str]],
+        "AllowedAccessControlHierarchyGroupId": NotRequired[str],
+    },
+)
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "LexBots": List[LexBotConfigTypeDef],
-        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+BatchGetAttachedFileMetadataResponseTypeDef = TypedDict(
+    "BatchGetAttachedFileMetadataResponseTypeDef",
+    {
+        "Files": List[AttachedFileTypeDef],
+        "Errors": List[AttachedFileErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ControlPlaneUserAttributeFilterTypeDef = TypedDict(
     "ControlPlaneUserAttributeFilterTypeDef",
     {
         "OrConditions": NotRequired[Sequence[AttributeAndConditionTypeDef]],
@@ -5802,17 +6076,17 @@
         "MaxResults": NotRequired[int],
     },
 )
 SearchContactsResponseTypeDef = TypedDict(
     "SearchContactsResponseTypeDef",
     {
         "Contacts": List[ContactSearchSummaryTypeDef],
-        "NextToken": str,
         "TotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeContactResponseTypeDef = TypedDict(
     "DescribeContactResponseTypeDef",
     {
         "Contact": ContactTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5821,44 +6095,28 @@
 DescribeEvaluationFormResponseTypeDef = TypedDict(
     "DescribeEvaluationFormResponseTypeDef",
     {
         "EvaluationForm": EvaluationFormTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribePredefinedAttributeResponseTypeDef = TypedDict(
-    "DescribePredefinedAttributeResponseTypeDef",
-    {
-        "PredefinedAttribute": PredefinedAttributeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-SearchPredefinedAttributesResponseTypeDef = TypedDict(
-    "SearchPredefinedAttributesResponseTypeDef",
-    {
-        "PredefinedAttributes": List[PredefinedAttributeTypeDef],
-        "NextToken": str,
-        "ApproximateTotalCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeQueueResponseTypeDef = TypedDict(
     "DescribeQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchQueuesResponseTypeDef = TypedDict(
     "SearchQueuesResponseTypeDef",
     {
         "Queues": List[QueueTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5952,23 +6210,39 @@
     {
         "InstanceId": str,
         "EvaluationId": str,
         "Answers": NotRequired[Mapping[str, EvaluationAnswerInputTypeDef]],
         "Notes": NotRequired[Mapping[str, EvaluationNoteTypeDef]],
     },
 )
+EvaluationFormNumericQuestionPropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
+    {
+        "MinValue": int,
+        "MaxValue": int,
+        "Options": NotRequired[List[EvaluationFormNumericQuestionOptionTypeDef]],
+        "Automation": NotRequired[EvaluationFormNumericQuestionAutomationTypeDef],
+    },
+)
 EvaluationFormNumericQuestionPropertiesTypeDef = TypedDict(
     "EvaluationFormNumericQuestionPropertiesTypeDef",
     {
         "MinValue": int,
         "MaxValue": int,
         "Options": NotRequired[Sequence[EvaluationFormNumericQuestionOptionTypeDef]],
         "Automation": NotRequired[EvaluationFormNumericQuestionAutomationTypeDef],
     },
 )
+EvaluationFormSingleSelectQuestionAutomationOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
+    {
+        "Options": List[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],
+        "DefaultOptionRefId": NotRequired[str],
+    },
+)
 EvaluationFormSingleSelectQuestionAutomationTypeDef = TypedDict(
     "EvaluationFormSingleSelectQuestionAutomationTypeDef",
     {
         "Options": Sequence[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],
         "DefaultOptionRefId": NotRequired[str],
     },
 )
@@ -5987,16 +6261,29 @@
         "Tags": NotRequired[Dict[str, str]],
     },
 )
 ListContactEvaluationsResponseTypeDef = TypedDict(
     "ListContactEvaluationsResponseTypeDef",
     {
         "EvaluationSummaryList": List[EvaluationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+CreateCaseActionDefinitionOutputTypeDef = TypedDict(
+    "CreateCaseActionDefinitionOutputTypeDef",
+    {
+        "Fields": List[FieldValueOutputTypeDef],
+        "TemplateId": str,
+    },
+)
+UpdateCaseActionDefinitionOutputTypeDef = TypedDict(
+    "UpdateCaseActionDefinitionOutputTypeDef",
+    {
+        "Fields": List[FieldValueOutputTypeDef],
     },
 )
 CreateCaseActionDefinitionTypeDef = TypedDict(
     "CreateCaseActionDefinitionTypeDef",
     {
         "Fields": Sequence[FieldValueTypeDef],
         "TemplateId": str,
@@ -6128,49 +6415,51 @@
 DescribeInstanceResponseTypeDef = TypedDict(
     "DescribeInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+TaskTemplateConstraintsOutputTypeDef = TypedDict(
+    "TaskTemplateConstraintsOutputTypeDef",
+    {
+        "RequiredFields": NotRequired[List[RequiredFieldInfoTypeDef]],
+        "ReadOnlyFields": NotRequired[List[ReadOnlyFieldInfoTypeDef]],
+        "InvisibleFields": NotRequired[List[InvisibleFieldInfoTypeDef]],
+    },
+)
 TaskTemplateConstraintsTypeDef = TypedDict(
     "TaskTemplateConstraintsTypeDef",
     {
         "RequiredFields": NotRequired[Sequence[RequiredFieldInfoTypeDef]],
         "ReadOnlyFields": NotRequired[Sequence[ReadOnlyFieldInfoTypeDef]],
         "InvisibleFields": NotRequired[Sequence[InvisibleFieldInfoTypeDef]],
     },
 )
-TaskTemplateDefaultsTypeDef = TypedDict(
-    "TaskTemplateDefaultsTypeDef",
+TaskTemplateDefaultsOutputTypeDef = TypedDict(
+    "TaskTemplateDefaultsOutputTypeDef",
     {
-        "DefaultFieldValues": NotRequired[Sequence[TaskTemplateDefaultFieldValueTypeDef]],
+        "DefaultFieldValues": NotRequired[List[TaskTemplateDefaultFieldValueTypeDef]],
     },
 )
-GetMetricDataV2RequestRequestTypeDef = TypedDict(
-    "GetMetricDataV2RequestRequestTypeDef",
+TaskTemplateDefaultsTypeDef = TypedDict(
+    "TaskTemplateDefaultsTypeDef",
     {
-        "ResourceArn": str,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-        "Filters": Sequence[FilterV2TypeDef],
-        "Metrics": Sequence[MetricV2TypeDef],
-        "Interval": NotRequired[IntervalDetailsTypeDef],
-        "Groupings": NotRequired[Sequence[str]],
-        "NextToken": NotRequired[str],
-        "MaxResults": NotRequired[int],
+        "DefaultFieldValues": NotRequired[Sequence[TaskTemplateDefaultFieldValueTypeDef]],
     },
 )
+TaskTemplateFieldUnionTypeDef = Union[TaskTemplateFieldTypeDef, TaskTemplateFieldOutputTypeDef]
 MetricDataV2TypeDef = TypedDict(
     "MetricDataV2TypeDef",
     {
-        "Metric": NotRequired[MetricV2TypeDef],
+        "Metric": NotRequired[MetricV2OutputTypeDef],
         "Value": NotRequired[float],
     },
 )
+MetricV2UnionTypeDef = Union[MetricV2TypeDef, MetricV2OutputTypeDef]
 SendChatIntegrationEventRequestRequestTypeDef = TypedDict(
     "SendChatIntegrationEventRequestRequestTypeDef",
     {
         "SourceId": str,
         "DestinationId": str,
         "Event": ChatEventTypeDef,
         "Subtype": NotRequired[str],
@@ -6179,21 +6468,28 @@
 )
 ChatParticipantRoleConfigTypeDef = TypedDict(
     "ChatParticipantRoleConfigTypeDef",
     {
         "ParticipantTimerConfigList": Sequence[ParticipantTimerConfigurationTypeDef],
     },
 )
-SearchPredefinedAttributesResponsePaginatorTypeDef = TypedDict(
-    "SearchPredefinedAttributesResponsePaginatorTypeDef",
+DescribePredefinedAttributeResponseTypeDef = TypedDict(
+    "DescribePredefinedAttributeResponseTypeDef",
+    {
+        "PredefinedAttribute": PredefinedAttributeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+SearchPredefinedAttributesResponseTypeDef = TypedDict(
+    "SearchPredefinedAttributesResponseTypeDef",
     {
-        "PredefinedAttributes": List[PredefinedAttributePaginatorTypeDef],
-        "NextToken": str,
+        "PredefinedAttributes": List[PredefinedAttributeTypeDef],
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateQuickConnectRequestRequestTypeDef = TypedDict(
     "CreateQuickConnectRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
@@ -6251,16 +6547,16 @@
         "TranscriptItems": List[RealTimeContactAnalysisTranscriptItemWithContentTypeDef],
     },
 )
 ListContactReferencesResponseTypeDef = TypedDict(
     "ListContactReferencesResponseTypeDef",
     {
         "ReferenceSummaryList": List[ReferenceSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchResourceTagsRequestRequestTypeDef = TypedDict(
     "SearchResourceTagsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceTypes": NotRequired[Sequence[str]],
@@ -6277,22 +6573,23 @@
         "SearchCriteria": NotRequired[ResourceTagsSearchCriteriaTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 GetTrafficDistributionResponseTypeDef = TypedDict(
     "GetTrafficDistributionResponseTypeDef",
     {
-        "TelephonyConfig": TelephonyConfigTypeDef,
+        "TelephonyConfig": TelephonyConfigOutputTypeDef,
         "Id": str,
         "Arn": str,
-        "SignInConfig": SignInConfigTypeDef,
-        "AgentConfig": AgentConfigTypeDef,
+        "SignInConfig": SignInConfigOutputTypeDef,
+        "AgentConfig": AgentConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SignInConfigUnionTypeDef = Union[SignInConfigTypeDef, SignInConfigOutputTypeDef]
 UpdateTrafficDistributionRequestRequestTypeDef = TypedDict(
     "UpdateTrafficDistributionRequestRequestTypeDef",
     {
         "Id": str,
         "TelephonyConfig": NotRequired[TelephonyConfigTypeDef],
         "SignInConfig": NotRequired[SignInConfigTypeDef],
         "AgentConfig": NotRequired[AgentConfigTypeDef],
@@ -6304,17 +6601,17 @@
         "Transcript": NotRequired[TranscriptTypeDef],
     },
 )
 SearchUsersResponseTypeDef = TypedDict(
     "SearchUsersResponseTypeDef",
     {
         "Users": List[UserSearchSummaryTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateViewResponseTypeDef = TypedDict(
     "CreateViewResponseTypeDef",
     {
         "View": ViewTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6476,27 +6773,27 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchRoutingProfilesResponseTypeDef = TypedDict(
     "SearchRoutingProfilesResponseTypeDef",
     {
         "RoutingProfiles": List[RoutingProfileTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetCurrentMetricDataResponseTypeDef = TypedDict(
     "GetCurrentMetricDataResponseTypeDef",
     {
-        "NextToken": str,
         "MetricResults": List[CurrentMetricResultTypeDef],
         "DataSnapshotTime": datetime,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
@@ -6510,27 +6807,35 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInstanceStorageConfigsResponseTypeDef = TypedDict(
     "ListInstanceStorageConfigsResponseTypeDef",
     {
         "StorageConfigs": List[InstanceStorageConfigTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "UpdateInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AssociationId": str,
         "ResourceType": InstanceStorageResourceTypeType,
         "StorageConfig": InstanceStorageConfigTypeDef,
     },
 )
+EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
+    {
+        "Options": List[EvaluationFormSingleSelectQuestionOptionTypeDef],
+        "DisplayAs": NotRequired[EvaluationFormSingleSelectQuestionDisplayModeType],
+        "Automation": NotRequired[EvaluationFormSingleSelectQuestionAutomationOutputTypeDef],
+    },
+)
 EvaluationFormSingleSelectQuestionPropertiesTypeDef = TypedDict(
     "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
     {
         "Options": Sequence[EvaluationFormSingleSelectQuestionOptionTypeDef],
         "DisplayAs": NotRequired[EvaluationFormSingleSelectQuestionDisplayModeType],
         "Automation": NotRequired[EvaluationFormSingleSelectQuestionAutomationTypeDef],
     },
@@ -6539,14 +6844,28 @@
     "DescribeContactEvaluationResponseTypeDef",
     {
         "Evaluation": EvaluationTypeDef,
         "EvaluationForm": EvaluationFormContentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "ActionType": ActionTypeType,
+        "TaskAction": NotRequired[TaskActionDefinitionOutputTypeDef],
+        "EventBridgeAction": NotRequired[EventBridgeActionDefinitionTypeDef],
+        "AssignContactCategoryAction": NotRequired[Dict[str, Any]],
+        "SendNotificationAction": NotRequired[SendNotificationActionDefinitionOutputTypeDef],
+        "CreateCaseAction": NotRequired[CreateCaseActionDefinitionOutputTypeDef],
+        "UpdateCaseAction": NotRequired[UpdateCaseActionDefinitionOutputTypeDef],
+        "EndAssociatedTasksAction": NotRequired[Dict[str, Any]],
+        "SubmitAutoEvaluationAction": NotRequired[SubmitAutoEvaluationActionDefinitionTypeDef],
+    },
+)
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "ActionType": ActionTypeType,
         "TaskAction": NotRequired[TaskActionDefinitionTypeDef],
         "EventBridgeAction": NotRequired[EventBridgeActionDefinitionTypeDef],
         "AssignContactCategoryAction": NotRequired[Mapping[str, Any]],
@@ -6556,18 +6875,18 @@
         "EndAssociatedTasksAction": NotRequired[Mapping[str, Any]],
         "SubmitAutoEvaluationAction": NotRequired[SubmitAutoEvaluationActionDefinitionTypeDef],
     },
 )
 GetCurrentUserDataResponseTypeDef = TypedDict(
     "GetCurrentUserDataResponseTypeDef",
     {
-        "NextToken": str,
         "UserDataList": List[UserDataTypeDef],
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeUserHierarchyGroupResponseTypeDef = TypedDict(
     "DescribeUserHierarchyGroupResponseTypeDef",
     {
         "HierarchyGroup": HierarchyGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6587,92 +6906,112 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchHoursOfOperationsResponseTypeDef = TypedDict(
     "SearchHoursOfOperationsResponseTypeDef",
     {
         "HoursOfOperations": List[HoursOfOperationTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-CreateTaskTemplateRequestRequestTypeDef = TypedDict(
-    "CreateTaskTemplateRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-        "Fields": Sequence[TaskTemplateFieldTypeDef],
-        "Description": NotRequired[str],
-        "ContactFlowId": NotRequired[str],
-        "Constraints": NotRequired[TaskTemplateConstraintsTypeDef],
-        "Defaults": NotRequired[TaskTemplateDefaultsTypeDef],
-        "Status": NotRequired[TaskTemplateStatusType],
-        "ClientToken": NotRequired[str],
-    },
-)
+TaskTemplateConstraintsUnionTypeDef = Union[
+    TaskTemplateConstraintsTypeDef, TaskTemplateConstraintsOutputTypeDef
+]
 GetTaskTemplateResponseTypeDef = TypedDict(
     "GetTaskTemplateResponseTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
-        "Constraints": TaskTemplateConstraintsTypeDef,
-        "Defaults": TaskTemplateDefaultsTypeDef,
-        "Fields": List[TaskTemplateFieldTypeDef],
+        "Constraints": TaskTemplateConstraintsOutputTypeDef,
+        "Defaults": TaskTemplateDefaultsOutputTypeDef,
+        "Fields": List[TaskTemplateFieldOutputTypeDef],
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateTaskTemplateRequestRequestTypeDef = TypedDict(
-    "UpdateTaskTemplateRequestRequestTypeDef",
-    {
-        "TaskTemplateId": str,
-        "InstanceId": str,
-        "Name": NotRequired[str],
-        "Description": NotRequired[str],
-        "ContactFlowId": NotRequired[str],
-        "Constraints": NotRequired[TaskTemplateConstraintsTypeDef],
-        "Defaults": NotRequired[TaskTemplateDefaultsTypeDef],
-        "Status": NotRequired[TaskTemplateStatusType],
-        "Fields": NotRequired[Sequence[TaskTemplateFieldTypeDef]],
-    },
-)
 UpdateTaskTemplateResponseTypeDef = TypedDict(
     "UpdateTaskTemplateResponseTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
-        "Constraints": TaskTemplateConstraintsTypeDef,
-        "Defaults": TaskTemplateDefaultsTypeDef,
-        "Fields": List[TaskTemplateFieldTypeDef],
+        "Constraints": TaskTemplateConstraintsOutputTypeDef,
+        "Defaults": TaskTemplateDefaultsOutputTypeDef,
+        "Fields": List[TaskTemplateFieldOutputTypeDef],
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+TaskTemplateDefaultsUnionTypeDef = Union[
+    TaskTemplateDefaultsTypeDef, TaskTemplateDefaultsOutputTypeDef
+]
+CreateTaskTemplateRequestRequestTypeDef = TypedDict(
+    "CreateTaskTemplateRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "Fields": Sequence[TaskTemplateFieldUnionTypeDef],
+        "Description": NotRequired[str],
+        "ContactFlowId": NotRequired[str],
+        "Constraints": NotRequired[TaskTemplateConstraintsTypeDef],
+        "Defaults": NotRequired[TaskTemplateDefaultsTypeDef],
+        "Status": NotRequired[TaskTemplateStatusType],
+        "ClientToken": NotRequired[str],
+    },
+)
+UpdateTaskTemplateRequestRequestTypeDef = TypedDict(
+    "UpdateTaskTemplateRequestRequestTypeDef",
+    {
+        "TaskTemplateId": str,
+        "InstanceId": str,
+        "Name": NotRequired[str],
+        "Description": NotRequired[str],
+        "ContactFlowId": NotRequired[str],
+        "Constraints": NotRequired[TaskTemplateConstraintsTypeDef],
+        "Defaults": NotRequired[TaskTemplateDefaultsTypeDef],
+        "Status": NotRequired[TaskTemplateStatusType],
+        "Fields": NotRequired[Sequence[TaskTemplateFieldUnionTypeDef]],
+    },
+)
 MetricResultV2TypeDef = TypedDict(
     "MetricResultV2TypeDef",
     {
         "Dimensions": NotRequired[Dict[str, str]],
         "MetricInterval": NotRequired[MetricIntervalTypeDef],
         "Collections": NotRequired[List[MetricDataV2TypeDef]],
     },
 )
+GetMetricDataV2RequestRequestTypeDef = TypedDict(
+    "GetMetricDataV2RequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Filters": Sequence[FilterV2TypeDef],
+        "Metrics": Sequence[MetricV2UnionTypeDef],
+        "Interval": NotRequired[IntervalDetailsTypeDef],
+        "Groupings": NotRequired[Sequence[str]],
+        "NextToken": NotRequired[str],
+        "MaxResults": NotRequired[int],
+    },
+)
 UpdateParticipantRoleConfigChannelInfoTypeDef = TypedDict(
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     {
         "Chat": NotRequired[ChatParticipantRoleConfigTypeDef],
     },
 )
 DescribeQuickConnectResponseTypeDef = TypedDict(
@@ -6682,17 +7021,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchQuickConnectsResponseTypeDef = TypedDict(
     "SearchQuickConnectsResponseTypeDef",
     {
         "QuickConnects": List[QuickConnectTypeDef],
-        "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RealTimeContactAnalysisCategoryDetailsTypeDef = TypedDict(
     "RealTimeContactAnalysisCategoryDetailsTypeDef",
     {
         "PointsOfInterest": List[RealTimeContactAnalysisPointOfInterestTypeDef],
     },
@@ -6740,74 +7079,59 @@
         "ConnectionData": ConnectionDataTypeDef,
         "ContactId": str,
         "ParticipantId": str,
         "ParticipantToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+EvaluationFormQuestionTypePropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
+    {
+        "Numeric": NotRequired[EvaluationFormNumericQuestionPropertiesOutputTypeDef],
+        "SingleSelect": NotRequired[EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef],
+    },
+)
 EvaluationFormQuestionTypePropertiesTypeDef = TypedDict(
     "EvaluationFormQuestionTypePropertiesTypeDef",
     {
         "Numeric": NotRequired[EvaluationFormNumericQuestionPropertiesTypeDef],
         "SingleSelect": NotRequired[EvaluationFormSingleSelectQuestionPropertiesTypeDef],
     },
 )
-CreateRuleRequestRequestTypeDef = TypedDict(
-    "CreateRuleRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-        "TriggerEventSource": RuleTriggerEventSourceTypeDef,
-        "Function": str,
-        "Actions": Sequence[RuleActionTypeDef],
-        "PublishStatus": RulePublishStatusType,
-        "ClientToken": NotRequired[str],
-    },
-)
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "Name": str,
         "RuleId": str,
         "RuleArn": str,
         "TriggerEventSource": RuleTriggerEventSourceTypeDef,
         "Function": str,
-        "Actions": List[RuleActionTypeDef],
+        "Actions": List[RuleActionOutputTypeDef],
         "PublishStatus": RulePublishStatusType,
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "LastUpdatedBy": str,
         "Tags": NotRequired[Dict[str, str]],
     },
 )
-UpdateRuleRequestRequestTypeDef = TypedDict(
-    "UpdateRuleRequestRequestTypeDef",
-    {
-        "RuleId": str,
-        "InstanceId": str,
-        "Name": str,
-        "Function": str,
-        "Actions": Sequence[RuleActionTypeDef],
-        "PublishStatus": RulePublishStatusType,
-    },
-)
+RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
 GetMetricDataResponseTypeDef = TypedDict(
     "GetMetricDataResponseTypeDef",
     {
-        "NextToken": str,
         "MetricResults": List[HistoricalMetricResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetMetricDataV2ResponseTypeDef = TypedDict(
     "GetMetricDataV2ResponseTypeDef",
     {
-        "NextToken": str,
         "MetricResults": List[MetricResultV2TypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateParticipantRoleConfigRequestRequestTypeDef = TypedDict(
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
@@ -6837,14 +7161,26 @@
         "InstanceId": str,
         "TimeRange": SearchContactsTimeRangeTypeDef,
         "SearchCriteria": NotRequired[SearchCriteriaTypeDef],
         "Sort": NotRequired[SortTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+EvaluationFormQuestionOutputTypeDef = TypedDict(
+    "EvaluationFormQuestionOutputTypeDef",
+    {
+        "Title": str,
+        "RefId": str,
+        "QuestionType": EvaluationFormQuestionTypeType,
+        "Instructions": NotRequired[str],
+        "NotApplicableEnabled": NotRequired[bool],
+        "QuestionTypeProperties": NotRequired[EvaluationFormQuestionTypePropertiesOutputTypeDef],
+        "Weight": NotRequired[float],
+    },
+)
 EvaluationFormQuestionTypeDef = TypedDict(
     "EvaluationFormQuestionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "QuestionType": EvaluationFormQuestionTypeType,
         "Instructions": NotRequired[str],
@@ -6856,34 +7192,64 @@
 DescribeRuleResponseTypeDef = TypedDict(
     "DescribeRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateRuleRequestRequestTypeDef = TypedDict(
+    "CreateRuleRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "TriggerEventSource": RuleTriggerEventSourceTypeDef,
+        "Function": str,
+        "Actions": Sequence[RuleActionUnionTypeDef],
+        "PublishStatus": RulePublishStatusType,
+        "ClientToken": NotRequired[str],
+    },
+)
+UpdateRuleRequestRequestTypeDef = TypedDict(
+    "UpdateRuleRequestRequestTypeDef",
+    {
+        "RuleId": str,
+        "InstanceId": str,
+        "Name": str,
+        "Function": str,
+        "Actions": Sequence[RuleActionUnionTypeDef],
+        "PublishStatus": RulePublishStatusType,
+    },
+)
 RealtimeContactAnalysisSegmentTypeDef = TypedDict(
     "RealtimeContactAnalysisSegmentTypeDef",
     {
         "Transcript": NotRequired[RealTimeContactAnalysisSegmentTranscriptTypeDef],
         "Categories": NotRequired[RealTimeContactAnalysisSegmentCategoriesTypeDef],
         "Issues": NotRequired[RealTimeContactAnalysisSegmentIssuesTypeDef],
         "Event": NotRequired[RealTimeContactAnalysisSegmentEventTypeDef],
         "Attachments": NotRequired[RealTimeContactAnalysisSegmentAttachmentsTypeDef],
     },
 )
+EvaluationFormItemOutputTypeDef = TypedDict(
+    "EvaluationFormItemOutputTypeDef",
+    {
+        "Section": NotRequired[Dict[str, Any]],
+        "Question": NotRequired[EvaluationFormQuestionOutputTypeDef],
+    },
+)
 EvaluationFormItemTypeDef = TypedDict(
     "EvaluationFormItemTypeDef",
     {
         "Section": NotRequired[Dict[str, Any]],
         "Question": NotRequired[EvaluationFormQuestionTypeDef],
     },
 )
 ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef = TypedDict(
     "ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef",
     {
         "Channel": RealTimeContactAnalysisSupportedChannelType,
         "Status": RealTimeContactAnalysisStatusType,
         "Segments": List[RealtimeContactAnalysisSegmentTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/PKG-INFO` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.34.82
-Summary: Type annotations for boto3.Connect 1.34.82 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.98
+Summary: Type annotations for boto3.Connect 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connect)](https://pepy.tech/project/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/SOURCES.txt` & `mypy_boto3_connect-1.34.98/mypy_boto3_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.82/setup.py` & `mypy_boto3_connect-1.34.98/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connect",
-    version="1.34.82",
+    version="1.34.98",
     packages=["mypy_boto3_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Connect 1.34.82 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Connect 1.34.98 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

