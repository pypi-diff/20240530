# Comparing `tmp/goldlink_client_python-0.0.4.tar.gz` & `tmp/goldlink_client_python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goldlink_client_python-0.0.4.tar", last modified: Wed May 29 15:49:41 2024, max compression
+gzip compressed data, was "goldlink_client_python-0.0.5.tar", last modified: Wed May 29 19:57:44 2024, max compression
```

## Comparing `goldlink_client_python-0.0.4.tar` & `goldlink_client_python-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 samweinberg   (501) staff       (20)        0 2024-05-29 15:49:41.853482 goldlink_client_python-0.0.4/
--rw-r--r--   0 samweinberg   (501) staff       (20)    11360 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/LICENSE
--rw-r--r--   0 samweinberg   (501) staff       (20)     1847 2024-05-29 15:49:41.853283 goldlink_client_python-0.0.4/PKG-INFO
--rw-r--r--   0 samweinberg   (501) staff       (20)      759 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/README.md
-drwxr-xr-x   0 samweinberg   (501) staff       (20)        0 2024-05-29 15:49:41.849705 goldlink_client_python-0.0.4/goldlink/
--rw-r--r--   0 samweinberg   (501) staff       (20)      222 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/__init__.py
-drwxr-xr-x   0 samweinberg   (501) staff       (20)        0 2024-05-29 15:49:41.851605 goldlink_client_python-0.0.4/goldlink/abi/
--rw-r--r--   0 samweinberg   (501) staff       (20)     5256 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/abi/erc20.json
--rw-r--r--   0 samweinberg   (501) staff       (20)     4559 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/abi/gmx-frf-account-getters.json
--rw-r--r--   0 samweinberg   (501) staff       (20)    82231 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/abi/gmx-frf-strategy-account.json
--rw-r--r--   0 samweinberg   (501) staff       (20)    31076 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/abi/gmx-frf-strategy-manager.json
--rw-r--r--   0 samweinberg   (501) staff       (20)    97179 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/abi/gmx_v2_reader.json
--rw-r--r--   0 samweinberg   (501) staff       (20)     7411 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/abi/strategy-account.json
--rw-r--r--   0 samweinberg   (501) staff       (20)    18013 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/abi/strategy-bank.json
--rw-r--r--   0 samweinberg   (501) staff       (20)    28277 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/abi/strategy-reserve.json
--rw-r--r--   0 samweinberg   (501) staff       (20)     2234 2024-05-29 15:49:35.000000 goldlink_client_python-0.0.4/goldlink/constants.py
--rw-r--r--   0 samweinberg   (501) staff       (20)      476 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/errors.py
--rw-r--r--   0 samweinberg   (501) staff       (20)     6809 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/goldlink_client.py
--rw-r--r--   0 samweinberg   (501) staff       (20)     1482 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/goldlink/helpers.py
-drwxr-xr-x   0 samweinberg   (501) staff       (20)        0 2024-05-29 15:49:41.853068 goldlink_client_python-0.0.4/goldlink_client_python.egg-info/
--rw-r--r--   0 samweinberg   (501) staff       (20)     1847 2024-05-29 15:49:41.000000 goldlink_client_python-0.0.4/goldlink_client_python.egg-info/PKG-INFO
--rw-r--r--   0 samweinberg   (501) staff       (20)      745 2024-05-29 15:49:41.000000 goldlink_client_python-0.0.4/goldlink_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 samweinberg   (501) staff       (20)        1 2024-05-29 15:49:41.000000 goldlink_client_python-0.0.4/goldlink_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 samweinberg   (501) staff       (20)       90 2024-05-29 15:49:41.000000 goldlink_client_python-0.0.4/goldlink_client_python.egg-info/requires.txt
--rw-r--r--   0 samweinberg   (501) staff       (20)       27 2024-05-29 15:49:41.000000 goldlink_client_python-0.0.4/goldlink_client_python.egg-info/top_level.txt
-drwxr-xr-x   0 samweinberg   (501) staff       (20)        0 2024-05-29 15:49:41.852840 goldlink_client_python-0.0.4/integration_tests/
--rw-r--r--   0 samweinberg   (501) staff       (20)        0 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/integration_tests/__init__.py
--rw-r--r--   0 samweinberg   (501) staff       (20)      199 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/integration_tests/constants.py
--rw-r--r--   0 samweinberg   (501) staff       (20)     1144 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.4/integration_tests/test_client.py
--rw-r--r--   0 samweinberg   (501) staff       (20)       38 2024-05-29 15:49:41.853515 goldlink_client_python-0.0.4/setup.cfg
--rw-r--r--   0 samweinberg   (501) staff       (20)     1388 2024-05-29 15:49:35.000000 goldlink_client_python-0.0.4/setup.py
+drwxr-xr-x   0 samweinberg   (501) staff       (20)        0 2024-05-29 19:57:44.847199 goldlink_client_python-0.0.5/
+-rw-r--r--   0 samweinberg   (501) staff       (20)    11360 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/LICENSE
+-rw-r--r--   0 samweinberg   (501) staff       (20)     1847 2024-05-29 19:57:44.846991 goldlink_client_python-0.0.5/PKG-INFO
+-rw-r--r--   0 samweinberg   (501) staff       (20)      759 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/README.md
+drwxr-xr-x   0 samweinberg   (501) staff       (20)        0 2024-05-29 19:57:44.841743 goldlink_client_python-0.0.5/goldlink/
+-rw-r--r--   0 samweinberg   (501) staff       (20)      222 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/__init__.py
+drwxr-xr-x   0 samweinberg   (501) staff       (20)        0 2024-05-29 19:57:44.843733 goldlink_client_python-0.0.5/goldlink/abi/
+-rw-r--r--   0 samweinberg   (501) staff       (20)     5256 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/abi/erc20.json
+-rw-r--r--   0 samweinberg   (501) staff       (20)     4559 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/abi/gmx-frf-account-getters.json
+-rw-r--r--   0 samweinberg   (501) staff       (20)    82231 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/abi/gmx-frf-strategy-account.json
+-rw-r--r--   0 samweinberg   (501) staff       (20)    31076 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/abi/gmx-frf-strategy-manager.json
+-rw-r--r--   0 samweinberg   (501) staff       (20)    97179 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/abi/gmx_v2_reader.json
+-rw-r--r--   0 samweinberg   (501) staff       (20)     7411 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/abi/strategy-account.json
+-rw-r--r--   0 samweinberg   (501) staff       (20)    18013 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/abi/strategy-bank.json
+-rw-r--r--   0 samweinberg   (501) staff       (20)    28277 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/abi/strategy-reserve.json
+-rw-r--r--   0 samweinberg   (501) staff       (20)     2234 2024-05-29 15:49:35.000000 goldlink_client_python-0.0.5/goldlink/constants.py
+-rw-r--r--   0 samweinberg   (501) staff       (20)      476 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/errors.py
+-rw-r--r--   0 samweinberg   (501) staff       (20)     6809 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/goldlink_client.py
+-rw-r--r--   0 samweinberg   (501) staff       (20)     1482 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/goldlink/helpers.py
+drwxr-xr-x   0 samweinberg   (501) staff       (20)        0 2024-05-29 19:57:44.846685 goldlink_client_python-0.0.5/goldlink_client_python.egg-info/
+-rw-r--r--   0 samweinberg   (501) staff       (20)     1847 2024-05-29 19:57:44.000000 goldlink_client_python-0.0.5/goldlink_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 samweinberg   (501) staff       (20)      745 2024-05-29 19:57:44.000000 goldlink_client_python-0.0.5/goldlink_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 samweinberg   (501) staff       (20)        1 2024-05-29 19:57:44.000000 goldlink_client_python-0.0.5/goldlink_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 samweinberg   (501) staff       (20)       90 2024-05-29 19:57:44.000000 goldlink_client_python-0.0.5/goldlink_client_python.egg-info/requires.txt
+-rw-r--r--   0 samweinberg   (501) staff       (20)       27 2024-05-29 19:57:44.000000 goldlink_client_python-0.0.5/goldlink_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 samweinberg   (501) staff       (20)        0 2024-05-29 19:57:44.846430 goldlink_client_python-0.0.5/integration_tests/
+-rw-r--r--   0 samweinberg   (501) staff       (20)        0 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/integration_tests/__init__.py
+-rw-r--r--   0 samweinberg   (501) staff       (20)      199 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/integration_tests/constants.py
+-rw-r--r--   0 samweinberg   (501) staff       (20)     1144 2024-05-22 16:04:27.000000 goldlink_client_python-0.0.5/integration_tests/test_client.py
+-rw-r--r--   0 samweinberg   (501) staff       (20)       38 2024-05-29 19:57:44.847256 goldlink_client_python-0.0.5/setup.cfg
+-rw-r--r--   0 samweinberg   (501) staff       (20)     1388 2024-05-29 19:57:20.000000 goldlink_client_python-0.0.5/setup.py
```

### Comparing `goldlink_client_python-0.0.4/LICENSE` & `goldlink_client_python-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/PKG-INFO` & `goldlink_client_python-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goldlink-client-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: GoldLink client for borrowing, lending and active management
 Home-page: https://github.com/GoldLink-Protocol/goldlink-client-python
 Author: GoldLink Protocol Inc.
 Author-email: info@goldlink.io
 License: Apache 2.0
 Keywords: goldlink defi arb arbitrum ethereum eth
 Classifier: Intended Audience :: Developers
```

### Comparing `goldlink_client_python-0.0.4/README.md` & `goldlink_client_python-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/abi/erc20.json` & `goldlink_client_python-0.0.5/goldlink/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/abi/gmx-frf-account-getters.json` & `goldlink_client_python-0.0.5/goldlink/abi/gmx-frf-account-getters.json`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/abi/gmx-frf-strategy-account.json` & `goldlink_client_python-0.0.5/goldlink/abi/gmx-frf-strategy-account.json`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/abi/gmx-frf-strategy-manager.json` & `goldlink_client_python-0.0.5/goldlink/abi/gmx-frf-strategy-manager.json`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/abi/gmx_v2_reader.json` & `goldlink_client_python-0.0.5/goldlink/abi/gmx_v2_reader.json`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/abi/strategy-account.json` & `goldlink_client_python-0.0.5/goldlink/abi/strategy-account.json`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/abi/strategy-bank.json` & `goldlink_client_python-0.0.5/goldlink/abi/strategy-bank.json`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/abi/strategy-reserve.json` & `goldlink_client_python-0.0.5/goldlink/abi/strategy-reserve.json`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/constants.py` & `goldlink_client_python-0.0.5/goldlink/constants.py`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/goldlink_client.py` & `goldlink_client_python-0.0.5/goldlink/goldlink_client.py`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink/helpers.py` & `goldlink_client_python-0.0.5/goldlink/helpers.py`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/goldlink_client_python.egg-info/PKG-INFO` & `goldlink_client_python-0.0.5/goldlink_client_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goldlink-client-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: GoldLink client for borrowing, lending and active management
 Home-page: https://github.com/GoldLink-Protocol/goldlink-client-python
 Author: GoldLink Protocol Inc.
 Author-email: info@goldlink.io
 License: Apache 2.0
 Keywords: goldlink defi arb arbitrum ethereum eth
 Classifier: Intended Audience :: Developers
```

### Comparing `goldlink_client_python-0.0.4/goldlink_client_python.egg-info/SOURCES.txt` & `goldlink_client_python-0.0.5/goldlink_client_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/integration_tests/test_client.py` & `goldlink_client_python-0.0.5/integration_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `goldlink_client_python-0.0.4/setup.py` & `goldlink_client_python-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'mpmath==1.0.0',
     'python-dotenv==0.17.1',
     'web3>=5.0.0,<6.0.0',
 ]
 
 setup(
     name='goldlink-client-python',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     package_data={
         'goldlink': [
             'abi/*.json',
         ],
     },
     description='GoldLink client for borrowing, lending and active management',
```

