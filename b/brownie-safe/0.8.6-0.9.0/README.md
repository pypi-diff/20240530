# Comparing `tmp/brownie_safe-0.8.6.tar.gz` & `tmp/brownie_safe-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brownie_safe-0.8.6.tar", max compression
+gzip compressed data, was "brownie_safe-0.9.0.tar", max compression
```

## Comparing `brownie_safe-0.8.6.tar` & `brownie_safe-0.9.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    18663 2024-04-10 17:41:39.063300 brownie_safe-0.8.6/brownie_safe.py
--rw-r--r--   0        0        0      539 2024-04-10 17:43:26.928908 brownie_safe-0.8.6/pyproject.toml
--rw-r--r--   0        0        0      910 2023-06-28 16:20:48.160418 brownie_safe-0.8.6/readme.md
--rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 brownie_safe-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0    16415 2024-05-30 13:27:01.023688 brownie_safe-0.9.0/brownie_safe.py
+-rw-r--r--   0        0        0      549 2024-05-30 13:27:01.025712 brownie_safe-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      910 2023-06-28 16:20:48.160418 brownie_safe-0.9.0/readme.md
+-rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 brownie_safe-0.9.0/PKG-INFO
```

### Comparing `brownie_safe-0.8.6/brownie_safe.py` & `brownie_safe-0.9.0/brownie_safe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,156 +1,104 @@
+from abc import ABCMeta
 import os
 import re
-import warnings
 from copy import copy
 from typing import Dict, List, Optional, Union
-from enum import Enum
 import click
-from gnosis.eth import EthereumClient, EthereumNetwork
 from web3 import Web3  # don't move below brownie import
 from brownie import Contract, accounts, chain, history, web3
 from brownie.convert.datatypes import EthAddress
 from brownie.network.account import LocalAccount
 from brownie.network.transaction import TransactionReceipt
-from eth_abi import encode_abi
+from eth_abi import encode
 from eth_utils import is_address, to_checksum_address, encode_hex, keccak
-from gnosis.safe import Safe, SafeOperation
+from gnosis.safe import Safe
+from gnosis.eth import EthereumClient
+from gnosis.safe.safe import SafeV111, SafeV120, SafeV130, SafeV141
+from gnosis.safe.enums import SafeOperationEnum
 from gnosis.safe.multi_send import MultiSend, MultiSendOperation, MultiSendTx
 from gnosis.safe.safe_tx import SafeTx
 from gnosis.safe.signatures import signature_split, signature_to_bytes
 from gnosis.safe.api import TransactionServiceApi
-from gnosis.eth.ethereum_client import EthereumNetworkNotSupported
 from hexbytes import HexBytes
 from trezorlib import ethereum, tools, ui
 from trezorlib.client import TrezorClient
 from trezorlib.messages import EthereumSignMessage
 from trezorlib.transport import get_transport
 from functools import cached_property
 
 
-class EthereumNetworkBackport(Enum):
-    ARBITRUM_ONE = 42161
-    AURORA_MAINNET = 1313161554
-    AVALANCHE_C_CHAIN = 43114
-    BASE = 8453
-    BASE_GOERLI = 84531
-    BINANCE_SMART_CHAIN_MAINNET = 56
-    CELO = 42220
-    ENERGY_WEB_CHAIN = 246
-    GOERLI = 5
-    MAINNET = 1
-    POLYGON = 137
-    OPTIMISM = 10
-    ENERGY_WEB_VOLTA_TESTNET = 73799
-    GNOSIS = 100
-    FANTOM = 250
-    BOBA_NETWORK = 288
-
-
-# MultiSendCallOnly doesn't allow delegatecalls
-# https://github.com/safe-global/safe-deployments/blob/main/src/assets/v1.3.0/multi_send_call_only.json
-DEFAULT_MULTISEND_CALL_ONLY = "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D"
-ALT_MULTISEND_CALL_ONLY = "0xA1dabEF33b3B82c7814B6D82A79e50F4AC44102B"
-CUSTOM_MULTISENDS = {
-    EthereumNetworkBackport.FANTOM: "0x10B62CC1E8D9a9f1Ad05BCC491A7984697c19f7E",
-    EthereumNetworkBackport.OPTIMISM: ALT_MULTISEND_CALL_ONLY,
-    EthereumNetworkBackport.BOBA_NETWORK: ALT_MULTISEND_CALL_ONLY,
-    EthereumNetworkBackport.BASE: ALT_MULTISEND_CALL_ONLY,
-    EthereumNetworkBackport.CELO: ALT_MULTISEND_CALL_ONLY,
-    EthereumNetworkBackport.AVALANCHE_C_CHAIN: ALT_MULTISEND_CALL_ONLY,
-    EthereumNetworkBackport.BASE_GOERLI: ALT_MULTISEND_CALL_ONLY,
-}
-
-class TransactionServiceBackport(TransactionServiceApi):
-    URL_BY_NETWORK = {
-        EthereumNetworkBackport.ARBITRUM_ONE: "https://safe-transaction-arbitrum.safe.global",
-        EthereumNetworkBackport.AURORA_MAINNET: "https://safe-transaction-aurora.safe.global",
-        EthereumNetworkBackport.AVALANCHE_C_CHAIN: "https://safe-transaction-avalanche.safe.global",
-        EthereumNetworkBackport.BASE: "https://safe-transaction-base.safe.global",
-        EthereumNetworkBackport.BASE_GOERLI: "https://safe-transaction-base-testnet.safe.global",
-        EthereumNetworkBackport.BINANCE_SMART_CHAIN_MAINNET: "https://safe-transaction-bsc.safe.global",
-        EthereumNetworkBackport.CELO: "https://safe-transaction-celo.safe.global",
-        EthereumNetworkBackport.ENERGY_WEB_CHAIN: "https://safe-transaction-ewc.safe.global",
-        EthereumNetworkBackport.GOERLI: "https://safe-transaction-goerli.safe.global",
-        EthereumNetworkBackport.MAINNET: "https://safe-transaction-mainnet.safe.global",
-        EthereumNetworkBackport.POLYGON: "https://safe-transaction-polygon.safe.global",
-        EthereumNetworkBackport.OPTIMISM: "https://safe-transaction-optimism.safe.global",
-        EthereumNetworkBackport.ENERGY_WEB_VOLTA_TESTNET: "https://safe-transaction-volta.safe.global",
-        EthereumNetworkBackport.GNOSIS: "https://safe-transaction-gnosis-chain.safe.global",
-        EthereumNetworkBackport.FANTOM: "https://safe-txservice.fantom.network",
-        EthereumNetworkBackport.BOBA_NETWORK: "https://safe-transaction.mainnet.boba.network",
-    }
-
-    def __init__(self, network: EthereumNetwork, ethereum_client: Optional[EthereumClient] = None, base_url: Optional[str] = None):
-        self.network = network
-        self.ethereum_client = ethereum_client
-        self.base_url = base_url or self.URL_BY_NETWORK.get(EthereumNetworkBackport(network.value))
-        if not self.base_url:
-            raise EthereumNetworkNotSupported(network)
-
-
-warnings.filterwarnings('ignore', 'The function signature for resolver.*')
-
-
 class ExecutionFailure(Exception):
     pass
 
 
 class ApiError(Exception):
     pass
 
 
-class BrownieSafe(Safe):
+class ContractWrapper:
+    def __init__(self, account, instance):
+        self.account = account
+        self.instance = instance
 
-    def __init__(self, address, base_url=None, multisend=None):
-        """
-        Create an BrownieSafe from an address or a ENS name and use a default connection.
-        """
-        address = to_checksum_address(address) if is_address(address) else web3.ens.resolve(address)
-        ethereum_client = EthereumClient(web3.provider.endpoint_uri)
-        self.transaction_service = TransactionServiceBackport(ethereum_client.get_network(), ethereum_client, base_url)
-        self.multisend = multisend or CUSTOM_MULTISENDS.get(EthereumNetworkBackport(chain.id), DEFAULT_MULTISEND_CALL_ONLY)
+    def __call__(self, address):
+        address = to_address(address)
+        return Contract(address, owner=self.account)
+    
+    def __getattr__(self, attr):
+        return getattr(self.instance, attr)
+    
+
+def to_address(address):
+    if is_address(address):
+        return to_checksum_address(address)
+    return web3.ens.address(address)
+
+
+class BrownieSafeBase(metaclass=ABCMeta):
+
+    def __init__(self, address, ethereum_client):
         super().__init__(address, ethereum_client)
+        
+        # safe-eth-py shadows the .contract method after 4.3.2
+        # we use a wrapper that satisfies both use cases
+        # 1. web3 safe contract instance using __getattr__
+        # 2. instantiating contract instance with safe as an owner using __call__
+        self.contract = ContractWrapper(self.account, self.contract)
+        
         if self.client == 'anvil':
             web3.manager.request_blocking('anvil_setNextBlockBaseFeePerGas', ['0x0'])
 
     def __str__(self):
         return EthAddress(self.address)
 
     def __repr__(self):
         return f'BrownieSafe("{self.address}")'
 
     @cached_property
     def client(self):
-        client_version = web3.clientVersion
+        client_version = web3.client_version
         match = re.search('(anvil|hardhat|ganache)', client_version.lower())
         return match.group(1) if match else client_version
 
     @property
     def account(self) -> LocalAccount:
         """
         Unlocked Brownie account for Gnosis Safe.
         """
         return accounts.at(self.address, force=True)
 
-    def contract(self, address) -> Contract:
-        """
-        Instantiate a Brownie Contract owned by Safe account.
-        """
-        address = to_checksum_address(address) if is_address(address) else web3.ens.resolve(address)
-        return Contract(address, owner=self.account)
-
     def pending_nonce(self) -> int:
         """
         Subsequent nonce which accounts for pending transactions in the transaction service.
         """
         results = self.transaction_service.get_transactions(self.address)
         return results[0]['nonce'] + 1 if results else 0
 
-    def tx_from_receipt(self, receipt: TransactionReceipt, operation: SafeOperation = SafeOperation.CALL, safe_nonce: int = None) -> SafeTx:
+    def tx_from_receipt(self, receipt: TransactionReceipt, operation: SafeOperationEnum = SafeOperationEnum.CALL, safe_nonce: int = None) -> SafeTx:
         """
         Convert Brownie transaction receipt to a Safe transaction.
         """
         if safe_nonce is None:
             safe_nonce = self.pending_nonce()
 
         return self.build_multisig_tx(receipt.receiver, receipt.value, receipt.input, operation=operation.value, safe_nonce=safe_nonce)
@@ -162,18 +110,16 @@
         if receipts is None:
             receipts = history.from_sender(self.address)
 
         if safe_nonce is None:
             safe_nonce = self.pending_nonce()
 
         txs = [MultiSendTx(MultiSendOperation.CALL, tx.receiver, tx.value, tx.input) for tx in receipts]
-        data = MultiSend(
-            ethereum_client=self.ethereum_client, address=self.multisend
-        ).build_tx_data(txs)
-        return self.build_multisig_tx(self.multisend, 0, data, SafeOperation.DELEGATE_CALL.value, safe_nonce=safe_nonce)
+        data = self.multisend.build_tx_data(txs)
+        return self.build_multisig_tx(self.multisend.address, 0, data, SafeOperationEnum.DELEGATE_CALL.value, safe_nonce=safe_nonce)
 
     def get_signer(self, signer: Optional[Union[LocalAccount, str]] = None) -> LocalAccount:
         if signer is None:
             signer = click.prompt('signer', type=click.Choice(accounts.load()))
 
         if isinstance(signer, str):
             # Avoids a previously impersonated account with no signing capabilities
@@ -288,15 +234,15 @@
         self.transaction_service.post_signatures(safe_tx.safe_tx_hash, signature)
 
     @property
     def pending_transactions(self) -> List[SafeTx]:
         """
         Retrieve pending transactions from the transaction service.
         """
-        results = self.transaction_service._get_request(f'/api/v1/safes/{self.address}/transactions/').json()['results']
+        results = self.transaction_service._get_request(f'/api/v1/safes/{self.address}/multisig-transactions/').json()['results']
         nonce = self.retrieve_nonce()
         transactions = [
             self.build_multisig_tx(
                 to=tx['to'],
                 value=int(tx['value']),
                 data=HexBytes(tx['data'] or b''),
                 operation=tx['operation'],
@@ -324,44 +270,44 @@
     def estimate_gas(self, safe_tx: SafeTx) -> int:
         """
         Estimate gas limit for successful execution.
         """
         return self.estimate_tx_gas(safe_tx.to, safe_tx.value, safe_tx.data, safe_tx.operation)
 
     def set_storage(self, account: str, slot: int, value: int):
-        params = [account, hex(slot), encode_hex(encode_abi(['uint'], [value]))]
+        params = [account, hex(slot), encode_hex(encode(['uint'], [value]))]
         method = {
             'anvil': 'anvil_setStorageAt',
             'hardhat': 'hardhat_setStorageAt',
             'ganache': 'evm_setAccountStorageAt',
         }
         web3.manager.request_blocking(method[self.client], params)
 
     def preview_tx(self, safe_tx: SafeTx, events=True, call_trace=False) -> TransactionReceipt:
         tx = copy(safe_tx)
-        safe = Contract.from_abi('Gnosis Safe', self.address, self.get_contract().abi)
+        safe = Contract.from_abi('Gnosis Safe', self.address, self.contract.abi)
         # Replace pending nonce with the subsequent nonce, this could change the safe_tx_hash
         tx.safe_nonce = safe.nonce()
         # Forge signatures from the needed amount of owners, skip the one which submits the tx
         # Owners must be sorted numerically, sorting as checksum addresses may yield wrong order
         threshold = safe.getThreshold()
         sorted_owners = sorted(safe.getOwners(), key=lambda x: int(x, 16))
         owners = [accounts.at(owner, force=True) for owner in sorted_owners[:threshold]]
         # Signautres are encoded as [bytes32 r, bytes32 s, bytes8 v]
         # Pre-validated signatures are encoded as r=owner, s unused and v=1.
         # https://docs.gnosis.io/safe/docs/contracts_signatures/#pre-validated-signatures
-        tx.signatures = b''.join([encode_abi(['address', 'uint'], [str(owner), 0]) + b'\x01' for owner in owners])
+        tx.signatures = b''.join([encode(['address', 'uint'], [str(owner), 0]) + b'\x01' for owner in owners])
 
         # approvedHashes are in slot 8 and have type of mapping(address => mapping(bytes32 => uint256))
         for owner in owners[:threshold]:
-            outer_key = keccak(encode_abi(['address', 'uint'], [str(owner), 8]))
+            outer_key = keccak(encode(['address', 'uint'], [str(owner), 8]))
             slot = int.from_bytes(keccak(tx.safe_tx_hash + outer_key), 'big')
             self.set_storage(tx.safe_address, slot, 1)
 
-        payload = tx.w3_tx.buildTransaction()
+        payload = tx.w3_tx.build_transaction()
         receipt = owners[0].transfer(payload['to'], payload['value'], gas_limit=payload['gas'], data=payload['data'])
 
         if 'ExecutionSuccess' not in receipt.events:
             receipt.info()
             receipt.call_trace(True)
             raise ExecutionFailure()
 
@@ -381,37 +327,75 @@
             self.preview_pending(events=events, call_trace=call_trace)
         return self.preview_tx(safe_tx, events=events, call_trace=call_trace)
 
     def execute_transaction(self, safe_tx: SafeTx, signer=None) -> TransactionReceipt:
         """
         Execute a fully signed transaction likely retrieved from the pending_transactions method.
         """
-        payload = safe_tx.w3_tx.buildTransaction()
+        payload = safe_tx.w3_tx.build_transaction()
         signer = self.get_signer(signer)
         receipt = signer.transfer(payload['to'], payload['value'], gas_limit=payload['gas'], data=payload['data'])
         return receipt
 
     def execute_transaction_with_frame(self, safe_tx: SafeTx, frame_rpc="http://127.0.0.1:1248") -> bytes:
         """
         Execute a fully signed transaction with frame. Use this option with hardware wallets.
         """
         # Requesting accounts triggers a connection prompt
         frame = Web3(Web3.HTTPProvider(frame_rpc, {'timeout': 600}))
         account = frame.eth.accounts[0]
         frame.manager.request_blocking('wallet_switchEthereumChain', [{'chainId': hex(chain.id)}])
-        payload = safe_tx.w3_tx.buildTransaction()
+        payload = safe_tx.w3_tx.build_transaction()
         tx = {
             "from": account,
             "to": self.address,
             "value": payload["value"],
             "nonce": frame.eth.get_transaction_count(account),
-            "gas": web3.toHex(payload["gas"]),
+            "gas": web3.to_hex(payload["gas"]),
             "data": HexBytes(payload["data"]),
         }
         frame.eth.send_transaction(tx)
 
     def preview_pending(self, events=True, call_trace=False):
         """
         Dry run all pending transactions in a forked environment.
         """
         for safe_tx in self.pending_transactions:
             self.preview_tx(safe_tx, events=events, call_trace=call_trace)
+
+
+class BrownieSafeV111(BrownieSafeBase, SafeV111):
+    pass
+
+class BrownieSafeV120(BrownieSafeBase, SafeV120):
+    pass
+
+class BrownieSafeV130(BrownieSafeBase, SafeV130):
+    pass
+
+class BrownieSafeV141(BrownieSafeBase, SafeV141):
+    pass
+
+
+PATCHED_SAFE_VERSIONS = {
+    '1.1.1': BrownieSafeV111,
+    '1.2.0': BrownieSafeV120,
+    '1.3.0': BrownieSafeV130,
+    '1.4.1': BrownieSafeV141,
+}
+
+
+def BrownieSafe(address, base_url=None, multisend=None):
+    """
+    Create an BrownieSafe from an address or a ENS name and use a default connection.
+    """
+    address = to_address(address)
+    ethereum_client = EthereumClient(web3.provider.endpoint_uri)
+    safe = Safe(address, ethereum_client)
+    version = safe.get_version()
+    
+    brownie_safe = PATCHED_SAFE_VERSIONS[version](address, ethereum_client)
+    brownie_safe.transaction_service = TransactionServiceApi(ethereum_client.get_network(), ethereum_client, base_url)
+    brownie_safe.multisend = MultiSend(ethereum_client, multisend, call_only=True)
+        
+    return brownie_safe
+
```

### Comparing `brownie_safe-0.8.6/pyproject.toml` & `brownie_safe-0.9.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "brownie-safe"
-version = "0.8.6"
+version = "0.9.0"
 description = "Build complex Gnosis Safe transactions and safely preview them in a forked environment."
 authors = ["banteg"]
 license = "MIT"
 repository = "https://github.com/banteg/brownie-safe"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
-eth-brownie = "1.19.2"
-safe-eth-py = "4.3.2"
-trezor = "0.13.7"
+python = ">=3.10,<3.13"
+eth-brownie = ">=1.20.5"
+safe-eth-py = ">=6.0.0b30"
+trezor = ">=0.13.8"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `brownie_safe-0.8.6/readme.md` & `brownie_safe-0.9.0/readme.md`

 * *Files identical despite different names*

### Comparing `brownie_safe-0.8.6/PKG-INFO` & `brownie_safe-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: brownie-safe
-Version: 0.8.6
+Version: 0.9.0
 Summary: Build complex Gnosis Safe transactions and safely preview them in a forked environment.
 Home-page: https://github.com/banteg/brownie-safe
 License: MIT
 Author: banteg
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: eth-brownie (==1.19.2)
-Requires-Dist: safe-eth-py (==4.3.2)
-Requires-Dist: trezor (==0.13.7)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: eth-brownie (>=1.20.5)
+Requires-Dist: safe-eth-py (>=6.0.0b30)
+Requires-Dist: trezor (>=0.13.8)
 Project-URL: Repository, https://github.com/banteg/brownie-safe
 Description-Content-Type: text/markdown
 
 # Brownie Safe: Gnosis Safe tx builder
 
 [Read Documentation](https://safe.ape.tax/)
```

