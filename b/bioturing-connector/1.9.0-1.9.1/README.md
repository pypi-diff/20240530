# Comparing `tmp/bioturing_connector-1.9.0.tar.gz` & `tmp/bioturing_connector-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioturing_connector-1.9.0.tar", max compression
+gzip compressed data, was "bioturing_connector-1.9.1.tar", max compression
```

## Comparing `bioturing_connector-1.9.0.tar` & `bioturing_connector-1.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      359 2024-03-12 03:29:03.485486 bioturing_connector-1.9.0/README.md
--rw-r--r--   0        0        0      299 2024-05-20 04:41:06.137549 bioturing_connector-1.9.0/bioturing_connector/__init__.py
--rw-r--r--   0        0        0    23448 2024-03-14 09:22:37.032097 bioturing_connector-1.9.0/bioturing_connector/bbrowserx_connector.py
--rw-r--r--   0        0        0      453 2024-03-12 03:29:03.485486 bioturing_connector-1.9.0/bioturing_connector/common/__init__.py
--rw-r--r--   0        0        0     2935 2024-05-20 01:33:59.237924 bioturing_connector-1.9.0/bioturing_connector/common/common.py
--rw-r--r--   0        0        0       16 2024-03-14 09:22:37.032097 bioturing_connector-1.9.0/bioturing_connector/common/constants.py
--rw-r--r--   0        0        0     2016 2024-05-20 01:53:13.390636 bioturing_connector-1.9.0/bioturing_connector/common/https_agent.py
--rw-r--r--   0        0        0    32724 2024-05-20 10:14:57.609699 bioturing_connector-1.9.0/bioturing_connector/connector.py
--rw-r--r--   0        0        0    14617 2024-03-12 03:29:03.485486 bioturing_connector-1.9.0/bioturing_connector/lens_bulk_connector.py
--rw-r--r--   0        0        0    25947 2024-03-12 03:29:03.485486 bioturing_connector-1.9.0/bioturing_connector/lens_sc_connector.py
--rw-r--r--   0        0        0     1837 2024-03-14 09:22:37.032097 bioturing_connector-1.9.0/bioturing_connector/typing/__init__.py
--rw-r--r--   0        0        0      525 2024-05-20 04:40:52.777031 bioturing_connector-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 bioturing_connector-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0      359 2024-03-12 03:29:03.485486 bioturing_connector-1.9.1/README.md
+-rw-r--r--   0        0        0      299 2024-05-30 03:17:37.095883 bioturing_connector-1.9.1/bioturing_connector/__init__.py
+-rw-r--r--   0        0        0    23448 2024-03-14 09:22:37.032097 bioturing_connector-1.9.1/bioturing_connector/bbrowserx_connector.py
+-rw-r--r--   0        0        0      453 2024-03-12 03:29:03.485486 bioturing_connector-1.9.1/bioturing_connector/common/__init__.py
+-rw-r--r--   0        0        0     2935 2024-05-20 01:33:59.237924 bioturing_connector-1.9.1/bioturing_connector/common/common.py
+-rw-r--r--   0        0        0       16 2024-03-14 09:22:37.032097 bioturing_connector-1.9.1/bioturing_connector/common/constants.py
+-rw-r--r--   0        0        0     2016 2024-05-20 01:53:13.390636 bioturing_connector-1.9.1/bioturing_connector/common/https_agent.py
+-rw-r--r--   0        0        0    32724 2024-05-30 03:16:02.824252 bioturing_connector-1.9.1/bioturing_connector/connector.py
+-rw-r--r--   0        0        0    14617 2024-03-12 03:29:03.485486 bioturing_connector-1.9.1/bioturing_connector/lens_bulk_connector.py
+-rw-r--r--   0        0        0    25947 2024-03-12 03:29:03.485486 bioturing_connector-1.9.1/bioturing_connector/lens_sc_connector.py
+-rw-r--r--   0        0        0     1837 2024-03-14 09:22:37.032097 bioturing_connector-1.9.1/bioturing_connector/typing/__init__.py
+-rw-r--r--   0        0        0      492 2024-05-30 03:17:25.599441 bioturing_connector-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bioturing_connector-1.9.1/PKG-INFO
```

### Comparing `bioturing_connector-1.9.0/bioturing_connector/bbrowserx_connector.py` & `bioturing_connector-1.9.1/bioturing_connector/bbrowserx_connector.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.9.0/bioturing_connector/common/common.py` & `bioturing_connector-1.9.1/bioturing_connector/common/common.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.9.0/bioturing_connector/common/https_agent.py` & `bioturing_connector-1.9.1/bioturing_connector/common/https_agent.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.9.0/bioturing_connector/connector.py` & `bioturing_connector-1.9.1/bioturing_connector/connector.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.9.0/bioturing_connector/lens_bulk_connector.py` & `bioturing_connector-1.9.1/bioturing_connector/lens_bulk_connector.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.9.0/bioturing_connector/lens_sc_connector.py` & `bioturing_connector-1.9.1/bioturing_connector/lens_sc_connector.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.9.0/bioturing_connector/typing/__init__.py` & `bioturing_connector-1.9.1/bioturing_connector/typing/__init__.py`

 * *Files identical despite different names*

