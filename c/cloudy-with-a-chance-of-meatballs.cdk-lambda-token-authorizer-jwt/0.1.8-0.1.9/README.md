# Comparing `tmp/cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8.tar.gz` & `tmp/cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8.tar", last modified: Mon Jan  9 20:00:16 2023, max compression
+gzip compressed data, was "cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9.tar", last modified: Mon Jan  9 22:48:33 2023, max compression
```

## Comparing `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8.tar` & `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:00:16.382638 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-09 20:00:02.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-09 20:00:02.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-01-09 20:00:16.382638 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-01-09 20:00:02.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-09 20:00:02.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 20:00:16.382638 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-01-09 20:00:02.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:00:16.382638 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:00:16.382638 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-01-09 20:00:15.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-09 20:00:16.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:00:15.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-09 20:00:16.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-09 20:00:16.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:00:16.382638 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/
--rw-r--r--   0 runner    (1001) docker     (123)    76452 2023-01-09 20:00:02.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:00:16.382638 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-09 20:00:02.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149978 2023-01-09 20:00:02.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/_jsii/cdk-lambda-token-authorizer-jwt@0.1.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:00:02.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:48:33.249735 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-09 22:48:19.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-09 22:48:19.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-01-09 22:48:33.249735 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-01-09 22:48:19.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-09 22:48:19.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 22:48:33.249735 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-01-09 22:48:19.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:48:33.245735 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:48:33.249735 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-01-09 22:48:32.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-09 22:48:33.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 22:48:32.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-09 22:48:33.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-09 22:48:33.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:48:33.249735 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)    76452 2023-01-09 22:48:19.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:48:33.249735 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-09 22:48:19.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149905 2023-01-09 22:48:19.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/_jsii/cdk-lambda-token-authorizer-jwt@0.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 22:48:19.000000 cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/py.typed
```

### Comparing `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/LICENSE` & `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/PKG-INFO` & `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt
-Version: 0.1.8
+Version: 0.1.9
 Summary: Add a lambda function to your aws-rest-api-gateway which can be used as a token authorizer
 Home-page: https://github.com/cloudy-with-a-chance-of-meatballs/cdk-lambda-token-authorizer-jwt.git
 Author: cfuerst<c.fuerst@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/cloudy-with-a-chance-of-meatballs/cdk-lambda-token-authorizer-jwt.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/README.md` & `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/setup.py` & `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt",
-    "version": "0.1.8",
+    "version": "0.1.9",
     "description": "Add a lambda function to your aws-rest-api-gateway which can be used as a token authorizer",
     "license": "MIT",
     "url": "https://github.com/cloudy-with-a-chance-of-meatballs/cdk-lambda-token-authorizer-jwt.git",
     "long_description_content_type": "text/markdown",
     "author": "cfuerst<c.fuerst@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt",
         "cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt._jsii"
     ],
     "package_data": {
         "cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt._jsii": [
-            "cdk-lambda-token-authorizer-jwt@0.1.8.jsii.tgz"
+            "cdk-lambda-token-authorizer-jwt@0.1.9.jsii.tgz"
         ],
         "cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/PKG-INFO` & `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt
-Version: 0.1.8
+Version: 0.1.9
 Summary: Add a lambda function to your aws-rest-api-gateway which can be used as a token authorizer
 Home-page: https://github.com/cloudy-with-a-chance-of-meatballs/cdk-lambda-token-authorizer-jwt.git
 Author: cfuerst<c.fuerst@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/cloudy-with-a-chance-of-meatballs/cdk-lambda-token-authorizer-jwt.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/SOURCES.txt` & `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/SOURCES.txt
 src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/dependency_links.txt
 src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/requires.txt
 src/cloudy_with_a_chance_of_meatballs.cdk_lambda_token_authorizer_jwt.egg-info/top_level.txt
 src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/__init__.py
 src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/py.typed
 src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/_jsii/__init__.py
-src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/_jsii/cdk-lambda-token-authorizer-jwt@0.1.8.jsii.tgz
+src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/_jsii/cdk-lambda-token-authorizer-jwt@0.1.9.jsii.tgz
```

### Comparing `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.8/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/__init__.py` & `cloudy-with-a-chance-of-meatballs.cdk-lambda-token-authorizer-jwt-0.1.9/src/cloudy_with_a_chance_of_meatballs_cdk_lambda_token_authorizer_jwt/__init__.py`

 * *Files identical despite different names*

