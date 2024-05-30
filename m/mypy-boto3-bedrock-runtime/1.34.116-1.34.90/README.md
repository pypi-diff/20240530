# Comparing `tmp/mypy_boto3_bedrock_runtime-1.34.116.tar.gz` & `tmp/mypy_boto3_bedrock_runtime-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_bedrock_runtime-1.34.116.tar", last modified: Thu May 30 20:33:06 2024, max compression
+gzip compressed data, was "mypy_boto3_bedrock_runtime-1.34.90.tar", last modified: Tue Apr 23 19:34:20 2024, max compression
```

## Comparing `mypy_boto3_bedrock_runtime-1.34.116.tar` & `mypy_boto3_bedrock_runtime-1.34.90.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:33:06.836227 mypy_boto3_bedrock_runtime-1.34.116/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 20:32:07.000000 mypy_boto3_bedrock_runtime-1.34.116/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-05-30 20:33:06.836227 mypy_boto3_bedrock_runtime-1.34.116/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-30 20:32:07.000000 mypy_boto3_bedrock_runtime-1.34.116/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:33:06.836227 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 20:32:07.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 20:32:07.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-30 20:32:07.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-30 20:32:07.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-30 20:32:07.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-30 20:32:08.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-30 20:32:08.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:32:07.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-05-30 20:32:08.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-05-30 20:32:08.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 20:32:07.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:33:06.836227 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-05-30 20:33:06.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-30 20:33:06.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 20:33:06.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 20:33:06.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 20:33:06.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 20:33:06.000000 mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 20:33:06.836227 mypy_boto3_bedrock_runtime-1.34.116/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-30 20:32:07.000000 mypy_boto3_bedrock_runtime-1.34.116/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.312567 mypy_boto3_bedrock_runtime-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-04-23 19:34:20.312567 mypy_boto3_bedrock_runtime-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.312567 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.312567 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:20.312567 mypy_boto3_bedrock_runtime-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/setup.py
```

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/LICENSE` & `mypy_boto3_bedrock_runtime-1.34.90/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/PKG-INFO` & `mypy_boto3_bedrock_runtime-1.34.90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-runtime
-Version: 1.34.116
-Summary: Type annotations for boto3.BedrockRuntime 1.34.116 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.90
+Summary: Type annotations for boto3.BedrockRuntime 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-runtime)](https://pepy.tech/project/mypy-boto3-bedrock-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BedrockRuntime 1.34.116](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
+[boto3.BedrockRuntime 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-bedrock-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,18 +280,18 @@
 `mypy_boto3_bedrock_runtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `BedrockRuntime` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/literals/).
 
 ```python
-from mypy_boto3_bedrock_runtime.literals import ConversationRoleType
+from mypy_boto3_bedrock_runtime.literals import TraceType
 
 
-def check_value(value: ConversationRoleType) -> bool: ...
+def check_value(value: TraceType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_bedrock_runtime.type_defs` module contains structures and shapes
```

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/README.md` & `mypy_boto3_bedrock_runtime-1.34.90/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-runtime)](https://pepy.tech/project/mypy-boto3-bedrock-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BedrockRuntime 1.34.116](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
+[boto3.BedrockRuntime 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-bedrock-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -247,18 +247,18 @@
 `mypy_boto3_bedrock_runtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `BedrockRuntime` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/literals/).
 
 ```python
-from mypy_boto3_bedrock_runtime.literals import ConversationRoleType
+from mypy_boto3_bedrock_runtime.literals import TraceType
 
 
-def check_value(value: ConversationRoleType) -> bool: ...
+def check_value(value: TraceType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_bedrock_runtime.type_defs` module contains structures and shapes
```

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/__main__.py` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BedrockRuntime 1.34.116\n"
-        "Version:         1.34.116\n"
-        "Builder version: 7.24.0\n"
+        "Type annotations for boto3.BedrockRuntime 1.34.90\n"
+        "Version:         1.34.90\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.116")
+    print("1.34.90")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/client.py` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,29 +10,23 @@
     from mypy_boto3_bedrock_runtime.client import BedrockRuntimeClient
 
     session = Session()
     client: BedrockRuntimeClient = session.client("bedrock-runtime")
     ```
 """
 
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import TraceType
 from .type_defs import (
     BlobTypeDef,
-    ConverseResponseTypeDef,
-    ConverseStreamResponseTypeDef,
-    InferenceConfigurationTypeDef,
     InvokeModelResponseTypeDef,
     InvokeModelWithResponseStreamResponseTypeDef,
-    MessageUnionTypeDef,
-    SystemContentBlockTypeDef,
-    ToolConfigurationTypeDef,
 )
 
 __all__ = ("BedrockRuntimeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
@@ -85,52 +79,14 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#close)
         """
 
-    def converse(
-        self,
-        *,
-        modelId: str,
-        messages: Sequence[MessageUnionTypeDef],
-        system: Sequence[SystemContentBlockTypeDef] = ...,
-        inferenceConfig: InferenceConfigurationTypeDef = ...,
-        toolConfig: ToolConfigurationTypeDef = ...,
-        additionalModelRequestFields: Mapping[str, Any] = ...,
-        additionalModelResponseFieldPaths: Sequence[str] = ...,
-    ) -> ConverseResponseTypeDef:
-        """
-        Sends messages to the specified Amazon Bedrock model.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.converse)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#converse)
-        """
-
-    def converse_stream(
-        self,
-        *,
-        modelId: str,
-        messages: Sequence[MessageUnionTypeDef],
-        system: Sequence[SystemContentBlockTypeDef] = ...,
-        inferenceConfig: InferenceConfigurationTypeDef = ...,
-        toolConfig: ToolConfigurationTypeDef = ...,
-        additionalModelRequestFields: Mapping[str, Any] = ...,
-        additionalModelResponseFieldPaths: Sequence[str] = ...,
-    ) -> ConverseStreamResponseTypeDef:
-        """
-        Sends messages to the specified Amazon Bedrock model and returns the response
-        in a
-        stream.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.converse_stream)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#converse_stream)
-        """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
```

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/client.pyi` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/client.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -10,29 +10,23 @@
     from mypy_boto3_bedrock_runtime.client import BedrockRuntimeClient
 
     session = Session()
     client: BedrockRuntimeClient = session.client("bedrock-runtime")
     ```
 """
 
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import TraceType
 from .type_defs import (
     BlobTypeDef,
-    ConverseResponseTypeDef,
-    ConverseStreamResponseTypeDef,
-    InferenceConfigurationTypeDef,
     InvokeModelResponseTypeDef,
     InvokeModelWithResponseStreamResponseTypeDef,
-    MessageUnionTypeDef,
-    SystemContentBlockTypeDef,
-    ToolConfigurationTypeDef,
 )
 
 __all__ = ("BedrockRuntimeClient",)
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
@@ -82,52 +76,14 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#close)
         """
 
-    def converse(
-        self,
-        *,
-        modelId: str,
-        messages: Sequence[MessageUnionTypeDef],
-        system: Sequence[SystemContentBlockTypeDef] = ...,
-        inferenceConfig: InferenceConfigurationTypeDef = ...,
-        toolConfig: ToolConfigurationTypeDef = ...,
-        additionalModelRequestFields: Mapping[str, Any] = ...,
-        additionalModelResponseFieldPaths: Sequence[str] = ...,
-    ) -> ConverseResponseTypeDef:
-        """
-        Sends messages to the specified Amazon Bedrock model.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.converse)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#converse)
-        """
-
-    def converse_stream(
-        self,
-        *,
-        modelId: str,
-        messages: Sequence[MessageUnionTypeDef],
-        system: Sequence[SystemContentBlockTypeDef] = ...,
-        inferenceConfig: InferenceConfigurationTypeDef = ...,
-        toolConfig: ToolConfigurationTypeDef = ...,
-        additionalModelRequestFields: Mapping[str, Any] = ...,
-        additionalModelResponseFieldPaths: Sequence[str] = ...,
-    ) -> ConverseStreamResponseTypeDef:
-        """
-        Sends messages to the specified Amazon Bedrock model and returns the response
-        in a
-        stream.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.converse_stream)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#converse_stream)
-        """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
```

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/literals.py` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/literals.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,42 +2,29 @@
 Type annotations for bedrock-runtime service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_bedrock_runtime.literals import ConversationRoleType
+    from mypy_boto3_bedrock_runtime.literals import TraceType
 
-    data: ConversationRoleType = "assistant"
+    data: TraceType = "DISABLED"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-__all__ = (
-    "ConversationRoleType",
-    "ImageFormatType",
-    "StopReasonType",
-    "ToolResultStatusType",
-    "TraceType",
-    "BedrockRuntimeServiceName",
-    "ServiceName",
-    "ResourceServiceName",
-)
+__all__ = ("TraceType", "BedrockRuntimeServiceName", "ServiceName", "ResourceServiceName")
 
-ConversationRoleType = Literal["assistant", "user"]
-ImageFormatType = Literal["gif", "jpeg", "png", "webp"]
-StopReasonType = Literal["content_filtered", "end_turn", "max_tokens", "stop_sequence", "tool_use"]
-ToolResultStatusType = Literal["error", "success"]
 TraceType = Literal["DISABLED", "ENABLED"]
 BedrockRuntimeServiceName = Literal["bedrock-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -253,15 +240,14 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
-    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
```

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime/literals.pyi` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/literals.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,42 +2,29 @@
 Type annotations for bedrock-runtime service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_bedrock_runtime.literals import ConversationRoleType
+    from mypy_boto3_bedrock_runtime.literals import TraceType
 
-    data: ConversationRoleType = "assistant"
+    data: TraceType = "DISABLED"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-__all__ = (
-    "ConversationRoleType",
-    "ImageFormatType",
-    "StopReasonType",
-    "ToolResultStatusType",
-    "TraceType",
-    "BedrockRuntimeServiceName",
-    "ServiceName",
-    "ResourceServiceName",
-)
+__all__ = ("TraceType", "BedrockRuntimeServiceName", "ServiceName", "ResourceServiceName")
 
-ConversationRoleType = Literal["assistant", "user"]
-ImageFormatType = Literal["gif", "jpeg", "png", "webp"]
-StopReasonType = Literal["content_filtered", "end_turn", "max_tokens", "stop_sequence", "tool_use"]
-ToolResultStatusType = Literal["error", "success"]
 TraceType = Literal["DISABLED", "ENABLED"]
 BedrockRuntimeServiceName = Literal["bedrock-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -253,15 +240,14 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
-    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
```

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime.egg-info/PKG-INFO` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-runtime
-Version: 1.34.116
-Summary: Type annotations for boto3.BedrockRuntime 1.34.116 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.90
+Summary: Type annotations for boto3.BedrockRuntime 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-runtime)](https://pepy.tech/project/mypy-boto3-bedrock-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BedrockRuntime 1.34.116](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
+[boto3.BedrockRuntime 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-bedrock-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,18 +280,18 @@
 `mypy_boto3_bedrock_runtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `BedrockRuntime` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/literals/).
 
 ```python
-from mypy_boto3_bedrock_runtime.literals import ConversationRoleType
+from mypy_boto3_bedrock_runtime.literals import TraceType
 
 
-def check_value(value: ConversationRoleType) -> bool: ...
+def check_value(value: TraceType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_bedrock_runtime.type_defs` module contains structures and shapes
```

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/mypy_boto3_bedrock_runtime.egg-info/SOURCES.txt` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_runtime-1.34.116/setup.py` & `mypy_boto3_bedrock_runtime-1.34.90/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-bedrock-runtime",
-    version="1.34.116",
+    version="1.34.90",
     packages=["mypy_boto3_bedrock_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.BedrockRuntime 1.34.116 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.BedrockRuntime 1.34.90 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

