# Comparing `tmp/cardex-0.2.0.dev82.tar.gz` & `tmp/cardex-0.2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardex-0.2.0.dev82.tar", max compression
+gzip compressed data, was "cardex-0.2.0.dev9.tar", max compression
```

## Comparing `cardex-0.2.0.dev82.tar` & `cardex-0.2.0.dev9.tar`

### file list

```diff
@@ -1,25 +1,22 @@
--rw-r--r--   0        0        0    35115 2023-11-25 19:28:16.618733 cardex-0.2.0.dev82/LICENSE
--rw-r--r--   0        0        0        0 2023-11-25 00:47:56.601477 cardex-0.2.0.dev82/README.md
--rw-r--r--   0        0        0      856 2024-05-30 00:23:28.933677 cardex-0.2.0.dev82/pyproject.toml
--rw-r--r--   0        0        0      718 2024-05-13 01:26:36.929746 cardex-0.2.0.dev82/src/cardex/__init__.py
--rw-r--r--   0        0        0        0 2023-11-25 19:37:10.561449 cardex-0.2.0.dev82/src/cardex/backend/__init__.py
--rw-r--r--   0        0        0        0 2023-12-20 00:40:05.071771 cardex-0.2.0.dev82/src/cardex/backend/blockfrost.py
--rw-r--r--   0        0        0    23803 2024-05-30 00:21:46.168230 cardex-0.2.0.dev82/src/cardex/backend/dbsync.py
--rw-r--r--   0        0        0        7 2023-12-15 21:46:07.338340 cardex-0.2.0.dev82/src/cardex/dataclasses/__init__.py
--rw-r--r--   0        0        0     3564 2024-05-06 00:06:36.903642 cardex-0.2.0.dev82/src/cardex/dataclasses/datums.py
--rw-r--r--   0        0        0     7421 2024-05-11 13:49:57.621509 cardex-0.2.0.dev82/src/cardex/dataclasses/models.py
--rw-r--r--   0        0        0        0 2024-04-04 01:56:10.132901 cardex-0.2.0.dev82/src/cardex/dexs/__init__.py
--rw-r--r--   0        0        0    14617 2024-05-07 22:51:26.006696 cardex-0.2.0.dev82/src/cardex/dexs/amm/amm_base.py
--rw-r--r--   0        0        0     9953 2024-04-29 00:59:04.877214 cardex-0.2.0.dev82/src/cardex/dexs/amm/amm_types.py
--rw-r--r--   0        0        0    15794 2024-05-04 16:03:57.924930 cardex-0.2.0.dev82/src/cardex/dexs/amm/minswap.py
--rw-r--r--   0        0        0     9679 2024-04-27 23:27:41.560074 cardex-0.2.0.dev82/src/cardex/dexs/amm/muesli.py
--rw-r--r--   0        0        0    11002 2024-05-05 12:16:58.444639 cardex-0.2.0.dev82/src/cardex/dexs/amm/spectrum.py
--rw-r--r--   0        0        0     8155 2024-05-07 01:58:21.047295 cardex-0.2.0.dev82/src/cardex/dexs/amm/sundae.py
--rw-r--r--   0        0        0     8409 2024-04-04 01:56:18.385016 cardex-0.2.0.dev82/src/cardex/dexs/amm/vyfi.py
--rw-r--r--   0        0        0    10591 2024-04-30 11:07:52.118401 cardex-0.2.0.dev82/src/cardex/dexs/amm/wingriders.py
--rw-r--r--   0        0        0     5816 2024-05-14 03:02:18.974655 cardex-0.2.0.dev82/src/cardex/dexs/core/base.py
--rw-r--r--   0        0        0      507 2023-12-28 16:46:32.412198 cardex-0.2.0.dev82/src/cardex/dexs/core/errors.py
--rw-r--r--   0        0        0    23552 2024-05-14 12:35:37.836910 cardex-0.2.0.dev82/src/cardex/dexs/ob/geniusyield.py
--rw-r--r--   0        0        0    12961 2024-05-13 01:26:45.621871 cardex-0.2.0.dev82/src/cardex/dexs/ob/ob_base.py
--rw-r--r--   0        0        0     4526 2023-12-28 16:45:45.031601 cardex-0.2.0.dev82/src/cardex/utility.py
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 cardex-0.2.0.dev82/PKG-INFO
+-rw-r--r--   0        0        0    35115 2023-11-25 19:28:16.618733 cardex-0.2.0.dev9/LICENSE
+-rw-r--r--   0        0        0        0 2023-11-25 00:47:56.601477 cardex-0.2.0.dev9/README.md
+-rw-r--r--   0        0        0      855 2023-12-30 03:53:05.864880 cardex-0.2.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0      439 2023-12-17 00:14:15.994916 cardex-0.2.0.dev9/src/cardex/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-25 19:37:10.561449 cardex-0.2.0.dev9/src/cardex/backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-20 00:40:05.071771 cardex-0.2.0.dev9/src/cardex/backend/blockfrost.py
+-rw-r--r--   0        0        0     6606 2023-12-28 22:25:53.312378 cardex-0.2.0.dev9/src/cardex/backend/dbsync.py
+-rw-r--r--   0        0        0        7 2023-12-15 21:46:07.338340 cardex-0.2.0.dev9/src/cardex/dataclasses/__init__.py
+-rw-r--r--   0        0        0     2460 2023-12-28 21:29:45.268356 cardex-0.2.0.dev9/src/cardex/dataclasses/datums.py
+-rw-r--r--   0        0        0     3620 2023-12-29 16:27:33.577720 cardex-0.2.0.dev9/src/cardex/dataclasses/models.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:07:11.663822 cardex-0.2.0.dev9/src/cardex/dexs/__init__.py
+-rw-r--r--   0        0        0    16538 2023-12-30 02:36:16.805252 cardex-0.2.0.dev9/src/cardex/dexs/amm_base.py
+-rw-r--r--   0        0        0     6785 2023-12-30 02:34:01.987381 cardex-0.2.0.dev9/src/cardex/dexs/amm_types.py
+-rw-r--r--   0        0        0      507 2023-12-28 16:46:32.412198 cardex-0.2.0.dev9/src/cardex/dexs/errors.py
+-rw-r--r--   0        0        0     5070 2023-12-29 03:02:11.760668 cardex-0.2.0.dev9/src/cardex/dexs/minswap.py
+-rw-r--r--   0        0        0     7172 2023-12-30 03:52:33.944459 cardex-0.2.0.dev9/src/cardex/dexs/muesli.py
+-rw-r--r--   0        0        0     8080 2023-12-29 16:27:33.577720 cardex-0.2.0.dev9/src/cardex/dexs/spectrum.py
+-rw-r--r--   0        0        0     6331 2023-12-29 03:03:12.669431 cardex-0.2.0.dev9/src/cardex/dexs/sundae.py
+-rw-r--r--   0        0        0     5967 2023-12-29 03:03:21.401540 cardex-0.2.0.dev9/src/cardex/dexs/vyfi.py
+-rw-r--r--   0        0        0     6819 2023-12-29 03:03:31.701670 cardex-0.2.0.dev9/src/cardex/dexs/wingriders.py
+-rw-r--r--   0        0        0     4526 2023-12-28 16:45:45.031601 cardex-0.2.0.dev9/src/cardex/utility.py
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 cardex-0.2.0.dev9/PKG-INFO
```

### Comparing `cardex-0.2.0.dev82/LICENSE` & `cardex-0.2.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev82/pyproject.toml` & `cardex-0.2.0.dev9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cardex"
-version = "0.2.0-dev82"
+version = "0.2.0-dev9"
 description = ""
 authors = ["Elder Millenial <eldermillenial@protonmail.com>"]
 readme = "README.md"
 packages = [{include = "cardex", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cardex-0.2.0.dev82/src/cardex/dataclasses/datums.py` & `cardex-0.2.0.dev9/src/cardex/dataclasses/datums.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,26 @@
 # noqa
 from dataclasses import dataclass
 from typing import Union
 
 from pycardano import Address
-from pycardano import DatumHash
 from pycardano import PlutusData
-from pycardano import VerificationKeyHash
 
 from cardex.dataclasses.models import Assets
 
 
 @dataclass
-class ReceiverDatum(PlutusData):
-    """The receiver address."""
-
-    CONSTR_ID = 0
-    datum_hash: Union[DatumHash, None] = None
-
-
-@dataclass
 class PlutusPartAddress(PlutusData):
     """Encode a plutus address part (i.e. payment, stake, etc)."""
 
     CONSTR_ID = 0
     address: bytes
 
 
 @dataclass
-class PlutusScriptPartAddress(PlutusPartAddress):
-    """Encode a plutus address part (i.e. payment, stake, etc)."""
-
-    CONSTR_ID = 1
-
-
-@dataclass
 class PlutusNone(PlutusData):
     """Placeholder for a receiver datum."""
 
     CONSTR_ID = 1
 
 
 @dataclass
@@ -50,50 +33,32 @@
 
 @dataclass
 class PlutusFullAddress(PlutusData):
     """A full address, including payment and staking keys."""
 
     CONSTR_ID = 0
     payment: PlutusPartAddress
-    stake: Union[_PlutusConstrWrapper, PlutusNone]
+    stake: _PlutusConstrWrapper
 
     @classmethod
     def from_address(cls, address: Address) -> "PlutusFullAddress":
         """Parse an Address object to a PlutusFullAddress."""
         error_msg = "Only addresses with staking and payment parts are accepted."
         if None in [address.staking_part, address.payment_part]:
             raise ValueError(error_msg)
-        if address.staking_part is not None:
-            stake = _PlutusConstrWrapper(
-                _PlutusConstrWrapper(
-                    PlutusPartAddress(bytes.fromhex(str(address.staking_part))),
-                ),
-            )
-        else:
-            stake = PlutusNone
+        stake = _PlutusConstrWrapper(
+            _PlutusConstrWrapper(
+                PlutusPartAddress(bytes.fromhex(str(address.staking_part))),
+            ),
+        )
         return PlutusFullAddress(
             PlutusPartAddress(bytes.fromhex(str(address.payment_part))),
             stake=stake,
         )
 
-    def to_address(self) -> Address:
-        payment_part = VerificationKeyHash(self.payment.address[:28])
-        if isinstance(self.stake, PlutusNone):
-            stake_part = None
-        else:
-            stake_part = VerificationKeyHash(self.stake.wrapped.wrapped.address[:28])
-        return Address(payment_part=payment_part, staking_part=stake_part)
-
-
-@dataclass
-class PlutusScriptAddress(PlutusFullAddress):
-    """A full address, including payment and staking keys."""
-
-    payment: PlutusScriptPartAddress
-
 
 @dataclass
 class AssetClass(PlutusData):
     """An asset class. Separates out token policy and asset name."""
 
     CONSTR_ID = 0
 
@@ -121,14 +86,7 @@
         """Convert back to assets."""
         if self.policy.hex() == "":
             asset = "lovelace"
         else:
             asset = self.policy.hex() + self.asset_name.hex()
 
         return Assets(root={asset: 0})
-
-
-@dataclass
-class CancelRedeemer(PlutusData):
-    """Cancel datum."""
-
-    CONSTR_ID = 1
```

### Comparing `cardex-0.2.0.dev82/src/cardex/dexs/amm/amm_base.py` & `cardex-0.2.0.dev9/src/cardex/dexs/amm_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,119 +1,165 @@
+from abc import ABC
 from abc import abstractmethod
 from decimal import Decimal
 
-from cardex.dataclasses.models import Assets
-from cardex.dexs.core.base import AbstractPairState
-from cardex.dexs.core.errors import InvalidPoolError
-from cardex.dexs.core.errors import NoAssetsError
-from cardex.dexs.core.errors import NotAPoolError
-from cardex.utility import Assets
-from cardex.utility import asset_to_value
-from cardex.utility import naturalize_assets
 from pycardano import Address
 from pycardano import DeserializeException
 from pycardano import PlutusData
+from pycardano import PlutusV1Script
+from pycardano import PlutusV2Script
 from pycardano import TransactionOutput
+from pydantic import BaseModel
 from pydantic import model_validator
 
+from cardex.dataclasses.models import Assets
+from cardex.dataclasses.models import PoolSelector
+from cardex.dexs.errors import InvalidPoolError
+from cardex.dexs.errors import NoAssetsError
+from cardex.dexs.errors import NotAPoolError
+from cardex.utility import Assets
+from cardex.utility import asset_to_value
+from cardex.utility import naturalize_assets
 
-class AbstractPoolState(AbstractPairState):
+
+class AbstractPoolState(BaseModel, ABC):
+    assets: Assets
+    block_time: int
+    block_index: int
     datum_cbor: str
     datum_hash: str
+    dex_nft: Assets | None = None
     inactive: bool = False
     lp_tokens: Assets | None = None
+    plutus_v2: bool
     pool_nft: Assets | None = None
     tx_index: int
     tx_hash: str
 
     _batcher_fee: Assets
-    _datum_parsed: PlutusData | None = None
-    _deposit: Assets
+    _datum_parsed: PlutusData
+    _deposit_fee: Assets
     _volume_fee: int | None = None
 
     @property
     @abstractmethod
     def pool_id(self) -> str:
         """A unique identifier for the pool.
 
         This is a unique string differentiating this pool from every other pool on the
         dex, and is necessary for dexs that have more than one pool for a pair but with
         different fee structures.
         """
         raise NotImplementedError("Unique pool id is not specified.")
 
+    @classmethod
+    @abstractmethod
+    def dex(self) -> str:
+        """Official dex name."""
+        raise NotImplementedError("DEX name is undefined.")
+
+    @classmethod
+    @abstractmethod
+    def pool_selector(self) -> PoolSelector:
+        """Pool selection information."""
+        raise NotImplementedError("DEX name is undefined.")
+
+    @abstractmethod
+    def get_amount_out(self, asset: Assets) -> tuple[Assets, float]:
+        raise NotImplementedError("")
+
+    @abstractmethod
+    def get_amount_in(self, asset: Assets) -> tuple[Assets, float]:
+        raise NotImplementedError("")
+
+    @property
+    @abstractmethod
+    def swap_forward(self) -> bool:
+        raise NotImplementedError
+
+    @property
+    def inline_datum(self) -> bool:
+        return self.plutus_v2
+
+    @property
+    @abstractmethod
+    def stake_address(self) -> Address:
+        raise NotImplementedError
+
     @property
     @abstractmethod
     def pool_datum_class(self) -> type[PlutusData]:
         raise NotImplementedError
 
     @property
+    @abstractmethod
+    def order_datum_class(self) -> type[PlutusData]:
+        raise NotImplementedError
+
+    @property
+    def script_class(self) -> type[PlutusV1Script] | type[PlutusV2Script]:
+        if self.plutus_v2:
+            return PlutusV2Script
+        else:
+            return PlutusV1Script
+
+    @property
     def pool_datum(self) -> PlutusData:
         """The pool state datum."""
-        return self.pool_datum_class.from_cbor(self.datum_cbor)
+        if not self._datum_parsed:
+            if not self.datum_cbor:
+                raise ValueError("No datum specified.")
+            self._datum_parsed = self.pool_datum_class.from_cbor(self.datum_cbor)
+
+        return self._datum_parsed
 
     def swap_datum(
         self,
-        address_source: Address,
+        address: Address,
         in_assets: Assets,
         out_assets: Assets,
-        extra_assets: Assets | None = None,
-        address_target: Address | None = None,
-        datum_target: PlutusData | None = None,
+        forward_address: Address | None = None,
     ) -> PlutusData:
-        if self.swap_forward and address_target is not None:
+        if self.swap_forward and forward_address is not None:
             print(f"{self.__class__.__name__} does not support swap forwarding.")
 
         return self.order_datum_class.create_datum(
-            address_source=address_source,
+            address=address,
             in_assets=in_assets,
             out_assets=out_assets,
-            batcher_fee=self.batcher_fee(
-                in_assets=in_assets,
-                out_assets=out_assets,
-                extra_assets=extra_assets,
-            ),
-            deposit=self.deposit(in_assets=in_assets, out_assets=out_assets),
-            address_target=address_target,
-            datum_target=datum_target,
+            batcher_fee=self.batcher_fee,
+            deposit=self.deposit,
+            forward_address=forward_address,
         )
 
     def swap_utxo(
         self,
-        address_source: Address,
+        address: Address,
         in_assets: Assets,
         out_assets: Assets,
-        extra_assets: Assets | None = None,
-        address_target: Address | None = None,
-        datum_target: PlutusData | None = None,
-    ) -> TransactionOutput:
+        forward_address: Address | None = None,
+    ):
         # Basic checks
         if len(in_assets) != 1 or len(out_assets) != 1:
             raise ValueError(
                 "Only one asset can be supplied as input, "
                 + "and one asset supplied as output.",
             )
 
         order_datum = self.swap_datum(
-            address_source=address_source,
+            address=address,
             in_assets=in_assets,
             out_assets=out_assets,
-            extra_assets=extra_assets,
-            address_target=address_target,
-            datum_target=datum_target,
+            forward_address=forward_address,
         )
 
         in_assets.root["lovelace"] = (
             in_assets["lovelace"]
-            + self.batcher_fee(
-                in_assets=in_assets,
-                out_assets=out_assets,
-                extra_assets=extra_assets,
-            ).quantity()
-            + self.deposit(in_assets=in_assets, out_assets=out_assets).quantity()
+            + self.batcher_fee.quantity()
+            + self.deposit.quantity()
         )
 
         if self.inline_datum:
             output = TransactionOutput(
                 address=self.stake_address,
                 amount=asset_to_value(in_assets),
                 datum=order_datum,
@@ -123,14 +169,29 @@
                 address=self.stake_address,
                 amount=asset_to_value(in_assets),
                 datum_hash=order_datum.hash(),
             )
 
         return output, order_datum
 
+    @property
+    def volume_fee(self) -> int:
+        """Swap fee of swap in basis points."""
+        return self.fee
+
+    @property
+    def batcher_fee(self) -> Assets:
+        """Batcher fee."""
+        return self._batcher
+
+    @property
+    def deposit(self) -> Assets:
+        """Batcher fee."""
+        return self._deposit
+
     @classmethod
     @property
     def pool_policy(cls) -> list[str] | None:
         """The pool nft policies.
 
         This should be the policy or policy+name of any pool nft policy that might be
         in the pool. Each pool must contain one of the NFTs in the list, and if this
@@ -159,14 +220,28 @@
 
         Returns:
             Optional[str]: policy or policy+name of lp tokens
         """
         return None
 
     @classmethod
+    @property
+    def dex_policy(cls) -> list[str] | None:
+        """The dex nft policy.
+
+        This should be the policy or policy+name of the dex nft.
+
+        If None, then the default dex nft check is skipped.
+
+        Returns:
+            Optional[str]: policy or policy+name of dex nft
+        """
+        return None
+
+    @classmethod
     def extract_dex_nft(cls, values: dict[str, ...]) -> Assets | None:
         """Extract the dex nft from the UTXO.
 
         Some DEXs put a DEX nft into the pool UTXO.
 
         This function checks to see if the DEX nft is in the UTXO if the DEX policy is
         defined.
@@ -377,20 +452,17 @@
 
         if cls.skip_init(values):
             return values
 
         # Parse the pool datum
         try:
             datum = cls.pool_datum_class.from_cbor(values["datum_cbor"])
-        except (DeserializeException, TypeError) as e:
+        except (DeserializeException, TypeError):
             raise NotAPoolError(
-                "Pool datum could not be deserialized: \n "
-                + f"    error={e}\n"
-                + f"    tx_hash={values['tx_hash']}\n"
-                + f"    datum={values['datum_cbor']}\n",
+                f"Pool datum could not be deserialized: {values['datum_cbor']}",
             )
 
         # To help prevent edge cases, remove pool tokens while running other checks
         pair = Assets({})
         if datum.pool_pair() is not None:
             for token in datum.pool_pair():
                 try:
@@ -412,14 +484,34 @@
         values["assets"].root.update(pair.root)
 
         cls.post_init(values)
 
         return values
 
     @property
+    def unit_a(self) -> str:
+        """Token name of asset A."""
+        return self.assets.unit(0)
+
+    @property
+    def unit_b(self) -> str:
+        """Token name of asset b."""
+        return self.assets.unit(1)
+
+    @property
+    def reserve_a(self) -> int:
+        """Reserve amount of asset A."""
+        return self.assets.quantity(0)
+
+    @property
+    def reserve_b(self) -> int:
+        """Reserve amount of asset B."""
+        return self.assets.quantity(1)
+
+    @property
     def price(self) -> tuple[Decimal, Decimal]:
         """Price of assets.
 
         Returns:
             A `Tuple[Decimal, Decimal] where the first `Decimal` is the price to buy
                 1 of token B in units of token A, and the second `Decimal` is the price
                 to buy 1 of token A in units of token B.
```

### Comparing `cardex-0.2.0.dev82/src/cardex/dexs/amm/amm_types.py` & `cardex-0.2.0.dev9/src/cardex/dexs/amm_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from cardex.dataclasses.models import Assets
-from cardex.dexs.amm.amm_base import AbstractPoolState
+from cardex.dexs.amm_base import AbstractPoolState
 
 
 class AbstractConstantProductPoolState(AbstractPoolState):
     def get_amount_out(
         self,
         asset: Assets,
         precise: bool = True,
@@ -65,15 +65,15 @@
             The estimated asset needed for input in the swap.
         """
         assert len(asset) == 1, "Asset should only have one token."
         assert asset.unit() in [
             self.unit_a,
             self.unit_b,
         ], f"Asset {asset.unit} is invalid for pool {self.unit_a}-{self.unit_b}"
-        if asset.unit() == self.unit_b:
+        if asset.unit == self.unit_b:
             reserve_in, reserve_out = self.reserve_a, self.reserve_b
             unit_out = self.unit_a
         else:
             reserve_in, reserve_out = self.reserve_b, self.reserve_a
             unit_out = self.unit_b
 
         # Estimate the required input
@@ -92,46 +92,23 @@
         price_denominator: int = reserve_out * numerator * 10000
         price_impact: float = price_numerator / price_denominator
 
         return amount_in, price_impact
 
 
 class AbstractStableSwapPoolState(AbstractPoolState):
-    asset_mulitipliers: list[int] = [1, 1]
-
-    @property
-    def reserve_a(self) -> int:
-        """Reserve amount of asset A."""
-        return self.assets.quantity(0) * self.asset_mulitipliers[0]
-
-    @property
-    def reserve_b(self) -> int:
-        """Reserve amount of asset B."""
-        return self.assets.quantity(1) * self.asset_mulitipliers[1]
-
     @property
-    def amp(self) -> Assets:
+    def amp(cls) -> Assets:
         return 75
 
-    def _get_ann(self):
-        """The modified amp value.
-
-        This is the derived amp value (ann) from the original stableswap paper. This is
-        implemented here as the default, but a common variant of this does not use the
-        exponent. The alternative version is provided in the
-        AbstractCommonStableSwapPoolState class. WingRiders uses this version.
-        """
-        N_COINS = 2
-        return self.amp * N_COINS**N_COINS
-
     def _get_D(self) -> float:
         """Regression to learn the stability constant."""
         # TODO: Expand this to operate on pools with more than one stable
         N_COINS = 2
-        Ann = self._get_ann()
+        Ann = self.amp * N_COINS**N_COINS
         S = self.reserve_a + self.reserve_b
         if S == 0:
             return 0
 
         # Iterate until the change in value is <1 unit.
         D = S
         for i in range(256):
@@ -140,154 +117,66 @@
             D = D * (Ann * S + D_P * N_COINS) / ((Ann - 1) * D + (N_COINS + 1) * D_P)
 
             if abs(D - D_prev) < 1:
                 break
 
         return D
 
-    def _get_y(
-        self,
-        in_assets: Assets,
-        out_unit: str,
-        precise: bool = True,
-        get_input=False,
-    ):
+    def _get_y(self, in_assets: Assets, out_unit: str):
         """Calculate the output amount using a regression."""
         N_COINS = 2
-        Ann = self._get_ann()
+        Ann = self.amp * N_COINS**N_COINS
         D = self._get_D()
 
-        if get_input:
-            subtract = -1
-        else:
-            subtract = 1
-
         # Make sure only one input supplied
         if len(in_assets) > 1:
             raise ValueError("Only one input asset allowed.")
         elif in_assets.unit() not in [self.unit_a, self.unit_b]:
             raise ValueError("Invalid input token.")
         elif out_unit not in [self.unit_a, self.unit_b]:
             raise ValueError("Invalid output token.")
 
-        in_quantity = in_assets.quantity()
+        in_quantity = in_assets.quantity() * (10000 - self.volume_fee) / 10000
         if in_assets.unit() == self.unit_a:
-            in_reserve = (
-                self.reserve_a + in_quantity * self.asset_mulitipliers[0] * subtract
-            )
-            out_multiplier = self.asset_mulitipliers[1]
+            in_reserve = self.reserve_a + in_quantity
         else:
-            in_reserve = (
-                self.reserve_b + in_quantity * self.asset_mulitipliers[1] * subtract
-            )
-            out_multiplier = self.asset_mulitipliers[0]
+            in_reserve = self.reserve_b + in_quantity
 
         S = in_reserve
         c = D**3 / (N_COINS**2 * Ann * in_reserve)
         b = S + D / Ann
         out_prev = 0
         out = D
 
         for i in range(256):
             out_prev = out
             out = (out**2 + c) / (2 * out + b - D)
 
             if abs(out - out_prev) < 1:
                 break
 
-        out /= out_multiplier
-        out_assets = Assets(**{out_unit: int(out)})
-        if not precise:
-            out_assets.root[out_unit] = out
-
-        return out_assets
+        return Assets(**{out_unit: int(out)})
 
-    def get_amount_out(
-        self,
-        asset: Assets,
-        precise: bool = True,
-        fee_on_input=True,
-    ) -> tuple[Assets, float]:
-        if fee_on_input:
-            in_asset = Assets(
-                **{
-                    asset.unit(): int(
-                        asset.quantity() * (10000 - self.volume_fee) / 10000,
-                    ),
-                },
-            )
-        else:
-            in_asset = asset
+    def get_amount_out(self, asset: Assets) -> tuple[Assets, float]:
         out_unit = self.unit_a if asset.unit() == self.unit_b else self.unit_b
-        out_asset = self._get_y(in_asset, out_unit, precise=precise)
-        out_reserve = (
-            self.reserve_b / self.asset_mulitipliers[1]
-            if out_unit == self.unit_b
-            else self.reserve_a / self.asset_mulitipliers[0]
-        )
-
-        out_asset.root[out_asset.unit()] = out_reserve - out_asset.quantity()
-        if not fee_on_input:
-            out_asset.root[out_asset.unit()] = int(
-                out_asset.quantity() * (10000 - self.volume_fee) / 10000,
-            )
-        if precise:
-            out_asset.root[out_asset.unit()] = int(out_asset.quantity())
-
+        out_asset = self._get_y(asset, out_unit)
+        out_reserve = self.reserve_b if out_unit == self.unit_b else self.reserve_a
+        out_asset.root[out_asset.unit()] = int(out_reserve - out_asset.quantity())
         return out_asset, 0
 
-    def get_amount_in(
-        self,
-        asset: Assets,
-        precise: bool = True,
-        fee_on_input=True,
-    ) -> tuple[Assets, float]:
-        if not fee_on_input:
-            out_asset = Assets(
-                **{
-                    asset.unit(): int(
-                        asset.quantity() * 10000 / (10000 - self.volume_fee),
-                    ),
-                },
-            )
-        else:
-            out_asset = asset
+    def get_amount_in(self, asset: Assets) -> tuple[Assets, float]:
         in_unit = self.unit_a if asset.unit() == self.unit_b else self.unit_b
-        in_asset = self._get_y(out_asset, in_unit, precise=precise, get_input=True)
-        in_reserve = (
-            (self.reserve_b / self.asset_mulitipliers[1])
-            if in_unit == self.unit_b
-            else (self.reserve_a / self.asset_mulitipliers[0])
-        )
-        in_asset.root[in_asset.unit()] = in_asset.quantity() - in_reserve
-        if fee_on_input:
-            in_asset.root[in_asset.unit()] = int(
-                in_asset.quantity() * 10000 / (10000 - self.volume_fee),
-            )
-        if precise:
-            in_asset.root[in_asset.unit()] = int(in_asset.quantity())
+        asset[asset.unit] = -asset[asset.unit]
+        in_asset = self._get_y(asset, in_unit)
+        in_reserve = self.reserve_b if in_unit == self.unit_b else self.reserve_a
+        in_asset.root[in_asset.unit()] = int(in_asset.quantity() - in_reserve)
+        asset[asset.unit] = -asset[asset.unit]
         return in_asset, 0
 
 
-class AbstractCommonStableSwapPoolState(AbstractStableSwapPoolState):
-    """The common variant of StableSwap.
-
-    This class implements the common variant of the stableswap algorithm. The main
-    difference is the
-    """
-
-    def _get_ann(self):
-        """The modified amp value.
-
-        This is the ann value in the common stableswap variant.
-        """
-        N_COINS = 2
-        return self.amp * N_COINS
-
-
 class AbstractConstantLiquidityPoolState(AbstractPoolState):
     def get_amount_out(self, asset: Assets) -> tuple[Assets, float]:
         raise NotImplementedError("CLPP amount out is not yet implemented.")
         return out_asset, 0
 
     def get_amount_in(self, asset: Assets) -> tuple[Assets, float]:
         raise NotImplementedError("CLPP amount out is not yet implemented.")
```

### Comparing `cardex-0.2.0.dev82/src/cardex/dexs/amm/muesli.py` & `cardex-0.2.0.dev9/src/cardex/dexs/muesli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,56 @@
 from dataclasses import dataclass
 from typing import Any
 from typing import ClassVar
 from typing import Optional
-from typing import Union
 
-from cardex.backend.dbsync import get_script_from_address
+from pycardano import Address
+from pycardano import PlutusData
+
 from cardex.dataclasses.datums import AssetClass
 from cardex.dataclasses.datums import PlutusFullAddress
 from cardex.dataclasses.datums import PlutusNone
-from cardex.dataclasses.models import OrderType
 from cardex.dataclasses.models import PoolSelector
-from cardex.dexs.amm.amm_types import AbstractConstantLiquidityPoolState
-from cardex.dexs.amm.amm_types import AbstractConstantProductPoolState
-from cardex.dexs.core.errors import InvalidPoolError
+from cardex.dexs.amm_types import AbstractConstantLiquidityPoolState
+from cardex.dexs.amm_types import AbstractConstantProductPoolState
+from cardex.dexs.errors import InvalidPoolError
 from cardex.utility import Assets
-from pycardano import Address
-from pycardano import PlutusData
-from pycardano import PlutusV1Script
-from pycardano import PlutusV2Script
-from pycardano import Redeemer
-from pycardano import TransactionId
-from pycardano import TransactionInput
-from pycardano import TransactionOutput
-from pycardano import UTxO
-from pycardano import Value
-
-
-@dataclass
-class MuesliSometimesNone(PlutusData):
-    CONSTR_ID = 0
 
 
 @dataclass
 class MuesliOrderConfig(PlutusData):
     CONSTR_ID = 0
 
     full_address: PlutusFullAddress
     token_out_policy: bytes
     token_out_name: bytes
     token_in_policy: bytes
     token_in_name: bytes
     min_receive: int
-    unknown: Union[MuesliSometimesNone, PlutusNone]
+    unknown: PlutusNone
     in_amount: int
 
 
 @dataclass
 class MuesliOrderDatum(PlutusData):
     CONSTR_ID = 0
 
     value: MuesliOrderConfig
 
     @classmethod
     def create_datum(
         cls,
-        address_source: Address,
+        address: Address,
         in_assets: Assets,
         out_assets: Assets,
         batcher_fee: Assets,
         deposit: Assets,
-        address_target: Address | None = None,
-        datum_target: PlutusData | None = None,
+        forward_address: Address | None = None,
     ):
-        full_address = PlutusFullAddress.from_address(address_source)
+        full_address = PlutusFullAddress.from_address(address)
 
         if in_assets.unit() == "lovelace":
             token_in_policy = b""
             token_in_name = b""
         else:
             token_in_policy = bytes.fromhex(in_assets.unit()[:56])
             token_in_name = bytes.fromhex(in_assets.unit()[56:])
@@ -87,26 +71,14 @@
             min_receive=out_assets.quantity(),
             unknown=PlutusNone(),
             in_amount=batcher_fee.quantity() + deposit.quantity(),
         )
 
         return cls(value=config)
 
-    def address_source(self) -> str:
-        return self.value.full_address.to_address()
-
-    def requested_amount(self) -> Assets:
-        token_out = self.value.token_out_policy.hex() + self.value.token_out_name.hex()
-        if token_out == "":
-            token_out = "lovelace"
-        return Assets({token_out: self.value.min_receive})
-
-    def order_type(self) -> OrderType:
-        return OrderType.swap
-
 
 @dataclass
 class MuesliPoolDatum(PlutusData):
     CONSTR_ID = 0
 
     asset_a: AssetClass
     asset_b: AssetClass
@@ -129,83 +101,42 @@
 class MuesliCLPoolDatum(MuesliPoolDatum):
     upper: PreciseFloat
     lower: PreciseFloat
     price_sqrt: PreciseFloat
     unknown: int
 
 
-@dataclass
-class MuesliCancelRedeemer(PlutusData):
-    CONSTR_ID = 0
-
-
 class MuesliSwapCPPState(AbstractConstantProductPoolState):
     fee: int = 30
     _batcher = Assets(lovelace=950000)
     _deposit = Assets(lovelace=1700000)
     _test_pool: ClassVar[
         str
     ] = "a8512101cb1163cc218e616bb4d4070349a1c9395313f1323cc583634d7565736c695377617054657374506f6f6c"
-    _stake_address: ClassVar[Address] = Address.from_primitive(
+    _stake_address = Address.from_primitive(
         "addr1zyq0kyrml023kwjk8zr86d5gaxrt5w8lxnah8r6m6s4jp4g3r6dxnzml343sx8jweqn4vn3fz2kj8kgu9czghx0jrsyqqktyhv",
     )
-    _reference_utxo: ClassVar[UTxO | None] = None
 
     @classmethod
     @property
     def dex(cls) -> str:
         return "MuesliSwap"
 
     @classmethod
     @property
-    def order_selector(self) -> list[str]:
-        return [self._stake_address.encode()]
-
-    @classmethod
-    @property
     def pool_selector(cls) -> PoolSelector:
         return PoolSelector(
             selector_type="assets",
             selector=cls.dex_policy,
         )
 
     @property
     def swap_forward(self) -> bool:
         return False
 
-    @classmethod
-    @property
-    def reference_utxo(cls) -> UTxO | None:
-        if cls._reference_utxo is None:
-            script_bytes = bytes.fromhex(
-                get_script_from_address(cls._stake_address).script,
-            )
-
-            script = cls.default_script_class()(script_bytes)
-
-            cls._reference_utxo = UTxO(
-                input=TransactionInput(
-                    transaction_id=TransactionId(
-                        bytes.fromhex(
-                            "7e4142b7a040eae45d14513000adf91ab42da33a1bd5ccffcfe851b3d93e1e5e",
-                        ),
-                    ),
-                    index=1,
-                ),
-                output=TransactionOutput(
-                    address=Address.decode(
-                        "addr1v9p0rc57dzkz7gg97dmsns8hngsuxl956xe6myjldaug7hse4elc6",
-                    ),
-                    amount=Value(coin=24269610),
-                    script=script,
-                ),
-            )
-
-        return cls._reference_utxo
-
     @property
     def stake_address(self) -> Address:
         return self._stake_address
 
     @classmethod
     @property
     def order_datum_class(cls) -> type[MuesliOrderDatum]:
@@ -285,22 +216,14 @@
                     f"MuesliSwap pools must have exactly one pool nft: assets={assets}",
                 )
             pool_nft = Assets(**{nfts[0]: assets.root.pop(nfts[0])})
             values["pool_nft"] = pool_nft
 
         return pool_nft
 
-    @classmethod
-    def default_script_class(self) -> type[PlutusV1Script] | type[PlutusV2Script]:
-        return PlutusV2Script
-
-    @classmethod
-    def cancel_redeemer(cls) -> PlutusData:
-        return Redeemer(MuesliCancelRedeemer())
-
 
 class MuesliSwapCLPState(AbstractConstantLiquidityPoolState, MuesliSwapCPPState):
     inactive: bool = True
 
     @classmethod
     @property
     def dex_policy(cls) -> list[str]:
```

### Comparing `cardex-0.2.0.dev82/src/cardex/dexs/amm/sundae.py` & `cardex-0.2.0.dev9/src/cardex/dexs/sundae.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from dataclasses import dataclass
-from typing import ClassVar
 from typing import Union
 
+from pycardano import Address
+from pycardano import PlutusData
+
 from cardex.dataclasses.datums import AssetClass
 from cardex.dataclasses.datums import PlutusFullAddress
 from cardex.dataclasses.datums import PlutusNone
-from cardex.dataclasses.datums import PlutusPartAddress
-from cardex.dataclasses.datums import PlutusScriptAddress
-from cardex.dataclasses.datums import ReceiverDatum
 from cardex.dataclasses.models import Assets
-from cardex.dataclasses.models import OrderType
 from cardex.dataclasses.models import PoolSelector
-from cardex.dexs.amm.amm_types import AbstractConstantProductPoolState
-from cardex.dexs.core.errors import InvalidPoolError
-from cardex.dexs.core.errors import NoAssetsError
-from cardex.dexs.core.errors import NotAPoolError
-from pycardano import Address
-from pycardano import PlutusData
+from cardex.dexs.amm_types import AbstractConstantProductPoolState
+from cardex.dexs.errors import InvalidPoolError
+from cardex.dexs.errors import NoAssetsError
+from cardex.dexs.errors import NotAPoolError
 
 
 @dataclass
 class AtoB(PlutusData):
     CONSTR_ID = 0
 
 
@@ -41,119 +37,72 @@
 
     direction: Union[AtoB, BtoA]
     amount_in: int
     amount_out: AmountOut
 
 
 @dataclass
-class DepositPairQuantity(PlutusData):
-    CONSTR_ID = 0
-    amount_a: int
-    amount_b: int
-
-
-@dataclass
-class DepositPair(PlutusData):
-    CONSTR_ID = 1
-    assets: DepositPairQuantity
-
-
-@dataclass
-class DepositConfig(PlutusData):
-    CONSTR_ID = 2
-
-    deposit_pair: DepositPair
-
-
-@dataclass
-class WithdrawConfig(PlutusData):
-    CONSTR_ID = 1
-
-    amount_lp: int
-
-
-@dataclass
-class SundaeAddressWithDatum(PlutusData):
+class SundaeAddressWithNone(PlutusData):
     CONSTR_ID = 0
 
-    address: Union[PlutusFullAddress, PlutusScriptAddress]
-    datum: Union[ReceiverDatum, PlutusNone]
+    address: PlutusFullAddress
+    null: PlutusNone
 
     @classmethod
     def from_address(cls, address: Address):
-        return cls(address=PlutusFullAddress.from_address(address), datum=PlutusNone())
+        return cls(address=PlutusFullAddress.from_address(address), null=PlutusNone())
 
 
 @dataclass
 class SundaeAddressWithDestination(PlutusData):
     """For now, destination is set to none, should be updated."""
 
     CONSTR_ID = 0
 
-    address: SundaeAddressWithDatum
-    destination: Union[PlutusPartAddress, PlutusNone]
+    address: SundaeAddressWithNone
+    destination: PlutusNone
 
     @classmethod
     def from_address(cls, address: Address):
-        null = SundaeAddressWithDatum.from_address(address)
+        null = SundaeAddressWithNone.from_address(address)
         return cls(address=null, destination=PlutusNone())
 
 
 @dataclass
 class SundaeOrderDatum(PlutusData):
     CONSTR_ID = 0
 
     ident: bytes
     address: SundaeAddressWithDestination
     fee: int
-    swap: Union[DepositConfig, SwapConfig, WithdrawConfig]
+    swap: SwapConfig
 
     @classmethod
     def create_datum(
         cls,
         ident: bytes,
-        address_source: Address,
+        address: Address,
         in_assets: Assets,
         out_assets: Assets,
         fee: int,
     ):
-        full_address = SundaeAddressWithDestination.from_address(address_source)
+        full_address = SundaeAddressWithDestination.from_address(address)
         merged = in_assets + out_assets
         if in_assets.unit() == merged.unit():
             direction = AtoB()
         else:
             direction = BtoA()
         swap = SwapConfig(
             direction=direction,
             amount_in=in_assets.quantity(),
             amount_out=AmountOut(min_receive=out_assets.quantity()),
         )
 
         return cls(ident=ident, address=full_address, fee=fee, swap=swap)
 
-    def address_source(self) -> Address:
-        return self.address.address.address.to_address()
-
-    def requested_amount(self) -> Assets:
-        if isinstance(self.swap, SwapConfig):
-            if isinstance(self.swap.direction, AtoB):
-                return Assets({"asset_b": self.swap.amount_out.min_receive})
-            else:
-                return Assets({"asset_a": self.swap.amount_out.min_receive})
-        else:
-            return Assets({})
-
-    def order_type(self) -> OrderType:
-        if isinstance(self.swap, SwapConfig):
-            return OrderType.swap
-        elif isinstance(self.swap, DepositConfig):
-            return OrderType.deposit
-        elif isinstance(self.swap, WithdrawConfig):
-            return OrderType.withdraw
-
 
 @dataclass
 class LPFee(PlutusData):
     CONSTR_ID = 0
     numerator: int
     denominator: int
 
@@ -177,30 +126,25 @@
         return self.assets.asset_a.assets + self.assets.asset_b.assets
 
 
 class SundaeSwapCPPState(AbstractConstantProductPoolState):
     fee: int
     _batcher = Assets(lovelace=2500000)
     _deposit = Assets(lovelace=2000000)
-    _stake_address: ClassVar[Address] = Address.from_primitive(
+    _stake_address = Address.from_primitive(
         "addr1wxaptpmxcxawvr3pzlhgnpmzz3ql43n2tc8mn3av5kx0yzs09tqh8",
     )
 
     @classmethod
     @property
     def dex(cls) -> str:
         return "SundaeSwap"
 
     @classmethod
     @property
-    def order_selector(self) -> list[str]:
-        return [self._stake_address.encode()]
-
-    @classmethod
-    @property
     def pool_selector(cls) -> PoolSelector:
         return PoolSelector(
             selector_type="addresses",
             selector=["addr1w9qzpelu9hn45pefc0xr4ac4kdxeswq7pndul2vuj59u8tqaxdznu"],
         )
 
     @property
@@ -273,26 +217,24 @@
 
         numerator = datum.fee.numerator
         denominator = datum.fee.denominator
         values["fee"] = int(numerator * 10000 / denominator)
 
     def swap_datum(
         self,
-        address_source: Address,
+        address: Address,
         in_assets: Assets,
         out_assets: Assets,
-        extra_assets: Assets | None = None,
-        address_target: Address | None = None,
-        datum_target: PlutusData | None = None,
+        forward_address: Address | None = None,
     ) -> PlutusData:
-        if self.swap_forward and address_target is not None:
+        if self.swap_forward and forward_address is not None:
             print(f"{self.__class__.__name__} does not support swap forwarding.")
 
         ident = bytes.fromhex(self.pool_nft.unit()[60:])
 
         return SundaeOrderDatum.create_datum(
             ident=ident,
-            address_source=address_source,
+            address=address,
             in_assets=in_assets,
             out_assets=out_assets,
-            fee=self.batcher_fee(in_assets=in_assets, out_assets=out_assets).quantity(),
+            fee=self.batcher_fee.quantity(),
         )
```

### Comparing `cardex-0.2.0.dev82/src/cardex/dexs/amm/wingriders.py` & `cardex-0.2.0.dev9/src/cardex/dexs/wingriders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from dataclasses import dataclass
 from datetime import datetime
 from datetime import timedelta
-from typing import ClassVar
 from typing import Union
 
+from pycardano import Address
+from pycardano import PlutusData
+
 from cardex.dataclasses.datums import AssetClass
 from cardex.dataclasses.datums import PlutusFullAddress
 from cardex.dataclasses.models import Assets
-from cardex.dataclasses.models import OrderType
 from cardex.dataclasses.models import PoolSelector
-from cardex.dexs.amm.amm_types import AbstractConstantProductPoolState
-from cardex.dexs.amm.amm_types import AbstractStableSwapPoolState
-from cardex.dexs.core.errors import NotAPoolError
-from pycardano import Address
-from pycardano import PlutusData
+from cardex.dexs.amm_types import AbstractConstantProductPoolState
+from cardex.dexs.amm_types import AbstractStableSwapPoolState
 
 
 @dataclass
 class WingriderAssetClass(PlutusData):
     CONSTR_ID = 0
 
     asset_a: AssetClass
@@ -35,35 +33,18 @@
             return cls(
                 asset_a=AssetClass.from_assets(out_assets),
                 asset_b=AssetClass.from_assets(in_assets),
             )
 
 
 @dataclass
-class RewardPlutusPartAddress(PlutusData):
-    """Encode a plutus address part (i.e. payment, stake, etc)."""
-
-    CONSTR_ID = 1
-    address: bytes
-
-
-@dataclass
-class RewardPlutusFullAddress(PlutusFullAddress):
-    """A full address, including payment and staking keys."""
-
-    CONSTR_ID = 0
-
-    payment: RewardPlutusPartAddress
-
-
-@dataclass
 class WingRiderOrderConfig(PlutusData):
     CONSTR_ID = 0
 
-    full_address: Union[PlutusFullAddress, RewardPlutusFullAddress]
+    full_address: PlutusFullAddress
     address: bytes
     expiration: int
     assets: WingriderAssetClass
 
     @classmethod
     def create_config(
         cls,
@@ -93,15 +74,15 @@
 
 @dataclass
 class BtoA(PlutusData):
     CONSTR_ID = 1
 
 
 @dataclass
-class WingRidersOrderDetail(PlutusData):
+class WingRiderOrderDetail(PlutusData):
     CONSTR_ID = 0
 
     direction: Union[AtoB, BtoA]
     min_receive: int
 
     @classmethod
     def from_assets(cls, in_assets: Assets, out_assets: Assets):
@@ -109,112 +90,45 @@
         if in_assets.unit() == merged.unit():
             return cls(direction=AtoB(), min_receive=out_assets.quantity())
         else:
             return cls(direction=BtoA(), min_receive=out_assets.quantity())
 
 
 @dataclass
-class WingRidersDepositDetail(PlutusData):
-    CONSTR_ID = 1
-
-    min_lp_receive: int
-
-
-@dataclass
-class WingRidersWithdrawDetail(PlutusData):
-    CONSTR_ID = 2
-
-    min_amount_a: int
-    min_amount_b: int
-
-
-@dataclass
-class WingRidersMaybeFeeClaimDetail(PlutusData):
-    CONSTR_ID = 3
-
-
-@dataclass
-class WingRidersStakeRewardDetail(PlutusData):
-    CONSTR_ID = 4
-
-
-@dataclass
 class WingRidersOrderDatum(PlutusData):
     CONSTR_ID = 0
 
     config: WingRiderOrderConfig
-    detail: Union[
-        WingRidersDepositDetail,
-        WingRidersMaybeFeeClaimDetail,
-        WingRidersStakeRewardDetail,
-        WingRidersOrderDetail,
-        WingRidersWithdrawDetail,
-    ]
+    detail: WingRiderOrderDetail
 
     @classmethod
     def create_datum(
         cls,
-        address_source: Address,
+        address: Address,
         in_assets: Assets,
         out_assets: Assets,
-        batcher_fee: Assets,
-        deposit: Assets,
-        address_target: Address | None = None,
-        datum_target: PlutusData | None = None,
+        batcher_fee: Assets | None = None,
+        deposit: Assets | None = None,
+        forward_address: Address | None = None,
     ):
         timeout = int(((datetime.utcnow() + timedelta(days=360)).timestamp()) * 1000)
 
         config = WingRiderOrderConfig.create_config(
-            address=address_source,
+            address=address,
             expiration=timeout,
             in_assets=in_assets,
             out_assets=out_assets,
         )
-        detail = WingRidersOrderDetail.from_assets(
+        detail = WingRiderOrderDetail.from_assets(
             in_assets=in_assets,
             out_assets=out_assets,
         )
 
         return cls(config=config, detail=detail)
 
-    def address_source(self) -> Address:
-        return self.config.full_address.to_address()
-
-    def requested_amount(self) -> Assets:
-        if isinstance(self.detail, WingRidersDepositDetail):
-            return Assets({"lp": self.detail.min_lp_receive})
-        elif isinstance(self.detail, WingRidersOrderDetail):
-            if isinstance(self.detail.direction, BtoA):
-                return Assets(
-                    {self.config.assets.asset_a.assets.unit(): self.detail.min_receive},
-                )
-            else:
-                return Assets(
-                    {self.config.assets.asset_b.assets.unit(): self.detail.min_receive},
-                )
-        elif isinstance(self.detail, WingRidersWithdrawDetail):
-            return Assets(
-                {
-                    self.config.assets.asset_a.assets.unit(): self.detail.min_amount_a,
-                    self.config.assets.asset_b.assets.unit(): self.detail.min_amount_b,
-                },
-            )
-        elif isinstance(self.detail, WingRidersMaybeFeeClaimDetail):
-            return Assets({})
-
-    def order_type(self) -> OrderType:
-        if isinstance(self.detail, WingRidersOrderDetail):
-            return OrderType.swap
-        elif isinstance(self.detail, WingRidersDepositDetail):
-            return OrderType.deposit
-        elif isinstance(self.detail, WingRidersWithdrawDetail):
-            return OrderType.withdraw
-        if isinstance(self.detail, WingRidersMaybeFeeClaimDetail):
-            return OrderType.withdraw
-
 
 @dataclass
 class LiquidityPoolAssets(PlutusData):
     CONSTR_ID = 0
     asset_a: AssetClass
     asset_b: AssetClass
 
@@ -238,30 +152,25 @@
         return self.datum.assets.asset_a.assets + self.datum.assets.asset_b.assets
 
 
 class WingRidersCPPState(AbstractConstantProductPoolState):
     fee: int = 35
     _batcher = Assets(lovelace=2000000)
     _deposit = Assets(lovelace=2000000)
-    _stake_address: ClassVar[Address] = Address.from_primitive(
+    _stake_address = Address.from_primitive(
         "addr1wxr2a8htmzuhj39y2gq7ftkpxv98y2g67tg8zezthgq4jkg0a4ul4",
     )
 
     @classmethod
     @property
     def dex(cls) -> str:
         return "WingRiders"
 
     @classmethod
     @property
-    def order_selector(self) -> list[str]:
-        return [self._stake_address.encode()]
-
-    @classmethod
-    @property
     def pool_selector(cls) -> PoolSelector:
         return PoolSelector(
             selector_type="assets",
             selector=cls.dex_policy,
         )
 
     @property
@@ -296,16 +205,14 @@
     def pool_id(self) -> str:
         """A unique identifier for the pool."""
         return self.pool_nft.unit()
 
     @classmethod
     def skip_init(cls, values) -> bool:
         if "pool_nft" in values and "dex_nft" in values:
-            if cls.dex_policy[0] not in values["dex_nft"]:
-                raise NotAPoolError("Invalid DEX NFT")
             if len(values["assets"]) == 3:
                 # Send the ADA token to the end
                 if isinstance(values["assets"], Assets):
                     values["assets"].root["lovelace"] = values["assets"].root.pop(
                         "lovelace",
                     )
                 else:
@@ -324,42 +231,14 @@
 
         if len(assets) == 2:
             assets.root[assets.unit(0)] -= 3000000
 
         assets.root[assets.unit(0)] -= datum.datum.quantity_a
         assets.root[assets.unit(1)] -= datum.datum.quantity_b
 
-    def deposit(
-        self,
-        in_assets: Assets | None = None,
-        out_assets: Assets | None = None,
-    ):
-        merged_assets = in_assets + out_assets
-        if "lovelace" in merged_assets:
-            return Assets(lovelace=4000000) - self.batcher_fee(
-                in_assets=in_assets,
-                out_assets=out_assets,
-            )
-        else:
-            return self._deposit
-
-    def batcher_fee(
-        self,
-        in_assets: Assets | None = None,
-        out_assets: Assets | None = None,
-        extra_assets: Assets | None = None,
-    ):
-        merged_assets = in_assets + out_assets
-        if "lovelace" in merged_assets:
-            if merged_assets["lovelace"] <= 250000000:
-                return Assets(lovelace=850000)
-            elif merged_assets["lovelace"] <= 500000000:
-                return Assets(lovelace=1500000)
-        return self._batcher
-
 
 class WingRidersSSPState(AbstractStableSwapPoolState, WingRidersCPPState):
     fee: int = 6
     _batcher = Assets(lovelace=1500000)
     _deposit = Assets(lovelace=2000000)
     _stake_address = Address.from_primitive(
         "addr1w8z7qwzszt2lqy93m3atg2axx22yq5k7yvs9rmrvuwlawts2wzadz",
```

### Comparing `cardex-0.2.0.dev82/src/cardex/utility.py` & `cardex-0.2.0.dev9/src/cardex/utility.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev82/PKG-INFO` & `cardex-0.2.0.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardex
-Version: 0.2.0.dev82
+Version: 0.2.0.dev9
 Summary: 
 Author: Elder Millenial
 Author-email: eldermillenial@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

