# Comparing `tmp/better_web3-4.0.0b8.tar.gz` & `tmp/better_web3-4.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-4.0.0b8.tar", max compression
+gzip compressed data, was "better_web3-4.0.0b9.tar", max compression
```

## Comparing `better_web3-4.0.0b8.tar` & `better_web3-4.0.0b9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      236 2024-05-26 06:57:16.536588 better_web3-4.0.0b8/better_web3/__init__.py
--rw-r--r--   0        0        0     1706 2024-05-25 06:30:15.222893 better_web3-4.0.0b8/better_web3/caip_2.py
--rw-r--r--   0        0        0    11063 2024-05-25 08:31:44.153820 better_web3-4.0.0b8/better_web3/chain.py
--rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b8/better_web3/contract.py
--rw-r--r--   0        0        0     1057 2024-05-26 06:51:13.939678 better_web3-4.0.0b8/better_web3/models.py
--rw-r--r--   0        0        0      343 2024-05-26 06:57:16.529867 better_web3-4.0.0b8/better_web3/utils.py
--rw-r--r--   0        0        0      521 2024-05-26 06:57:28.235630 better_web3-4.0.0b8/pyproject.toml
--rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b8/README.md
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0      236 2024-05-26 06:57:16.536588 better_web3-4.0.0b9/better_web3/__init__.py
+-rw-r--r--   0        0        0     1706 2024-05-25 06:30:15.222893 better_web3-4.0.0b9/better_web3/caip_2.py
+-rw-r--r--   0        0        0    10983 2024-05-26 07:00:02.700832 better_web3-4.0.0b9/better_web3/chain.py
+-rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b9/better_web3/contract.py
+-rw-r--r--   0        0        0     1057 2024-05-26 06:51:13.939678 better_web3-4.0.0b9/better_web3/models.py
+-rw-r--r--   0        0        0      343 2024-05-26 06:57:16.529867 better_web3-4.0.0b9/better_web3/utils.py
+-rw-r--r--   0        0        0      521 2024-05-26 07:00:14.842706 better_web3-4.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b9/README.md
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b9/PKG-INFO
```

### Comparing `better_web3-4.0.0b8/better_web3/caip_2.py` & `better_web3-4.0.0b9/better_web3/caip_2.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b8/better_web3/chain.py` & `better_web3-4.0.0b9/better_web3/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from web3.types import (
     BlockIdentifier,
     Nonce,
     TxParams,
     Wei,
 )
 
-from .utils import tx_url
 from .models import Explorer, NativeCurrency
 
 
 class Chain(AsyncWeb3):
     provider: AsyncHTTPProvider
 
     def __init__(
@@ -100,22 +99,22 @@
         if isinstance(proxy, str):
             self._proxy = Proxy.from_str(proxy)
 
         self.provider._request_kwargs["proxy"] = self._proxy.as_url
 
     def tx_urls(
             self, tx_hash: HexBytes | HexStr | str,
-    ) -> dict[str: str]:  # dict[explorer_name: url]
+    ) -> list[str]:
         if not self.explorers:
             raise ValueError("No explorers")
 
         if isinstance(tx_hash, HexBytes):
             tx_hash = tx_hash.hex()
 
-        return {explorer.name: tx_url(explorer.url, tx_hash) for explorer in self.explorers}
+        return [explorer.tx_url(tx_hash) for explorer in self.explorers]
 
     async def is_eip1559_supported(self) -> bool:
         """
         :return: True if EIP1559 is supported by the node, False otherwise
         """
         last_block = await self.eth.get_block("latest")
         return True if "baseFeePerGas" in last_block else False
```

### Comparing `better_web3-4.0.0b8/better_web3/models.py` & `better_web3-4.0.0b9/better_web3/models.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b8/pyproject.toml` & `better_web3-4.0.0b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "better-web3"
-version = "4.0.0.b8"
+version = "4.0.0.b9"
 description = "Web3 stuff"
 authors = ["Alen <alen.kimov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/alenkimov/better_web3"
 packages = [{include = "better_web3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `better_web3-4.0.0b8/README.md` & `better_web3-4.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b8/PKG-INFO` & `better_web3-4.0.0b9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 4.0.0b8
+Version: 4.0.0b9
 Summary: Web3 stuff
 Home-page: https://github.com/alenkimov/better_web3
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

