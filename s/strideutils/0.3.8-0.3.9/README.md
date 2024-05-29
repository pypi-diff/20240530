# Comparing `tmp/strideutils-0.3.8.tar.gz` & `tmp/strideutils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strideutils-0.3.8.tar", max compression
+gzip compressed data, was "strideutils-0.3.9.tar", max compression
```

## Comparing `strideutils-0.3.8.tar` & `strideutils-0.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1835 2024-05-15 17:08:23.022040 strideutils-0.3.8/README.md
--rw-r--r--   0        0        0     1046 2024-05-15 17:08:23.022040 strideutils-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      373 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/Makefile
--rw-r--r--   0        0        0        0 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/__init__.py
--rw-r--r--   0        0        0     6064 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/coingecko.py
--rw-r--r--   0        0        0     5673 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/config_examples/strideutils_config.yaml.example
--rw-r--r--   0        0        0      443 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/config_examples/strideutils_secrets.yaml.example
--rw-r--r--   0        0        0     1270 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/cryptography.py
--rw-r--r--   0        0        0     1835 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/exec_tx.py
--rw-r--r--   0        0        0     1664 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/invariant_helpers.py
--rw-r--r--   0        0        0     1551 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/run_safely.py
--rw-r--r--   0        0        0     6793 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/sheets_connector.py
--rw-r--r--   0        0        0     1594 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/slack_connector.py
--rw-r--r--   0        0        0     5642 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/stride_alerts.py
--rw-r--r--   0        0        0    13348 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/stride_config.py
--rw-r--r--   0        0        0    42613 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/stride_requests.py
--rw-r--r--   0        0        0     2438 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/stride_upstash.py
--rw-r--r--   0        0        0     1064 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/twilio_connector.py
--rw-r--r--   0        0        0      659 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/types.py
--rw-r--r--   0        0        0        0 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/__init__.pyi
--rw-r--r--   0        0        0      257 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/coingecko.pyi
--rw-r--r--   0        0        0      139 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/cryptography.pyi
--rw-r--r--   0        0        0      511 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/exec_tx.pyi
--rw-r--r--   0        0        0      237 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/invariant_helpers.pyi
--rw-r--r--   0        0        0      290 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/run_safely.pyi
--rw-r--r--   0        0        0      803 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/sheets_connector.pyi
--rw-r--r--   0        0        0      242 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/slack_connector.pyi
--rw-r--r--   0        0        0      987 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/stride_alerts.pyi
--rw-r--r--   0        0        0     4591 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/stride_config.pyi
--rw-r--r--   0        0        0     3977 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/stride_requests.pyi
--rw-r--r--   0        0        0      419 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/stride_upstash.pyi
--rw-r--r--   0        0        0      245 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/twilio_connector.pyi
--rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 strideutils-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1835 2024-05-15 17:53:53.597882 strideutils-0.3.9/README.md
+-rw-r--r--   0        0        0     1046 2024-05-15 17:53:53.597882 strideutils-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      373 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils/Makefile
+-rw-r--r--   0        0        0        0 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils/__init__.py
+-rw-r--r--   0        0        0     6064 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils/coingecko.py
+-rw-r--r--   0        0        0     5673 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils/config_examples/strideutils_config.yaml.example
+-rw-r--r--   0        0        0      443 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils/config_examples/strideutils_secrets.yaml.example
+-rw-r--r--   0        0        0     1270 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/cryptography.py
+-rw-r--r--   0        0        0     1901 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/exec_tx.py
+-rw-r--r--   0        0        0     1664 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/invariant_helpers.py
+-rw-r--r--   0        0        0     1551 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/run_safely.py
+-rw-r--r--   0        0        0     6793 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/sheets_connector.py
+-rw-r--r--   0        0        0     1594 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/slack_connector.py
+-rw-r--r--   0        0        0     5642 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/stride_alerts.py
+-rw-r--r--   0        0        0    13348 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/stride_config.py
+-rw-r--r--   0        0        0    42613 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/stride_requests.py
+-rw-r--r--   0        0        0     2438 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/stride_upstash.py
+-rw-r--r--   0        0        0     1064 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/twilio_connector.py
+-rw-r--r--   0        0        0      659 2024-05-15 17:53:53.601882 strideutils-0.3.9/strideutils/types.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/__init__.pyi
+-rw-r--r--   0        0        0      257 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/coingecko.pyi
+-rw-r--r--   0        0        0      139 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/cryptography.pyi
+-rw-r--r--   0        0        0      511 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/exec_tx.pyi
+-rw-r--r--   0        0        0      237 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/invariant_helpers.pyi
+-rw-r--r--   0        0        0      290 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/run_safely.pyi
+-rw-r--r--   0        0        0      803 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/sheets_connector.pyi
+-rw-r--r--   0        0        0      242 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/slack_connector.pyi
+-rw-r--r--   0        0        0      987 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/stride_alerts.pyi
+-rw-r--r--   0        0        0     4591 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/stride_config.pyi
+-rw-r--r--   0        0        0     3977 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/stride_requests.pyi
+-rw-r--r--   0        0        0      419 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/stride_upstash.pyi
+-rw-r--r--   0        0        0      245 2024-05-15 17:53:53.597882 strideutils-0.3.9/strideutils-stubs/twilio_connector.pyi
+-rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 strideutils-0.3.9/PKG-INFO
```

### Comparing `strideutils-0.3.8/README.md` & `strideutils-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/pyproject.toml` & `strideutils-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strideutils"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 include = ["strideutils", "strideutils-stubs"]
 
 [tool.poetry.dependencies]
 python = ">=3.11"
```

### Comparing `strideutils-0.3.8/strideutils/coingecko.py` & `strideutils-0.3.9/strideutils/coingecko.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/config_examples/strideutils_config.yaml.example` & `strideutils-0.3.9/strideutils/config_examples/strideutils_config.yaml.example`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/cryptography.py` & `strideutils-0.3.9/strideutils/cryptography.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/exec_tx.py` & `strideutils-0.3.9/strideutils/exec_tx.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     tx_hash = ""
     for output_line in standard_out.split('\n'):
         if 'txhash' in output_line:
             tx_hash = output_line.split(': ')[-1]
 
     tx_response = None
     response_success = False
-    raw_log = ""
+    raw_log = "Transaction not found on chain after one minute"  # default message
     if not error_out:
         event_filters = [(f"tx.hash='{tx_hash}'")]
-        for _ in range(15):
+        for _ in range(30):
             time.sleep(2)
             tx_response = stride_requests.get_txs(event_filters, api_endpoint)
             if tx_response['total'] != '0':
                 try:
                     response_code = tx_response['tx_responses'][0]['code']
                     raw_log = tx_response['tx_responses'][0]['raw_log']
                     response_success = response_code == 0
```

### Comparing `strideutils-0.3.8/strideutils/invariant_helpers.py` & `strideutils-0.3.9/strideutils/invariant_helpers.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/run_safely.py` & `strideutils-0.3.9/strideutils/run_safely.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/sheets_connector.py` & `strideutils-0.3.9/strideutils/sheets_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/slack_connector.py` & `strideutils-0.3.9/strideutils/slack_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/stride_alerts.py` & `strideutils-0.3.9/strideutils/stride_alerts.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/stride_config.py` & `strideutils-0.3.9/strideutils/stride_config.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/stride_requests.py` & `strideutils-0.3.9/strideutils/stride_requests.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/stride_upstash.py` & `strideutils-0.3.9/strideutils/stride_upstash.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/twilio_connector.py` & `strideutils-0.3.9/strideutils/twilio_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils/types.py` & `strideutils-0.3.9/strideutils/types.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils-stubs/sheets_connector.pyi` & `strideutils-0.3.9/strideutils-stubs/sheets_connector.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils-stubs/stride_alerts.pyi` & `strideutils-0.3.9/strideutils-stubs/stride_alerts.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils-stubs/stride_config.pyi` & `strideutils-0.3.9/strideutils-stubs/stride_config.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/strideutils-stubs/stride_requests.pyi` & `strideutils-0.3.9/strideutils-stubs/stride_requests.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.8/PKG-INFO` & `strideutils-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strideutils
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

