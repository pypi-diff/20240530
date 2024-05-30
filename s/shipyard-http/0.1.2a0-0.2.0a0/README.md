# Comparing `tmp/shipyard_http-0.1.2a0.tar.gz` & `tmp/shipyard_http-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_http-0.1.2a0.tar", max compression
+gzip compressed data, was "shipyard_http-0.2.0a0.tar", max compression
```

## Comparing `shipyard_http-0.1.2a0.tar` & `shipyard_http-0.2.0a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.742554 shipyard_http-0.1.2a0/README.md
--rw-r--r--   0        0        0      482 2024-05-30 12:29:35.179457 shipyard_http-0.1.2a0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.743381 shipyard_http-0.1.2a0/shipyard_http/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.743456 shipyard_http-0.1.2a0/shipyard_http/cli/__init__.py
--rw-r--r--   0        0        0     3730 2024-05-30 12:28:19.751765 shipyard_http-0.1.2a0/shipyard_http/cli/download_file.py
--rw-r--r--   0        0        0     3604 2024-04-18 20:05:24.191484 shipyard_http-0.1.2a0/shipyard_http/cli/execute_request.py
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 shipyard_http-0.1.2a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.742554 shipyard_http-0.2.0a0/README.md
+-rw-r--r--   0        0        0      482 2024-04-10 16:43:09.554796 shipyard_http-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.743381 shipyard_http-0.2.0a0/shipyard_http/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.743456 shipyard_http-0.2.0a0/shipyard_http/cli/__init__.py
+-rw-r--r--   0        0        0     3694 2024-04-09 21:08:58.774558 shipyard_http-0.2.0a0/shipyard_http/cli/download_file.py
+-rw-r--r--   0        0        0     3604 2024-04-10 14:36:58.578755 shipyard_http-0.2.0a0/shipyard_http/cli/execute_request.py
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 shipyard_http-0.2.0a0/PKG-INFO
```

### Comparing `shipyard_http-0.1.2a0/shipyard_http/cli/download_file.py` & `shipyard_http-0.2.0a0/shipyard_http/cli/download_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,15 @@
         authentication_headers = json.loads(args.authentication_headers)
     destination_file_name = args.destination_file_name or extract_filename_from_url(url)
     destination_folder_name = shipyard.clean_folder_name(args.destination_folder_name)
     destination_name = shipyard.combine_folder_and_file_name(destination_folder_name, destination_file_name)
     headers = {}
     params = {}
 
-    if destination_folder_name:
-        shipyard.create_folder_if_dne(destination_folder_name)
+    shipyard.create_folder_if_dne(destination_folder_name)
     if custom_headers:
         for key, value in custom_headers.items():
             headers = add_to_headers(headers, key, value)
     if authentication_headers:
         for key, value in custom_headers.items():
             headers = add_to_headers(headers, key, value)
```

### Comparing `shipyard_http-0.1.2a0/shipyard_http/cli/execute_request.py` & `shipyard_http-0.2.0a0/shipyard_http/cli/execute_request.py`

 * *Files identical despite different names*

### Comparing `shipyard_http-0.1.2a0/PKG-INFO` & `shipyard_http-0.2.0a0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-http
-Version: 0.1.2a0
+Version: 0.2.0a0
 Summary: 
 Author: johnathan-rodriguez
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

