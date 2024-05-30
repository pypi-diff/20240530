# Comparing `tmp/paicorelib-1.1.2.tar.gz` & `tmp/paicorelib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paicorelib-1.1.2.tar", max compression
+gzip compressed data, was "paicorelib-1.1.3.tar", max compression
```

## Comparing `paicorelib-1.1.2.tar` & `paicorelib-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0      308 2024-05-20 06:16:24.892903 paicorelib-1.1.2/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-05-20 06:16:24.892903 paicorelib-1.1.2/LICENSE
--rw-r--r--   0        0        0      833 2024-05-20 06:16:24.892903 paicorelib-1.1.2/README.md
--rw-r--r--   0        0        0     1775 2024-05-20 06:16:24.892903 paicorelib-1.1.2/docs/Table-of-Terms.md
--rw-r--r--   0        0        0     1188 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/__init__.py
--rw-r--r--   0        0        0    15668 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/coordinate.py
--rw-r--r--   0        0        0       81 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/__init__.py
--rw-r--r--   0        0        0     5212 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/base.py
--rw-r--r--   0        0        0     7009 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/frame_defs.py
--rw-r--r--   0        0        0     9900 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/frame_gen.py
--rw-r--r--   0        0        0    22228 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/frames.py
--rw-r--r--   0        0        0      736 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/types.py
--rw-r--r--   0        0        0     4077 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/utils.py
--rw-r--r--   0        0        0     1532 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/hw_defs.py
--rw-r--r--   0        0        0     2312 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/hw_types.py
--rw-r--r--   0        0        0     7488 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/ram_model.py
--rw-r--r--   0        0        0     2618 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/ram_types.py
--rw-r--r--   0        0        0     5816 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/reg_model.py
--rw-r--r--   0        0        0     4265 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/reg_types.py
--rw-r--r--   0        0        0     5747 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/routing_defs.py
--rw-r--r--   0        0        0     1729 2024-05-20 06:16:24.892903 paicorelib-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 paicorelib-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-30 06:30:30.729359 paicorelib-1.1.3/LICENSE
+-rw-r--r--   0        0        0      823 2024-05-30 06:30:30.729359 paicorelib-1.1.3/README.md
+-rw-r--r--   0        0        0     1188 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/__init__.py
+-rw-r--r--   0        0        0    15655 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/coordinate.py
+-rw-r--r--   0        0        0       81 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/framelib/__init__.py
+-rw-r--r--   0        0        0     5550 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/framelib/base.py
+-rw-r--r--   0        0        0     7009 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/framelib/frame_defs.py
+-rw-r--r--   0        0        0     9894 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/framelib/frame_gen.py
+-rw-r--r--   0        0        0    22318 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/framelib/frames.py
+-rw-r--r--   0        0        0      723 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/framelib/types.py
+-rw-r--r--   0        0        0     4257 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/framelib/utils.py
+-rw-r--r--   0        0        0     1532 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/hw_defs.py
+-rw-r--r--   0        0        0     2306 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/hw_types.py
+-rw-r--r--   0        0        0     7463 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/ram_model.py
+-rw-r--r--   0        0        0     2618 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/ram_types.py
+-rw-r--r--   0        0        0     5816 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/reg_model.py
+-rw-r--r--   0        0        0     4234 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/reg_types.py
+-rw-r--r--   0        0        0     5730 2024-05-30 06:30:30.729359 paicorelib-1.1.3/paicorelib/routing_defs.py
+-rw-r--r--   0        0        0     1624 2024-05-30 06:30:30.729359 paicorelib-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 paicorelib-1.1.3/PKG-INFO
```

### Comparing `paicorelib-1.1.2/LICENSE` & `paicorelib-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.2/paicorelib/__init__.py` & `paicorelib-1.1.3/paicorelib/__init__.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.2/paicorelib/coordinate.py` & `paicorelib-1.1.3/paicorelib/coordinate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 import sys
 from abc import ABC, abstractmethod
 from enum import Enum, auto
-from typing import List, Sequence, Tuple, TypeVar, Union, final, overload
+from typing import Sequence, TypeVar, Union, final, overload
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 from pydantic import Field
@@ -24,15 +24,15 @@
     "RIdLike",
     "to_coord",
     "to_coords",
     "to_coordoffset",
     "to_rid",
 ]
 
-CoordTuple: TypeAlias = Tuple[int, int]
+CoordTuple: TypeAlias = tuple[int, int]
 CoordAddr: TypeAlias = int
 
 
 def _xy_parser(other: Union[CoordTuple, "CoordOffset"]) -> CoordTuple:
     """Parse the coordinate in tuple format."""
     if not isinstance(other, (tuple, CoordOffset)):
         raise TypeError(f"unsupported type: {type(other)}.")
@@ -497,15 +497,15 @@
             )
 
         return Coord(*coordlike)
 
     return coordlike
 
 
-def to_coords(coordlikes: Sequence[CoordLike]) -> List[Coord]:
+def to_coords(coordlikes: Sequence[CoordLike]) -> list[Coord]:
     return [to_coord(coordlike) for coordlike in coordlikes]
 
 
 def to_coordoffset(offset: int) -> CoordOffset:
     return CoordOffset(
         offset % (HwParams.CORE_X_MAX + 1), offset // (HwParams.CORE_Y_MAX + 1)
     )
```

### Comparing `paicorelib-1.1.2/paicorelib/framelib/base.py` & `paicorelib-1.1.3/paicorelib/framelib/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         4 bits         10 bits             10 bits             10 bits         30 bits
     """
 
     header: FH
     chip_coord: Coord
     core_coord: Coord
     rid: RId
-    payload: Union[int, FRAME_DTYPE, FrameArrayType] = field(
+    payload: Union[FRAME_DTYPE, FrameArrayType] = field(
         default_factory=lambda: np.empty(0, dtype=FRAME_DTYPE)
     )
 
     @classmethod
     def _decode(
         cls,
         header: FH,
@@ -61,15 +61,15 @@
     @property
     def rid_addr(self) -> int:
         return self.rid.address
 
     @property
     def value(self) -> FrameArrayType:
         """Get the full frames of the single frame."""
-        if isinstance(self.payload, (int, np.integer)):
+        if isinstance(self.payload, np.integer):
             pl = np.asarray([self.payload], dtype=FRAME_DTYPE)
         else:
             pl = self.payload
 
         value = self._frame_common + (pl & FF.GENERAL_PAYLOAD_MASK)
         value = np.asarray(value, dtype=FRAME_DTYPE)
         value.setflags(write=False)
@@ -100,15 +100,15 @@
             f"Chip address:         {self.chip_coord}\n"
             f"Core address:         {self.core_coord}\n"
             f"Replication address:  {self.rid}\n"
             f"Payload:              {self.payload}\n"
         )
 
     def __deepcopy__(self) -> "Frame":
-        """Deep copy the payload only, and return a new `Frame`."""
+        """Deep copy the frame and return a new `Frame`."""
         return Frame(
             self.header,
             self.chip_coord,
             self.core_coord,
             self.rid,
             copy.deepcopy(self.payload),
         )
@@ -121,15 +121,15 @@
     1. [Header(sub type)] + [chip coordinate] + [core coordinate] + [replication id] + [payload]
             4 bits               10 bits            10 bits            10 bits          30 bits
     2. [contents[0]], 64 bits.
     N+1. [contents[N-1]], 64 bits.
 
     """
 
-    payload: FRAME_DTYPE
+    payload: FRAME_DTYPE = FRAME_DTYPE(0)
     packages: FrameArrayType = field(
         default_factory=lambda: np.empty(0, dtype=FRAME_DTYPE)
     )
 
     @classmethod
     def _decode(
         cls,
@@ -172,7 +172,18 @@
             f"Data:\n"
         )
 
         for i in range(self.n_package):
             _present += f"#{i}: {self.packages[i]}\n"
 
         return _present
+
+    def __deepcopy__(self) -> "FramePackage":
+        """Deep copy the frame package and return a new `FramePackage`."""
+        return FramePackage(
+            self.header,
+            self.chip_coord,
+            self.core_coord,
+            self.rid,
+            self.payload.copy(),
+            copy.deepcopy(self.packages),
+        )
```

### Comparing `paicorelib-1.1.2/paicorelib/framelib/frame_defs.py` & `paicorelib-1.1.3/paicorelib/framelib/frame_defs.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.2/paicorelib/framelib/frame_gen.py` & `paicorelib-1.1.3/paicorelib/framelib/frame_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Union, overload
+from typing import Any, Union, overload
 
 import numpy as np
 from numpy.typing import NDArray
 
 from paicorelib import LCN_EX, Coord, NeuronAttrs, NeuronDestInfo, ParamsReg
 from paicorelib import ReplicationId as RId
 from paicorelib import WeightPrecision as WP
@@ -27,24 +27,24 @@
     def gen_config_frame2(
         chip_coord: Coord, core_coord: Coord, rid: RId, /, params_reg: ParamsReg
     ) -> OfflineConfigFrame2: ...
 
     @overload
     @staticmethod
     def gen_config_frame2(
-        chip_coord: Coord, core_coord: Coord, rid: RId, /, params_reg: Dict[str, Any]
+        chip_coord: Coord, core_coord: Coord, rid: RId, /, params_reg: dict[str, Any]
     ) -> OfflineConfigFrame2: ...
 
     @staticmethod
     def gen_config_frame2(
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
-        params_reg: Union[ParamsReg, Dict[str, Any]],
+        params_reg: Union[ParamsReg, dict[str, Any]],
     ) -> OfflineConfigFrame2:
         if isinstance(params_reg, ParamsReg):
             _params_reg = params_reg.model_dump(by_alias=True)
         else:
             _params_reg = params_reg
 
         return OfflineConfigFrame2(chip_coord, core_coord, rid, _params_reg)
@@ -70,31 +70,31 @@
     def gen_config_frame3(
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
         sram_start_addr: IntScalarType,
         n_neuron: IntScalarType,
-        attrs: Dict[str, Any],
-        dest_info: Dict[str, Any],
+        attrs: dict[str, Any],
+        dest_info: dict[str, Any],
         *,
         lcn_ex: LCN_EX = LCN_EX.LCN_1X,
         weight_precision: WP = WP.WEIGHT_WIDTH_1BIT,
     ) -> OfflineConfigFrame3: ...
 
     @staticmethod
     def gen_config_frame3(
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
         sram_start_addr: IntScalarType,
         n_neuron: IntScalarType,
-        attrs: Union[NeuronAttrs, Dict[str, Any]],
-        dest_info: Union[NeuronDestInfo, Dict[str, Any]],
+        attrs: Union[NeuronAttrs, dict[str, Any]],
+        dest_info: Union[NeuronDestInfo, dict[str, Any]],
         *,
         lcn_ex: LCN_EX = LCN_EX.LCN_1X,
         weight_precision: WP = WP.WEIGHT_WIDTH_1BIT,
     ) -> OfflineConfigFrame3:
         if isinstance(attrs, NeuronAttrs):
             _attrs = attrs.model_dump(by_alias=True)
         else:
@@ -185,24 +185,24 @@
     @overload
     @staticmethod
     def gen_testout_frame2(
         test_chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
-        params_reg: Dict[str, Any],
+        params_reg: dict[str, Any],
     ) -> OfflineTestOutFrame2: ...
 
     @staticmethod
     def gen_testout_frame2(
         test_chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
-        params_reg: Union[ParamsReg, Dict[str, Any]],
+        params_reg: Union[ParamsReg, dict[str, Any]],
     ) -> OfflineTestOutFrame2:
         if isinstance(params_reg, ParamsReg):
             pr = params_reg.model_dump(by_alias=True)
         else:
             pr = params_reg
 
         return OfflineTestOutFrame2(test_chip_coord, core_coord, rid, pr)
@@ -224,16 +224,16 @@
     def gen_testout_frame3(
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
         sram_start_addr: IntScalarType,
         n_neuron: IntScalarType,
-        attrs: Union[NeuronAttrs, Dict[str, Any]],
-        dest_info: Union[NeuronDestInfo, Dict[str, Any]],
+        attrs: Union[NeuronAttrs, dict[str, Any]],
+        dest_info: Union[NeuronDestInfo, dict[str, Any]],
         *,
         lcn_ex: LCN_EX = LCN_EX.LCN_1X,
         weight_precision: WP = WP.WEIGHT_WIDTH_1BIT,
     ) -> OfflineTestOutFrame3:
         if isinstance(attrs, NeuronAttrs):
             _attrs = attrs.model_dump(by_alias=True)
         else:
@@ -285,15 +285,15 @@
             int(sram_start_addr),
             int(n_data_package),
             weight_ram,
         )
 
     @staticmethod
     def gen_work_frame1(
-        one_input_node: Dict[str, Any],
+        one_input_node: dict[str, Any],
         data: DataArrayType,
     ) -> FrameArrayType:
         """Generate the common part of the input spike frames by given the info \
             of one input node.
 
         Args:
             - one_input_node: a dictionary of one input node.
```

### Comparing `paicorelib-1.1.2/paicorelib/framelib/frames.py` & `paicorelib-1.1.3/paicorelib/framelib/frames.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import Any, ClassVar, Dict, Literal, Optional, Union
+from typing import Any, ClassVar, Literal, Optional, Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 from paicorelib import Coord, CoordLike
 from paicorelib import ReplicationId as RId
 from paicorelib import RIdLike, to_coord, to_rid
@@ -92,23 +92,23 @@
 class _ParamRAMFrame(Frame):
     def __init__(
         self,
         header: FH,
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
-        params_reg_dict: Dict[str, Any],
+        params_reg_dict: dict[str, Any],
     ) -> None:
         payload = self._payload_reorganized(params_reg_dict)
 
         super().__init__(header, chip_coord, core_coord, rid, payload)
 
     @staticmethod
     @params_check(ParamsRegChecker)
-    def _payload_reorganized(reg_dict: Dict[str, Any]) -> FrameArrayType:
+    def _payload_reorganized(reg_dict: dict[str, Any]) -> FrameArrayType:
         # High 8 bits & low 7 bits of tick_wait_start
         tws_high8, tws_low7 = bin_split(reg_dict["tick_wait_start"], 7, 8)
         # High 3 bits & low 7 bits of test_chip_addr
         tca_high3, tca_low7 = bin_split(reg_dict["test_chip_addr"], 7, 3)
 
         reg_frame1 = (
             (reg_dict["weight_width"] & RegF.WEIGHT_WIDTH_MASK)
@@ -169,16 +169,16 @@
         self,
         header: FH,
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         sram_start_addr: int,
         neuron_num: int,
-        neuron_attrs: Dict[str, Any],
-        neuron_dest_info: Dict[str, Any],
+        neuron_attrs: dict[str, Any],
+        neuron_dest_info: dict[str, Any],
         repeat: int,
     ) -> None:
         n_package = 4 * neuron_num * repeat
         payload = _package_arg_check(
             sram_start_addr, n_package, _L_PACKAGE_TYPE_CONF_TESTOUT
         )
         packages = self._packages_reorganized(
@@ -189,16 +189,16 @@
         )
 
         super().__init__(header, chip_coord, core_coord, rid, payload, packages)
 
     @staticmethod
     @params_check2(NeuronAttrsChecker, NeuronDestInfoChecker)
     def _packages_reorganized(
-        attrs: Dict[str, Any],
-        dest_info: Dict[str, Any],
+        attrs: dict[str, Any],
+        dest_info: dict[str, Any],
         neuron_num: int,
         repeat: int,
     ) -> FrameArrayType:
         tick_relative = dest_info["tick_relative"]
         addr_axon = dest_info["addr_axon"]
 
         if len(tick_relative) != len(addr_axon):
@@ -368,15 +368,15 @@
 
     def __init__(
         self,
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
-        params_reg_dict: Dict[str, Any],
+        params_reg_dict: dict[str, Any],
     ) -> None:
         super().__init__(self.header, chip_coord, core_coord, rid, params_reg_dict)
 
 
 class OfflineConfigFrame3(_NeuronRAMFrame):
     header: ClassVar[FH] = FH.CONFIG_TYPE3
 
@@ -384,16 +384,16 @@
         self,
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
         sram_start_addr: int,
         neuron_num: int,
-        neuron_attrs: Dict[str, Any],
-        neuron_dest_info: Dict[str, Any],
+        neuron_attrs: dict[str, Any],
+        neuron_dest_info: dict[str, Any],
         repeat: int = 1,
     ) -> None:
         super().__init__(
             self.header,
             chip_coord,
             core_coord,
             rid,
@@ -429,15 +429,15 @@
         )
 
 
 class OfflineTestInFrame1(Frame):
     header: ClassVar[FH] = FH.TEST_TYPE1
 
     def __init__(self, chip_coord: Coord, core_coord: Coord, rid: RId, /) -> None:
-        super().__init__(self.header, chip_coord, core_coord, rid, 0)
+        super().__init__(self.header, chip_coord, core_coord, rid, FRAME_DTYPE(0))
 
 
 class OfflineTestOutFrame1(_RandomSeedFrame):
     header: ClassVar[FH] = FH.TEST_TYPE1
 
     def __init__(
         self,
@@ -450,27 +450,27 @@
         super().__init__(self.header, test_chip_coord, core_coord, rid, random_seed)
 
 
 class OfflineTestInFrame2(Frame):
     header: ClassVar[FH] = FH.TEST_TYPE2
 
     def __init__(self, chip_coord: Coord, core_coord: Coord, rid: RId, /) -> None:
-        super().__init__(self.header, chip_coord, core_coord, rid, 0)
+        super().__init__(self.header, chip_coord, core_coord, rid, FRAME_DTYPE(0))
 
 
 class OfflineTestOutFrame2(_ParamRAMFrame):
     header: ClassVar[FH] = FH.TEST_TYPE2
 
     def __init__(
         self,
         test_chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
-        params_reg_dict: Dict[str, Any],
+        params_reg_dict: dict[str, Any],
     ) -> None:
         super().__init__(self.header, test_chip_coord, core_coord, rid, params_reg_dict)
 
 
 class OfflineTestInFrame3(Frame):
     header: ClassVar[FH] = FH.TEST_TYPE3
 
@@ -497,16 +497,16 @@
         self,
         test_chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
         sram_start_addr: int,
         neuron_num: int,
-        neuron_attrs: Dict[str, Any],
-        neuron_dest_info: Dict[str, Any],
+        neuron_attrs: dict[str, Any],
+        neuron_dest_info: dict[str, Any],
         repeat: int = 1,
     ) -> None:
         super().__init__(
             self.header,
             test_chip_coord,
             core_coord,
             rid,
@@ -604,15 +604,15 @@
 
     @property
     def target_axon(self) -> int:
         return self._axon
 
     @staticmethod
     @params_check(NeuronDestInfoChecker)
-    def _frame_dest_reorganized(dest_info: Dict[str, Any]) -> FrameArrayType:
+    def _frame_dest_reorganized(dest_info: dict[str, Any]) -> FrameArrayType:
         return OfflineWorkFrame1.concat_frame_dest(
             (dest_info["addr_chip_x"], dest_info["addr_chip_y"]),
             (dest_info["addr_core_x"], dest_info["addr_core_y"]),
             (dest_info["addr_core_x_ex"], dest_info["addr_core_y_ex"]),
             dest_info["addr_axon"],
             dest_info["tick_relative"],
         )
@@ -689,22 +689,26 @@
         )
 
 
 class OfflineWorkFrame3(Frame):
     header: ClassVar[FH] = FH.WORK_TYPE3
 
     def __init__(self, chip_coord: Coord) -> None:
-        super().__init__(self.header, chip_coord, Coord(0, 0), RId(0, 0), 0)
+        super().__init__(
+            self.header, chip_coord, Coord(0, 0), RId(0, 0), FRAME_DTYPE(0)
+        )
 
 
 class OfflineWorkFrame4(Frame):
     header: ClassVar[FH] = FH.WORK_TYPE4
 
     def __init__(self, chip_coord: Coord) -> None:
-        super().__init__(self.header, chip_coord, Coord(0, 0), RId(0, 0), 0)
+        super().__init__(
+            self.header, chip_coord, Coord(0, 0), RId(0, 0), FRAME_DTYPE(0)
+        )
 
 
 def _package_arg_check(
     sram_start_addr: int, data_package_num: int, package_type: Literal[0, 1]
 ) -> FRAME_DTYPE:
     if sram_start_addr > RAMF.GENERAL_PACKAGE_SRAM_ADDR_MASK or sram_start_addr < 0:
         raise ValueError(f"SRAM start address out of range, {sram_start_addr}.")
```

### Comparing `paicorelib-1.1.2/paicorelib/framelib/types.py` & `paicorelib-1.1.3/paicorelib/framelib/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import sys
-from typing import List, Tuple, TypeVar
+from typing import TypeVar
 
 import numpy as np
 from numpy.typing import NDArray
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 FRAME_DTYPE: TypeAlias = np.uint64
 FrameArrayType: TypeAlias = NDArray[FRAME_DTYPE]
-ArrayType = TypeVar("ArrayType", List[int], Tuple[int, ...], np.ndarray)
+ArrayType = TypeVar("ArrayType", list[int], tuple[int, ...], np.ndarray)
 BasicFrameArray = TypeVar(
-    "BasicFrameArray", int, List[int], Tuple[int, ...], NDArray[FRAME_DTYPE]
+    "BasicFrameArray", int, list[int], tuple[int, ...], NDArray[FRAME_DTYPE]
 )
 IntScalarType = TypeVar("IntScalarType", int, np.bool_, np.integer)
 DataType = TypeVar("DataType", int, np.bool_, np.integer, np.ndarray)
 DataArrayType = TypeVar(
-    "DataArrayType", int, np.bool_, np.integer, List[int], Tuple[int, ...], np.ndarray
+    "DataArrayType", int, np.bool_, np.integer, list[int], tuple[int, ...], np.ndarray
 )
```

### Comparing `paicorelib-1.1.2/paicorelib/framelib/utils.py` & `paicorelib-1.1.3/paicorelib/framelib/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+import sys
 import warnings
 from functools import wraps
 from pathlib import Path
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Optional
 
 import numpy as np
 from pydantic import TypeAdapter
 
 from .frame_defs import FrameFormat as FF
 from .frame_defs import FrameHeader as FH
 from .frame_defs import FrameType as FT
 from .frame_defs import _mask
 from .types import FRAME_DTYPE, BasicFrameArray, FrameArrayType
 
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias
+else:
+    from typing_extensions import TypeAlias
+
 
 class FrameIllegalError(ValueError):
     """Frame is illegal."""
 
     pass
 
 
@@ -101,19 +107,25 @@
 
 def np2txt(fp: Path, d: np.ndarray) -> None:
     with open(fp, "w") as f:
         for i in range(d.size):
             f.write("{:064b}\n".format(d[i]))
 
 
-def bin_split(x: int, pos: int, high_mask_bit: Optional[int] = None) -> Tuple[int, int]:
-    """Split an integer, return the high and low part.
+HighBit: TypeAlias = int
+LowBit: TypeAlias = int
+
+
+def bin_split(
+    x: int, pos: int, high_mask_bit: Optional[int] = None
+) -> tuple[HighBit, LowBit]:
+    """Split an integer and return the high & low bits.
 
     Argument:
-        - x: the integer
+        - x: the integer.
         - pos: the position (LSB) to split the binary.
         - high_mask: mask for the high part. Optional.
 
     Example::
 
         >>> bin_split(0b1100001001, 3)
         97(0b1100001), 1
@@ -127,27 +139,27 @@
 
     return high, low
 
 
 def params_check(checker: TypeAdapter):
     def inner(func):
         @wraps(func)
-        def wrapper(params: Dict[str, Any], *args, **kwargs):
+        def wrapper(params: dict[str, Any], *args, **kwargs):
             checked = checker.validate_python(params)
             return func(checked, *args, **kwargs)
 
         return wrapper
 
     return inner
 
 
 def params_check2(checker1: TypeAdapter, checker2: TypeAdapter):
     def inner(func):
         @wraps(func)
-        def wrapper(params1: Dict[str, Any], params2: Dict[str, Any], *args, **kwargs):
+        def wrapper(params1: dict[str, Any], params2: dict[str, Any], *args, **kwargs):
             checked1 = checker1.validate_python(params1)
             checked2 = checker2.validate_python(params2)
             return func(checked1, checked2, *args, **kwargs)
 
         return wrapper
 
     return inner
```

### Comparing `paicorelib-1.1.2/paicorelib/hw_defs.py` & `paicorelib-1.1.3/paicorelib/hw_defs.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.2/paicorelib/hw_types.py` & `paicorelib-1.1.3/paicorelib/hw_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import ClassVar, List, NamedTuple
+from typing import ClassVar, NamedTuple
 
 from .hw_defs import HwParams
 from .reg_types import CoreMode
 
 __all__ = ["NeuronSegment", "AxonCoord", "AxonSegment", "HwCore"]
 
 
@@ -44,15 +44,15 @@
             raise ValueError(
                 f"RAM address out of range {HwParams.ADDR_RAM_MAX} ({_addr_max})."
             )
 
         return _addr_max
 
     @property
-    def addr_ram(self) -> List[int]:
+    def addr_ram(self) -> list[int]:
         """Convert index of neuron into RAM address."""
         return list(range(self.addr_offset, self.addr_max, 1))
 
     @property
     def addr_slice(self) -> slice:
         """Display the RAM address in slice format."""
         return slice(
```

### Comparing `paicorelib-1.1.2/paicorelib/ram_model.py` & `paicorelib-1.1.3/paicorelib/ram_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List
-
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     InstanceOf,
     field_serializer,
     field_validator,
@@ -61,19 +59,19 @@
     addr_core_y_ex: NonNegativeInt = Field(
         lt=(1 << ADDR_CORE_Y_EX_BIT_MAX),
         description="Broadcast address Y of destination core.",
     )
 
 
 class NeuronDestInfo(_BasicNeuronDest):
-    tick_relative: List[InstanceOf[NonNegativeInt]] = Field(
+    tick_relative: list[InstanceOf[NonNegativeInt]] = Field(
         description="Information of relative ticks.",
     )
 
-    addr_axon: List[InstanceOf[NonNegativeInt]] = Field(
+    addr_axon: list[InstanceOf[NonNegativeInt]] = Field(
         description="Destination axon address."
     )
 
     @field_validator("tick_relative")
     @classmethod
     def _tick_relative_check(cls, v):
         if any(tr >= (1 << TICK_RELATIVE_BIT_MAX) or tr < 0 for tr in v):
@@ -235,13 +233,13 @@
 
     addr_core_x: int
     addr_core_y: int
     addr_core_x_ex: int
     addr_core_y_ex: int
     addr_chip_x: int
     addr_chip_y: int
-    tick_relative: List[int]
-    addr_axon: List[int]
+    tick_relative: list[int]
+    addr_axon: list[int]
 
 
 NeuronAttrsChecker = TypeAdapter(_NeuronAttrsDict)
 NeuronDestInfoChecker = TypeAdapter(_NeuronDestInfoDict)
```

### Comparing `paicorelib-1.1.2/paicorelib/ram_types.py` & `paicorelib-1.1.3/paicorelib/ram_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,22 @@
     MODE_NONRESET = 2
 
 
 @unique
 class LeakComparisonMode(Enum):
     """Leak after comparison or before. 1-bit.
 
-    - `LEAK_BEFORE_COMP`: leak before comparison.
-    - `LEAK_AFTER_COMP`: leak after comparison. Default value.
+    - `LEAK_BEFORE_COMP`: leak before comparison. Default value.
+    - `LEAK_AFTER_COMP`: leak after comparison.
 
     NOTE: Same as `leak_post` in V2.1.
     """
 
-    LEAK_BEFORE_COMP = 0
-    LEAK_AFTER_COMP = 1  # Default value.
+    LEAK_BEFORE_COMP = 0  # Default value.
+    LEAK_AFTER_COMP = 1
 
 
 @unique
 class NegativeThresholdMode(Enum):
     """Modes of negative threshold. 1-bit.
 
     - `MODE_RESET`: reset mode. Default value.
```

### Comparing `paicorelib-1.1.2/paicorelib/reg_model.py` & `paicorelib-1.1.3/paicorelib/reg_model.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.2/paicorelib/reg_types.py` & `paicorelib-1.1.3/paicorelib/reg_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import sys
 from enum import Enum, IntEnum, unique
-from typing import Dict, Tuple
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 __all__ = [
@@ -135,18 +134,18 @@
     MODE_BANN = 1  # SNN mode like.
     MODE_ANN = 2
     MODE_BANN_OR_SNN_TO_ANN = 3
     MODE_BANN_OR_SNN_TO_SNN = 4
     MODE_ANN_TO_BANN_OR_SNN = 5
 
 
-_ModeParamRef: TypeAlias = Tuple[
+_ModeParamRef: TypeAlias = tuple[
     InputWidthFormatType, SpikeWidthFormatType, SNNModeEnableType
 ]
-CoreModeDict: Dict[CoreMode, _ModeParamRef] = {
+CoreModeDict: dict[CoreMode, _ModeParamRef] = {
     CoreMode.MODE_BANN: (
         InputWidthFormatType.WIDTH_1BIT,
         SpikeWidthFormatType.WIDTH_1BIT,
         SNNModeEnableType.DISABLE,
     ),
     CoreMode.MODE_SNN: (
         InputWidthFormatType.WIDTH_1BIT,
```

### Comparing `paicorelib-1.1.2/paicorelib/routing_defs.py` & `paicorelib-1.1.3/paicorelib/routing_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum, IntEnum, unique
-from typing import NamedTuple, Sequence, Set
+from typing import NamedTuple, Sequence
 
 from .coordinate import Coord
 from .coordinate import ReplicationId as RId
 from .hw_defs import HwParams
 
 __all__ = [
     "RoutingLevel",
@@ -197,16 +197,16 @@
 
     for coord in coords[1:]:
         rid |= base_coord ^ coord
 
     return rid
 
 
-def get_multicast_cores(base_coord: Coord, rid: RId) -> Set[Coord]:
-    cores: Set[Coord] = set()
+def get_multicast_cores(base_coord: Coord, rid: RId) -> set[Coord]:
+    cores = set()
     corex = set()
     corey = set()
     temp = set()
 
     corex.add(base_coord.x)
     corey.add(base_coord.y)
```

### Comparing `paicorelib-1.1.2/pyproject.toml` & `paicorelib-1.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paicorelib"
-version = "1.1.2"
+version = "1.1.3"
 description = "Library of PAICORE 2.0"
 authors = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
 maintainers = [
     "Hongtu Xia <hongtux@pku.edu.cn>",
     "Siyuan Gao <siyuan-gao@outlook.com>",
     "Zhaoyang Hao <hzyang2218@gmail.com>",
     "Ziru Pan <zrpan@stu.pku.edu.cn>",
@@ -16,34 +16,30 @@
 documentation = "https://github.com/PAICookers/PAIlib#readme"
 keywords = ["PAICORE 2.0", "PAICORE library", "PAILib"]
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [{ include = "paicorelib" }]
 
-# Includes the document
-include = ["docs", "CHANGELOG.md"]
-
 [tool.poetry.dependencies]
-python = "^3.8"
-numpy = "^1.24.0"
+python = "^3.9"
+numpy = "^1.26.0"
 pydantic = "^2.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = { version = "^8.0.0", python = "^3.8" }
+pytest = { version = "^8.0.0", python = "^3.9" }
 pytest-md = "^0.2.0"
 
 
 [tool.pytest.ini_options]
 minversion = "7.0.0"
 testpaths = ["tests"]
```

### Comparing `paicorelib-1.1.2/PKG-INFO` & `paicorelib-1.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 Metadata-Version: 2.1
 Name: paicorelib
-Version: 1.1.2
+Version: 1.1.3
 Summary: Library of PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAIlib
 License: GPL-3.0-or-later
 Keywords: PAICORE 2.0,PAICORE library,PAILib
 Author: Ziru Pan
 Author-email: zrpan@stu.pku.edu.cn
 Maintainer: Hongtu Xia
 Maintainer-email: hongtux@pku.edu.cn
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: numpy (>=1.26.0,<2.0.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Documentation, https://github.com/PAICookers/PAIlib#readme
 Project-URL: Repository, https://github.com/PAICookers/PAIlib
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # Library of PAICORE 2.0
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIlib/blob/master/pyproject.toml">
-        <img src="https://img.shields.io/pypi/pyversions/paicorelib">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/paicorelib">
     </a>
-    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.2"
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?color=orange">
+    <a href="https://pypi.org/project/paicorelib/">
+        <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/paicorelib?color=pink">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIlib">
-      <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIlib/master?color=red">
+        <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIlib?color=orange">
     </a>
-    <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIlib/master">
-	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIlib/master.svg" alt="pre-commit.ci status">
+    <a href="https://wakatime.com/badge/github/PAICookers/PAIlib">
+        <img alt="wakatime" src="https://wakatime.com/badge/github/PAICookers/PAIlib.svg">
     </a>
-
 </p>
 
 [Changelog](./CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 2.1 Name: paicorelib Version: 1.1.2 Summary: Library of
+Metadata-Version: 2.1 Name: paicorelib Version: 1.1.3 Summary: Library of
 PAICORE 2.0 Home-page: https://github.com/PAICookers/PAIlib License: GPL-3.0-
 or-later Keywords: PAICORE 2.0,PAICORE library,PAILib Author: Ziru Pan Author-
 email: zrpan@stu.pku.edu.cn Maintainer: Hongtu Xia Maintainer-email:
-hongtux@pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
+hongtux@pku.edu.cn Requires-Python: >=3.9,<4.0 Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries Requires-Dist: numpy (>=1.24.0,<2.0.0) Requires-Dist:
-pydantic (>=2.0,<3.0) Project-URL: Documentation, https://github.com/
-PAICookers/PAIlib#readme Project-URL: Repository, https://github.com/
-PAICookers/PAIlib Description-Content-Type: text/markdown
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries Requires-Dist: numpy
+(>=1.26.0,<2.0.0) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL:
+Documentation, https://github.com/PAICookers/PAIlib#readme Project-URL:
+Repository, https://github.com/PAICookers/PAIlib Description-Content-Type:
+text/markdown
                            # Library of PAICORE 2.0
-     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_c_o_r_e_l_i_b_]img src="https://
-       img.shields.io/github/v/release/PAICookers/PAIlib?color=orange">
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_/
-_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
+      _[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_C_o_d_e_F_a_c_t_o_r_ _G_r_a_d_e_]_[_w_a_k_a_t_i_m_e_]
 [Changelog](./CHANGELOG.md)
```

