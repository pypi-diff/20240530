# Comparing `tmp/projen-0.82.1.tar.gz` & `tmp/projen-0.82.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.82.1.tar", last modified: Tue May 28 13:23:46 2024, max compression
+gzip compressed data, was "projen-0.82.2.tar", last modified: Wed May 29 23:22:23 2024, max compression
```

## Comparing `projen-0.82.1.tar` & `projen-0.82.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.058049 projen-0.82.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-28 13:23:35.000000 projen-0.82.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 13:23:35.000000 projen-0.82.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-28 13:23:46.058049 projen-0.82.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-05-28 13:23:35.000000 projen-0.82.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 13:23:35.000000 projen-0.82.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:23:46.058049 projen-0.82.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-28 13:23:35.000000 projen-0.82.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.042049 projen-0.82.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.046049 projen-0.82.1/src/projen/
--rw-r--r--   0 runner    (1001) docker     (127)   653934 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.046049 projen-0.82.1/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.050049 projen-0.82.1/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (127)  2649379 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/_jsii/projen@0.82.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.050049 projen-0.82.1/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.050049 projen-0.82.1/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.050049 projen-0.82.1/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.050049 projen-0.82.1/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.054049 projen-0.82.1/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.054049 projen-0.82.1/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.054049 projen-0.82.1/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (127)   425340 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.054049 projen-0.82.1/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.054049 projen-0.82.1/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)   202836 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.054049 projen-0.82.1/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.054049 projen-0.82.1/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)   845441 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.058049 projen-0.82.1/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.058049 projen-0.82.1/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.058049 projen-0.82.1/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.058049 projen-0.82.1/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.058049 projen-0.82.1/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-05-28 13:23:35.000000 projen-0.82.1/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:23:46.046049 projen-0.82.1/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-28 13:23:46.000000 projen-0.82.1/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-28 13:23:46.000000 projen-0.82.1/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:23:46.000000 projen-0.82.1/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 13:23:46.000000 projen-0.82.1/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 13:23:46.000000 projen-0.82.1/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.022223 projen-0.82.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 23:22:12.000000 projen-0.82.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 23:22:12.000000 projen-0.82.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-29 23:22:23.022223 projen-0.82.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-05-29 23:22:12.000000 projen-0.82.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 23:22:12.000000 projen-0.82.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 23:22:23.022223 projen-0.82.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-29 23:22:12.000000 projen-0.82.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.002223 projen-0.82.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.006223 projen-0.82.2/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (127)   653934 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.006223 projen-0.82.2/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.010223 projen-0.82.2/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (127)  2650958 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/_jsii/projen@0.82.2.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.010223 projen-0.82.2/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (127)   425340 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)   202836 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)   847962 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.006223 projen-0.82.2/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-29 23:22:22.000000 projen-0.82.2/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-29 23:22:22.000000 projen-0.82.2/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 23:22:22.000000 projen-0.82.2/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-29 23:22:22.000000 projen-0.82.2/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 23:22:22.000000 projen-0.82.2/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.82.1/LICENSE` & `projen-0.82.2/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/PKG-INFO` & `projen-0.82.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.82.1
+Version: 0.82.2
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.82.1/README.md` & `projen-0.82.2/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/setup.py` & `projen-0.82.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.82.1",
+    "version": "0.82.2",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.82.1.jsii.tgz"
+            "projen@0.82.2.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `projen-0.82.1/src/projen/__init__.py` & `projen-0.82.2/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/awscdk/__init__.py` & `projen-0.82.2/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/build/__init__.py` & `projen-0.82.2/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/cdk/__init__.py` & `projen-0.82.2/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/cdk8s/__init__.py` & `projen-0.82.2/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/cdktf/__init__.py` & `projen-0.82.2/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/circleci/__init__.py` & `projen-0.82.2/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/github/__init__.py` & `projen-0.82.2/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/github/workflows/__init__.py` & `projen-0.82.2/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/gitlab/__init__.py` & `projen-0.82.2/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/java/__init__.py` & `projen-0.82.2/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/javascript/__init__.py` & `projen-0.82.2/src/projen/javascript/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9836,14 +9836,15 @@
         "inline_source_map": "inlineSourceMap",
         "inline_sources": "inlineSources",
         "isolated_modules": "isolatedModules",
         "jsx": "jsx",
         "jsx_import_source": "jsxImportSource",
         "lib": "lib",
         "module": "module",
+        "module_detection": "moduleDetection",
         "module_resolution": "moduleResolution",
         "no_emit": "noEmit",
         "no_emit_on_error": "noEmitOnError",
         "no_fallthrough_cases_in_switch": "noFallthroughCasesInSwitch",
         "no_implicit_any": "noImplicitAny",
         "no_implicit_override": "noImplicitOverride",
         "no_implicit_returns": "noImplicitReturns",
@@ -9902,14 +9903,15 @@
         inline_source_map: typing.Optional[builtins.bool] = None,
         inline_sources: typing.Optional[builtins.bool] = None,
         isolated_modules: typing.Optional[builtins.bool] = None,
         jsx: typing.Optional["TypeScriptJsxMode"] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         lib: typing.Optional[typing.Sequence[builtins.str]] = None,
         module: typing.Optional[builtins.str] = None,
+        module_detection: typing.Optional["TypeScriptModuleDetection"] = None,
         module_resolution: typing.Optional["TypeScriptModuleResolution"] = None,
         no_emit: typing.Optional[builtins.bool] = None,
         no_emit_on_error: typing.Optional[builtins.bool] = None,
         no_fallthrough_cases_in_switch: typing.Optional[builtins.bool] = None,
         no_implicit_any: typing.Optional[builtins.bool] = None,
         no_implicit_override: typing.Optional[builtins.bool] = None,
         no_implicit_returns: typing.Optional[builtins.bool] = None,
@@ -9964,14 +9966,15 @@
         :param inline_source_map: (experimental) When set, instead of writing out a .js.map file to provide source maps, TypeScript will embed the source map content in the .js files. Default: true
         :param inline_sources: (experimental) When set, TypeScript will include the original content of the .ts file as an embedded string in the source map. This is often useful in the same cases as inlineSourceMap. Default: true
         :param isolated_modules: (experimental) Perform additional checks to ensure that separate compilation (such as with transpileModule or. Default: false
         :param jsx: (experimental) Support JSX in .tsx files: "react", "preserve", "react-native" etc. Default: undefined
         :param jsx_import_source: (experimental) Declares the module specifier to be used for importing the jsx and jsxs factory functions when using jsx. Default: undefined
         :param lib: (experimental) Reference for type definitions / libraries to use (eg. ES2016, ES5, ES2018). Default: [ "es2018" ]
         :param module: (experimental) Sets the module system for the program. See https://www.typescriptlang.org/docs/handbook/modules.html#ambient-modules. Default: "CommonJS"
+        :param module_detection: (experimental) This setting controls how TypeScript determines whether a file is a `script or a module <https://www.typescriptlang.org/docs/handbook/modules/theory.html#scripts-and-modules-in-javascript>`_. Default: "auto"
         :param module_resolution: (experimental) Determine how modules get resolved. Either "Node" for Node.js/io.js style resolution, or "Classic". Default: "node"
         :param no_emit: (experimental) Do not emit outputs. Default: false
         :param no_emit_on_error: (experimental) Do not emit compiler output files like JavaScript source code, source-maps or declarations if any errors were reported. Default: true
         :param no_fallthrough_cases_in_switch: (experimental) Report errors for fallthrough cases in switch statements. Ensures that any non-empty case inside a switch statement includes either break or return. This means you won’t accidentally ship a case fallthrough bug. Default: true
         :param no_implicit_any: (experimental) In some cases where no type annotations are present, TypeScript will fall back to a type of any for a variable when it cannot infer the type. Default: true
         :param no_implicit_override: (experimental) Using ``noImplicitOverride``, you can ensure that sub-classes never go out of sync as they are required to explicitly declare that they are overriding a member using the ``override`` keyword. This also improves readability of the programmer's intent. Available with TypeScript 4.3 and newer. Default: false
         :param no_implicit_returns: (experimental) When enabled, TypeScript will check all code paths in a function to ensure they return a value. Default: true
@@ -10029,14 +10032,15 @@
             check_type(argname="argument inline_source_map", value=inline_source_map, expected_type=type_hints["inline_source_map"])
             check_type(argname="argument inline_sources", value=inline_sources, expected_type=type_hints["inline_sources"])
             check_type(argname="argument isolated_modules", value=isolated_modules, expected_type=type_hints["isolated_modules"])
             check_type(argname="argument jsx", value=jsx, expected_type=type_hints["jsx"])
             check_type(argname="argument jsx_import_source", value=jsx_import_source, expected_type=type_hints["jsx_import_source"])
             check_type(argname="argument lib", value=lib, expected_type=type_hints["lib"])
             check_type(argname="argument module", value=module, expected_type=type_hints["module"])
+            check_type(argname="argument module_detection", value=module_detection, expected_type=type_hints["module_detection"])
             check_type(argname="argument module_resolution", value=module_resolution, expected_type=type_hints["module_resolution"])
             check_type(argname="argument no_emit", value=no_emit, expected_type=type_hints["no_emit"])
             check_type(argname="argument no_emit_on_error", value=no_emit_on_error, expected_type=type_hints["no_emit_on_error"])
             check_type(argname="argument no_fallthrough_cases_in_switch", value=no_fallthrough_cases_in_switch, expected_type=type_hints["no_fallthrough_cases_in_switch"])
             check_type(argname="argument no_implicit_any", value=no_implicit_any, expected_type=type_hints["no_implicit_any"])
             check_type(argname="argument no_implicit_override", value=no_implicit_override, expected_type=type_hints["no_implicit_override"])
             check_type(argname="argument no_implicit_returns", value=no_implicit_returns, expected_type=type_hints["no_implicit_returns"])
@@ -10119,14 +10123,16 @@
             self._values["jsx"] = jsx
         if jsx_import_source is not None:
             self._values["jsx_import_source"] = jsx_import_source
         if lib is not None:
             self._values["lib"] = lib
         if module is not None:
             self._values["module"] = module
+        if module_detection is not None:
+            self._values["module_detection"] = module_detection
         if module_resolution is not None:
             self._values["module_resolution"] = module_resolution
         if no_emit is not None:
             self._values["no_emit"] = no_emit
         if no_emit_on_error is not None:
             self._values["no_emit_on_error"] = no_emit_on_error
         if no_fallthrough_cases_in_switch is not None:
@@ -10554,14 +10560,25 @@
 
         :stability: experimental
         '''
         result = self._values.get("module")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def module_detection(self) -> typing.Optional["TypeScriptModuleDetection"]:
+        '''(experimental) This setting controls how TypeScript determines whether a file is a `script or a module <https://www.typescriptlang.org/docs/handbook/modules/theory.html#scripts-and-modules-in-javascript>`_.
+
+        :default: "auto"
+
+        :stability: experimental
+        '''
+        result = self._values.get("module_detection")
+        return typing.cast(typing.Optional["TypeScriptModuleDetection"], result)
+
+    @builtins.property
     def module_resolution(self) -> typing.Optional["TypeScriptModuleResolution"]:
         '''(experimental) Determine how modules get resolved.
 
         Either "Node" for Node.js/io.js style resolution, or "Classic".
 
         :default: "node"
 
@@ -10992,14 +11009,42 @@
     REACT_JSXDEV = "REACT_JSXDEV"
     '''(experimental) Same as ``REACT_JSX`` with additional debug data.
 
     :stability: experimental
     '''
 
 
+@jsii.enum(jsii_type="projen.javascript.TypeScriptModuleDetection")
+class TypeScriptModuleDetection(enum.Enum):
+    '''(experimental) This setting controls how TypeScript determines whether a file is a script or a module.
+
+    :see: https://www.typescriptlang.org/docs/handbook/modules/theory.html#scripts-and-modules-in-javascript
+    :stability: experimental
+    '''
+
+    AUTO = "AUTO"
+    '''(experimental) TypeScript will not only look for import and export statements, but it will also check whether the "type" field in a package.json is set to "module" when running with module: nodenext or node16, and check whether the current file is a JSX file when running under jsx: react-jsx.
+
+    :see: https://www.typescriptlang.org/tsconfig/#moduleDetection
+    :stability: experimental
+    '''
+    LEGACY = "LEGACY"
+    '''(experimental) The same behavior as 4.6 and prior, usings import and export statements to determine whether a file is a module.
+
+    :see: https://www.typescriptlang.org/tsconfig/#moduleDetection
+    :stability: experimental
+    '''
+    FORCE = "FORCE"
+    '''(experimental) Ensures that every non-declaration file is treated as a module.
+
+    :see: https://www.typescriptlang.org/tsconfig/#moduleDetection
+    :stability: experimental
+    '''
+
+
 @jsii.enum(jsii_type="projen.javascript.TypeScriptModuleResolution")
 class TypeScriptModuleResolution(enum.Enum):
     '''(experimental) Determines how modules get resolved.
 
     :see: https://www.typescriptlang.org/docs/handbook/module-resolution.html
     :stability: experimental
     '''
@@ -15311,14 +15356,15 @@
     "ScopedPackagesOptions",
     "SourceMapMode",
     "TrailingComma",
     "Transform",
     "TypeScriptCompilerOptions",
     "TypeScriptImportsNotUsedAsValues",
     "TypeScriptJsxMode",
+    "TypeScriptModuleDetection",
     "TypeScriptModuleResolution",
     "TypescriptConfig",
     "TypescriptConfigExtends",
     "TypescriptConfigOptions",
     "UpdateSnapshot",
     "UpgradeDependencies",
     "UpgradeDependenciesOptions",
@@ -16346,14 +16392,15 @@
     inline_source_map: typing.Optional[builtins.bool] = None,
     inline_sources: typing.Optional[builtins.bool] = None,
     isolated_modules: typing.Optional[builtins.bool] = None,
     jsx: typing.Optional[TypeScriptJsxMode] = None,
     jsx_import_source: typing.Optional[builtins.str] = None,
     lib: typing.Optional[typing.Sequence[builtins.str]] = None,
     module: typing.Optional[builtins.str] = None,
+    module_detection: typing.Optional[TypeScriptModuleDetection] = None,
     module_resolution: typing.Optional[TypeScriptModuleResolution] = None,
     no_emit: typing.Optional[builtins.bool] = None,
     no_emit_on_error: typing.Optional[builtins.bool] = None,
     no_fallthrough_cases_in_switch: typing.Optional[builtins.bool] = None,
     no_implicit_any: typing.Optional[builtins.bool] = None,
     no_implicit_override: typing.Optional[builtins.bool] = None,
     no_implicit_returns: typing.Optional[builtins.bool] = None,
```

### Comparing `projen-0.82.1/src/projen/python/__init__.py` & `projen-0.82.2/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/release/__init__.py` & `projen-0.82.2/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/typescript/__init__.py` & `projen-0.82.2/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/vscode/__init__.py` & `projen-0.82.2/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen/web/__init__.py` & `projen-0.82.2/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.1/src/projen.egg-info/PKG-INFO` & `projen-0.82.2/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.82.1
+Version: 0.82.2
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.82.1/src/projen.egg-info/SOURCES.txt` & `projen-0.82.2/src/projen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.82.1.jsii.tgz
+src/projen/_jsii/projen@0.82.2.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

