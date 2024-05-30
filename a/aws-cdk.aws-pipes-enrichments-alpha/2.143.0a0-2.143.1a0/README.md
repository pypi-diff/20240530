# Comparing `tmp/aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0.tar.gz` & `tmp/aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0.tar", last modified: Fri May 24 02:44:49 2024, max compression
+gzip compressed data, was "aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0.tar", last modified: Thu May 30 02:13:21 2024, max compression
```

## Comparing `aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0.tar` & `aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 02:44:49.204138 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2024-05-24 02:44:37.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-24 02:44:37.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2024-05-24 02:44:37.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2428 2024-05-24 02:44:49.204138 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1442 2024-05-24 02:44:37.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-05-24 02:44:37.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 02:44:49.204138 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1963 2024-05-24 02:44:37.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 02:44:49.204138 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 02:44:49.204138 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 02:44:49.204138 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk/aws_pipes_enrichments_alpha/
--rw-r--r--   0 root         (0) root         (0)     8767 2024-05-24 02:44:37.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk/aws_pipes_enrichments_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 02:44:49.204138 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      576 2024-05-24 02:44:37.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22203 2024-05-24 02:44:37.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/aws-pipes-enrichments-alpha@2.143.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 02:44:37.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk/aws_pipes_enrichments_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 02:44:49.204138 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2428 2024-05-24 02:44:49.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      632 2024-05-24 02:44:49.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 02:44:49.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      148 2024-05-24 02:44:49.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-24 02:44:49.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:13:21.742751 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2024-05-30 02:13:11.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 02:13:11.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2024-05-30 02:13:11.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-05-30 02:13:21.742751 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1442 2024-05-30 02:13:11.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-05-30 02:13:11.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 02:13:21.742751 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1963 2024-05-30 02:13:11.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:13:21.742751 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:13:21.742751 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:13:21.742751 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk/aws_pipes_enrichments_alpha/
+-rw-r--r--   0 root         (0) root         (0)     8767 2024-05-30 02:13:11.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk/aws_pipes_enrichments_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:13:21.742751 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      576 2024-05-30 02:13:11.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22203 2024-05-30 02:13:11.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/aws-pipes-enrichments-alpha@2.143.1-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 02:13:11.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk/aws_pipes_enrichments_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:13:21.742751 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-05-30 02:13:21.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-30 02:13:21.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 02:13:21.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-30 02:13:21.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 02:13:21.000000 aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/LICENSE` & `aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/PKG-INFO` & `aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-pipes-enrichments-alpha
-Version: 2.143.0a0
+Version: 2.143.1a0
 Summary: The CDK Construct Library for Amazon EventBridge Pipes Enrichments
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/README.md` & `aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/setup.py` & `aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-pipes-enrichments-alpha",
-    "version": "2.143.0.a0",
+    "version": "2.143.1.a0",
     "description": "The CDK Construct Library for Amazon EventBridge Pipes Enrichments",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "aws_cdk.aws_pipes_enrichments_alpha",
         "aws_cdk.aws_pipes_enrichments_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_pipes_enrichments_alpha._jsii": [
-            "aws-pipes-enrichments-alpha@2.143.0-alpha.0.jsii.tgz"
+            "aws-pipes-enrichments-alpha@2.143.1-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_pipes_enrichments_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.143.0, <3.0.0",
-        "aws-cdk.aws-pipes-alpha==2.143.0.a0",
+        "aws-cdk-lib>=2.143.1, <3.0.0",
+        "aws-cdk.aws-pipes-alpha==2.143.1.a0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk/aws_pipes_enrichments_alpha/__init__.py` & `aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk/aws_pipes_enrichments_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/__init__.py` & `aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import aws_cdk.aws_pipes_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-cdk/aws-pipes-enrichments-alpha",
-    "2.143.0-alpha.0",
+    "2.143.1-alpha.0",
     __name__[0:-6],
-    "aws-pipes-enrichments-alpha@2.143.0-alpha.0.jsii.tgz",
+    "aws-pipes-enrichments-alpha@2.143.1-alpha.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-pipes-enrichments-alpha
-Version: 2.143.0a0
+Version: 2.143.1a0
 Summary: The CDK Construct Library for Amazon EventBridge Pipes Enrichments
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-pipes-enrichments-alpha-2.143.0a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-pipes-enrichments-alpha-2.143.1a0/src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/requires.txt
 src/aws_cdk.aws_pipes_enrichments_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_pipes_enrichments_alpha/__init__.py
 src/aws_cdk/aws_pipes_enrichments_alpha/py.typed
 src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/__init__.py
-src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/aws-pipes-enrichments-alpha@2.143.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_pipes_enrichments_alpha/_jsii/aws-pipes-enrichments-alpha@2.143.1-alpha.0.jsii.tgz
```

