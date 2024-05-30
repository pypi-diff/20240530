# Comparing `tmp/ssi-fctrading-2.4.2.tar.gz` & `tmp/ssi-fctrading-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssi-fctrading-2.4.2.tar", last modified: Mon Aug 14 07:12:01 2023, max compression
+gzip compressed data, was "ssi-fctrading-2.5.0.tar", last modified: Thu May 30 06:43:49 2024, max compression
```

## Comparing `ssi-fctrading-2.4.2.tar` & `ssi-fctrading-2.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.112280 ssi-fctrading-2.4.2/
--rw-r--r--   0 root         (0) root         (0)     1188 2023-08-14 07:12:01.112280 ssi-fctrading-2.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      561 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.108280 ssi-fctrading-2.4.2/examples/
--rw-r--r--   0 root         (0) root         (0)       23 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11717 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/examples/fc_client_ex.py
--rw-r--r--   0 root         (0) root         (0)      183 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/examples/fc_config.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/examples/fc_stream_ex.py
--rw-r--r--   0 root         (0) root         (0)      341 2023-08-14 07:12:01.112280 ssi-fctrading-2.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.108280 ssi-fctrading-2.4.2/ssi_fctrading/
--rw-r--r--   0 root         (0) root         (0)      112 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.108280 ssi-fctrading-2.4.2/ssi_fctrading/constant/
--rw-r--r--   0 root         (0) root         (0)       17 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/constant/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/constant/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.108280 ssi-fctrading-2.4.2/ssi_fctrading/core/
--rw-r--r--   0 root         (0) root         (0)       52 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/core/core_crypto.py
--rw-r--r--   0 root         (0) root         (0)      427 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/core/core_helper.py
--rw-r--r--   0 root         (0) root         (0)     7178 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/fc_client.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/fc_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.108280 ssi-fctrading-2.4.2/ssi_fctrading/models/
--rw-r--r--   0 root         (0) root         (0)      665 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/models/AccessTokenModel.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/models/Requests.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/models/Responses.py
--rw-r--r--   0 root         (0) root         (0)      134 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.112280 ssi-fctrading-2.4.2/ssi_fctrading/signalr/
--rw-r--r--   0 root         (0) root         (0)       59 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2155 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/_connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.112280 ssi-fctrading-2.4.2/ssi_fctrading/signalr/events/
--rw-r--r--   0 root         (0) root         (0)       31 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)      550 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/events/_events.py
--rw-r--r--   0 root         (0) root         (0)     2756 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.112280 ssi-fctrading-2.4.2/ssi_fctrading/signalr/hubs/
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/hubs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1638 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/hubs/_hub.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/hubs/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.112280 ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/
--rw-r--r--   0 root         (0) root         (0)       42 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/__init__.py
--rw-r--r--   0 root         (0) root         (0)       51 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/_parameters.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/_queue_events.py
--rw-r--r--   0 root         (0) root         (0)     8064 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/_transport.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/base_transport.py
--rw-r--r--   0 root         (0) root         (0)      132 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/connection.py
--rw-r--r--   0 root         (0) root         (0)     2593 2023-08-14 07:11:58.000000 ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/reconnection.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-14 07:11:59.000000 ssi-fctrading-2.4.2/ssi_fctrading/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 07:12:01.108280 ssi-fctrading-2.4.2/ssi_fctrading.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1188 2023-08-14 07:12:01.000000 ssi-fctrading-2.4.2/ssi_fctrading.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1396 2023-08-14 07:12:01.000000 ssi-fctrading-2.4.2/ssi_fctrading.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-14 07:12:01.000000 ssi-fctrading-2.4.2/ssi_fctrading.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-08-14 07:12:01.000000 ssi-fctrading-2.4.2/ssi_fctrading.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-08-14 07:12:01.000000 ssi-fctrading-2.4.2/ssi_fctrading.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.566558 ssi-fctrading-2.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-30 06:43:49.566558 ssi-fctrading-2.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      561 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.558558 ssi-fctrading-2.5.0/examples/
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14820 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/examples/fc_client_ex.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/examples/fc_config.py
+-rw-r--r--   0 root         (0) root         (0)      849 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/examples/fc_stream_ex.py
+-rw-r--r--   0 root         (0) root         (0)      341 2024-05-30 06:43:49.566558 ssi-fctrading-2.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.558558 ssi-fctrading-2.5.0/ssi_fctrading/
+-rw-r--r--   0 root         (0) root         (0)      112 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.562558 ssi-fctrading-2.5.0/ssi_fctrading/constant/
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/constant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/constant/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.562558 ssi-fctrading-2.5.0/ssi_fctrading/core/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/core/core_crypto.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/core/core_helper.py
+-rw-r--r--   0 root         (0) root         (0)     9706 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/fc_client.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/fc_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.562558 ssi-fctrading-2.5.0/ssi_fctrading/models/
+-rw-r--r--   0 root         (0) root         (0)      665 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/models/AccessTokenModel.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/models/Requests.py
+-rw-r--r--   0 root         (0) root         (0)      191 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/models/Responses.py
+-rw-r--r--   0 root         (0) root         (0)      134 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.562558 ssi-fctrading-2.5.0/ssi_fctrading/signalr/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/_connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.562558 ssi-fctrading-2.5.0/ssi_fctrading/signalr/events/
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      550 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/events/_events.py
+-rw-r--r--   0 root         (0) root         (0)     2756 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.562558 ssi-fctrading-2.5.0/ssi_fctrading/signalr/hubs/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/hubs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/hubs/_hub.py
+-rw-r--r--   0 root         (0) root         (0)      166 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/hubs/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.566558 ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/_queue_events.py
+-rw-r--r--   0 root         (0) root         (0)     8064 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/_transport.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/base_transport.py
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/connection.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2024-05-30 06:43:46.000000 ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/reconnection.py
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-30 06:43:47.000000 ssi-fctrading-2.5.0/ssi_fctrading/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:43:49.562558 ssi-fctrading-2.5.0/ssi_fctrading.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-30 06:43:49.000000 ssi-fctrading-2.5.0/ssi_fctrading.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-05-30 06:43:49.000000 ssi-fctrading-2.5.0/ssi_fctrading.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 06:43:49.000000 ssi-fctrading-2.5.0/ssi_fctrading.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-30 06:43:49.000000 ssi-fctrading-2.5.0/ssi_fctrading.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 06:43:49.000000 ssi-fctrading-2.5.0/ssi_fctrading.egg-info/top_level.txt
```

### Comparing `ssi-fctrading-2.4.2/PKG-INFO` & `ssi-fctrading-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssi-fctrading
-Version: 2.4.2
+Version: 2.5.0
 Summary: FastConnect TradingAPI client by Python
 Home-page: https://github.com/SSI-Securities-Corporation/python-fctrading
 Author: ducdv
 Author-email: ducdv@ssi.com.vn
 License: MIT
 Platform: POSIX
 Platform: Windows
```

### Comparing `ssi-fctrading-2.4.2/README.md` & `ssi-fctrading-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/examples/fc_client_ex.py` & `ssi-fctrading-2.5.0/examples/fc_client_ex.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ssi_fctrading import FCTradingClient
 from ssi_fctrading.models import fcmodel_requests
 from . import fc_config
 from typing import Union
 
-from fastapi import FastAPI
+from fastapi import FastAPI, Depends
 app = FastAPI()
 
 import random
 client = FCTradingClient(fc_config.Url, fc_config.ConsumerID,
 	fc_config.ConsumerSecret, fc_config.PrivateKey, fc_config.TwoFAType)
 print('Read token: ' + client.get_access_token())
 @app.get("/getOtp")
@@ -367,8 +367,100 @@
 	Returns:
 		[str]: json string
 	"""
 	
 	fc_rq = fcmodel_requests.AuditOrderBook(str(account))
 
 	res = client.get_audit_order_book(fc_rq)
-	return res
+	return res
+
+@app.get("/rateLimit")
+async def fc_rateLimit():
+	"""Get ratelimit
+
+	Returns:
+		[str]: json string
+	"""
+	
+	res = client.get_ratelimit()
+	return res
+
+@app.get("/cash/cashInAdvanceAmount", tags=["cash"])
+async def fc_cia_amount(models: fcmodel_requests.CashInAdvanceAmount = Depends()):
+
+	res = client.get_cash_cia_amount(models)
+	return res
+
+@app.get("/cash/unsettleSoldTransaction", tags=["cash"])
+async def fc_cash_unsettleSoldTransaction(models: fcmodel_requests.UnsettleSoldTransaction = Depends()):
+
+	res = client.get_cash_unsettle_sold_transaction(models)
+	return res
+@app.get("/cash/transferHistories", tags=["cash"])
+async def fc_cash_transferHistories(models: fcmodel_requests.CashTransferHistory = Depends()):
+
+	res = client.get_cash_cia_amount(models)
+	return res
+@app.get("/cash/cashInAdvanceHistories", tags=["cash"])
+async def fc_cash_cashInAdvanceHistories(models: fcmodel_requests.CashInAdvanceHistory = Depends()):
+
+	res = client.get_cash_cia_history(models)
+	return res
+@app.get("/cash/estCashInAdvanceFee", tags=["cash"])
+async def fc_cash_estCashInAdvanceFee(models: fcmodel_requests.CashInAdvanceEstFee = Depends()):
+
+	res = client.get_cash_cia_est_fee(models)
+	return res
+@app.post("/cash/vsdCashDW", tags=["cash"])
+async def fc_cash_vsdCashDW(models: fcmodel_requests.CashTransferVSD):
+
+	res = client.create_cash_transfer_vsd(models)
+	return res
+@app.post("/cash/transferInternal", tags=["cash"])
+async def fc_cash_transferInternal(models: fcmodel_requests.CashTransfer):
+
+	res = client.create_cash_transfer(models)
+	return res
+@app.post("/cash/createCashInAdvance", tags=["cash"])
+async def fc_cash_createCashInAdvance(models: fcmodel_requests.CashCIA):
+
+	res = client.create_cia(models)
+	return res
+
+#ORS
+@app.get("/ors/dividend", tags=["online right subscription"])
+async def fc_ors_dividend(models: fcmodel_requests.OrsDividend = Depends()):
+
+	res = client.get_ors_dividend(models)
+	return res
+@app.get("/ors/exercisableQuantity", tags=["online right subscription"])
+async def fc_ors_exercisableQuantity(models: fcmodel_requests.OrsExercisableQuantity = Depends()):
+
+	res = client.get_ors_exercisable_quantity(models)
+	return res
+@app.get("/ors/histories", tags=["online right subscription"])
+async def fc_ors_histories(models: fcmodel_requests.OrsHistory = Depends()):
+
+	res = client.get_ors_history(models)
+	return res
+@app.post("/ors/create", tags=["online right subscription"])
+async def fc_ors_create(models: fcmodel_requests.Ors):
+
+	res = client.create_ors(models)
+	return res
+
+#STOCK
+@app.get("/stock/transferable", tags=["stock"])
+async def fc_stock_exercisableQuantity(models: fcmodel_requests.StockTransferable = Depends()):
+
+	res = client.get_stock_transferable(models)
+	return res
+@app.get("/stock/transferHistories", tags=["stock"])
+async def fc_stock_histories(models: fcmodel_requests.StockTransferHistory = Depends()):
+
+	res = client.get_stock_transfer_history(models)
+	return res
+@app.post("/stock/transfer", tags=["stock"])
+async def fc_stock_create(models: fcmodel_requests.StockTransfer):
+
+	res = client.create_stock_transfer(models)
+	return res
```

### Comparing `ssi-fctrading-2.4.2/examples/fc_stream_ex.py` & `ssi-fctrading-2.5.0/examples/fc_stream_ex.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/setup.py` & `ssi-fctrading-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/core/core_crypto.py` & `ssi-fctrading-2.5.0/ssi_fctrading/core/core_crypto.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/fc_client.py` & `ssi-fctrading-2.5.0/ssi_fctrading/fc_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,15 +28,18 @@
         self._write_access_token: AccessTokenModel = None
         self._read_access_token: AccessTokenModel = None
         self.get_access_token()
 
     def _fc_make_request_get(self, _api_url: str, _request_object: object):
         _headers = self._headers
         _headers["Authorization"] = "Bearer " + self.get_access_token()
-        tapi_response = requests.get(self.url + _api_url , asdict(_request_object), 
+        param = None
+        if _request_object is not None:
+            param = asdict(_request_object)
+        tapi_response = requests.get(self.url + _api_url , param, 
             headers=_headers)
 
         return tapi_response.json()
         
 
     def _fc_make_request_post(self, _api_url: str, _request_object: object):
         payload = json.dumps(dataclasses.asdict(_request_object))
@@ -150,8 +153,51 @@
     def der_cancle_order(self, model: fcmodel_requests.CancelOrder):
         return self._fc_make_request_post(api.FC_DER_CANCEL_ORDER, model)
     
     def get_order_book(self, model: fcmodel_requests.OrderBook):
         return self._fc_make_request_get(api.FC_GET_ORDER_BOOK, model)
     
     def get_audit_order_book(self, model: fcmodel_requests.AuditOrderBook):
-        return self._fc_make_request_get(api.FC_GET_AUDIT_ORDER_BOOK, model)
+        return self._fc_make_request_get(api.FC_GET_AUDIT_ORDER_BOOK, model)
+    
+    def get_ratelimit(self):
+        return self._fc_make_request_get(api.FC_GET_RATELIMIT, None)
+    
+    #CASH
+    def get_cash_cia_amount(self, model: fcmodel_requests.CashInAdvanceAmount):
+        return self._fc_make_request_get(api.FC_CASH_CIA_AMOUNT, model)
+    def get_cash_unsettle_sold_transaction(self, model: fcmodel_requests.UnsettleSoldTransaction):
+        return self._fc_make_request_get(api.FC_CASH_UNSETTLE_SOLD_TRANSACTION, model)
+    def get_cash_transfer_history(self, model: fcmodel_requests.CashTransferHistory):
+        return self._fc_make_request_get(api.FC_CASH_TRANSFER_HISTORY, model)
+    def get_cash_cia_history(self, model: fcmodel_requests.CashInAdvanceHistory):
+        return self._fc_make_request_get(api.FC_CASH_CIA_HISTORY, model)
+    def get_cash_cia_est_fee(self, model: fcmodel_requests.CashInAdvanceEstFee):
+        return self._fc_make_request_get(api.FC_CASH_CIA_EST_FEE, model)
+    
+    def create_cash_transfer_vsd(self, model: fcmodel_requests.CashTransferVSD):
+        return self._fc_make_request_post(api.FC_CASH_VSD_DW, model)
+    def create_cash_transfer(self, model: fcmodel_requests.CashTransfer):
+        return self._fc_make_request_post(api.FC_CASH_TRANSFER, model)
+    def create_cia(self, model: fcmodel_requests.CashCIA):
+        return self._fc_make_request_post(api.FC_CASH_CIA, model)
+    
+    #ONLINE RIGHT SUBSCRIPTION
+    
+    def get_ors_dividend(self, model: fcmodel_requests.OrsDividend):
+        return self._fc_make_request_get(api.FC_ORS_DIVIDEND, model)
+    def get_ors_exercisable_quantity(self, model: fcmodel_requests.OrsExercisableQuantity):
+        return self._fc_make_request_get(api.FC_ORS_EXCERCISABLE_QTY, model)
+    def get_ors_history(self, model: fcmodel_requests.OrsHistory):
+        return self._fc_make_request_get(api.FC_ORS_HISTORY, model)
+    
+    def create_ors(self, model: fcmodel_requests.Ors):
+        return self._fc_make_request_post(api.FC_ORS, model)
+    
+    #STOCK
+    def get_stock_transferable(self, model: fcmodel_requests.StockTransferable):
+        return self._fc_make_request_get(api.FC_STOCK_TRANSFERABLE, model)
+    def get_stock_transfer_history(self, model: fcmodel_requests.StockTransferHistory):
+        return self._fc_make_request_get(api.FC_STOCK_HISTORY, model)
+    
+    def create_stock_transfer(self, model: fcmodel_requests.StockTransfer):
+        return self._fc_make_request_post(api.FC_STOCK_TRANSFER, model)
```

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/fc_stream.py` & `ssi-fctrading-2.5.0/ssi_fctrading/fc_stream.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/models/AccessTokenModel.py` & `ssi-fctrading-2.5.0/ssi_fctrading/models/AccessTokenModel.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/signalr/_connection.py` & `ssi-fctrading-2.5.0/ssi_fctrading/signalr/_connection.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/signalr/events/_events.py` & `ssi-fctrading-2.5.0/ssi_fctrading/signalr/events/_events.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/signalr/helpers.py` & `ssi-fctrading-2.5.0/ssi_fctrading/signalr/helpers.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/signalr/hubs/_hub.py` & `ssi-fctrading-2.5.0/ssi_fctrading/signalr/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/_parameters.py` & `ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/_transport.py` & `ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/base_transport.py` & `ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/base_transport.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading/signalr/transports/reconnection.py` & `ssi-fctrading-2.5.0/ssi_fctrading/signalr/transports/reconnection.py`

 * *Files identical despite different names*

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading.egg-info/PKG-INFO` & `ssi-fctrading-2.5.0/ssi_fctrading.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssi-fctrading
-Version: 2.4.2
+Version: 2.5.0
 Summary: FastConnect TradingAPI client by Python
 Home-page: https://github.com/SSI-Securities-Corporation/python-fctrading
 Author: ducdv
 Author-email: ducdv@ssi.com.vn
 License: MIT
 Platform: POSIX
 Platform: Windows
```

### Comparing `ssi-fctrading-2.4.2/ssi_fctrading.egg-info/SOURCES.txt` & `ssi-fctrading-2.5.0/ssi_fctrading.egg-info/SOURCES.txt`

 * *Files identical despite different names*

