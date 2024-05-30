# Comparing `tmp/chain_harvester-0.8.2.tar.gz` & `tmp/chain_harvester-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chain_harvester-0.8.2.tar", max compression
+gzip compressed data, was "chain_harvester-0.9.0.tar", max compression
```

## Comparing `chain_harvester-0.8.2.tar` & `chain_harvester-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1073 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/LICENSE
--rw-r--r--   0        0        0      205 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/README.md
--rw-r--r--   0        0        0        0 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/__init__.py
--rw-r--r--   0        0        0    10821 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/chain.py
--rw-r--r--   0        0        0    13902 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/constants.py
--rw-r--r--   0        0        0      632 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/decoders.py
--rw-r--r--   0        0        0     7217 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/multicall.py
--rw-r--r--   0        0        0        0 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/networks/__init__.py
--rw-r--r--   0        0        0        0 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/networks/ethereum/__init__.py
--rw-r--r--   0        0        0     1543 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/networks/ethereum/goerli.py
--rw-r--r--   0        0        0     1470 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/networks/ethereum/mainnet.py
--rw-r--r--   0        0        0        0 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/networks/gnosis/__init__.py
--rw-r--r--   0        0        0     1469 2023-08-30 19:17:53.177004 chain_harvester-0.8.2/chain_harvester/networks/gnosis/mainnet.py
--rw-r--r--   0        0        0     1557 2023-08-30 19:18:13.293019 chain_harvester-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 chain_harvester-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/LICENSE
+-rw-r--r--   0        0        0      205 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/__init__.py
+-rw-r--r--   0        0        0    11385 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/chain.py
+-rw-r--r--   0        0        0    13902 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/constants.py
+-rw-r--r--   0        0        0      632 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/decoders.py
+-rw-r--r--   0        0        0     7217 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/multicall.py
+-rw-r--r--   0        0        0        0 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/networks/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/networks/ethereum/__init__.py
+-rw-r--r--   0        0        0     1543 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/networks/ethereum/goerli.py
+-rw-r--r--   0        0        0     1470 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/networks/ethereum/mainnet.py
+-rw-r--r--   0        0        0        0 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/networks/gnosis/__init__.py
+-rw-r--r--   0        0        0     1469 2023-08-31 20:58:21.230572 chain_harvester-0.9.0/chain_harvester/networks/gnosis/mainnet.py
+-rw-r--r--   0        0        0     1557 2023-08-31 20:58:46.806823 chain_harvester-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 chain_harvester-0.9.0/PKG-INFO
```

### Comparing `chain_harvester-0.8.2/LICENSE` & `chain_harvester-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chain_harvester-0.8.2/chain_harvester/chain.py` & `chain_harvester-0.9.0/chain_harvester/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 import os
 
 import requests
+from eth_utils import event_abi_to_log_topic
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from web3 import Web3
 from web3.middleware import geth_poa_middleware
 
 from chain_harvester.decoders import EventLogDecoder
 from chain_harvester.multicall import Call, Multicall
@@ -293,7 +294,20 @@
         multicalls = []
         for address, function, response in calls:
             multicalls.append(Call(address, function, [response]))
 
         multi = Multicall(multicalls, self.chain_id, _w3=self.w3, block_identifier=block_identifier)
 
         return multi()
+
+    def abi_to_event_topics(self, contract_address, events=None):
+        if events and not isinstance(events, list):
+            raise TypeError("whitelist_events must be a list")
+
+        contract = self.get_contract(contract_address)
+        event_abis = [
+            abi
+            for abi in contract.abi
+            if abi["type"] == "event" and (events is None or abi["name"] in events)
+        ]
+        signed_abis = {event_abi_to_log_topic(abi).hex(): abi for abi in event_abis}
+        return signed_abis
```

### Comparing `chain_harvester-0.8.2/chain_harvester/constants.py` & `chain_harvester-0.9.0/chain_harvester/constants.py`

 * *Files identical despite different names*

### Comparing `chain_harvester-0.8.2/chain_harvester/decoders.py` & `chain_harvester-0.9.0/chain_harvester/decoders.py`

 * *Files identical despite different names*

### Comparing `chain_harvester-0.8.2/chain_harvester/multicall.py` & `chain_harvester-0.9.0/chain_harvester/multicall.py`

 * *Files identical despite different names*

### Comparing `chain_harvester-0.8.2/chain_harvester/networks/ethereum/goerli.py` & `chain_harvester-0.9.0/chain_harvester/networks/ethereum/goerli.py`

 * *Files identical despite different names*

### Comparing `chain_harvester-0.8.2/chain_harvester/networks/ethereum/mainnet.py` & `chain_harvester-0.9.0/chain_harvester/networks/ethereum/mainnet.py`

 * *Files identical despite different names*

### Comparing `chain_harvester-0.8.2/chain_harvester/networks/gnosis/mainnet.py` & `chain_harvester-0.9.0/chain_harvester/networks/gnosis/mainnet.py`

 * *Files identical despite different names*

### Comparing `chain_harvester-0.8.2/pyproject.toml` & `chain_harvester-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chain_harvester"
-version = "v0.8.2"
+version = "v0.9.0"
 description = "A Python library designed to interface with various blockchain networks, enabling the retrieval of data."
 authors = ["0xCommanderKeen <f91289621+0xCommanderKeen@users.noreply.github.com>"]
 repository = "https://github.com/blockanalitica/chain-harvester"
 documentation = "https://blockanalitica.github.io/chain-harvester/"
 readme = "README.md"
 packages = [
   {include = "chain_harvester"}
```

### Comparing `chain_harvester-0.8.2/PKG-INFO` & `chain_harvester-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chain_harvester
-Version: 0.8.2
+Version: 0.9.0
 Summary: A Python library designed to interface with various blockchain networks, enabling the retrieval of data.
 Home-page: https://github.com/blockanalitica/chain-harvester
 Author: 0xCommanderKeen
 Author-email: f91289621+0xCommanderKeen@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

