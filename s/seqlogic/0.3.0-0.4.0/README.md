# Comparing `tmp/seqlogic-0.3.0.tar.gz` & `tmp/seqlogic-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqlogic-0.3.0.tar", last modified: Tue May 28 01:40:32 2024, max compression
+gzip compressed data, was "seqlogic-0.4.0.tar", last modified: Wed May 29 05:45:48 2024, max compression
```

## Comparing `seqlogic-0.3.0.tar` & `seqlogic-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.366601 seqlogic-0.3.0/
--rw-rw-rw-   0        0        0      956 2024-05-28 01:40:32.362720 seqlogic-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      740 2024-03-11 04:13:25.000000 seqlogic-0.3.0/README.md
--rw-rw-rw-   0        0        0      263 2024-05-28 01:39:22.000000 seqlogic-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 01:40:32.366601 seqlogic-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.280326 seqlogic-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.304640 seqlogic-0.3.0/src/seqlogic/
--rw-rw-rw-   0        0        0      357 2024-05-27 19:30:40.000000 seqlogic-0.3.0/src/seqlogic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.334312 seqlogic-0.3.0/src/seqlogic/algorithms/
--rw-rw-rw-   0        0        0       27 2023-11-27 07:28:50.000000 seqlogic-0.3.0/src/seqlogic/algorithms/__init__.py
--rw-rw-rw-   0        0        0    12685 2024-03-10 17:38:01.000000 seqlogic-0.3.0/src/seqlogic/algorithms/aes.py
--rw-rw-rw-   0        0        0      285 2024-04-30 03:11:09.000000 seqlogic-0.3.0/src/seqlogic/algorithms/gray.py
--rw-rw-rw-   0        0        0    21662 2024-05-08 03:13:26.000000 seqlogic-0.3.0/src/seqlogic/bits.py
--rw-rw-rw-   0        0        0    10371 2024-05-28 01:31:22.000000 seqlogic-0.3.0/src/seqlogic/design.py
--rw-rw-rw-   0        0        0     2962 2024-05-22 04:04:04.000000 seqlogic-0.3.0/src/seqlogic/hier.py
--rw-rw-rw-   0        0        0    83927 2024-05-28 01:31:22.000000 seqlogic-0.3.0/src/seqlogic/lbool.py
--rw-rw-rw-   0        0        0    13223 2024-05-20 01:17:15.000000 seqlogic-0.3.0/src/seqlogic/sim.py
--rw-rw-rw-   0        0        0     1368 2024-05-05 19:08:40.000000 seqlogic-0.3.0/src/seqlogic/util.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.361164 seqlogic-0.3.0/src/seqlogic.egg-info/
--rw-rw-rw-   0        0        0      956 2024-05-28 01:40:32.000000 seqlogic-0.3.0/src/seqlogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2024-05-28 01:40:32.000000 seqlogic-0.3.0/src/seqlogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 01:40:32.000000 seqlogic-0.3.0/src/seqlogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-28 01:40:32.000000 seqlogic-0.3.0/src/seqlogic.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.358161 seqlogic-0.3.0/tests/
--rw-rw-rw-   0        0        0     4281 2024-05-08 03:13:26.000000 seqlogic-0.3.0/tests/test_aes.py
--rw-rw-rw-   0        0        0    24103 2024-05-25 00:21:44.000000 seqlogic-0.3.0/tests/test_bits.py
--rw-rw-rw-   0        0        0     3205 2024-05-25 00:21:32.000000 seqlogic-0.3.0/tests/test_enum.py
--rw-rw-rw-   0        0        0     4731 2024-05-25 00:21:22.000000 seqlogic-0.3.0/tests/test_fsm.py
--rw-rw-rw-   0        0        0      684 2024-04-21 07:30:53.000000 seqlogic-0.3.0/tests/test_gray.py
--rw-rw-rw-   0        0        0      705 2024-03-11 02:48:00.000000 seqlogic-0.3.0/tests/test_hier.py
--rw-rw-rw-   0        0        0    30042 2024-05-25 01:36:05.000000 seqlogic-0.3.0/tests/test_lbool.py
--rw-rw-rw-   0        0        0     3533 2024-05-05 19:08:40.000000 seqlogic-0.3.0/tests/test_lfsr.py
--rw-rw-rw-   0        0        0    30595 2024-05-28 01:31:22.000000 seqlogic-0.3.0/tests/test_riscv.py
--rw-rw-rw-   0        0        0     4327 2024-05-25 00:20:36.000000 seqlogic-0.3.0/tests/test_sim.py
--rw-rw-rw-   0        0        0     3024 2024-05-25 00:21:22.000000 seqlogic-0.3.0/tests/test_struct.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:45:48.790954 seqlogic-0.4.0/
+-rw-rw-rw-   0        0        0      956 2024-05-29 05:45:48.789854 seqlogic-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2024-03-11 04:13:25.000000 seqlogic-0.4.0/README.md
+-rw-rw-rw-   0        0        0      263 2024-05-29 05:43:39.000000 seqlogic-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 05:45:48.791996 seqlogic-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 05:45:48.697339 seqlogic-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 05:45:48.725695 seqlogic-0.4.0/src/seqlogic/
+-rw-rw-rw-   0        0        0      357 2024-05-27 19:30:40.000000 seqlogic-0.4.0/src/seqlogic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:45:48.757986 seqlogic-0.4.0/src/seqlogic/algorithms/
+-rw-rw-rw-   0        0        0       27 2023-11-27 07:28:50.000000 seqlogic-0.4.0/src/seqlogic/algorithms/__init__.py
+-rw-rw-rw-   0        0        0    12685 2024-03-10 17:38:01.000000 seqlogic-0.4.0/src/seqlogic/algorithms/aes.py
+-rw-rw-rw-   0        0        0      285 2024-04-30 03:11:09.000000 seqlogic-0.4.0/src/seqlogic/algorithms/gray.py
+-rw-rw-rw-   0        0        0    21662 2024-05-08 03:13:26.000000 seqlogic-0.4.0/src/seqlogic/bits.py
+-rw-rw-rw-   0        0        0    11246 2024-05-29 05:36:43.000000 seqlogic-0.4.0/src/seqlogic/design.py
+-rw-rw-rw-   0        0        0     3210 2024-05-29 05:40:42.000000 seqlogic-0.4.0/src/seqlogic/hier.py
+-rw-rw-rw-   0        0        0    83927 2024-05-28 01:31:22.000000 seqlogic-0.4.0/src/seqlogic/lbool.py
+-rw-rw-rw-   0        0        0    13367 2024-05-29 03:21:10.000000 seqlogic-0.4.0/src/seqlogic/sim.py
+-rw-rw-rw-   0        0        0     1368 2024-05-05 19:08:40.000000 seqlogic-0.4.0/src/seqlogic/util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:45:48.783566 seqlogic-0.4.0/src/seqlogic.egg-info/
+-rw-rw-rw-   0        0        0      956 2024-05-29 05:45:48.000000 seqlogic-0.4.0/src/seqlogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2024-05-29 05:45:48.000000 seqlogic-0.4.0/src/seqlogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 05:45:48.000000 seqlogic-0.4.0/src/seqlogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 05:45:48.000000 seqlogic-0.4.0/src/seqlogic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 05:45:48.782517 seqlogic-0.4.0/tests/
+-rw-rw-rw-   0        0        0     4281 2024-05-08 03:13:26.000000 seqlogic-0.4.0/tests/test_aes.py
+-rw-rw-rw-   0        0        0    24103 2024-05-25 00:21:44.000000 seqlogic-0.4.0/tests/test_bits.py
+-rw-rw-rw-   0        0        0     3205 2024-05-25 00:21:32.000000 seqlogic-0.4.0/tests/test_enum.py
+-rw-rw-rw-   0        0        0     4731 2024-05-25 00:21:22.000000 seqlogic-0.4.0/tests/test_fsm.py
+-rw-rw-rw-   0        0        0      684 2024-04-21 07:30:53.000000 seqlogic-0.4.0/tests/test_gray.py
+-rw-rw-rw-   0        0        0      705 2024-03-11 02:48:00.000000 seqlogic-0.4.0/tests/test_hier.py
+-rw-rw-rw-   0        0        0    30042 2024-05-25 01:36:05.000000 seqlogic-0.4.0/tests/test_lbool.py
+-rw-rw-rw-   0        0        0     3533 2024-05-05 19:08:40.000000 seqlogic-0.4.0/tests/test_lfsr.py
+-rw-rw-rw-   0        0        0    31491 2024-05-29 03:21:10.000000 seqlogic-0.4.0/tests/test_riscv.py
+-rw-rw-rw-   0        0        0     4327 2024-05-25 00:20:36.000000 seqlogic-0.4.0/tests/test_sim.py
+-rw-rw-rw-   0        0        0     3024 2024-05-25 00:21:22.000000 seqlogic-0.4.0/tests/test_struct.py
```

### Comparing `seqlogic-0.3.0/PKG-INFO` & `seqlogic-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqlogic
-Version: 0.3.0
+Version: 0.4.0
 Summary: Sequential Logic
 Project-URL: Repository, https://github.com/cjdrake/seqlogic.git
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Sequential Logic
```

### Comparing `seqlogic-0.3.0/README.md` & `seqlogic-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/src/seqlogic/algorithms/aes.py` & `seqlogic-0.4.0/src/seqlogic/algorithms/aes.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/src/seqlogic/bits.py` & `seqlogic-0.4.0/src/seqlogic/bits.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/src/seqlogic/design.py` & `seqlogic-0.4.0/src/seqlogic/design.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from __future__ import annotations
 
 import inspect
 import re
 from abc import ABC
 from collections import defaultdict
-from collections.abc import Callable
+from collections.abc import Callable, Sequence
 
 from vcd.writer import VarValue
 from vcd.writer import VCDWriter as VcdWriter
 
 from .hier import Branch, Leaf
 from .lbool import Vec, VecEnum, lit2vec
 from .sim import Aggregate, Region, SimAwaitable, Singular, State, changed, get_loop, resume
@@ -99,74 +99,120 @@
 
     def dump_vcd(self, vcdw: VcdWriter, pattern: str):
         for child in self._children:
             assert isinstance(child, _TraceIf)
             child.dump_vcd(vcdw, pattern)
 
     def bits(self, name: str, dtype: type, port: bool = False) -> Bits:
-        # TODO(cjdrake): Check name
+        self._check_name(name)
         node = Bits(name, parent=self, dtype=dtype)
         setattr(self, f"_{name}", node)
         if port:
             setattr(self, name, node)
         return node
 
     def bit(self, name: str, port: bool = False) -> Bit:
-        # TODO(cjdrake): Check name
+        self._check_name(name)
         node = Bit(name, parent=self)
         setattr(self, f"_{name}", node)
         if port:
             setattr(self, name, node)
         return node
 
     def array(self, name: str, dtype: type) -> Array:
-        # TODO(cjdrake): Check name
+        self._check_name(name)
         node = Array(name, parent=self, dtype=dtype)
         setattr(self, f"_{name}", node)
         return node
 
     def submod(self, name: str, mod: type, **params) -> Module:
-        # TODO(cjdrake): Check name
+        self._check_name(name)
         node = mod(name, parent=self, **params)
         setattr(self, f"_{name}", node)
         return node
 
-    def combi(self, y: Bits, f: Callable, *xs: Bits):
+    def combi(self, y: Bits, f: Callable, *xs: State):
         """Combinational logic."""
 
         async def proc():
             while True:
                 await changed(*xs)
                 y.next = f(*[x.value for x in xs])
 
         self._procs.append((Region.REACTIVE, proc, (), {}))
 
-    def combis(self, ys: list[Bits], f: Callable, *xs: Bits):
+    def combis(self, ys: Sequence[Bits], f: Callable, *xs: State):
         """Combinational logic."""
 
         async def proc():
             while True:
                 await changed(*xs)
-                ret = f(*[x.value for x in xs])
-                assert len(ys) == len(ret)
-                for i, y in enumerate(ys):
-                    y.next = ret[i]
+                yns = f(*[x.value for x in xs])
+                assert len(ys) == len(yns)
+                for y, yn in zip(ys, yns):
+                    y.next = yn
 
         self._procs.append((Region.REACTIVE, proc, (), {}))
 
     def connect(self, y: Bits, x: Bits):
         """Connect input to output."""
 
         async def proc():
             while True:
                 await changed(x)
                 y.next = x.value
 
         self._procs.append((Region.REACTIVE, proc, (), {}))
 
+    def dff(self, q: Bits, d: Bits, clk: Bit):
+        """D Flip Flop."""
+
+        async def proc():
+            while True:
+                state = await resume((clk, clk.is_posedge))
+                if state is clk:
+                    q.next = d.value
+                else:
+                    assert False
+
+        self._procs.append((Region.ACTIVE, proc, (), {}))
+
+    def dff_ar(self, q: Bits, d: Bits, clk: Bit, rst: Bit, rval: Vec):
+        """D Flip Flop with async reset."""
+
+        async def proc():
+            while True:
+                state = await resume(
+                    (rst, rst.is_posedge),
+                    (clk, lambda: clk.is_posedge() and rst.is_neg()),
+                )
+                if state is rst:
+                    q.next = rval
+                elif state is clk:
+                    q.next = d.value
+                else:
+                    assert False
+
+        self._procs.append((Region.ACTIVE, proc, (), {}))
+
+    def dff_en(self, q: Bits, d: Bits, en: Bit, clk: Bit):
+        """D Flip Flop with enable."""
+
+        async def proc():
+            while True:
+                state = await resume(
+                    (clk, lambda: clk.is_posedge() and en.value == "1b1"),
+                )
+                if state is clk:
+                    q.next = d.value
+                else:
+                    assert False
+
+        self._procs.append((Region.ACTIVE, proc, (), {}))
+
     def dff_en_ar(self, q: Bits, d: Bits, en: Bit, clk: Bit, rst: Bit, rval: Vec):
         """D Flip Flop with enable, and async reset."""
 
         async def proc():
             while True:
                 state = await resume(
                     (rst, rst.is_posedge),
@@ -219,35 +265,45 @@
                 t = self._sim.time
                 waves[t][self] = self._next_value
 
             self._waves_change = change
 
     def dump_vcd(self, vcdw, pattern: str):
         assert isinstance(self._parent, Module)
+
         if issubclass(self._dtype, VecEnum):
             if re.match(pattern, self.qualname):
                 var = vcdw.register_var(
                     scope=self._parent.scope,
                     name=self.name,
                     var_type="string",
                     init=self._value.name,
                 )
-                self._vcd_change = lambda: vcdw.change(var, self._sim.time, self._next_value.name)
+
+                def f():
+                    value = self._next_value.name
+                    return vcdw.change(var, self._sim.time, value)
+
+                self._vcd_change = f
+
         elif issubclass(self._dtype, Vec):
             if re.match(pattern, self.qualname):
                 var = vcdw.register_var(
                     scope=self._parent.scope,
                     name=self.name,
                     var_type="reg",
                     size=len(self._value),
                     init=_vec2vcd(self._value),
                 )
-                self._vcd_change = lambda: vcdw.change(
-                    var, self._sim.time, _vec2vcd(self._next_value)
-                )
+
+                def f():
+                    value = _vec2vcd(self._next_value)
+                    return vcdw.change(var, self._sim.time, value)
+
+                self._vcd_change = f
 
 
 class Bit(Bits):
     """One-bit specialization of Bits that supports edge detection."""
 
     def __init__(self, name: str, parent: Module):
         super().__init__(name, parent, dtype=Vec[1])
@@ -286,42 +342,14 @@
 
     def __init__(self, name: str, parent: Module, dtype: type):
         Leaf.__init__(self, name, parent)
         Aggregate.__init__(self, dtype.xes())
         _ProcIf.__init__(self)
         self._dtype = dtype
 
-    def __getitem__(self, key: int | Vec):
-        if isinstance(key, int):
-            return super().__getitem__(key)
-        if isinstance(key, Vec):
-            try:
-                i = key.to_uint()
-            except ValueError:
-                return _ArrayXPropItem(self._dtype)
-            return super().__getitem__(i)
-        assert TypeError("Expected key to be int or Vec")
-
-
-class _ArrayXPropItem:
-    """Array X-Prop item helper."""
-
-    def __init__(self, dtype: type):
-        self._dtype = dtype
-
-    def _get_value(self):
-        return self._dtype.xes()
-
-    value = property(fget=_get_value)
-
-    def _set_next(self, value):
-        pass
-
-    next = property(fset=_set_next)
-
 
 def simify(d: Module | Bits | Bit | Array):
     """Add design processes to the simulator."""
     loop = get_loop()
     for node in d.iter_bfs():
         assert isinstance(node, _ProcIf)
         for region, func, args, kwargs in node.procs:
```

### Comparing `seqlogic-0.3.0/src/seqlogic/hier.py` & `seqlogic-0.4.0/src/seqlogic/hier.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     def __init__(self, name: str, parent: Branch | None):
         """Initialize.
 
         Args:
             name: Name of this tree node.
             parent: Parent tree node, or None.
         """
+        self._check_name(name)
         self._name = name
         self._parent = parent
 
     @property
     def name(self) -> str:
         """Return the design element name."""
         return self._name
@@ -44,14 +45,20 @@
     def iter_bfs(self) -> Generator[Hierarchy, None, None]:
         """Iterate through the design hierarchy in BFS order."""
 
     @abstractmethod
     def iter_dfs(self) -> Generator[Hierarchy, None, None]:
         """Iterate through the design hierarchy in DFS order."""
 
+    @staticmethod
+    def _check_name(name: str):
+        valid = name.isidentifier() and not name.startswith("_")
+        if not valid:
+            raise ValueError(f"Expected public identifier, got {name}")
+
 
 class Branch(Hierarchy):
     """Design hierarchy branch node."""
 
     def __init__(self, name: str, parent: Branch | None = None):
         super().__init__(name, parent)
         self._children: list[Branch | Leaf] = []
```

### Comparing `seqlogic-0.3.0/src/seqlogic/lbool.py` & `seqlogic-0.4.0/src/seqlogic/lbool.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/src/seqlogic/sim.py` & `seqlogic-0.4.0/src/seqlogic/sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 https://www.youtube.com/watch?v=Y4Gt3Xjd7G8
 """
 
 import heapq
 import inspect
 from abc import ABC
 from collections import defaultdict
-from collections.abc import Awaitable, Callable, Coroutine, Generator
+from collections.abc import Awaitable, Callable, Coroutine, Generator, Hashable
 from enum import IntEnum, auto
 from functools import partial
 from typing import TypeAlias
 
 _INIT_TIME = -1
 _START_TIME = 0
 
@@ -28,16 +28,21 @@
 class State(ABC):
     """Model component."""
 
     def __init__(self):
         # Reference to the event loop
         self._sim = _sim
 
+    def get_value(self):
+        raise NotImplementedError()
+
+    value = property(fget=get_value)
+
     def changed(self) -> bool:
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def update(self):
         raise NotImplementedError()
 
 
 class Singular(State):
     """Model state organized as a single unit."""
@@ -76,57 +81,59 @@
 
 
 class Aggregate(State):
     """Model state organized as multiple units."""
 
     def __init__(self, value):
         super().__init__()
-        self._values = defaultdict(lambda: value)
-        self._next_values = defaultdict(lambda: value)
-        self._changed = set()
+        self._value = defaultdict(lambda: value)
+        self._next_value = defaultdict(lambda: value)
+        self._changed: set[Hashable] = set()
 
-    def __getitem__(self, key: int):
+    def __getitem__(self, key: Hashable):
         return _AggrItem(self, key)
 
-    def get_value(self, index: int):
+    def get_value(self):
         if self._sim.region == Region.REACTIVE:
-            return self._next_values[index]
-        return self._values[index]
+            return self._next_value.copy()
+        return self._value.copy()
+
+    value = property(fget=get_value)
 
-    def set_next(self, index: int, value):
-        if value != self._next_values[index]:
-            self._changed.add(index)
-        self._next_values[index] = value
+    def set_next(self, key: Hashable, value):
+        if value != self._next_value[key]:
+            self._changed.add(key)
+        self._next_value[key] = value
 
         # Notify the event loop
         _sim.touch(self)
 
     def changed(self) -> bool:
         return bool(self._changed)
 
     def update(self):
-        for index in self._changed:
-            self._values[index] = self._next_values[index]
+        for key in self._changed:
+            self._value[key] = self._next_value[key]
         self._changed.clear()
 
 
 class _AggrItem:
     """Wrap Aggregate item getter/setter."""
 
-    def __init__(self, obj: Aggregate, index: int):
-        self._obj = obj
-        self._index = index
+    def __init__(self, aggr: Aggregate, key: Hashable):
+        self._aggr = aggr
+        self._key = key
 
     def get_value(self):
-        return self._obj.get_value(self._index)
+        return self._aggr.value[self._key]
 
     value = property(fget=get_value)
 
     def set_next(self, value):
-        self._obj.set_next(self._index, value)
+        self._aggr.set_next(self._key, value)
 
     next = property(fset=set_next)
 
 
 _SimQueueItem: TypeAlias = tuple[int, Region, Coroutine, State | None]
```

### Comparing `seqlogic-0.3.0/src/seqlogic/util.py` & `seqlogic-0.4.0/src/seqlogic/util.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/src/seqlogic.egg-info/PKG-INFO` & `seqlogic-0.4.0/src/seqlogic.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqlogic
-Version: 0.3.0
+Version: 0.4.0
 Summary: Sequential Logic
 Project-URL: Repository, https://github.com/cjdrake/seqlogic.git
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Sequential Logic
```

### Comparing `seqlogic-0.3.0/src/seqlogic.egg-info/SOURCES.txt` & `seqlogic-0.4.0/src/seqlogic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/tests/test_aes.py` & `seqlogic-0.4.0/tests/test_aes.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/tests/test_bits.py` & `seqlogic-0.4.0/tests/test_bits.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/tests/test_enum.py` & `seqlogic-0.4.0/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/tests/test_fsm.py` & `seqlogic-0.4.0/tests/test_fsm.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/tests/test_gray.py` & `seqlogic-0.4.0/tests/test_gray.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/tests/test_hier.py` & `seqlogic-0.4.0/tests/test_hier.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/tests/test_lbool.py` & `seqlogic-0.4.0/tests/test_lbool.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/tests/test_lfsr.py` & `seqlogic-0.4.0/tests/test_lfsr.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/tests/test_riscv.py` & `seqlogic-0.4.0/tests/test_riscv.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # pyright: reportCallIssue=false
 
 from collections import defaultdict
 
 from seqlogic import get_loop, simify
 from seqlogic.lbool import uint2vec
 
-from .riscv.core import AluOp, CtlAluA, CtlAluB, CtlPc, Inst, Opcode
+from .riscv.core import AluOp, CtlAluA, CtlAluB, CtlPc, CtlWriteBack, Inst, Opcode
 from .riscv.core.top import Top
 
 loop = get_loop()
 
 
 X32 = "32bXXXX_XXXX_XXXX_XXXX_XXXX_XXXX_XXXX_XXXX"
 W32 = "32b----_----_----_----_----_----_----_----"
@@ -69,15 +69,17 @@
     top.dump_waves(waves, r"/top/core/datapath.data_mem_wr_data")
 
     simify(top)
 
     # Initialize instruction memory
     text = get_mem("tests/riscv/tests/add.text")
     for i, d in enumerate(text):
-        top._text_mem_bus._text_mem._mem.set_next(i, uint2vec(d, 32))
+        addr = uint2vec(i, 10)
+        data = uint2vec(d, 32)
+        top._text_mem_bus._text_mem._mem[addr].next = data
 
     loop.run(until=50)
 
     exp = {
         # Initialize everything to X'es
         -1: {
             # Top
@@ -88,15 +90,15 @@
             top.bus_wr_data: X32,
             top.bus_rd_en: "1bX",
             # Decode
             top._core._datapath._immediate: X32,
             # Control
             top._core._datapath.alu_op_a_sel: CtlAluA.X,
             top._core._datapath.alu_op_b_sel: CtlAluB.X,
-            top._core._datapath.reg_writeback_sel: "3bXXX",
+            top._core._datapath.reg_writeback_sel: CtlWriteBack.X,
             # ALU
             top._core._datapath._alu_result: X32,
             top._core._datapath.alu_result_eq_zero: "1bX",
             top._core._datapath.alu_func: AluOp.X,
             top._core._datapath._alu_op_a: X32,
             top._core._datapath._alu_op_b: X32,
             # PC
@@ -130,15 +132,15 @@
             top.bus_wr_data: "32h0000_0000",
             top.bus_rd_en: "1b0",
             # Decode
             top._core._datapath._immediate: "32h0000_0000",
             # Control
             top._core._datapath.alu_op_a_sel: CtlAluA.RS1,
             top._core._datapath.alu_op_b_sel: CtlAluB.IMM,
-            top._core._datapath.reg_writeback_sel: "3b000",
+            top._core._datapath.reg_writeback_sel: CtlWriteBack.ALU,
             # ALU
             top._core._datapath._alu_result: "32h0000_0000",
             top._core._datapath.alu_result_eq_zero: "1b1",
             top._core._datapath.alu_func: AluOp.ADD,
             top._core._datapath._alu_op_a: "32h0000_0000",
             top._core._datapath._alu_op_b: "32h0000_0000",
             # PC
@@ -473,30 +475,30 @@
                 rd="5b00010",
                 funct3="3b000",
                 rs1="5b00000",
                 rs2="5b00111",
                 funct7="7b0000000",
             ),
             top.bus_addr: "32h0000_0007",
-            top.bus_wr_data: "32h0000_0000",
+            top.bus_wr_data: "32bXXXXXXXX_00000000_00000000_00000000",
             # Decode
             top._core._datapath._immediate: "32h0000_0007",
             # ALU
             top._core._datapath._alu_result: "32h0000_0007",
             top._core._datapath._alu_op_b: "32h0000_0007",
             # PC
             top._core._datapath._pc_next: "32h0040_0038",
             top._core._datapath._pc_plus_4: "32h0040_0038",
             top._core._datapath._pc_plus_immediate: "32h0040_003B",
             # Regfile
             top._core._datapath._wr_data: "32h0000_0007",
-            top._core._datapath._rs2_data: "32h0000_0000",
+            top._core._datapath._rs2_data: X32,
             # Data Mem
             top._core._datapath.data_mem_addr: "32h0000_0007",
-            top._core._datapath.data_mem_wr_data: "32h0000_0000",
+            top._core._datapath.data_mem_wr_data: X32,
         },
         # @(posedge clock)
         37: {
             top._pc: "32h0040_0038",
             top._inst: Inst(
                 opcode=Opcode.OP,
                 rd="5b00011",
@@ -533,44 +535,45 @@
                 opcode=Opcode.OP_IMM,
                 rd="5b11101",
                 funct3="3b000",
                 rs1="5b00000",
                 rs2="5b01010",
                 funct7="7b0000000",
             ),
-            top.bus_wr_data: "32h0000_0000",
+            top.bus_wr_data: "32bXXXXXXXX_XXXXXXXX_00000000_00000000",
             # Decode
             top._core._datapath._immediate: "32h0000_000A",
             # Control
             top._core._datapath.alu_op_b_sel: CtlAluB.IMM,
             # ALU
             top._core._datapath._alu_op_a: "32h0000_0000",
             top._core._datapath._alu_op_b: "32h0000_000A",
             # PC
             top._core._datapath._pc_next: "32h0040_0040",
             top._core._datapath._pc_plus_4: "32h0040_0040",
             top._core._datapath._pc_plus_immediate: "32h0040_0046",
             # Regfile
             top._core._datapath._rs1_data: "32h0000_0000",
-            top._core._datapath._rs2_data: "32h0000_0000",
+            top._core._datapath._rs2_data: X32,
             # Data Mem
-            top._core._datapath.data_mem_wr_data: "32h0000_0000",
+            top._core._datapath.data_mem_wr_data: X32,
         },
         # @(posedge clock)
         41: {
             top._pc: "32h0040_0040",
             top._inst: Inst(
                 opcode=Opcode.OP_IMM,
                 rd="5b11100",
                 funct3="3b000",
                 rs1="5b00000",
                 rs2="5b00100",
                 funct7="7b0000000",
             ),
             top.bus_addr: "32h0000_0004",
+            top.bus_wr_data: X32,
             # Decode
             top._core._datapath._immediate: "32h0000_0004",
             # ALU
             top._core._datapath._alu_result: "32h0000_0004",
             top._core._datapath._alu_op_b: "32h0000_0004",
             # PC
             top._core._datapath._pc_next: "32h0040_0044",
@@ -659,25 +662,37 @@
                 opcode=Opcode.LUI,
                 rd="5b00010",
                 funct3="3b000",
                 rs1="5b11111",
                 rs2="5b11111",
                 funct7="7b1111111",
             ),
+            top.bus_addr: X32,
+            top.bus_wr_data: X32,
             # Decode
             top._core._datapath._immediate: "32hFFFF_8000",
             # Control
             top._core._datapath.alu_op_b_sel: CtlAluB.RS2,
-            top._core._datapath.reg_writeback_sel: "3b011",
+            top._core._datapath.reg_writeback_sel: CtlWriteBack.IMM,
+            # ALU
+            top._core._datapath._alu_result: X32,
+            top._core._datapath.alu_result_eq_zero: "1bX",
+            top._core._datapath._alu_op_a: X32,
+            top._core._datapath._alu_op_b: X32,
             # PC
             top._core._datapath._pc_next: "32h0040_0050",
             top._core._datapath._pc_plus_4: "32h0040_0050",
             top._core._datapath._pc_plus_immediate: "32h003F_804C",
             # Regfile
             top._core._datapath._wr_data: "32hFFFF_8000",
+            top._core._datapath._rs1_data: X32,
+            top._core._datapath._rs2_data: X32,
+            # Data Mem
+            top._core._datapath.data_mem_addr: X32,
+            top._core._datapath.data_mem_wr_data: X32,
         },
         # @(posedge clock)
         49: {
             top._pc: "32h0040_0050",
             top._inst: Inst(
                 opcode=Opcode.OP,
                 rd="5b00011",
@@ -687,24 +702,26 @@
                 funct7="7b0000000",
             ),
             top.bus_addr: "32hFFFF_8000",
             top.bus_wr_data: "32hFFFF_8000",
             # Decode
             top._core._datapath._immediate: W32,
             # Control
-            top._core._datapath.reg_writeback_sel: "3b000",
+            top._core._datapath.reg_writeback_sel: CtlWriteBack.ALU,
             # ALU
             top._core._datapath._alu_result: "32hFFFF_8000",
             top._core._datapath.alu_result_eq_zero: "1b0",
+            top._core._datapath._alu_op_a: "32h0000_0000",
             top._core._datapath._alu_op_b: "32hFFFF_8000",
             # Next PC
             top._core._datapath._pc_next: "32h0040_0054",
             top._core._datapath._pc_plus_4: "32h0040_0054",
             top._core._datapath._pc_plus_immediate: W32,
             # Regfile
+            top._core._datapath._rs1_data: "32h0000_0000",
             top._core._datapath._rs2_data: "32hFFFF_8000",
             # Data Mem
             top._core._datapath.data_mem_addr: "32hFFFF_8000",
             top._core._datapath.data_mem_wr_data: "32hFFFF_8000",
         },
     }
     assert waves == exp
@@ -717,20 +734,24 @@
     top = Top(name="top")
 
     simify(top)
 
     # Initialize instruction memory
     text = get_mem(f"tests/riscv/tests/{name}.text")
     for i, d in enumerate(text):
-        top._text_mem_bus._text_mem._mem.set_next(i, uint2vec(d, 32))
+        addr = uint2vec(i, 10)
+        data = uint2vec(d, 32)
+        top._text_mem_bus._text_mem._mem[addr].next = data
 
     # Initialize data memory
     data = get_mem(f"tests/riscv/tests/{name}.data")
     for i, d in enumerate(data):
-        top._data_mem_bus._data_mem._mem.set_next(i, uint2vec(d, 32))
+        addr = uint2vec(i, 10)
+        data = uint2vec(d, 32)
+        top._data_mem_bus._data_mem._mem[addr].next = data
 
     # Run the simulation
     for _ in loop.iter(until=10000):
         if top.bus_wr_en.value == "1b1" and top.bus_addr.value == DEBUG_REG:
             if top.bus_wr_data.value == "32h0000_0001":
                 return PASS
             else:
```

### Comparing `seqlogic-0.3.0/tests/test_sim.py` & `seqlogic-0.4.0/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.3.0/tests/test_struct.py` & `seqlogic-0.4.0/tests/test_struct.py`

 * *Files identical despite different names*

