# Comparing `tmp/evmchains-0.0.8.tar.gz` & `tmp/evmchains-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evmchains-0.0.8.tar", last modified: Mon May 20 15:07:10 2024, max compression
+gzip compressed data, was "evmchains-0.0.9.tar", last modified: Thu May 30 21:13:21 2024, max compression
```

## Comparing `evmchains-0.0.8.tar` & `evmchains-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.545918 evmchains-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.541918 evmchains-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.541918 evmchains-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-20 15:06:53.000000 evmchains-0.0.8/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-20 15:06:53.000000 evmchains-0.0.8/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-20 15:06:53.000000 evmchains-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-20 15:06:53.000000 evmchains-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-20 15:06:53.000000 evmchains-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-05-20 15:07:10.545918 evmchains-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-20 15:06:53.000000 evmchains-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.541918 evmchains-0.0.8/evmchains/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 15:06:53.000000 evmchains-0.0.8/evmchains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    35091 2024-05-20 15:06:53.000000 evmchains-0.0.8/evmchains/chains.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:06:53.000000 evmchains-0.0.8/evmchains/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-20 15:06:53.000000 evmchains-0.0.8/evmchains/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.545918 evmchains-0.0.8/evmchains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-20 15:06:53.000000 evmchains-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.545918 evmchains-0.0.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-20 15:06:53.000000 evmchains-0.0.8/scripts/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-20 15:07:10.545918 evmchains-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 15:06:53.000000 evmchains-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.545918 evmchains-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-20 15:06:53.000000 evmchains-0.0.8/tests/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:13:21.616963 evmchains-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:13:21.612963 evmchains-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:13:21.616963 evmchains-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-30 21:13:06.000000 evmchains-0.0.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-30 21:13:06.000000 evmchains-0.0.9/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-30 21:13:06.000000 evmchains-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-30 21:13:06.000000 evmchains-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-30 21:13:06.000000 evmchains-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-05-30 21:13:21.616963 evmchains-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-30 21:13:06.000000 evmchains-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:13:21.616963 evmchains-0.0.9/evmchains/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-30 21:13:06.000000 evmchains-0.0.9/evmchains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 21:13:21.000000 evmchains-0.0.9/evmchains/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36656 2024-05-30 21:13:06.000000 evmchains-0.0.9/evmchains/chains.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:13:06.000000 evmchains-0.0.9/evmchains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-30 21:13:06.000000 evmchains-0.0.9/evmchains/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:13:21.616963 evmchains-0.0.9/evmchains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-05-30 21:13:21.000000 evmchains-0.0.9/evmchains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-30 21:13:21.000000 evmchains-0.0.9/evmchains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:13:21.000000 evmchains-0.0.9/evmchains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 21:13:21.000000 evmchains-0.0.9/evmchains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 21:13:21.000000 evmchains-0.0.9/evmchains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-30 21:13:06.000000 evmchains-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:13:21.616963 evmchains-0.0.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-30 21:13:06.000000 evmchains-0.0.9/scripts/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-30 21:13:21.620963 evmchains-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 21:13:06.000000 evmchains-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:13:21.616963 evmchains-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-30 21:13:06.000000 evmchains-0.0.9/tests/test_func.py
```

### Comparing `evmchains-0.0.8/.github/workflows/release.yaml` & `evmchains-0.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.8/.github/workflows/test.yaml` & `evmchains-0.0.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.8/.gitignore` & `evmchains-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.8/CONTRIBUTING.md` & `evmchains-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.8/LICENSE` & `evmchains-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.8/PKG-INFO` & `evmchains-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evmchains
-Version: 0.0.8
+Version: 0.0.9
 Summary: Packaged metadata on Ethereum Virtual Machine (EVM) chains
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `evmchains-0.0.8/README.md` & `evmchains-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.8/evmchains/__init__.py` & `evmchains-0.0.9/evmchains/__init__.py`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.8/evmchains/chains.py` & `evmchains-0.0.9/evmchains/chains.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is auto-generated by scripts/update.py
-# 2024-05-17 16:06:29.822636
+# 2024-05-30 20:30:00.884580
 # Do not edit this file directly.
 from typing import Any, Dict
 
 PUBLIC_CHAIN_META: Dict[str, Dict[str, Dict[str, Any]]] = {
     "arbitrum": {
         "mainnet": {
             "chain": "ETH",
@@ -448,14 +448,57 @@
                 "https://rpc.goerli.mudit.blog/",
                 "https://ethereum-goerli-rpc.publicnode.com",
                 "https://goerli.gateway.tenderly.co",
             ],
             "shortName": "gor",
             "slip44": 1,
         },
+        "holesky": {
+            "chain": "ETH",
+            "chainId": 17000,
+            "ens": None,
+            "explorers": [
+                {
+                    "icon": "ethereum",
+                    "name": "Holesky Explorer",
+                    "standard": "EIP3091",
+                    "url": "https://holesky.beaconcha.in",
+                },
+                {
+                    "icon": "ethereum",
+                    "name": "otterscan-holesky",
+                    "standard": "EIP3091",
+                    "url": "https://holesky.otterscan.io",
+                },
+                {
+                    "icon": "ethereum",
+                    "name": "Holesky Etherscan",
+                    "standard": "EIP3091",
+                    "url": "https://holesky.etherscan.io",
+                },
+            ],
+            "faucets": [
+                "https://faucet.holesky.ethpandaops.io",
+                "https://holesky-faucet.pk910.de",
+            ],
+            "features": None,
+            "icon": "ethereum",
+            "infoURL": "https://holesky.ethpandaops.io",
+            "name": "Holesky",
+            "nativeCurrency": {"decimals": 18, "name": "Testnet ETH", "symbol": "ETH"},
+            "networkId": 17000,
+            "rpc": [
+                "https://rpc.holesky.ethpandaops.io",
+                "https://ethereum-holesky-rpc.publicnode.com",
+                "https://holesky.drpc.org",
+                "https://rpc-holesky.rockx.com",
+            ],
+            "shortName": "holesky",
+            "slip44": 1,
+        },
         "sepolia": {
             "chain": "ETH",
             "chainId": 11155111,
             "ens": None,
             "explorers": [
                 {
                     "name": "etherscan-sepolia",
```

### Comparing `evmchains-0.0.8/evmchains.egg-info/PKG-INFO` & `evmchains-0.0.9/evmchains.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evmchains
-Version: 0.0.8
+Version: 0.0.9
 Summary: Packaged metadata on Ethereum Virtual Machine (EVM) chains
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `evmchains-0.0.8/pyproject.toml` & `evmchains-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.8/scripts/update.py` & `evmchains-0.0.9/scripts/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     "bsc": {
         "mainnet": 56,
         "testnet": 97,
     },
     "ethereum": {
         "mainnet": 1,
         "goerli": 5,
+        "holesky": 17000,
         "sepolia": 11155111,
     },
     "fantom": {
         "mainnet": 250,
         "testnet": 4002,
     },
     "gnosis": {
```

### Comparing `evmchains-0.0.8/tests/test_func.py` & `evmchains-0.0.9/tests/test_func.py`

 * *Files identical despite different names*

