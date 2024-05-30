# Comparing `tmp/mypy_boto3_emr_serverless-1.34.85.tar.gz` & `tmp/mypy_boto3_emr_serverless-1.34.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_emr_serverless-1.34.85.tar", last modified: Tue Apr 16 19:33:14 2024, max compression
+gzip compressed data, was "mypy_boto3_emr_serverless-1.34.87.tar", last modified: Thu Apr 18 19:34:21 2024, max compression
```

## Comparing `mypy_boto3_emr_serverless-1.34.85.tar` & `mypy_boto3_emr_serverless-1.34.87.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:14.752305 mypy_boto3_emr_serverless-1.34.85/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-16 19:33:14.752305 mypy_boto3_emr_serverless-1.34.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11624 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:14.748305 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:32:49.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:14.752305 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 19:33:14.000000 mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:14.752305 mypy_boto3_emr_serverless-1.34.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-16 19:32:48.000000 mypy_boto3_emr_serverless-1.34.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:21.468631 mypy_boto3_emr_serverless-1.34.87/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-18 19:34:21.468631 mypy_boto3_emr_serverless-1.34.87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11624 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:21.468631 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-18 19:31:59.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-18 19:31:59.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-18 19:31:59.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18106 2024-04-18 19:31:59.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18106 2024-04-18 19:31:59.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:21.468631 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-18 19:34:21.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 19:34:21.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:21.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:21.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 19:34:21.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 19:34:21.000000 mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:34:21.468631 mypy_boto3_emr_serverless-1.34.87/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-18 19:31:58.000000 mypy_boto3_emr_serverless-1.34.87/setup.py
```

### Comparing `mypy_boto3_emr_serverless-1.34.85/LICENSE` & `mypy_boto3_emr_serverless-1.34.87/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_emr_serverless-1.34.85/PKG-INFO` & `mypy_boto3_emr_serverless-1.34.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.34.85
-Summary: Type annotations for boto3.EMRServerless 1.34.85 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.87
+Summary: Type annotations for boto3.EMRServerless 1.34.87 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_emr_serverless-1.34.85/README.md` & `mypy_boto3_emr_serverless-1.34.87/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__init__.py` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__init__.pyi` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/__main__.py` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRServerless 1.34.85\n"
-        "Version:         1.34.85\n"
+        "Type annotations for boto3.EMRServerless 1.34.87\n"
+        "Version:         1.34.87\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.85")
+    print("1.34.87")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/client.py` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/client.pyi` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/literals.py` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/literals.pyi` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/paginator.py` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/paginator.pyi` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/type_defs.py` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
     "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
+    "PrometheusMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "WorkerTypeSpecificationTypeDef",
     "CancelJobRunResponseTypeDef",
@@ -286,14 +287,20 @@
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": NotRequired[bool],
         "encryptionKeyArn": NotRequired[str],
     },
 )
+PrometheusMonitoringConfigurationTypeDef = TypedDict(
+    "PrometheusMonitoringConfigurationTypeDef",
+    {
+        "remoteWriteUrl": NotRequired[str],
+    },
+)
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": NotRequired[str],
         "encryptionKeyArn": NotRequired[str],
     },
 )
@@ -437,14 +444,15 @@
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": NotRequired[S3MonitoringConfigurationTypeDef],
         "managedPersistenceMonitoringConfiguration": NotRequired[
             ManagedPersistenceMonitoringConfigurationTypeDef
         ],
         "cloudWatchLoggingConfiguration": NotRequired[CloudWatchLoggingConfigurationTypeDef],
+        "prometheusMonitoringConfiguration": NotRequired[PrometheusMonitoringConfigurationTypeDef],
     },
 )
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "applicationId": str,
         "arn": str,
```

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless/type_defs.pyi` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
     "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
+    "PrometheusMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "WorkerTypeSpecificationTypeDef",
     "CancelJobRunResponseTypeDef",
@@ -286,14 +287,20 @@
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": NotRequired[bool],
         "encryptionKeyArn": NotRequired[str],
     },
 )
+PrometheusMonitoringConfigurationTypeDef = TypedDict(
+    "PrometheusMonitoringConfigurationTypeDef",
+    {
+        "remoteWriteUrl": NotRequired[str],
+    },
+)
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": NotRequired[str],
         "encryptionKeyArn": NotRequired[str],
     },
 )
@@ -437,14 +444,15 @@
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": NotRequired[S3MonitoringConfigurationTypeDef],
         "managedPersistenceMonitoringConfiguration": NotRequired[
             ManagedPersistenceMonitoringConfigurationTypeDef
         ],
         "cloudWatchLoggingConfiguration": NotRequired[CloudWatchLoggingConfigurationTypeDef],
+        "prometheusMonitoringConfiguration": NotRequired[PrometheusMonitoringConfigurationTypeDef],
     },
 )
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "applicationId": str,
         "arn": str,
```

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/PKG-INFO` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.34.85
-Summary: Type annotations for boto3.EMRServerless 1.34.85 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.87
+Summary: Type annotations for boto3.EMRServerless 1.34.87 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_emr_serverless-1.34.85/mypy_boto3_emr_serverless.egg-info/SOURCES.txt` & `mypy_boto3_emr_serverless-1.34.87/mypy_boto3_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_emr_serverless-1.34.85/setup.py` & `mypy_boto3_emr_serverless-1.34.87/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-serverless",
-    version="1.34.85",
+    version="1.34.87",
     packages=["mypy_boto3_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EMRServerless 1.34.85 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.EMRServerless 1.34.87 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

