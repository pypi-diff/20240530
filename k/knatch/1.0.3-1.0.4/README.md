# Comparing `tmp/knatch-1.0.3.tar.gz` & `tmp/knatch-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knatch-1.0.3.tar", max compression
+gzip compressed data, was "knatch-1.0.4.tar", max compression
```

## Comparing `knatch-1.0.3.tar` & `knatch-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2024-04-16 08:21:57.539971 knatch-1.0.3/LICENSE
--rw-r--r--   0        0        0      160 2024-04-16 08:21:57.539971 knatch-1.0.3/README.md
--rw-r--r--   0        0        0      421 2024-04-16 08:21:57.791971 knatch-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      107 2024-04-16 08:21:57.543971 knatch-1.0.3/src/knatch/__init__.py
--rw-r--r--   0        0        0     2640 2024-04-16 08:21:57.543971 knatch-1.0.3/src/knatch/quarto.py
--rw-r--r--   0        0        0      569 2024-04-16 08:21:57.543971 knatch-1.0.3/src/knatch/utils.py
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 knatch-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-30 07:07:57.607736 knatch-1.0.4/LICENSE
+-rw-r--r--   0        0        0      160 2024-05-30 07:07:57.607736 knatch-1.0.4/README.md
+-rw-r--r--   0        0        0      421 2024-05-30 07:07:57.859738 knatch-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-05-30 07:07:57.607736 knatch-1.0.4/src/knatch/__init__.py
+-rw-r--r--   0        0        0     2640 2024-05-30 07:07:57.607736 knatch-1.0.4/src/knatch/quarto.py
+-rw-r--r--   0        0        0      569 2024-05-30 07:07:57.607736 knatch-1.0.4/src/knatch/utils.py
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 knatch-1.0.4/PKG-INFO
```

### Comparing `knatch-1.0.3/LICENSE` & `knatch-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `knatch-1.0.3/src/knatch/quarto.py` & `knatch-1.0.4/src/knatch/quarto.py`

 * *Files identical despite different names*

### Comparing `knatch-1.0.3/src/knatch/utils.py` & `knatch-1.0.4/src/knatch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import backoff
 import requests
 
 
-@backoff.on_exception(backoff.expo, requests.exceptions.RequestException, max_tries=5)
+@backoff.on_exception(backoff.expo, requests.exceptions.RequestException, max_tries=8)
 def put_with_retries(url, multipart_form_data, token):
   return requests.put(url, headers={"Authorization": f"Bearer {token}"},
                       files=multipart_form_data)
 
 
-@backoff.on_exception(backoff.expo, requests.exceptions.RequestException, max_tries=5)
+@backoff.on_exception(backoff.expo, requests.exceptions.RequestException, max_tries=8)
 def patch_with_retries(url, multipart_form_data, token):
   return requests.patch(url, headers={"Authorization": f"Bearer {token}"},
                         files=multipart_form_data)
```

### Comparing `knatch-1.0.3/PKG-INFO` & `knatch-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: knatch
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: Erik Vattekar
 Author-email: erik.vattekar@nav.no
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # knatch
 
 ## Installasjon
 ```bash
 $ pip install knatch
```

