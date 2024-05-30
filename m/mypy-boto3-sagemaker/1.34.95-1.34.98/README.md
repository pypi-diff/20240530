# Comparing `tmp/mypy_boto3_sagemaker-1.34.95.tar.gz` & `tmp/mypy_boto3_sagemaker-1.34.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_sagemaker-1.34.95.tar", last modified: Tue Apr 30 19:34:54 2024, max compression
+gzip compressed data, was "mypy_boto3_sagemaker-1.34.98.tar", last modified: Fri May  3 19:32:43 2024, max compression
```

## Comparing `mypy_boto3_sagemaker-1.34.95.tar` & `mypy_boto3_sagemaker-1.34.98.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:54.659064 mypy_boto3_sagemaker-1.34.95/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25764 2024-04-30 19:34:54.659064 mypy_boto3_sagemaker-1.34.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24201 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:54.659064 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/
--rw-r--r--   0 runner    (1001) docker     (127)    19369 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19369 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   278981 2024-04-30 19:34:24.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   278978 2024-04-30 19:34:23.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    66994 2024-04-30 19:34:26.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    66994 2024-04-30 19:34:26.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   102768 2024-04-30 19:34:25.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)   102695 2024-04-30 19:34:24.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   543580 2024-04-30 19:34:37.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   543580 2024-04-30 19:34:33.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-30 19:34:25.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-04-30 19:34:25.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:54.659064 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25764 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:34:54.659064 mypy_boto3_sagemaker-1.34.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:43.077299 mypy_boto3_sagemaker-1.34.98/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 19:32:13.000000 mypy_boto3_sagemaker-1.34.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25764 2024-05-03 19:32:43.077299 mypy_boto3_sagemaker-1.34.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24201 2024-05-03 19:32:13.000000 mypy_boto3_sagemaker-1.34.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:43.077299 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)    19369 2024-05-03 19:32:13.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19369 2024-05-03 19:32:13.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-03 19:32:13.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278981 2024-05-03 19:32:16.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278978 2024-05-03 19:32:14.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    68359 2024-05-03 19:32:18.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68359 2024-05-03 19:32:18.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   102768 2024-05-03 19:32:17.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102695 2024-05-03 19:32:16.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:13.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   543580 2024-05-03 19:32:28.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   543580 2024-05-03 19:32:24.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 19:32:13.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-05-03 19:32:17.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-05-03 19:32:17.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:43.077299 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25764 2024-05-03 19:32:43.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-03 19:32:43.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:43.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:43.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 19:32:43.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 19:32:43.000000 mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:32:43.077299 mypy_boto3_sagemaker-1.34.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-03 19:32:12.000000 mypy_boto3_sagemaker-1.34.98/setup.py
```

### Comparing `mypy_boto3_sagemaker-1.34.95/LICENSE` & `mypy_boto3_sagemaker-1.34.98/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/PKG-INFO` & `mypy_boto3_sagemaker-1.34.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker
-Version: 1.34.95
-Summary: Type annotations for boto3.SageMaker 1.34.95 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.98
+Summary: Type annotations for boto3.SageMaker 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker)](https://pepy.tech/project/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_sagemaker-1.34.95/README.md` & `mypy_boto3_sagemaker-1.34.98/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker)](https://pepy.tech/project/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__init__.py` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__init__.pyi` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__main__.py` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMaker 1.34.95\n"
-        "Version:         1.34.95\n"
+        "Type annotations for boto3.SageMaker 1.34.98\n"
+        "Version:         1.34.98\n"
         "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.95")
+    print("1.34.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/client.py` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/client.pyi` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/literals.py` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1723,37 +1723,99 @@
     "ml.c4.8xlarge",
     "ml.c4.xlarge",
     "ml.c5.18xlarge",
     "ml.c5.2xlarge",
     "ml.c5.4xlarge",
     "ml.c5.9xlarge",
     "ml.c5.xlarge",
+    "ml.c6i.12xlarge",
+    "ml.c6i.16xlarge",
+    "ml.c6i.24xlarge",
+    "ml.c6i.2xlarge",
+    "ml.c6i.32xlarge",
+    "ml.c6i.4xlarge",
+    "ml.c6i.8xlarge",
+    "ml.c6i.large",
+    "ml.c6i.xlarge",
+    "ml.c7i.12xlarge",
+    "ml.c7i.16xlarge",
+    "ml.c7i.24xlarge",
+    "ml.c7i.2xlarge",
+    "ml.c7i.48xlarge",
+    "ml.c7i.4xlarge",
+    "ml.c7i.8xlarge",
+    "ml.c7i.large",
+    "ml.c7i.xlarge",
     "ml.g4dn.12xlarge",
     "ml.g4dn.16xlarge",
     "ml.g4dn.2xlarge",
     "ml.g4dn.4xlarge",
     "ml.g4dn.8xlarge",
     "ml.g4dn.xlarge",
+    "ml.g5.12xlarge",
+    "ml.g5.16xlarge",
+    "ml.g5.24xlarge",
+    "ml.g5.2xlarge",
+    "ml.g5.48xlarge",
+    "ml.g5.4xlarge",
+    "ml.g5.8xlarge",
+    "ml.g5.xlarge",
     "ml.m4.10xlarge",
     "ml.m4.16xlarge",
     "ml.m4.2xlarge",
     "ml.m4.4xlarge",
     "ml.m4.xlarge",
     "ml.m5.12xlarge",
     "ml.m5.24xlarge",
     "ml.m5.2xlarge",
     "ml.m5.4xlarge",
     "ml.m5.large",
     "ml.m5.xlarge",
+    "ml.m6i.12xlarge",
+    "ml.m6i.16xlarge",
+    "ml.m6i.24xlarge",
+    "ml.m6i.2xlarge",
+    "ml.m6i.32xlarge",
+    "ml.m6i.4xlarge",
+    "ml.m6i.8xlarge",
+    "ml.m6i.large",
+    "ml.m6i.xlarge",
+    "ml.m7i.12xlarge",
+    "ml.m7i.16xlarge",
+    "ml.m7i.24xlarge",
+    "ml.m7i.2xlarge",
+    "ml.m7i.48xlarge",
+    "ml.m7i.4xlarge",
+    "ml.m7i.8xlarge",
+    "ml.m7i.large",
+    "ml.m7i.xlarge",
     "ml.p2.16xlarge",
     "ml.p2.8xlarge",
     "ml.p2.xlarge",
     "ml.p3.16xlarge",
     "ml.p3.2xlarge",
     "ml.p3.8xlarge",
+    "ml.r6i.12xlarge",
+    "ml.r6i.16xlarge",
+    "ml.r6i.24xlarge",
+    "ml.r6i.2xlarge",
+    "ml.r6i.32xlarge",
+    "ml.r6i.4xlarge",
+    "ml.r6i.8xlarge",
+    "ml.r6i.large",
+    "ml.r6i.xlarge",
+    "ml.r7i.12xlarge",
+    "ml.r7i.16xlarge",
+    "ml.r7i.24xlarge",
+    "ml.r7i.2xlarge",
+    "ml.r7i.48xlarge",
+    "ml.r7i.4xlarge",
+    "ml.r7i.8xlarge",
+    "ml.r7i.large",
+    "ml.r7i.xlarge",
 ]
 TransformJobCompletedOrStoppedWaiterName = Literal["transform_job_completed_or_stopped"]
 TransformJobStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping"]
 TrialComponentPrimaryStatusType = Literal[
     "Completed", "Failed", "InProgress", "Stopped", "Stopping"
 ]
 TtlDurationUnitType = Literal["Days", "Hours", "Minutes", "Seconds", "Weeks"]
```

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/literals.pyi` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1723,37 +1723,99 @@
     "ml.c4.8xlarge",
     "ml.c4.xlarge",
     "ml.c5.18xlarge",
     "ml.c5.2xlarge",
     "ml.c5.4xlarge",
     "ml.c5.9xlarge",
     "ml.c5.xlarge",
+    "ml.c6i.12xlarge",
+    "ml.c6i.16xlarge",
+    "ml.c6i.24xlarge",
+    "ml.c6i.2xlarge",
+    "ml.c6i.32xlarge",
+    "ml.c6i.4xlarge",
+    "ml.c6i.8xlarge",
+    "ml.c6i.large",
+    "ml.c6i.xlarge",
+    "ml.c7i.12xlarge",
+    "ml.c7i.16xlarge",
+    "ml.c7i.24xlarge",
+    "ml.c7i.2xlarge",
+    "ml.c7i.48xlarge",
+    "ml.c7i.4xlarge",
+    "ml.c7i.8xlarge",
+    "ml.c7i.large",
+    "ml.c7i.xlarge",
     "ml.g4dn.12xlarge",
     "ml.g4dn.16xlarge",
     "ml.g4dn.2xlarge",
     "ml.g4dn.4xlarge",
     "ml.g4dn.8xlarge",
     "ml.g4dn.xlarge",
+    "ml.g5.12xlarge",
+    "ml.g5.16xlarge",
+    "ml.g5.24xlarge",
+    "ml.g5.2xlarge",
+    "ml.g5.48xlarge",
+    "ml.g5.4xlarge",
+    "ml.g5.8xlarge",
+    "ml.g5.xlarge",
     "ml.m4.10xlarge",
     "ml.m4.16xlarge",
     "ml.m4.2xlarge",
     "ml.m4.4xlarge",
     "ml.m4.xlarge",
     "ml.m5.12xlarge",
     "ml.m5.24xlarge",
     "ml.m5.2xlarge",
     "ml.m5.4xlarge",
     "ml.m5.large",
     "ml.m5.xlarge",
+    "ml.m6i.12xlarge",
+    "ml.m6i.16xlarge",
+    "ml.m6i.24xlarge",
+    "ml.m6i.2xlarge",
+    "ml.m6i.32xlarge",
+    "ml.m6i.4xlarge",
+    "ml.m6i.8xlarge",
+    "ml.m6i.large",
+    "ml.m6i.xlarge",
+    "ml.m7i.12xlarge",
+    "ml.m7i.16xlarge",
+    "ml.m7i.24xlarge",
+    "ml.m7i.2xlarge",
+    "ml.m7i.48xlarge",
+    "ml.m7i.4xlarge",
+    "ml.m7i.8xlarge",
+    "ml.m7i.large",
+    "ml.m7i.xlarge",
     "ml.p2.16xlarge",
     "ml.p2.8xlarge",
     "ml.p2.xlarge",
     "ml.p3.16xlarge",
     "ml.p3.2xlarge",
     "ml.p3.8xlarge",
+    "ml.r6i.12xlarge",
+    "ml.r6i.16xlarge",
+    "ml.r6i.24xlarge",
+    "ml.r6i.2xlarge",
+    "ml.r6i.32xlarge",
+    "ml.r6i.4xlarge",
+    "ml.r6i.8xlarge",
+    "ml.r6i.large",
+    "ml.r6i.xlarge",
+    "ml.r7i.12xlarge",
+    "ml.r7i.16xlarge",
+    "ml.r7i.24xlarge",
+    "ml.r7i.2xlarge",
+    "ml.r7i.48xlarge",
+    "ml.r7i.4xlarge",
+    "ml.r7i.8xlarge",
+    "ml.r7i.large",
+    "ml.r7i.xlarge",
 ]
 TransformJobCompletedOrStoppedWaiterName = Literal["transform_job_completed_or_stopped"]
 TransformJobStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping"]
 TrialComponentPrimaryStatusType = Literal[
     "Completed", "Failed", "InProgress", "Stopped", "Stopping"
 ]
 TtlDurationUnitType = Literal["Days", "Hours", "Minutes", "Seconds", "Weeks"]
```

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/paginator.py` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/paginator.pyi` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/type_defs.py` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/type_defs.pyi` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/waiter.py` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/waiter.pyi` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/PKG-INFO` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker
-Version: 1.34.95
-Summary: Type annotations for boto3.SageMaker 1.34.95 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.98
+Summary: Type annotations for boto3.SageMaker 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker)](https://pepy.tech/project/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/SOURCES.txt` & `mypy_boto3_sagemaker-1.34.98/mypy_boto3_sagemaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.95/setup.py` & `mypy_boto3_sagemaker-1.34.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker",
-    version="1.34.95",
+    version="1.34.98",
     packages=["mypy_boto3_sagemaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.SageMaker 1.34.95 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.SageMaker 1.34.98 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

