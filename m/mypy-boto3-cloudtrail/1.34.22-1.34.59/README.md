# Comparing `tmp/mypy-boto3-cloudtrail-1.34.22.tar.gz` & `tmp/mypy-boto3-cloudtrail-1.34.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudtrail-1.34.22.tar", last modified: Thu Jan 18 20:32:38 2024, max compression
+gzip compressed data, was "mypy-boto3-cloudtrail-1.34.59.tar", last modified: Fri Mar  8 20:21:19 2024, max compression
```

## Comparing `mypy-boto3-cloudtrail-1.34.22.tar` & `mypy-boto3-cloudtrail-1.34.59.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 20:32:38.478007 mypy-boto3-cloudtrail-1.34.22/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 20:32:10.000000 mypy-boto3-cloudtrail-1.34.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-01-18 20:32:38.478007 mypy-boto3-cloudtrail-1.34.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11838 2024-01-18 20:32:10.000000 mypy-boto3-cloudtrail-1.34.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 20:32:38.474007 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-18 20:32:10.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-18 20:32:10.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-18 20:32:10.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41913 2024-01-18 20:32:11.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    41910 2024-01-18 20:32:11.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-01-18 20:32:12.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-01-18 20:32:12.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-01-18 20:32:11.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-01-18 20:32:11.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 20:32:10.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39292 2024-01-18 20:32:12.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    39292 2024-01-18 20:32:12.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-18 20:32:10.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 20:32:38.478007 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-01-18 20:32:38.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 20:32:38.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 20:32:38.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 20:32:38.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 20:32:38.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 20:32:38.000000 mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 20:32:38.478007 mypy-boto3-cloudtrail-1.34.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 20:32:10.000000 mypy-boto3-cloudtrail-1.34.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:19.954139 mypy-boto3-cloudtrail-1.34.59/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-08 20:20:55.000000 mypy-boto3-cloudtrail-1.34.59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-03-08 20:21:19.954139 mypy-boto3-cloudtrail-1.34.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11838 2024-03-08 20:20:55.000000 mypy-boto3-cloudtrail-1.34.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:19.950139 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-08 20:20:55.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-08 20:20:55.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-08 20:20:55.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41913 2024-03-08 20:20:56.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41910 2024-03-08 20:20:55.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-03-08 20:20:56.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-03-08 20:20:56.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-03-08 20:20:56.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-03-08 20:20:56.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:20:55.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    39305 2024-03-08 20:20:57.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39305 2024-03-08 20:20:57.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-08 20:20:55.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:21:19.954139 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-03-08 20:21:19.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-08 20:21:19.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:21:19.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:21:19.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-08 20:21:19.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-08 20:21:19.000000 mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 20:21:19.954139 mypy-boto3-cloudtrail-1.34.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-08 20:20:55.000000 mypy-boto3-cloudtrail-1.34.59/setup.py
```

### Comparing `mypy-boto3-cloudtrail-1.34.22/LICENSE` & `mypy-boto3-cloudtrail-1.34.59/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.34.22/PKG-INFO` & `mypy-boto3-cloudtrail-1.34.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.34.22
-Summary: Type annotations for boto3.CloudTrail 1.34.22 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.59
+Summary: Type annotations for boto3.CloudTrail 1.34.59 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.34.22](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.34.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudtrail-1.34.22/README.md` & `mypy-boto3-cloudtrail-1.34.59/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.34.22](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.34.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/__init__.py` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/__init__.pyi` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/__main__.py` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudTrail 1.34.22\nVersion:         1.34.22\nBuilder version:"
-        " 7.23.1\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.CloudTrail 1.34.59\n"
+        "Version:         1.34.59\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.22")
+    print("1.34.59")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/client.py` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/client.pyi` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/literals.py` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -132,14 +133,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
```

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/literals.pyi` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -132,14 +133,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
```

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/paginator.py` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/paginator.pyi` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/type_defs.py` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,18 +194,18 @@
         "EventDataStore": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "ChannelArn": NotRequired[str],
         "Name": NotRequired[str],
```

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail/type_defs.pyi` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -194,18 +194,18 @@
         "EventDataStore": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "ChannelArn": NotRequired[str],
         "Name": NotRequired[str],
```

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail.egg-info/PKG-INFO` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.34.22
-Summary: Type annotations for boto3.CloudTrail 1.34.22 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.59
+Summary: Type annotations for boto3.CloudTrail 1.34.59 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.34.22](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.34.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudtrail-1.34.22/mypy_boto3_cloudtrail.egg-info/SOURCES.txt` & `mypy-boto3-cloudtrail-1.34.59/mypy_boto3_cloudtrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.34.22/setup.py` & `mypy-boto3-cloudtrail-1.34.59/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudtrail",
-    version="1.34.22",
+    version="1.34.59",
     packages=["mypy_boto3_cloudtrail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.CloudTrail 1.34.22 service generated with mypy-boto3-builder"
-        " 7.23.1"
-    ),
+    description="Type annotations for boto3.CloudTrail 1.34.59 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

