# Comparing `tmp/node-ec2-instance-0.0.5.tar.gz` & `tmp/node-ec2-instance-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node-ec2-instance-0.0.5.tar", last modified: Sun May 26 01:28:14 2024, max compression
+gzip compressed data, was "node-ec2-instance-0.0.6.tar", last modified: Thu May 30 13:42:25 2024, max compression
```

## Comparing `node-ec2-instance-0.0.5.tar` & `node-ec2-instance-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:14.865232 node-ec2-instance-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-26 01:28:00.000000 node-ec2-instance-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 01:28:00.000000 node-ec2-instance-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-26 01:28:14.865232 node-ec2-instance-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-26 01:28:00.000000 node-ec2-instance-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-26 01:28:00.000000 node-ec2-instance-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 01:28:14.865232 node-ec2-instance-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-26 01:28:00.000000 node-ec2-instance-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:14.865232 node-ec2-instance-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:14.865232 node-ec2-instance-0.0.5/src/node_ec2_instance/
--rw-r--r--   0 runner    (1001) docker     (127)    50392 2024-05-26 01:28:00.000000 node-ec2-instance-0.0.5/src/node_ec2_instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:14.865232 node-ec2-instance-0.0.5/src/node_ec2_instance/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-26 01:28:00.000000 node-ec2-instance-0.0.5/src/node_ec2_instance/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24394 2024-05-26 01:28:00.000000 node-ec2-instance-0.0.5/src/node_ec2_instance/_jsii/cdk-node-ec2-instance@0.0.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:28:00.000000 node-ec2-instance-0.0.5/src/node_ec2_instance/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:14.865232 node-ec2-instance-0.0.5/src/node_ec2_instance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-26 01:28:14.000000 node-ec2-instance-0.0.5/src/node_ec2_instance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-26 01:28:14.000000 node-ec2-instance-0.0.5/src/node_ec2_instance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:28:14.000000 node-ec2-instance-0.0.5/src/node_ec2_instance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-26 01:28:14.000000 node-ec2-instance-0.0.5/src/node_ec2_instance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 01:28:14.000000 node-ec2-instance-0.0.5/src/node_ec2_instance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:42:25.348305 node-ec2-instance-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-30 13:42:15.000000 node-ec2-instance-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 13:42:15.000000 node-ec2-instance-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-30 13:42:25.348305 node-ec2-instance-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-30 13:42:15.000000 node-ec2-instance-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 13:42:15.000000 node-ec2-instance-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:42:25.348305 node-ec2-instance-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-30 13:42:15.000000 node-ec2-instance-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:42:25.348305 node-ec2-instance-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:42:25.348305 node-ec2-instance-0.0.6/src/node_ec2_instance/
+-rw-r--r--   0 runner    (1001) docker     (127)    50392 2024-05-30 13:42:15.000000 node-ec2-instance-0.0.6/src/node_ec2_instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:42:25.348305 node-ec2-instance-0.0.6/src/node_ec2_instance/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 13:42:15.000000 node-ec2-instance-0.0.6/src/node_ec2_instance/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24430 2024-05-30 13:42:15.000000 node-ec2-instance-0.0.6/src/node_ec2_instance/_jsii/cdk-node-ec2-instance@0.0.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:42:15.000000 node-ec2-instance-0.0.6/src/node_ec2_instance/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:42:25.348305 node-ec2-instance-0.0.6/src/node_ec2_instance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-30 13:42:25.000000 node-ec2-instance-0.0.6/src/node_ec2_instance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 13:42:25.000000 node-ec2-instance-0.0.6/src/node_ec2_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:42:25.000000 node-ec2-instance-0.0.6/src/node_ec2_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 13:42:25.000000 node-ec2-instance-0.0.6/src/node_ec2_instance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 13:42:25.000000 node-ec2-instance-0.0.6/src/node_ec2_instance.egg-info/top_level.txt
```

### Comparing `node-ec2-instance-0.0.5/LICENSE` & `node-ec2-instance-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `node-ec2-instance-0.0.5/PKG-INFO` & `node-ec2-instance-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node-ec2-instance
-Version: 0.0.5
+Version: 0.0.6
 Summary: CDK construct library for creating an EC2 instance with Node.js installed
 Home-page: https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `node-ec2-instance-0.0.5/README.md` & `node-ec2-instance-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `node-ec2-instance-0.0.5/setup.py` & `node-ec2-instance-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "node-ec2-instance",
-    "version": "0.0.5",
+    "version": "0.0.6",
     "description": "CDK construct library for creating an EC2 instance with Node.js installed",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-node-ec2-instance.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "node_ec2_instance",
         "node_ec2_instance._jsii"
     ],
     "package_data": {
         "node_ec2_instance._jsii": [
-            "cdk-node-ec2-instance@0.0.5.jsii.tgz"
+            "cdk-node-ec2-instance@0.0.6.jsii.tgz"
         ],
         "node_ec2_instance": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `node-ec2-instance-0.0.5/src/node_ec2_instance/__init__.py` & `node-ec2-instance-0.0.6/src/node_ec2_instance/__init__.py`

 * *Files identical despite different names*

### Comparing `node-ec2-instance-0.0.5/src/node_ec2_instance.egg-info/PKG-INFO` & `node-ec2-instance-0.0.6/src/node_ec2_instance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node-ec2-instance
-Version: 0.0.5
+Version: 0.0.6
 Summary: CDK construct library for creating an EC2 instance with Node.js installed
 Home-page: https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-node-ec2-instance.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

