# Comparing `tmp/strledger-0.7.0.tar.gz` & `tmp/strledger-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strledger-0.7.0.tar", max compression
+gzip compressed data, was "strledger-0.8.0.tar", max compression
```

## Comparing `strledger-0.7.0.tar` & `strledger-0.8.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-23 09:34:52.502126 strledger-0.7.0/LICENSE
--rw-r--r--   0        0        0     1176 2024-05-07 09:21:50.097703 strledger-0.7.0/README.md
--rw-r--r--   0        0        0     1405 2024-05-07 09:21:50.098181 strledger-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      120 2024-05-07 09:21:50.098639 strledger-0.7.0/strledger/__init__.py
--rw-r--r--   0        0        0    10505 2024-05-07 09:21:50.099037 strledger-0.7.0/strledger/cli.py
--rw-r--r--   0        0        0     7836 2024-05-07 09:21:50.099451 strledger-0.7.0/strledger/core.py
--rw-r--r--   0        0        0        0 2024-04-23 09:34:52.506030 strledger-0.7.0/strledger/py.typed
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 strledger-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-30 10:21:00.383647 strledger-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1177 2024-05-30 10:21:00.383647 strledger-0.8.0/README.md
+-rw-r--r--   0        0        0     1407 2024-05-30 10:21:00.387647 strledger-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-30 10:21:00.387647 strledger-0.8.0/strledger/__init__.py
+-rw-r--r--   0        0        0     9620 2024-05-30 10:21:00.387647 strledger-0.8.0/strledger/cli.py
+-rw-r--r--   0        0        0    10025 2024-05-30 10:21:00.387647 strledger-0.8.0/strledger/core.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:21:00.387647 strledger-0.8.0/strledger/py.typed
+-rw-r--r--   0        0        0     2458 1970-01-01 00:00:00.000000 strledger-0.8.0/PKG-INFO
```

### Comparing `strledger-0.7.0/LICENSE` & `strledger-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strledger-0.7.0/README.md` & `strledger-0.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# strledger - Sign Stellar Transaction with Ledger on the command line.
+# strledger - Ledger Hardware Wallet Stellar Python bindings.
 
 ![example](https://github.com/lightsail-network/strledger/blob/main/img/example.png)
 
 ## Installation
 ```shell
 pip install -U strledger
 ```
 
 ## Cli Usage
 ```text
 Usage: strledger [OPTIONS] COMMAND [ARGS]...
 
   Stellar Ledger commands.
 
-  This project is built on the basis of ledgerctl, you can check ledgerctl for
+  This project is built on the basis of ledgerwallet, you can check ledgerwallet for
   more features.
 
 Options:
   -v, --verbose  Display exchanged APDU.
   --help         Show this message and exit.
 
 Commands:
-  app-info      Get Stellar app info.
-  get-address   Get Stellar public address.
-  sign-auth     Sign a base64-encoded soroban authorization...
-  sign-tx       Sign a base64-encoded transaction envelope.
-  sign-tx-hash  Sign a hex encoded hash.
-  version       Get strledger version info.
+  app-info     Get Stellar app configuration info.
+  get-address  Get Stellar public address.
+  sign-auth    Sign a base64-encoded soroban authorization (HashIDPreimage).
+  sign-hash    Sign a hex encoded hash.
+  sign-tx      Sign a base64-encoded transaction envelope.
+  version      Get strledger version info.
 ```
 
 ## Library Usage
 
 ```python
-from strledger import get_default_client
+from strledger import StrLedger
 
-client = get_default_client()
+client = StrLedger()
 # Use the Stellar Python SDK to build a transaction, see https://github.com/StellarCN/py-stellar-base
 transaction_envelope = ...
 client.sign_transaction(transaction_envelope=transaction_envelope, keypair_index=0)
 print(f"signed tx: {transaction_envelope.to_xdr()}")
 ```
```

### Comparing `strledger-0.7.0/pyproject.toml` & `strledger-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "strledger"
-version = "0.7.0"
-description = "Sign Stellar Transaction with Ledger on the command line."
+version = "0.8.0"
+description = "Ledger Hardware Wallet Stellar Python bindings."
 authors = ["overcat <4catcode@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/lightsail-network/strledger"
 repository = "https://github.com/lightsail-network/strledger"
 documentation = "https://github.com/lightsail-network/strledger"
 keywords = ["stellar", "ledger"]
@@ -14,30 +14,32 @@
     "Development Status :: 4 - Beta",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/lightsail-network/strledger/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 click = "^8.1.7"
-stellar-sdk = { version = ">=9,<10" }
+stellar-sdk = { version = ">=9,<11" }
 ledgerwallet = "^0.4.0"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.2.1"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 strledger = "strledger.cli:cli"
```

### Comparing `strledger-0.7.0/strledger/cli.py` & `strledger-0.8.0/strledger/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,145 @@
 import base64
 import sys
-from typing import Callable, Any
+from typing import Callable, Any, Union
 from urllib.parse import urljoin
 
 import click
+
 from ledgerwallet import __version__ as ledger_wallet_version
 from ledgerwallet import utils
-from ledgerwallet.client import CommException
 from stellar_sdk import (
     DecoratedSignature,
     Network,
     parse_transaction_envelope_from_xdr,
     Server,
     TransactionEnvelope,
     FeeBumpTransactionEnvelope,
 )
 from stellar_sdk.xdr import HashIDPreimage
 from stellar_sdk.exceptions import BaseRequestError
 from stellar_sdk import __version__ as stellar_sdk_version
 from strledger import __issue__
 from strledger import __version__ as strledger_version
 from strledger.core import (
-    SW,
     StrLedger,
     DEFAULT_KEYPAIR_INDEX,
-    get_default_client,
     DeviceNotFoundException,
+    BaseError,
 )
 from stellar_sdk.utils import sha256
 
-_DEFAULT_HORIZON_SERVER_URL = "https://horizon.stellar.org"
+DEFAULT_HORIZON_SERVER_URL = "https://horizon.stellar.org"
+DEFAULT_NETWORK_PASSPHRASE = Network.PUBLIC_NETWORK_PASSPHRASE
+TESTNET_NETWORK_PASSPHRASE = Network.TESTNET_NETWORK_PASSPHRASE
 
 
 def echo_normal(message: str) -> None:
     click.echo(message)
 
 
 def echo_success(message: str) -> None:
     click.echo(click.style(message, fg="green"))
 
 
 def echo_error(message: Any) -> None:
     click.echo(click.style(message, fg="red"), err=True)
 
 
+def parse_xdr(
+    xdr: str, network_passphrase: str
+) -> Union[TransactionEnvelope, FeeBumpTransactionEnvelope]:
+    try:
+        return parse_transaction_envelope_from_xdr(
+            xdr=xdr, network_passphrase=network_passphrase
+        )
+    except Exception:
+        echo_error(
+            "Failed to parse XDR.\n"
+            "Make sure to pass a valid base64-encoded transaction envelope.\n"
+            "You can check whether the data you submitted is valid "
+            "through XDR Viewer - https://laboratory.stellar.org/#xdr-viewer"
+        )
+        sys.exit(1)
+
+
+def parse_soroban_auth(xdr: str) -> HashIDPreimage:
+    try:
+        return HashIDPreimage.from_xdr(xdr)
+    except Exception:
+        echo_error(
+            "Failed to parse XDR.\n"
+            "Make sure to pass a valid base64-encoded soroban authorization."
+        )
+        sys.exit(1)
+
+
+def submit_transaction(
+    te: Union[TransactionEnvelope, FeeBumpTransactionEnvelope], horizon_url: str
+) -> None:
+    echo_normal("Submitting to the network...")
+    server = Server(horizon_url)
+    try:
+        server.submit_transaction(te)
+    except BaseRequestError as e:
+        echo_error("Submit failed, error info:")
+        echo_error(e)
+        sys.exit(1)
+
+    echo_success("Successfully submitted.")
+    tx_hash = te.hash_hex()
+    if te.network_passphrase == Network.PUBLIC_NETWORK_PASSPHRASE:
+        url = f"https://stellar.expert/explorer/public/tx/{tx_hash}"
+    elif te.network_passphrase == Network.TESTNET_NETWORK_PASSPHRASE:
+        url = f"https://stellar.expert/explorer/testnet/tx/{tx_hash}"
+    else:
+        url = urljoin(horizon_url, f"/transactions/{tx_hash}")
+    echo_success(f"Stellar Explorer: {url}")
+
+
 @click.group()
 @click.option("-v", "--verbose", is_flag=True, help="Display exchanged APDU.")
 @click.pass_context
 def cli(ctx, verbose):
     """Stellar Ledger commands.
 
-    This project is built on the basis of ledgerctl,
-    you can check ledgerctl for more features.
+    This project is built on the basis of ledgerwallet,
+    you can check ledgerwallet for more features.
     """
-
     if verbose:
         utils.enable_apdu_log()
 
     def get_client() -> StrLedger:
         try:
-            return get_default_client()
+            return StrLedger()
         except DeviceNotFoundException:
             echo_error("No Ledger device has been found.")
             sys.exit(1)
 
     ctx.obj = get_client
 
 
 @cli.command(name="app-info")
 @click.pass_obj
 def get_app_info(get_client: Callable[[], StrLedger]) -> None:
-    """Get Stellar app info."""
+    """Get Stellar app configuration info."""
     client = get_client()
     data = client.get_app_info()
     echo_success(f"Stellar App Version: {data.version}")
     enabled = "Yes" if data.hash_signing_enabled else "No"
     echo_success(f"Hash Signing Enabled: {enabled}")
+    if data.max_data_size is not None:
+        echo_success(f"Max Data Size: {data.max_data_size} bytes")
 
 
 @cli.command(name="sign-tx")
 @click.option(
     "-n",
     "--network-passphrase",
-    default=Network.PUBLIC_NETWORK_PASSPHRASE,
+    default=DEFAULT_NETWORK_PASSPHRASE,
     required=False,
     help="Network passphrase (blank for public network).",
 )
 @click.option(
     "-i",
     "--keypair-index",
     type=int,
@@ -104,46 +157,31 @@
 @click.option("-s", "--submit", is_flag=True, help="Submit to Stellar Network.")
 @click.option(
     "-u",
     "--horizon-url",
     type=str,
     required=False,
     help="Horizon Server URL.",
-    default=_DEFAULT_HORIZON_SERVER_URL,
+    default=DEFAULT_HORIZON_SERVER_URL,
     show_default=True,
 )
 @click.argument("transaction_envelope")
 @click.pass_obj
 def sign_transaction(
     get_client: Callable[[], StrLedger],
     network_passphrase: str,
     transaction_envelope: str,
     keypair_index: int,
     hash_signing: bool,
     submit: bool,
     horizon_url: str,
 ):
-    """Sign a base64-encoded transaction envelope.
-
-    For testnet transactions, use the following network passphrase:
-    'Test SDF Network ; September 2015'
-    """
+    """Sign a base64-encoded transaction envelope."""
     client = get_client()
-    try:
-        te = parse_transaction_envelope_from_xdr(
-            xdr=transaction_envelope, network_passphrase=network_passphrase
-        )
-    except Exception:
-        echo_error(
-            "Failed to parse XDR.\n"
-            "Make sure to pass a valid base64-encoded transaction envelope.\n"
-            "You can check whether the data you submitted is valid "
-            "through XDR Viewer - https://laboratory.stellar.org/#xdr-viewer"
-        )
-        sys.exit(1)
+    te = parse_xdr(transaction_envelope, network_passphrase)
 
     tx_hash = te.hash_hex()
     echo_normal(f"Network Passphrase: {network_passphrase}")
     echo_normal(f"Transaction Hash: {tx_hash}")
     echo_normal("Please confirm the transaction on Ledger.")
 
     try:
@@ -152,92 +190,54 @@
             keypair = client.get_keypair(keypair_index=keypair_index)
             decorated_signature = DecoratedSignature(
                 keypair.signature_hint(), signature
             )
             te.signatures.append(decorated_signature)
         else:
             assert isinstance(te, (TransactionEnvelope, FeeBumpTransactionEnvelope))
-            client.sign_transaction(
+            te = client.sign_transaction(
                 transaction_envelope=te, keypair_index=keypair_index
             )
-    except CommException as e:
-        if hash_signing and e.sw == SW.TX_HASH_SIGNING_MODE_NOT_ENABLED:
-            echo_error(
-                "Hash signing is not enabled on this device.\n"
-                "Please enable it on the device and try again."
-            )
-        elif e.sw == SW.DENY:
-            echo_error("The request to sign the transaction was denied.")
-        elif e.sw == SW.SW_REQUEST_DATA_TOO_LARGE:
-            echo_error(
-                "The request data is too large, please try to sign a smaller transaction, or sign the hash only."
-            )
-        else:
-            echo_error(
-                f"Unknown exception, you can report the problem here: {__issue__}"
-            )
-            raise
+    except BaseError as e:
+        echo_error(e)
         sys.exit(1)
-
+    except Exception as e:
+        echo_error(f"Unknown exception, you can report the problem here: {__issue__}")
+        raise e
     echo_success("Signed successfully.")
     echo_success("Base64-encoded signed transaction envelope:")
     echo_success(te.to_xdr())
 
     if submit:
-        echo_normal("Submitting to the network...")
-        server = Server(horizon_url)
-        try:
-            server.submit_transaction(te)
-        except BaseRequestError as e:
-            echo_error("Submit failed, error info:")
-            echo_error(e)
-            sys.exit(1)
-
-        echo_success("Successfully submitted.")
-        if network_passphrase == Network.PUBLIC_NETWORK_PASSPHRASE:
-            url = f"https://stellar.expert/explorer/public/tx/{tx_hash}"
-        elif network_passphrase == Network.TESTNET_NETWORK_PASSPHRASE:
-            url = f"https://stellar.expert/explorer/testnet/tx/{tx_hash}"
-        else:
-            url = urljoin(horizon_url, f"/transactions/{tx_hash}")
-        echo_success(f"Stellar Explorer: {url}")
+        submit_transaction(te, horizon_url)
 
 
 @cli.command(name="sign-hash")
 @click.option(
     "-i",
     "--keypair-index",
     type=int,
     required=False,
     help="Keypair Index.",
     default=DEFAULT_KEYPAIR_INDEX,
     show_default=True,
 )
 @click.argument("hash")
 @click.pass_obj
-def sign_hash(
-    get_client: Callable[[], StrLedger],
-    hash: str,
-    keypair_index: int,
-):
+def sign_hash(get_client: Callable[[], StrLedger], hash: str, keypair_index: int):
     """Sign a hex encoded hash."""
     client = get_client()
     try:
         signature = client.sign_hash(hash, keypair_index)
-    except CommException as e:
-        if e.sw == SW.TX_HASH_SIGNING_MODE_NOT_ENABLED:
-            echo_error(
-                "Hash signing is not enabled on this device.\n"
-                "Please enable it on the device and try again."
-            )
-        elif e.sw == SW.DENY:
-            echo_error("The request to sign the transaction hash was denied.")
-        else:
-            raise e
+    except BaseError as e:
+        echo_error(e)
         sys.exit(1)
+    except Exception as e:
+        echo_error(f"Unknown exception, you can report the problem here: {__issue__}")
+        raise e
     signature_base64 = base64.b64encode(signature).decode()
     echo_success(signature_base64)
 
 
 @cli.command(name="get-address")
 @click.option(
     "-i",
@@ -253,20 +253,20 @@
 def get_address(
     get_client: Callable[[], StrLedger], keypair_index: int, confirm: bool
 ) -> None:
     """Get Stellar public address."""
     client = get_client()
     try:
         keypair = client.get_keypair(keypair_index, confirm)
-    except CommException as e:
-        if e.sw == SW.DENY:
-            echo_error("The request to confirm the address was denied.")
-            sys.exit(1)
-        else:
-            raise e
+    except BaseError as e:
+        echo_error(e)
+        sys.exit(1)
+    except Exception as e:
+        echo_error(f"Unknown exception, you can report the problem here: {__issue__}")
+        raise e
     echo_success(keypair.public_key)
 
 
 @cli.command(name="sign-auth")
 @click.option(
     "-i",
     "--keypair-index",
@@ -288,52 +288,33 @@
     get_client: Callable[[], StrLedger],
     keypair_index: int,
     hash_signing: bool,
     soroban_authorization: str,
 ):
     """Sign a base64-encoded soroban authorization (HashIDPreimage)."""
     client = get_client()
-    try:
-        auth = HashIDPreimage.from_xdr(soroban_authorization)
-    except Exception:
-        echo_error(
-            "Failed to parse XDR.\n"
-            "Make sure to pass a valid base64-encoded soroban authorization."
-        )
-        sys.exit(1)
+    auth = parse_soroban_auth(soroban_authorization)
 
     preimage_hash = sha256(auth.to_xdr_bytes()).hex()
     echo_normal(f"HashIDPreimage Hash: {preimage_hash}")
     echo_normal("Please confirm the Soroban authorization on Ledger.")
 
     try:
         if hash_signing:
             signature = client.sign_hash(preimage_hash, keypair_index)
         else:
             signature = client.sign_soroban_authorization(
                 auth, keypair_index=keypair_index
             )
-    except CommException as e:
-        if hash_signing and e.sw == SW.TX_HASH_SIGNING_MODE_NOT_ENABLED:
-            echo_error(
-                "Hash signing is not enabled on this device.\n"
-                "Please enable it on the device and try again."
-            )
-        elif e.sw == SW.DENY:
-            echo_error("The request to sign the Soroban authorization was denied.")
-        elif e.sw == SW.SW_REQUEST_DATA_TOO_LARGE:
-            echo_error(
-                "The request data is too large, please try to sign a Soroban authorization, or sign the hash only."
-            )
-        else:
-            echo_error(
-                f"Unknown exception, you can report the problem here: {__issue__}"
-            )
-            raise
+    except BaseError as e:
+        echo_error(e)
         sys.exit(1)
+    except Exception as e:
+        echo_error(f"Unknown exception, you can report the problem here: {__issue__}")
+        raise e
 
     echo_success("Signed successfully.")
     echo_success("Base64-encoded signature:")
     echo_success(base64.b64encode(signature).decode())
 
 
 @cli.command(name="version")
```

### Comparing `strledger-0.7.0/strledger/core.py` & `strledger-0.8.0/strledger/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import binascii
+import copy
 import dataclasses
 from enum import IntEnum
 from typing import Optional, Union
 
-from ledgerwallet.client import LedgerClient
+from ledgerwallet.client import LedgerClient, CommException
 from ledgerwallet.params import Bip32Path
 from ledgerwallet.transport import enumerate_devices
 from stellar_sdk import (
     Keypair,
     TransactionEnvelope,
     DecoratedSignature,
     FeeBumpTransactionEnvelope,
 )
 from stellar_sdk.xdr import HashIDPreimage, EnvelopeType
 
 __all__ = [
-    "get_default_client",
-    "DeviceNotFoundException",
-    "DEFAULT_KEYPAIR_INDEX",
-    "Ins",
-    "P1",
-    "P2",
-    "SW",
-    "AppInfo",
     "StrLedger",
+    "BaseError",
+    "DeviceNotFoundException",
+    "HashSigningNotEnabledError",
+    "UserRefusedError",
+    "DataParsingFailedError",
+    "RequestDataTooLargeError",
 ]
 
+APDU_MAX_PAYLOAD = 255
 DEFAULT_KEYPAIR_INDEX = 0
 
 
 class Ins(IntEnum):
     """Instruction enum for APDU commands."""
 
     GET_PK = 0x02
@@ -61,76 +61,64 @@
 
     See https://github.com/lightsail-network/app-stellar/blob/develop/docs/COMMANDS.md#status-words
     """
 
     # Status word for denied by user.
     DENY = 0x6985
     # Status word for hash signing model not enabled.
-    TX_HASH_SIGNING_MODE_NOT_ENABLED = 0x6C66
+    HASH_SIGNING_MODE_NOT_ENABLED = 0x6C66
     # Status word for data too large.
-    SW_REQUEST_DATA_TOO_LARGE = 0x6C67
+    REQUEST_DATA_TOO_LARGE = 0xB004
+    # Status word for data parsing fail.
+    DATA_PARSING_FAIL = 0xB005
     # Status word for success.
     OK = 0x9000
 
 
-class DeviceNotFoundException(Exception):
-    """Exception raised when no Ledger device is found."""
-
-    pass
-
-
-def get_default_client() -> "StrLedger":
-    """Get the default Ledger client.
-
-    Returns:
-        StrLedger: The default Ledger client instance.
-
-    Raises:
-        DeviceNotFoundException: If no Ledger device is found.
-    """
-    devices = enumerate_devices()
-    if len(devices) == 0:
-        raise DeviceNotFoundException
-    client = LedgerClient(devices[0])
-    return StrLedger(client)
-
-
 @dataclasses.dataclass
-class AppInfo:
+class AppConfiguration:
     """App configuration information."""
 
     version: str
     """The version of the app."""
     hash_signing_enabled: bool
     """Whether hash signing is enabled."""
+    max_data_size: Optional[int] = None
+    """The maximum data size in bytes that the device can sign"""
 
 
 class StrLedger:
     """Stellar Ledger client class."""
 
-    def __init__(self, client: LedgerClient) -> None:
+    def __init__(self, client: LedgerClient = None) -> None:
         """Initialize the Stellar Ledger client.
 
         Args:
-            client (LedgerClient): The Ledger client instance.
+            client (LedgerClient): The Ledger client instance, or None to use the default client.
         """
+        if client is None:
+            client = _get_default_client()
         self.client = client
 
-    def get_app_info(self) -> AppInfo:
+    def get_app_info(self) -> AppConfiguration:
         """Get the app configuration information.
 
         Returns:
-            AppInfo: The app configuration information.
+            AppConfiguration: The app configuration information.
         """
-        data = self.client.apdu_exchange(
-            ins=Ins.GET_CONF, p1=P1.FIRST_APDU, p2=P2.LAST_APDU
+        data = self._send_payload(Ins.GET_CONF, b"")
+        hash_signing_enabled = data[0] == 0x01
+        major, minor, patch = data[1], data[2], data[3]
+        version = f"{major}.{minor}.{patch}"
+        max_data_size = (data[4] << 8 | data[5]) if len(data) > 4 else None
+        return AppConfiguration(
+            version=version,
+            hash_signing_enabled=hash_signing_enabled,
+            max_data_size=max_data_size,
         )
-        hash_signing_enabled = bool(data[0])
-        version = f"{data[1]}.{data[2]}.{data[3]}"
-        return AppInfo(version=version, hash_signing_enabled=hash_signing_enabled)
 
     def get_keypair(
         self,
         keypair_index: int = DEFAULT_KEYPAIR_INDEX,
         confirm_on_device: bool = False,
     ) -> Keypair:
         """Get the public key for the specified keypair index.
@@ -139,43 +127,51 @@
             keypair_index (int): The keypair index (default is 0).
             confirm_on_device (bool): Whether to confirm the action on the device (default is False).
 
         Returns:
             Keypair: The keypair instance.
         """
         path = Bip32Path.build(f"44'/148'/{keypair_index}'")
-        data = self.client.apdu_exchange(
-            ins=Ins.GET_PK,
-            data=path,
-            p1=P1.NONE,
-            p2=P2.CONFIRM if confirm_on_device else P2.NON_CONFIRM,
-        )
+        try:
+            data = self.client.apdu_exchange(
+                ins=Ins.GET_PK,
+                data=path,
+                p1=P1.NONE,
+                p2=P2.CONFIRM if confirm_on_device else P2.NON_CONFIRM,
+            )
+        except CommException as e:
+            raise _remap_error(e) from e
         keypair = Keypair.from_raw_ed25519_public_key(data)
         return keypair
 
     def sign_transaction(
         self,
         transaction_envelope: Union[TransactionEnvelope, FeeBumpTransactionEnvelope],
         keypair_index: int = DEFAULT_KEYPAIR_INDEX,
-    ) -> None:
+    ) -> Union[TransactionEnvelope, FeeBumpTransactionEnvelope]:
         """Sign a transaction envelope.
 
         Args:
             transaction_envelope (Union[TransactionEnvelope, FeeBumpTransactionEnvelope]): The transaction envelope to sign.
             keypair_index (int): The keypair index (default is 0).
+
+        Returns:
+            Union[TransactionEnvelope, FeeBumpTransactionEnvelope]: The signed transaction envelope.
         """
         sign_data = transaction_envelope.signature_base()
         keypair = self.get_keypair(keypair_index=keypair_index)
 
         path = Bip32Path.build(f"44'/148'/{keypair_index}'")
         payload = path + sign_data
         signature = self._send_payload(Ins.SIGN_TX, payload)
         assert isinstance(signature, bytes)
         decorated_signature = DecoratedSignature(keypair.signature_hint(), signature)
-        transaction_envelope.signatures.append(decorated_signature)
+        copy_transaction_envelope = copy.deepcopy(transaction_envelope)
+        copy_transaction_envelope.signatures.append(decorated_signature)
+        return copy_transaction_envelope
 
     def sign_hash(
         self,
         transaction_hash: Union[str, bytes],
         keypair_index: int = DEFAULT_KEYPAIR_INDEX,
     ) -> bytes:
         """Sign a transaction hash.
@@ -187,19 +183,16 @@
         Returns:
             bytes: The signature.
         """
         if isinstance(transaction_hash, str):
             transaction_hash = binascii.unhexlify(transaction_hash)
         path = Bip32Path.build(f"44'/148'/{keypair_index}'")
         payload = path + transaction_hash
-
-        data = self.client.apdu_exchange(
-            ins=Ins.SIGN_HASH, data=payload, p1=P1.FIRST_APDU, p2=P2.LAST_APDU
-        )
-        return data
+        signature = self._send_payload(Ins.SIGN_HASH, payload)
+        return signature
 
     def sign_soroban_authorization(
         self,
         soroban_authorization: Union[str, bytes, HashIDPreimage],
         keypair_index: int = DEFAULT_KEYPAIR_INDEX,
     ) -> bytes:
         """Sign a Soroban authorization.
@@ -225,39 +218,104 @@
         ):
             raise ValueError(
                 f"Invalid type, expected {EnvelopeType.ENVELOPE_TYPE_SOROBAN_AUTHORIZATION}, but got {soroban_authorization.type}"
             )
         path = Bip32Path.build(f"44'/148'/{keypair_index}'")
         payload = path + soroban_authorization.to_xdr_bytes()
         signature = self._send_payload(Ins.SIGN_SOROBAN_AUTHORIZATION, payload)
-        assert isinstance(signature, bytes)
         return signature
 
-    def _send_payload(self, ins: Ins, payload) -> Optional[Union[int, bytes]]:
+    def _send_payload(self, ins: Ins, payload) -> bytes:
         """Send a payload to the Ledger device.
 
         Args:
             ins (Ins): The instruction for the APDU command.
             payload: The payload to send.
 
         Returns:
             Optional[Union[int, bytes]]: The response from the Ledger device.
         """
-        chunk_size = 255
-        first = True
-        while payload:
-            if first:
-                p1 = P1.FIRST_APDU
-                first = False
-            else:
-                p1 = P1.MORE_APDU
-
-            size = min(len(payload), chunk_size)
-            if size != len(payload):
-                p2 = P2.MORE_APDU
-            else:
-                p2 = P2.LAST_APDU
-
-            resp = self.client.apdu_exchange(ins, payload[:size], p1, p2)
-            if resp:
-                return resp
-            payload = payload[size:]
+        response = b""
+        remaining = len(payload)
+        while True:
+            chunk_size = min(remaining, APDU_MAX_PAYLOAD)
+            p1 = P1.FIRST_APDU if remaining == len(payload) else P1.MORE_APDU
+            p2 = P2.LAST_APDU if remaining - chunk_size == 0 else P2.MORE_APDU
+            chunk = payload[
+                len(payload) - remaining : len(payload) - remaining + chunk_size
+            ]
+            try:
+                response = self.client.apdu_exchange(ins=ins, p1=p1, p2=p2, data=chunk)
+            except CommException as e:
+                raise _remap_error(e) from e
+            remaining -= chunk_size
+            if remaining == 0:
+                break
+        return response
+
+
+class BaseError(Exception):
+    """Base exception class for Ledger errors."""
+
+    pass
+
+
+class DeviceNotFoundException(BaseError):
+    """Exception raised when no Ledger device is found."""
+
+    pass
+
+
+class HashSigningNotEnabledError(BaseError):
+    """Exception raised when hash signing is not enabled on the Ledger device."""
+
+    pass
+
+
+class RequestDataTooLargeError(BaseError):
+    """Exception raised when the request data is too large."""
+
+    pass
+
+
+class DataParsingFailedError(BaseError):
+    """Exception raised when parsing Stellar data fails."""
+
+    pass
+
+
+class UserRefusedError(BaseError):
+    """Exception raised when the user refuses the action."""
+
+    pass
+
+
+def _get_default_client() -> LedgerClient:
+    """Get the default Ledger client.
+
+    Returns:
+        LedgerClient: The default Ledger client instance.
+
+    Raises:
+        DeviceNotFoundException: If no Ledger device is found.
+    """
+    devices = enumerate_devices()
+    if len(devices) == 0:
+        raise DeviceNotFoundException("No Ledger device found")
+    return LedgerClient(devices[0])
+
+
+def _remap_error(e: CommException) -> Exception:
+    status = e.sw
+    if status == SW.DENY:
+        return UserRefusedError("User refused the request")
+    elif status == SW.DATA_PARSING_FAIL:
+        return DataParsingFailedError("Unable to parse the provided data")
+    elif status == SW.HASH_SIGNING_MODE_NOT_ENABLED:
+        return HashSigningNotEnabledError(
+            "Hash signing not allowed. Have you enabled it in the app settings?"
+        )
+    elif status == SW.REQUEST_DATA_TOO_LARGE:
+        return RequestDataTooLargeError(
+            "The provided data is too large for the device to process"
+        )
+    return e
```

### Comparing `strledger-0.7.0/PKG-INFO` & `strledger-0.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: strledger
-Version: 0.7.0
-Summary: Sign Stellar Transaction with Ledger on the command line.
+Version: 0.8.0
+Summary: Ledger Hardware Wallet Stellar Python bindings.
 Home-page: https://github.com/lightsail-network/strledger
 License: MIT
 Keywords: stellar,ledger
 Author: overcat
 Author-email: 4catcode@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,60 +16,58 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Typing :: Typed
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: ledgerwallet (>=0.4.0,<0.5.0)
-Requires-Dist: stellar-sdk (>=9,<10)
+Requires-Dist: stellar-sdk (>=9,<11)
 Project-URL: Bug Tracker, https://github.com/lightsail-network/strledger/issues
 Project-URL: Documentation, https://github.com/lightsail-network/strledger
 Project-URL: Repository, https://github.com/lightsail-network/strledger
 Description-Content-Type: text/markdown
 
-# strledger - Sign Stellar Transaction with Ledger on the command line.
+# strledger - Ledger Hardware Wallet Stellar Python bindings.
 
 ![example](https://github.com/lightsail-network/strledger/blob/main/img/example.png)
 
 ## Installation
 ```shell
 pip install -U strledger
 ```
 
 ## Cli Usage
 ```text
 Usage: strledger [OPTIONS] COMMAND [ARGS]...
 
   Stellar Ledger commands.
 
-  This project is built on the basis of ledgerctl, you can check ledgerctl for
+  This project is built on the basis of ledgerwallet, you can check ledgerwallet for
   more features.
 
 Options:
   -v, --verbose  Display exchanged APDU.
   --help         Show this message and exit.
 
 Commands:
-  app-info      Get Stellar app info.
-  get-address   Get Stellar public address.
-  sign-auth     Sign a base64-encoded soroban authorization...
-  sign-tx       Sign a base64-encoded transaction envelope.
-  sign-tx-hash  Sign a hex encoded hash.
-  version       Get strledger version info.
+  app-info     Get Stellar app configuration info.
+  get-address  Get Stellar public address.
+  sign-auth    Sign a base64-encoded soroban authorization (HashIDPreimage).
+  sign-hash    Sign a hex encoded hash.
+  sign-tx      Sign a base64-encoded transaction envelope.
+  version      Get strledger version info.
 ```
 
 ## Library Usage
 
 ```python
-from strledger import get_default_client
+from strledger import StrLedger
 
-client = get_default_client()
+client = StrLedger()
 # Use the Stellar Python SDK to build a transaction, see https://github.com/StellarCN/py-stellar-base
 transaction_envelope = ...
 client.sign_transaction(transaction_envelope=transaction_envelope, keypair_index=0)
 print(f"signed tx: {transaction_envelope.to_xdr()}")
 ```
```

