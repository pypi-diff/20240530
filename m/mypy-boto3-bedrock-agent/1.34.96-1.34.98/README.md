# Comparing `tmp/mypy_boto3_bedrock_agent-1.34.96.tar.gz` & `tmp/mypy_boto3_bedrock_agent-1.34.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_bedrock_agent-1.34.96.tar", last modified: Wed May  1 19:21:15 2024, max compression
+gzip compressed data, was "mypy_boto3_bedrock_agent-1.34.98.tar", last modified: Fri May  3 19:32:41 2024, max compression
```

## Comparing `mypy_boto3_bedrock_agent-1.34.96.tar` & `mypy_boto3_bedrock_agent-1.34.98.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.448320 mypy_boto3_bedrock_agent-1.34.96/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-05-01 19:21:15.448320 mypy_boto3_bedrock_agent-1.34.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.448320 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34440 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34437 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-05-01 19:19:59.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    45674 2024-05-01 19:19:59.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    45674 2024-05-01 19:19:59.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.448320 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:21:15.448320 mypy_boto3_bedrock_agent-1.34.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:41.305277 mypy_boto3_bedrock_agent-1.34.98/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-05-03 19:32:41.305277 mypy_boto3_bedrock_agent-1.34.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:41.301277 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34440 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34437 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    45788 2024-05-03 19:31:48.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45788 2024-05-03 19:31:48.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:41.301277 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-05-03 19:32:41.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-03 19:32:41.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:41.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:41.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 19:32:41.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 19:32:41.000000 mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:32:41.305277 mypy_boto3_bedrock_agent-1.34.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-03 19:31:47.000000 mypy_boto3_bedrock_agent-1.34.98/setup.py
```

### Comparing `mypy_boto3_bedrock_agent-1.34.96/LICENSE` & `mypy_boto3_bedrock_agent-1.34.98/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.96/PKG-INFO` & `mypy_boto3_bedrock_agent-1.34.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-agent
-Version: 1.34.96
-Summary: Type annotations for boto3.AgentsforBedrock 1.34.96 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.98
+Summary: Type annotations for boto3.AgentsforBedrock 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_bedrock_agent-1.34.96/README.md` & `mypy_boto3_bedrock_agent-1.34.98/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__init__.py` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__init__.pyi` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__main__.py` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AgentsforBedrock 1.34.96\n"
-        "Version:         1.34.96\n"
+        "Type annotations for boto3.AgentsforBedrock 1.34.98\n"
+        "Version:         1.34.98\n"
         "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.96")
+    print("1.34.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/client.py` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/client.pyi` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/literals.py` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/literals.pyi` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/paginator.py` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/paginator.pyi` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/type_defs.py` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,16 @@
         "updatedAt": datetime,
         "description": NotRequired[str],
     },
 )
 AgentAliasRoutingConfigurationListItemTypeDef = TypedDict(
     "AgentAliasRoutingConfigurationListItemTypeDef",
     {
-        "agentVersion": str,
+        "agentVersion": NotRequired[str],
+        "provisionedThroughput": NotRequired[str],
     },
 )
 AgentKnowledgeBaseSummaryTypeDef = TypedDict(
     "AgentKnowledgeBaseSummaryTypeDef",
     {
         "knowledgeBaseId": str,
         "knowledgeBaseState": KnowledgeBaseStateType,
@@ -1060,14 +1061,15 @@
         "agentId": str,
         "createdAt": datetime,
         "routingConfiguration": List[AgentAliasRoutingConfigurationListItemTypeDef],
         "updatedAt": datetime,
         "agentAliasHistoryEvents": NotRequired[List[AgentAliasHistoryEventTypeDef]],
         "clientToken": NotRequired[str],
         "description": NotRequired[str],
+        "failureReasons": NotRequired[List[str]],
     },
 )
 ListAgentAliasesResponseTypeDef = TypedDict(
     "ListAgentAliasesResponseTypeDef",
     {
         "agentAliasSummaries": List[AgentAliasSummaryTypeDef],
         "nextToken": str,
```

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/type_defs.pyi` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,16 @@
         "updatedAt": datetime,
         "description": NotRequired[str],
     },
 )
 AgentAliasRoutingConfigurationListItemTypeDef = TypedDict(
     "AgentAliasRoutingConfigurationListItemTypeDef",
     {
-        "agentVersion": str,
+        "agentVersion": NotRequired[str],
+        "provisionedThroughput": NotRequired[str],
     },
 )
 AgentKnowledgeBaseSummaryTypeDef = TypedDict(
     "AgentKnowledgeBaseSummaryTypeDef",
     {
         "knowledgeBaseId": str,
         "knowledgeBaseState": KnowledgeBaseStateType,
@@ -1060,14 +1061,15 @@
         "agentId": str,
         "createdAt": datetime,
         "routingConfiguration": List[AgentAliasRoutingConfigurationListItemTypeDef],
         "updatedAt": datetime,
         "agentAliasHistoryEvents": NotRequired[List[AgentAliasHistoryEventTypeDef]],
         "clientToken": NotRequired[str],
         "description": NotRequired[str],
+        "failureReasons": NotRequired[List[str]],
     },
 )
 ListAgentAliasesResponseTypeDef = TypedDict(
     "ListAgentAliasesResponseTypeDef",
     {
         "agentAliasSummaries": List[AgentAliasSummaryTypeDef],
         "nextToken": str,
```

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/PKG-INFO` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-agent
-Version: 1.34.96
-Summary: Type annotations for boto3.AgentsforBedrock 1.34.96 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.98
+Summary: Type annotations for boto3.AgentsforBedrock 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt` & `mypy_boto3_bedrock_agent-1.34.98/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.96/setup.py` & `mypy_boto3_bedrock_agent-1.34.98/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-bedrock-agent",
-    version="1.34.96",
+    version="1.34.98",
     packages=["mypy_boto3_bedrock_agent"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.AgentsforBedrock 1.34.96 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.AgentsforBedrock 1.34.98 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

