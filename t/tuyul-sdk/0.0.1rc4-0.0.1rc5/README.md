# Comparing `tmp/tuyul_sdk-0.0.1rc4.tar.gz` & `tmp/tuyul_sdk-0.0.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuyul_sdk-0.0.1rc4.tar", max compression
+gzip compressed data, was "tuyul_sdk-0.0.1rc5.tar", max compression
```

## Comparing `tuyul_sdk-0.0.1rc4.tar` & `tuyul_sdk-0.0.1rc5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      608 2024-05-30 06:51:40.203419 tuyul_sdk-0.0.1rc4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 00:34:07.019714 tuyul_sdk-0.0.1rc4/README.md
--rw-r--r--   0        0        0      735 2024-05-30 03:42:18.398424 tuyul_sdk-0.0.1rc4/tuyul_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.0.1rc4/tuyul_sdk/_certificate/__init__.py
--rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.0.1rc4/tuyul_sdk/_certificate/cacert.pem
--rw-r--r--   0        0        0     8658 2024-05-30 02:19:24.831329 tuyul_sdk-0.0.1rc4/tuyul_sdk/_Cipher.py
--rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.0.1rc4/tuyul_sdk/_Color.py
--rw-r--r--   0        0        0     7153 2024-05-30 06:51:32.411276 tuyul_sdk-0.0.1rc4/tuyul_sdk/_Connection.py
--rw-r--r--   0        0        0     2654 2024-05-30 03:57:45.352001 tuyul_sdk-0.0.1rc4/tuyul_sdk/_Database.py
--rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.0.1rc4/tuyul_sdk/_input.py
--rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.0.1rc4/tuyul_sdk/_Line.py
--rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.0.1rc4/tuyul_sdk/_Log.py
--rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.0.1rc4/tuyul_sdk/_Progress.py
--rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.0.1rc4/tuyul_sdk/_Reset.py
--rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.0.1rc4/tuyul_sdk/_UserAgent.py
--rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.0.1rc4/tuyul_sdk/sql.py
--rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc4/setup.py
--rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc4/PKG-INFO
+-rw-r--r--   0        0        0      608 2024-05-30 07:06:41.466356 tuyul_sdk-0.0.1rc5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 00:34:07.019714 tuyul_sdk-0.0.1rc5/README.md
+-rw-r--r--   0        0        0      726 2024-05-30 07:06:45.616867 tuyul_sdk-0.0.1rc5/tuyul_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.0.1rc5/tuyul_sdk/_certificate/__init__.py
+-rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.0.1rc5/tuyul_sdk/_certificate/cacert.pem
+-rw-r--r--   0        0        0     8658 2024-05-30 02:19:24.831329 tuyul_sdk-0.0.1rc5/tuyul_sdk/_Cipher.py
+-rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.0.1rc5/tuyul_sdk/_Color.py
+-rw-r--r--   0        0        0     7153 2024-05-30 06:51:32.411276 tuyul_sdk-0.0.1rc5/tuyul_sdk/_Connection.py
+-rw-r--r--   0        0        0     2654 2024-05-30 03:57:45.352001 tuyul_sdk-0.0.1rc5/tuyul_sdk/_Database.py
+-rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.0.1rc5/tuyul_sdk/_input.py
+-rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.0.1rc5/tuyul_sdk/_Line.py
+-rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.0.1rc5/tuyul_sdk/_Log.py
+-rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.0.1rc5/tuyul_sdk/_Progress.py
+-rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.0.1rc5/tuyul_sdk/_Reset.py
+-rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.0.1rc5/tuyul_sdk/_UserAgent.py
+-rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.0.1rc5/tuyul_sdk/sql.py
+-rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc5/setup.py
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc5/PKG-INFO
```

### Comparing `tuyul_sdk-0.0.1rc4/pyproject.toml` & `tuyul_sdk-0.0.1rc5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuyul-sdk"
-version = "0.0.1rc4"
+version = "0.0.1rc5"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "tuyul_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `tuyul_sdk-0.0.1rc4/tuyul_sdk/__init__.py` & `tuyul_sdk-0.0.1rc5/tuyul_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from ._input import Input
 from ._Line import Line
 from ._Log import Log
 from ._Progress import ProgressBar, ProgressWait
 from ._Reset import Reset
 from ._UserAgent import UserAgent
 from ._Database import Database, TypeConnection
-Reset()
 import importlib.metadata
 version = importlib.metadata.version('tuyul_sdk')
 from ._Cipher import AES, Password, Salt
 from ._Connection import Connections, ProxyParams, ProxyType, TypeInjector
 
 __all__ = [
     'Color',
```

### Comparing `tuyul_sdk-0.0.1rc4/tuyul_sdk/_certificate/cacert.pem` & `tuyul_sdk-0.0.1rc5/tuyul_sdk/_certificate/cacert.pem`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc4/tuyul_sdk/_Cipher.py` & `tuyul_sdk-0.0.1rc5/tuyul_sdk/_Cipher.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc4/tuyul_sdk/_Connection.py` & `tuyul_sdk-0.0.1rc5/tuyul_sdk/_Connection.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc4/tuyul_sdk/_Database.py` & `tuyul_sdk-0.0.1rc5/tuyul_sdk/_Database.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc4/tuyul_sdk/_Line.py` & `tuyul_sdk-0.0.1rc5/tuyul_sdk/_Line.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc4/tuyul_sdk/_Log.py` & `tuyul_sdk-0.0.1rc5/tuyul_sdk/_Log.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc4/tuyul_sdk/_Progress.py` & `tuyul_sdk-0.0.1rc5/tuyul_sdk/_Progress.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc4/tuyul_sdk/_UserAgent.py` & `tuyul_sdk-0.0.1rc5/tuyul_sdk/_UserAgent.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc4/setup.py` & `tuyul_sdk-0.0.1rc5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'random-user-agent>=1.0.1,<2.0.0',
  'requests>=2.32.3,<3.0.0',
  'sqlalchemy-utils>=0.41.2,<0.42.0',
  'sqlalchemy>=2.0.30,<3.0.0']
 
 setup_kwargs = {
     'name': 'tuyul-sdk',
-    'version': '0.0.1rc4',
+    'version': '0.0.1rc5',
     'description': '',
     'long_description': '',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tuyul_sdk-0.0.1rc4/PKG-INFO` & `tuyul_sdk-0.0.1rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuyul-sdk
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

