# Comparing `tmp/tqbus_sdk-0.1.4.tar.gz` & `tmp/tqbus_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tqbus_sdk-0.1.4.tar", max compression
+gzip compressed data, was "tqbus_sdk-0.1.5.tar", max compression
```

## Comparing `tqbus_sdk-0.1.4.tar` & `tqbus_sdk-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      458 2024-02-13 06:18:58.506084 tqbus_sdk-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       12 2023-11-15 21:04:15.502823 tqbus_sdk-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-11-15 18:40:13.714237 tqbus_sdk-0.1.4/tqbus_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-11-13 11:55:42.031309 tqbus_sdk-0.1.4/tqbus_sdk/crm/__init__.py
--rw-r--r--   0        0        0      669 2023-11-15 19:01:56.021570 tqbus_sdk-0.1.4/tqbus_sdk/crm/countries.py
--rw-r--r--   0        0        0     4540 2024-02-06 11:54:17.792232 tqbus_sdk-0.1.4/tqbus_sdk/crm/tqclients.py
--rw-r--r--   0        0        0        0 2023-11-13 18:55:58.789766 tqbus_sdk-0.1.4/tqbus_sdk/gis/__init__.py
--rw-r--r--   0        0        0      782 2023-11-15 19:03:34.374402 tqbus_sdk-0.1.4/tqbus_sdk/gis/endorsements.py
--rw-r--r--   0        0        0      670 2023-11-15 19:03:50.603675 tqbus_sdk-0.1.4/tqbus_sdk/gis/policies.py
--rw-r--r--   0        0        0     5008 2023-11-24 17:32:12.760902 tqbus_sdk-0.1.4/tqbus_sdk/gis/quotations.py
--rw-r--r--   0        0        0        0 2024-02-06 12:05:31.332208 tqbus_sdk-0.1.4/tqbus_sdk/lms/__init__.py
--rw-r--r--   0        0        0      802 2024-02-13 06:17:36.133149 tqbus_sdk-0.1.4/tqbus_sdk/lms/generics.py
--rw-r--r--   0        0        0     5874 2024-02-06 13:08:45.730208 tqbus_sdk-0.1.4/tqbus_sdk/tqsystem.py
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 tqbus_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      472 2024-05-30 10:16:02.866464 tqbus_sdk-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-05-30 09:11:32.888104 tqbus_sdk-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 09:11:32.892145 tqbus_sdk-0.1.5/tqbus_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:11:32.893143 tqbus_sdk-0.1.5/tqbus_sdk/crm/__init__.py
+-rw-r--r--   0        0        0      891 2024-05-30 09:11:32.894145 tqbus_sdk-0.1.5/tqbus_sdk/crm/countries.py
+-rw-r--r--   0        0        0     6530 2024-05-30 09:11:32.894145 tqbus_sdk-0.1.5/tqbus_sdk/crm/tqclients.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:11:32.894145 tqbus_sdk-0.1.5/tqbus_sdk/gis/__init__.py
+-rw-r--r--   0        0        0     1439 2024-05-30 09:11:32.895147 tqbus_sdk-0.1.5/tqbus_sdk/gis/endorsements.py
+-rw-r--r--   0        0        0     1703 2024-05-30 09:11:32.895147 tqbus_sdk-0.1.5/tqbus_sdk/gis/policies.py
+-rw-r--r--   0        0        0     6250 2024-05-30 09:11:32.895147 tqbus_sdk-0.1.5/tqbus_sdk/gis/quotations.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:11:32.896474 tqbus_sdk-0.1.5/tqbus_sdk/lms/__init__.py
+-rw-r--r--   0        0        0     1611 2024-05-30 09:11:32.896474 tqbus_sdk-0.1.5/tqbus_sdk/lms/generics.py
+-rw-r--r--   0        0        0     8793 2024-05-30 09:11:32.896474 tqbus_sdk-0.1.5/tqbus_sdk/tqsystem.py
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 tqbus_sdk-0.1.5/PKG-INFO
```

### Comparing `tqbus_sdk-0.1.4/PKG-INFO` & `tqbus_sdk-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: tqbus-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Rigan Gor
 Author-email: rigan.gor@turnkeyafrica.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: exrex
-Requires-Dist: pydantic (>=2.4.2,<3.0.0)
+Requires-Dist: pydantic (==2.*)
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # tqbus_sdk
```

