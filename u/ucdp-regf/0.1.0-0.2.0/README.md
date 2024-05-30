# Comparing `tmp/ucdp_regf-0.1.0.tar.gz` & `tmp/ucdp_regf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucdp_regf-0.1.0.tar", last modified: Mon May 20 23:00:19 2024, max compression
+gzip compressed data, was "ucdp_regf-0.2.0.tar", last modified: Thu May 30 07:03:23 2024, max compression
```

## Comparing `ucdp_regf-0.1.0.tar` & `ucdp_regf-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,31 @@
--rw-r--r--   0        0        0     1067 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/LICENSE
--rw-r--r--   0        0        0     1030 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/README.md
--rw-r--r--   0        0        0     2389 2024-05-20 23:00:19.174228 ucdp_regf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1162 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/__init__.py
--rw-r--r--   0        0        0      491 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/example/simple/src/uart/uart/rtl/uart_core.sv
--rw-r--r--   0        0        0     1809 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/fileliststandard.py
--rw-r--r--   0        0        0     1140 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/glbl/__init__.py
--rw-r--r--   0        0        0     3243 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/glbl/bus.py
--rw-r--r--   0        0        0     1777 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/glbl/bus2mem.py
--rw-r--r--   0        0        0     1673 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/glbl/clk_gate.py
--rw-r--r--   0        0        0     1503 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/glbl/regf.py
--rw-r--r--   0        0        0      491 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/src/glbl/bus2mem/rtl/bus2mem.sv
--rw-r--r--   0        0        0     1129 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/uart/__init__.py
--rw-r--r--   0        0        0     2631 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/uart/uart.py
--rw-r--r--   0        0        0     4944 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/templates/ucdp_regf.sv.mako
--rw-r--r--   0        0        0     7753 2024-05-20 23:00:05.854359 ucdp_regf-0.1.0/src/ucdp_regf/ucdp_regf.py
--rw-r--r--   0        0        0       13 2024-05-20 23:00:05.858359 ucdp_regf-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      384 2024-05-20 23:00:05.858359 ucdp_regf-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0    35497 2024-05-20 23:00:05.858359 ucdp_regf-0.1.0/tests/refdata/tests.test_svmako/test_full/tests/full/full.sv
--rw-r--r--   0        0        0    60394 2024-05-20 23:00:05.858359 ucdp_regf-0.1.0/tests/refdata/tests.test_svmako/test_full/tests/full/full_regf.sv
--rw-r--r--   0        0        0     2694 2024-05-20 23:00:05.858359 ucdp_regf-0.1.0/tests/refdata/tests.test_svmako/test_top/uart/uart/rtl/uart.sv
--rw-r--r--   0        0        0      750 2024-05-20 23:00:05.858359 ucdp_regf-0.1.0/tests/refdata/tests.test_svmako/test_top/uart/uart/rtl/uart_core.sv
--rw-r--r--   0        0        0     1898 2024-05-20 23:00:05.858359 ucdp_regf-0.1.0/tests/refdata/tests.test_svmako/test_top/uart/uart/rtl/uart_regf.sv
--rw-r--r--   0        0        0     2988 2024-05-20 23:00:05.858359 ucdp_regf-0.1.0/tests/test_svmako.py
--rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 ucdp_regf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-30 07:03:10.859559 ucdp_regf-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1030 2024-05-30 07:03:10.859559 ucdp_regf-0.2.0/README.md
+-rw-r--r--   0        0        0     2389 2024-05-30 07:03:23.171628 ucdp_regf-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1162 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/__init__.py
+-rw-r--r--   0        0        0      491 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/example/simple/src/uart/uart/rtl/uart_core.sv
+-rw-r--r--   0        0        0     1809 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/fileliststandard.py
+-rw-r--r--   0        0        0     1140 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/glbl/__init__.py
+-rw-r--r--   0        0        0     3243 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/glbl/bus.py
+-rw-r--r--   0        0        0     1777 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/glbl/bus2mem.py
+-rw-r--r--   0        0        0     1673 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/glbl/clk_gate.py
+-rw-r--r--   0        0        0     1503 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/glbl/regf.py
+-rw-r--r--   0        0        0      491 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/src/glbl/bus2mem/rtl/bus2mem.sv
+-rw-r--r--   0        0        0     1129 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/uart/__init__.py
+-rw-r--r--   0        0        0     2631 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/uart/uart.py
+-rw-r--r--   0        0        0    14015 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/templates/ucdp_regf.sv.mako
+-rw-r--r--   0        0        0     9077 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/src/ucdp_regf/ucdp_regf.py
+-rw-r--r--   0        0        0       13 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      384 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     3523 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_corner/tests/corner/corner.sv
+-rw-r--r--   0        0        0    11337 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_corner/tests/corner/corner_regf.sv
+-rw-r--r--   0        0        0    35381 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_full/tests/full/full.sv
+-rw-r--r--   0        0        0    77607 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_full/tests/full/full_regf.sv
+-rw-r--r--   0        0        0     4571 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_portgroup/tests/portgroup/portgroup.sv
+-rw-r--r--   0        0        0     5350 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_portgroup/tests/portgroup/portgroup_regf.sv
+-rw-r--r--   0        0        0      864 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_portgroup/tests/portgroup/portgroup_rx.sv
+-rw-r--r--   0        0        0      738 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_portgroup/tests/portgroup/portgroup_tx.sv
+-rw-r--r--   0        0        0     2651 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_top/uart/uart/rtl/uart.sv
+-rw-r--r--   0        0        0      750 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_top/uart/uart/rtl/uart_core.sv
+-rw-r--r--   0        0        0     3109 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_top/uart/uart/rtl/uart_regf.sv
+-rw-r--r--   0        0        0     6626 2024-05-30 07:03:10.863559 ucdp_regf-0.2.0/tests/test_svmako.py
+-rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 ucdp_regf-0.2.0/PKG-INFO
```

### Comparing `ucdp_regf-0.1.0/LICENSE` & `ucdp_regf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/README.md` & `ucdp_regf-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/pyproject.toml` & `ucdp_regf-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "ucdp-regf"
-version = "0.1.0"
+version = "0.2.0"
 description = "Unified Chip Design Platform - Register File"
 readme = "README.md"
 authors = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.10.0,<4.0"
 dependencies = [
-    "ucdp-glbl>=0.1.0",
-    "ucdp>=0.3.0",
+    "ucdp>=0.4.1",
+    "ucdp-glbl>=0.2.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/nbiotcloud/ucdp-regf"
 Documentation = "https://ucdp-regf.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/nbiotcloud/ucdp-regf/issues"
 
@@ -30,15 +30,15 @@
     "pre-commit>=3.5.0",
 ]
 test = [
     "contextlib-chdir>=1.0.2",
     "coveralls>=3.3.1",
     "pytest-cov>=5.0.0",
     "test2ref>=0.4.2",
-    "ucdp-sv>=0.1.0",
+    "ucdp-sv>=0.2.0",
 ]
 checktypes = [
     "mypy>=1.9.0",
 ]
 doc = [
     "mkdocs-include-markdown-plugin>=6.0.5",
     "mkdocs-literate-nav>=0.6.1",
```

### Comparing `ucdp_regf-0.1.0/src/ucdp_regf/__init__.py` & `ucdp_regf-0.2.0/src/ucdp_regf/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/fileliststandard.py` & `ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/fileliststandard.py`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/glbl/__init__.py` & `ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/glbl/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/glbl/bus.py` & `ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/glbl/bus.py`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/glbl/bus2mem.py` & `ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/glbl/bus2mem.py`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/glbl/clk_gate.py` & `ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/glbl/clk_gate.py`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/glbl/regf.py` & `ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/glbl/regf.py`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/uart/__init__.py` & `ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/uart/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/src/ucdp_regf/examples/simple/uart/uart.py` & `ucdp_regf-0.2.0/src/ucdp_regf/examples/simple/uart/uart.py`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/src/ucdp_regf/ucdp_regf.py` & `ucdp_regf-0.2.0/src/ucdp_regf/ucdp_regf.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 """
 Address Space.
 
 Accesses
 """
 
 from functools import cached_property
-from typing import ClassVar
+from typing import ClassVar, TypeAlias
 
 import ucdp as u
 from icdutil.num import calc_unsigned_width
 from tabulate import tabulate
 from ucdp_glbl import addrspace as _addrspace
 from ucdp_glbl.mem import MemIoType
 
-ACCESSES = _addrspace.ACCESSES
-Access = _addrspace.Access
-ReadOp = _addrspace.ReadOp
-WriteOp = _addrspace.WriteOp
+ACCESSES: TypeAlias = _addrspace.ACCESSES
+Access: TypeAlias = _addrspace.Access
+ReadOp: TypeAlias = _addrspace.ReadOp
+WriteOp: TypeAlias = _addrspace.WriteOp
 
 _IN_REGF_DEFAULTS = {
     _addrspace.RO: False,
     _addrspace.WO: False,
     _addrspace.RW: True,
 }
 
@@ -65,24 +65,51 @@
     """Word."""
 
     portgroups: tuple[str, ...] | None = None
     """Default Portgroups for Fields."""
     in_regf: bool | None = None
     """Default Implementation within Regf."""
 
-    def _create_field(self, name, bus, portgroups=None, signame=None, in_regf=None, **kwargs) -> Field:
+    def _create_field(self, name, bus, core, portgroups=None, signame=None, in_regf=None, **kwargs) -> Field:
         if portgroups is None:
             portgroups = self.portgroups
         if signame is None:
             signame = f"{self.name}_{name}"
         if in_regf is None:
             in_regf = self.in_regf
         if in_regf is None:
-            in_regf = _IN_REGF_DEFAULTS.get(bus, True)
-        return Field(name=name, bus=bus, portgroups=portgroups, signame=signame, in_regf=in_regf, **kwargs)
+            in_regf = get_in_regf(bus, core)
+        field = Field(name=name, bus=bus, core=core, portgroups=portgroups, signame=signame, in_regf=in_regf, **kwargs)
+        check_field(field)
+        return field
+
+
+def get_in_regf(bus: Access, core: Access) -> bool:
+    """Calculate whether field is in regf."""
+    if bus == _addrspace.RO and core == _addrspace.RO:
+        return True
+    return _IN_REGF_DEFAULTS.get(bus, True)
+
+
+def check_field(field: Field) -> None:
+    """Check for Corner Cases On Field."""
+    # Multiple Portgroups are not allowed for driven fields
+    multigrp = field.portgroups and (len(field.portgroups) > 1)
+    provide_coreval = False
+    if field.in_regf:
+        if field.core and field.core.write and field.core.write.write is not None:
+            provide_coreval = True
+    elif field.bus and field.bus.read:
+        provide_coreval = True
+    if multigrp and provide_coreval:
+        raise ValueError(f"Field {field.name!r} cannot be part of multiple portgroups when core provides a value!")
+
+    # constant value with two locations
+    if field.bus == _addrspace.RO and field.core == _addrspace.RO and not field.in_regf:
+        raise ValueError(f"Field {field.name!r} with constant value must be in_regf.")
 
 
 class Addrspace(_addrspace.Addrspace):
     """Address Space."""
 
     portgroups: tuple[str, ...] | None = None
     """Default Portgroups for Words."""
@@ -129,30 +156,30 @@
     def add_word(self, *args, **kwargs):
         """Add Word."""
         return self.addrspace.add_word(*args, **kwargs)
 
     def get_overview(self) -> str:
         """Overview."""
         data = []
+        rslvr = u.ExprResolver(namespace=self.namespace)
         for word in self.addrspace.words:
-            data.append((f"+{word.slice}", word.name, "", "", "", "", ""))
+            data.append((f"+{word.slice}", word.name, "", "", "", ""))
             for field in word.fields:
                 impl = "regf" if field.in_regf else "core"
                 data.append(
                     (
                         "",
-                        "",
+                        rslvr._resolve_slice(field.slice),
                         f".{field.name}",
-                        str(field.slice),
                         str(field.access),
                         f"{field.is_const}",
                         impl,
                     )
                 )
-        headers = ("Offset", "Word", "Field", "Bits", "Bus/Core", "Const", "Impl")
+        headers = ("Offset", "Word", "Field", "Bus/Core", "Const", "Impl")
         return tabulate(data, headers=headers)
 
 
 def _get_regfiotype(addrspace: Addrspace) -> u.DynamicStructType:
     portgroupmap: dict[str | None, u.DynamicStrucType] = {}
     portgroupmap[None] = regfiotype = u.DynamicStructType()
     for word in addrspace.words:
@@ -160,15 +187,18 @@
             for portgroup in field.portgroups or [None]:
                 try:
                     iotype = portgroupmap[portgroup]
                 except KeyError:
                     portgroupmap[portgroup] = iotype = u.DynamicStructType()
                     regfiotype.add(portgroup, iotype)
                 comment = f"bus={field.bus} core={field.core} in_regf={field.in_regf}"
-                iotype.add(field.signame, FieldIoType(field=field), comment=comment)
+                fieldiotype = FieldIoType(field=field)
+                if word.depth:
+                    fieldiotype = u.ArrayType(fieldiotype, word.depth)
+                iotype.add(field.signame, fieldiotype, comment=comment)
     return regfiotype
 
 
 def _create_route(mod: u.BaseMod, addrspace: Addrspace) -> None:
     for word in addrspace.words:
         for field in word.fields:
             if field.route:
```

### Comparing `ucdp_regf-0.1.0/tests/refdata/tests.test_svmako/test_full/tests/full/full.sv` & `ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_full/tests/full/full.sv`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,19 @@
   // ------------------------------------------------------
   full_regf u_regf (
     // main_i
     .main_clk_i         (1'b0        ), // TODO
     .main_rst_an_i      (1'b0        ), // TODO - Async Reset (Low-Active)
     // mem_i
     .mem_ena_i          (1'b0        ), // TODO
-    .mem_addr_i         (16'h0000    ), // TODO
+    .mem_addr_i         (13'h0000    ), // TODO
     .mem_wena_i         (1'b0        ), // TODO
     .mem_wdata_i        (32'h00000000), // TODO
     .mem_rdata_o        (            ), // TODO
-    .mem_err_i          (1'b0        ), // TODO
+    .mem_err_o          (            ), // TODO
     // regf_o
     // regf_w0_f0_o: bus=None core=RO in_regf=False
     // regf_w0_f2_o: bus=None core=RO in_regf=True
     .regf_w0_f2_rval_o  (            ), // TODO - Core Read Value
     // regf_w0_f4_o: bus=None core=RC in_regf=False
     // regf_w0_f6_o: bus=None core=RC in_regf=True
     .regf_w0_f6_rval_o  (            ), // TODO - Core Read Value
@@ -59,532 +59,530 @@
     .regf_w0_f30_wval_i (2'h0        ), // TODO - Core Write Value
     .regf_w0_f30_wr_i   (1'b0        ), // TODO - Core Write Strobe
     // regf_w1_f0_o: bus=None core=RW1S in_regf=False
     // regf_w1_f2_o: bus=None core=RW1S in_regf=True
     .regf_w1_f2_rval_o  (            ), // TODO - Core Read Value
     .regf_w1_f2_wval_i  (2'h0        ), // TODO - Core Write Value
     .regf_w1_f2_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w1_f4_o: bus=RO core=RO in_regf=False
-    .regf_w1_f4_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    // regf_w1_f6_o: bus=RO core=RO in_regf=True
-    .regf_w1_f6_rval_o  (            ), // TODO - Core Read Value
-    // regf_w1_f8_o: bus=RO core=RC in_regf=False
-    .regf_w1_f8_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    // regf_w1_f10_o: bus=RO core=RC in_regf=True
-    .regf_w1_f10_rval_o (            ), // TODO - Core Read Value
-    .regf_w1_f10_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w1_f12_o: bus=RO core=RS in_regf=False
-    .regf_w1_f12_rbus_i (2'h0        ), // TODO - Bus Read Value
-    // regf_w1_f14_o: bus=RO core=RS in_regf=True
-    .regf_w1_f14_rval_o (            ), // TODO - Core Read Value
-    .regf_w1_f14_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w1_f16_o: bus=RO core=WO in_regf=False
-    .regf_w1_f16_rbus_i (2'h0        ), // TODO - Bus Read Value
-    // regf_w1_f18_o: bus=RO core=WO in_regf=True
-    .regf_w1_f18_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w1_f18_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w1_f20_o: bus=RO core=W1C in_regf=False
-    .regf_w1_f20_rbus_i (2'h0        ), // TODO - Bus Read Value
-    // regf_w1_f22_o: bus=RO core=W1C in_regf=True
-    .regf_w1_f22_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w1_f22_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w1_f24_o: bus=RO core=W1S in_regf=False
-    .regf_w1_f24_rbus_i (2'h0        ), // TODO - Bus Read Value
-    // regf_w1_f26_o: bus=RO core=W1S in_regf=True
-    .regf_w1_f26_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w1_f26_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w1_f28_o: bus=RO core=RW in_regf=False
-    .regf_w1_f28_rbus_i (2'h0        ), // TODO - Bus Read Value
-    // regf_w1_f30_o: bus=RO core=RW in_regf=True
-    .regf_w1_f30_rval_o (            ), // TODO - Core Read Value
-    .regf_w1_f30_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w1_f30_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w2_f0_o: bus=RO core=RW1C in_regf=False
-    .regf_w2_f0_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    // regf_w2_f2_o: bus=RO core=RW1C in_regf=True
-    .regf_w2_f2_rval_o  (            ), // TODO - Core Read Value
-    .regf_w2_f2_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w2_f2_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w2_f4_o: bus=RO core=RW1S in_regf=False
-    .regf_w2_f4_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    // regf_w2_f6_o: bus=RO core=RW1S in_regf=True
-    .regf_w2_f6_rval_o  (            ), // TODO - Core Read Value
-    .regf_w2_f6_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w2_f6_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w2_f8_o: bus=RC core=RO in_regf=False
-    .regf_w2_f8_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w2_f8_rd_o    (            ), // TODO - Bus Read Strobe
-    // regf_w2_f10_o: bus=RC core=RO in_regf=True
-    .regf_w2_f10_rval_o (            ), // TODO - Core Read Value
-    // regf_w2_f12_o: bus=RC core=RC in_regf=False
-    .regf_w2_f12_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w2_f12_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w2_f14_o: bus=RC core=RC in_regf=True
-    .regf_w2_f14_rval_o (            ), // TODO - Core Read Value
-    .regf_w2_f14_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w2_f16_o: bus=RC core=RS in_regf=False
-    .regf_w2_f16_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w2_f16_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w2_f18_o: bus=RC core=RS in_regf=True
-    .regf_w2_f18_rval_o (            ), // TODO - Core Read Value
-    .regf_w2_f18_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w2_f20_o: bus=RC core=WO in_regf=False
-    .regf_w2_f20_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w2_f20_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w2_f22_o: bus=RC core=WO in_regf=True
-    .regf_w2_f22_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w2_f22_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w2_f24_o: bus=RC core=W1C in_regf=False
-    .regf_w2_f24_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w2_f24_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w2_f26_o: bus=RC core=W1C in_regf=True
-    .regf_w2_f26_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w2_f26_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w2_f28_o: bus=RC core=W1S in_regf=False
-    .regf_w2_f28_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w2_f28_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w2_f30_o: bus=RC core=W1S in_regf=True
-    .regf_w2_f30_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w2_f30_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w3_f0_o: bus=RC core=RW in_regf=False
-    .regf_w3_f0_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w3_f0_rd_o    (            ), // TODO - Bus Read Strobe
-    // regf_w3_f2_o: bus=RC core=RW in_regf=True
-    .regf_w3_f2_rval_o  (            ), // TODO - Core Read Value
-    .regf_w3_f2_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w3_f2_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w3_f4_o: bus=RC core=RW1C in_regf=False
-    .regf_w3_f4_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w3_f4_rd_o    (            ), // TODO - Bus Read Strobe
-    // regf_w3_f6_o: bus=RC core=RW1C in_regf=True
-    .regf_w3_f6_rval_o  (            ), // TODO - Core Read Value
-    .regf_w3_f6_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w3_f6_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w3_f8_o: bus=RC core=RW1S in_regf=False
-    .regf_w3_f8_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w3_f8_rd_o    (            ), // TODO - Bus Read Strobe
-    // regf_w3_f10_o: bus=RC core=RW1S in_regf=True
-    .regf_w3_f10_rval_o (            ), // TODO - Core Read Value
-    .regf_w3_f10_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w3_f10_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w3_f12_o: bus=RS core=RO in_regf=False
-    .regf_w3_f12_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w3_f12_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w3_f14_o: bus=RS core=RO in_regf=True
-    .regf_w3_f14_rval_o (            ), // TODO - Core Read Value
-    // regf_w3_f16_o: bus=RS core=RC in_regf=False
-    .regf_w3_f16_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w3_f16_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w3_f18_o: bus=RS core=RC in_regf=True
-    .regf_w3_f18_rval_o (            ), // TODO - Core Read Value
-    .regf_w3_f18_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w3_f20_o: bus=RS core=RS in_regf=False
-    .regf_w3_f20_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w3_f20_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w3_f22_o: bus=RS core=RS in_regf=True
-    .regf_w3_f22_rval_o (            ), // TODO - Core Read Value
-    .regf_w3_f22_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w3_f24_o: bus=RS core=WO in_regf=False
-    .regf_w3_f24_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w3_f24_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w3_f26_o: bus=RS core=WO in_regf=True
-    .regf_w3_f26_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w3_f26_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w3_f28_o: bus=RS core=W1C in_regf=False
-    .regf_w3_f28_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w3_f28_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w3_f30_o: bus=RS core=W1C in_regf=True
-    .regf_w3_f30_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w3_f30_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w4_f0_o: bus=RS core=W1S in_regf=False
-    .regf_w4_f0_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w4_f0_rd_o    (            ), // TODO - Bus Read Strobe
-    // regf_w4_f2_o: bus=RS core=W1S in_regf=True
-    .regf_w4_f2_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w4_f2_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w4_f4_o: bus=RS core=RW in_regf=False
-    .regf_w4_f4_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w4_f4_rd_o    (            ), // TODO - Bus Read Strobe
-    // regf_w4_f6_o: bus=RS core=RW in_regf=True
-    .regf_w4_f6_rval_o  (            ), // TODO - Core Read Value
-    .regf_w4_f6_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w4_f6_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w4_f8_o: bus=RS core=RW1C in_regf=False
-    .regf_w4_f8_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w4_f8_rd_o    (            ), // TODO - Bus Read Strobe
-    // regf_w4_f10_o: bus=RS core=RW1C in_regf=True
-    .regf_w4_f10_rval_o (            ), // TODO - Core Read Value
-    .regf_w4_f10_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w4_f10_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w4_f12_o: bus=RS core=RW1S in_regf=False
-    .regf_w4_f12_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w4_f12_rd_o   (            ), // TODO - Bus Read Strobe
-    // regf_w4_f14_o: bus=RS core=RW1S in_regf=True
-    .regf_w4_f14_rval_o (            ), // TODO - Core Read Value
-    .regf_w4_f14_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w4_f14_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w4_f16_o: bus=WO core=RO in_regf=False
-    .regf_w4_f16_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w4_f16_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w4_f18_o: bus=WO core=RO in_regf=True
-    .regf_w4_f18_rval_o (            ), // TODO - Core Read Value
-    // regf_w4_f20_o: bus=WO core=RC in_regf=False
-    .regf_w4_f20_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w4_f20_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w4_f22_o: bus=WO core=RC in_regf=True
-    .regf_w4_f22_rval_o (            ), // TODO - Core Read Value
-    .regf_w4_f22_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w4_f24_o: bus=WO core=RS in_regf=False
-    .regf_w4_f24_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w4_f24_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w4_f26_o: bus=WO core=RS in_regf=True
-    .regf_w4_f26_rval_o (            ), // TODO - Core Read Value
-    .regf_w4_f26_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w4_f28_o: bus=WO core=WO in_regf=False
-    .regf_w4_f28_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w4_f28_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w4_f30_o: bus=WO core=WO in_regf=True
-    .regf_w4_f30_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w4_f30_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w5_f0_o: bus=WO core=W1C in_regf=False
-    .regf_w5_f0_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w5_f0_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w5_f2_o: bus=WO core=W1C in_regf=True
-    .regf_w5_f2_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w5_f2_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w5_f4_o: bus=WO core=W1S in_regf=False
-    .regf_w5_f4_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w5_f4_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w5_f6_o: bus=WO core=W1S in_regf=True
-    .regf_w5_f6_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w5_f6_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w5_f8_o: bus=WO core=RW in_regf=False
-    .regf_w5_f8_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w5_f8_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w5_f10_o: bus=WO core=RW in_regf=True
-    .regf_w5_f10_rval_o (            ), // TODO - Core Read Value
-    .regf_w5_f10_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w5_f10_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w5_f12_o: bus=WO core=RW1C in_regf=False
-    .regf_w5_f12_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w5_f12_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w5_f14_o: bus=WO core=RW1C in_regf=True
-    .regf_w5_f14_rval_o (            ), // TODO - Core Read Value
-    .regf_w5_f14_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w5_f14_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w5_f16_o: bus=WO core=RW1S in_regf=False
-    .regf_w5_f16_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w5_f16_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w5_f18_o: bus=WO core=RW1S in_regf=True
-    .regf_w5_f18_rval_o (            ), // TODO - Core Read Value
-    .regf_w5_f18_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w5_f18_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w5_f20_o: bus=W1C core=RO in_regf=False
-    .regf_w5_f20_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w5_f20_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w5_f22_o: bus=W1C core=RO in_regf=True
-    .regf_w5_f22_rval_o (            ), // TODO - Core Read Value
-    // regf_w5_f24_o: bus=W1C core=RC in_regf=False
-    .regf_w5_f24_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w5_f24_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w5_f26_o: bus=W1C core=RC in_regf=True
-    .regf_w5_f26_rval_o (            ), // TODO - Core Read Value
-    .regf_w5_f26_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w5_f28_o: bus=W1C core=RS in_regf=False
-    .regf_w5_f28_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w5_f28_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w5_f30_o: bus=W1C core=RS in_regf=True
-    .regf_w5_f30_rval_o (            ), // TODO - Core Read Value
-    .regf_w5_f30_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w6_f0_o: bus=W1C core=WO in_regf=False
-    .regf_w6_f0_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w6_f0_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w6_f2_o: bus=W1C core=WO in_regf=True
-    .regf_w6_f2_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w6_f2_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w6_f4_o: bus=W1C core=W1C in_regf=False
-    .regf_w6_f4_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w6_f4_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w6_f6_o: bus=W1C core=W1C in_regf=True
-    .regf_w6_f6_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w6_f6_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w6_f8_o: bus=W1C core=W1S in_regf=False
-    .regf_w6_f8_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w6_f8_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w6_f10_o: bus=W1C core=W1S in_regf=True
-    .regf_w6_f10_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w6_f10_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w6_f12_o: bus=W1C core=RW in_regf=False
-    .regf_w6_f12_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w6_f12_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w6_f14_o: bus=W1C core=RW in_regf=True
-    .regf_w6_f14_rval_o (            ), // TODO - Core Read Value
-    .regf_w6_f14_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w6_f14_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w6_f16_o: bus=W1C core=RW1C in_regf=False
-    .regf_w6_f16_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w6_f16_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w6_f18_o: bus=W1C core=RW1C in_regf=True
-    .regf_w6_f18_rval_o (            ), // TODO - Core Read Value
-    .regf_w6_f18_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w6_f18_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w6_f20_o: bus=W1C core=RW1S in_regf=False
-    .regf_w6_f20_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w6_f20_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w6_f22_o: bus=W1C core=RW1S in_regf=True
-    .regf_w6_f22_rval_o (            ), // TODO - Core Read Value
-    .regf_w6_f22_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w6_f22_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w6_f24_o: bus=W1S core=RO in_regf=False
-    .regf_w6_f24_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w6_f24_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w6_f26_o: bus=W1S core=RO in_regf=True
-    .regf_w6_f26_rval_o (            ), // TODO - Core Read Value
-    // regf_w6_f28_o: bus=W1S core=RC in_regf=False
-    .regf_w6_f28_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w6_f28_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w6_f30_o: bus=W1S core=RC in_regf=True
-    .regf_w6_f30_rval_o (            ), // TODO - Core Read Value
-    .regf_w6_f30_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w7_f0_o: bus=W1S core=RS in_regf=False
-    .regf_w7_f0_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w7_f0_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w7_f2_o: bus=W1S core=RS in_regf=True
-    .regf_w7_f2_rval_o  (            ), // TODO - Core Read Value
-    .regf_w7_f2_rd_i    (1'b0        ), // TODO - Core Read Strobe
-    // regf_w7_f4_o: bus=W1S core=WO in_regf=False
-    .regf_w7_f4_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w7_f4_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w7_f6_o: bus=W1S core=WO in_regf=True
-    .regf_w7_f6_wval_i  (2'h0        ), // TODO - Core Write Value
-    .regf_w7_f6_wr_i    (1'b0        ), // TODO - Core Write Strobe
-    // regf_w7_f8_o: bus=W1S core=W1C in_regf=False
-    .regf_w7_f8_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w7_f8_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w7_f10_o: bus=W1S core=W1C in_regf=True
-    .regf_w7_f10_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w7_f10_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w7_f12_o: bus=W1S core=W1S in_regf=False
-    .regf_w7_f12_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w7_f12_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w7_f14_o: bus=W1S core=W1S in_regf=True
-    .regf_w7_f14_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w7_f14_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w7_f16_o: bus=W1S core=RW in_regf=False
-    .regf_w7_f16_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w7_f16_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w7_f18_o: bus=W1S core=RW in_regf=True
-    .regf_w7_f18_rval_o (            ), // TODO - Core Read Value
-    .regf_w7_f18_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w7_f18_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w7_f20_o: bus=W1S core=RW1C in_regf=False
-    .regf_w7_f20_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w7_f20_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w7_f22_o: bus=W1S core=RW1C in_regf=True
-    .regf_w7_f22_rval_o (            ), // TODO - Core Read Value
-    .regf_w7_f22_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w7_f22_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w7_f24_o: bus=W1S core=RW1S in_regf=False
-    .regf_w7_f24_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w7_f24_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w7_f26_o: bus=W1S core=RW1S in_regf=True
-    .regf_w7_f26_rval_o (            ), // TODO - Core Read Value
-    .regf_w7_f26_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w7_f26_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w7_f28_o: bus=RW core=RO in_regf=False
-    .regf_w7_f28_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w7_f28_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w7_f28_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w7_f30_o: bus=RW core=RO in_regf=True
-    .regf_w7_f30_rval_o (            ), // TODO - Core Read Value
-    // regf_w8_f0_o: bus=RW core=RC in_regf=False
-    .regf_w8_f0_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w8_f0_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w8_f0_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w8_f2_o: bus=RW core=RC in_regf=True
-    .regf_w8_f2_rval_o  (            ), // TODO - Core Read Value
-    .regf_w8_f2_rd_i    (1'b0        ), // TODO - Core Read Strobe
-    // regf_w8_f4_o: bus=RW core=RS in_regf=False
-    .regf_w8_f4_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w8_f4_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w8_f4_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w8_f6_o: bus=RW core=RS in_regf=True
-    .regf_w8_f6_rval_o  (            ), // TODO - Core Read Value
-    .regf_w8_f6_rd_i    (1'b0        ), // TODO - Core Read Strobe
-    // regf_w8_f8_o: bus=RW core=WO in_regf=False
-    .regf_w8_f8_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w8_f8_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w8_f8_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w8_f10_o: bus=RW core=WO in_regf=True
-    .regf_w8_f10_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w8_f10_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w8_f12_o: bus=RW core=W1C in_regf=False
-    .regf_w8_f12_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w8_f12_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w8_f12_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w8_f14_o: bus=RW core=W1C in_regf=True
-    .regf_w8_f14_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w8_f14_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w8_f16_o: bus=RW core=W1S in_regf=False
-    .regf_w8_f16_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w8_f16_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w8_f16_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w8_f18_o: bus=RW core=W1S in_regf=True
-    .regf_w8_f18_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w8_f18_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w8_f20_o: bus=RW core=RW in_regf=False
-    .regf_w8_f20_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w8_f20_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w8_f20_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w8_f22_o: bus=RW core=RW in_regf=True
-    .regf_w8_f22_rval_o (            ), // TODO - Core Read Value
-    .regf_w8_f22_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w8_f22_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w8_f24_o: bus=RW core=RW1C in_regf=False
-    .regf_w8_f24_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w8_f24_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w8_f24_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w8_f26_o: bus=RW core=RW1C in_regf=True
-    .regf_w8_f26_rval_o (            ), // TODO - Core Read Value
-    .regf_w8_f26_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w8_f26_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w8_f28_o: bus=RW core=RW1S in_regf=False
-    .regf_w8_f28_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w8_f28_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w8_f28_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w8_f30_o: bus=RW core=RW1S in_regf=True
-    .regf_w8_f30_rval_o (            ), // TODO - Core Read Value
-    .regf_w8_f30_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w8_f30_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w9_f0_o: bus=RW1C core=RO in_regf=False
-    .regf_w9_f0_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w9_f0_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w9_f0_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w9_f2_o: bus=RW1C core=RO in_regf=True
-    .regf_w9_f2_rval_o  (            ), // TODO - Core Read Value
-    // regf_w9_f4_o: bus=RW1C core=RC in_regf=False
-    .regf_w9_f4_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w9_f4_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w9_f4_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w9_f6_o: bus=RW1C core=RC in_regf=True
-    .regf_w9_f6_rval_o  (            ), // TODO - Core Read Value
-    .regf_w9_f6_rd_i    (1'b0        ), // TODO - Core Read Strobe
-    // regf_w9_f8_o: bus=RW1C core=RS in_regf=False
-    .regf_w9_f8_rbus_i  (2'h0        ), // TODO - Bus Read Value
-    .regf_w9_f8_wbus_o  (            ), // TODO - Bus Write Value
-    .regf_w9_f8_wr_o    (            ), // TODO - Bus Write Strobe
-    // regf_w9_f10_o: bus=RW1C core=RS in_regf=True
-    .regf_w9_f10_rval_o (            ), // TODO - Core Read Value
-    .regf_w9_f10_rd_i   (1'b0        ), // TODO - Core Read Strobe
-    // regf_w9_f12_o: bus=RW1C core=WO in_regf=False
-    .regf_w9_f12_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w9_f12_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w9_f12_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w9_f14_o: bus=RW1C core=WO in_regf=True
-    .regf_w9_f14_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w9_f14_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w9_f16_o: bus=RW1C core=W1C in_regf=False
-    .regf_w9_f16_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w9_f16_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w9_f16_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w9_f18_o: bus=RW1C core=W1C in_regf=True
-    .regf_w9_f18_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w9_f18_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w9_f20_o: bus=RW1C core=W1S in_regf=False
-    .regf_w9_f20_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w9_f20_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w9_f20_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w9_f22_o: bus=RW1C core=W1S in_regf=True
-    .regf_w9_f22_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w9_f22_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w9_f24_o: bus=RW1C core=RW in_regf=False
-    .regf_w9_f24_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w9_f24_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w9_f24_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w9_f26_o: bus=RW1C core=RW in_regf=True
-    .regf_w9_f26_rval_o (            ), // TODO - Core Read Value
-    .regf_w9_f26_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w9_f26_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w9_f28_o: bus=RW1C core=RW1C in_regf=False
-    .regf_w9_f28_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w9_f28_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w9_f28_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w9_f30_o: bus=RW1C core=RW1C in_regf=True
-    .regf_w9_f30_rval_o (            ), // TODO - Core Read Value
-    .regf_w9_f30_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w9_f30_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w10_f0_o: bus=RW1C core=RW1S in_regf=False
-    .regf_w10_f0_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w10_f0_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w10_f0_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w10_f2_o: bus=RW1C core=RW1S in_regf=True
-    .regf_w10_f2_rval_o (            ), // TODO - Core Read Value
-    .regf_w10_f2_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w10_f2_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w10_f4_o: bus=RW1S core=RO in_regf=False
-    .regf_w10_f4_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w10_f4_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w10_f4_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w10_f6_o: bus=RW1S core=RO in_regf=True
-    .regf_w10_f6_rval_o (            ), // TODO - Core Read Value
-    // regf_w10_f8_o: bus=RW1S core=RC in_regf=False
-    .regf_w10_f8_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w10_f8_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w10_f8_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w10_f10_o: bus=RW1S core=RC in_regf=True
-    .regf_w10_f10_rval_o(            ), // TODO - Core Read Value
-    .regf_w10_f10_rd_i  (1'b0        ), // TODO - Core Read Strobe
-    // regf_w10_f12_o: bus=RW1S core=RS in_regf=False
-    .regf_w10_f12_rbus_i(2'h0        ), // TODO - Bus Read Value
-    .regf_w10_f12_wbus_o(            ), // TODO - Bus Write Value
-    .regf_w10_f12_wr_o  (            ), // TODO - Bus Write Strobe
-    // regf_w10_f14_o: bus=RW1S core=RS in_regf=True
-    .regf_w10_f14_rval_o(            ), // TODO - Core Read Value
-    .regf_w10_f14_rd_i  (1'b0        ), // TODO - Core Read Strobe
-    // regf_w10_f16_o: bus=RW1S core=WO in_regf=False
-    .regf_w10_f16_rbus_i(2'h0        ), // TODO - Bus Read Value
-    .regf_w10_f16_wbus_o(            ), // TODO - Bus Write Value
-    .regf_w10_f16_wr_o  (            ), // TODO - Bus Write Strobe
-    // regf_w10_f18_o: bus=RW1S core=WO in_regf=True
-    .regf_w10_f18_wval_i(2'h0        ), // TODO - Core Write Value
-    .regf_w10_f18_wr_i  (1'b0        ), // TODO - Core Write Strobe
-    // regf_w10_f20_o: bus=RW1S core=W1C in_regf=False
-    .regf_w10_f20_rbus_i(2'h0        ), // TODO - Bus Read Value
-    .regf_w10_f20_wbus_o(            ), // TODO - Bus Write Value
-    .regf_w10_f20_wr_o  (            ), // TODO - Bus Write Strobe
-    // regf_w10_f22_o: bus=RW1S core=W1C in_regf=True
-    .regf_w10_f22_wval_i(2'h0        ), // TODO - Core Write Value
-    .regf_w10_f22_wr_i  (1'b0        ), // TODO - Core Write Strobe
-    // regf_w10_f24_o: bus=RW1S core=W1S in_regf=False
-    .regf_w10_f24_rbus_i(2'h0        ), // TODO - Bus Read Value
-    .regf_w10_f24_wbus_o(            ), // TODO - Bus Write Value
-    .regf_w10_f24_wr_o  (            ), // TODO - Bus Write Strobe
-    // regf_w10_f26_o: bus=RW1S core=W1S in_regf=True
-    .regf_w10_f26_wval_i(2'h0        ), // TODO - Core Write Value
-    .regf_w10_f26_wr_i  (1'b0        ), // TODO - Core Write Strobe
-    // regf_w10_f28_o: bus=RW1S core=RW in_regf=False
-    .regf_w10_f28_rbus_i(2'h0        ), // TODO - Bus Read Value
-    .regf_w10_f28_wbus_o(            ), // TODO - Bus Write Value
-    .regf_w10_f28_wr_o  (            ), // TODO - Bus Write Strobe
-    // regf_w10_f30_o: bus=RW1S core=RW in_regf=True
-    .regf_w10_f30_rval_o(            ), // TODO - Core Read Value
-    .regf_w10_f30_wval_i(2'h0        ), // TODO - Core Write Value
-    .regf_w10_f30_wr_i  (1'b0        ), // TODO - Core Write Strobe
-    // regf_w11_f0_o: bus=RW1S core=RW1C in_regf=False
-    .regf_w11_f0_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w11_f0_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w11_f0_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w11_f2_o: bus=RW1S core=RW1C in_regf=True
-    .regf_w11_f2_rval_o (            ), // TODO - Core Read Value
-    .regf_w11_f2_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w11_f2_wr_i   (1'b0        ), // TODO - Core Write Strobe
-    // regf_w11_f4_o: bus=RW1S core=RW1S in_regf=False
-    .regf_w11_f4_rbus_i (2'h0        ), // TODO - Bus Read Value
-    .regf_w11_f4_wbus_o (            ), // TODO - Bus Write Value
-    .regf_w11_f4_wr_o   (            ), // TODO - Bus Write Strobe
-    // regf_w11_f6_o: bus=RW1S core=RW1S in_regf=True
-    .regf_w11_f6_rval_o (            ), // TODO - Core Read Value
-    .regf_w11_f6_wval_i (2'h0        ), // TODO - Core Write Value
-    .regf_w11_f6_wr_i   (1'b0        )  // TODO - Core Write Strobe
+    // regf_w1_f4_o: bus=RO core=RO in_regf=True
+    .regf_w1_f4_rval_o  (            ), // TODO - Core Read Value
+    // regf_w1_f6_o: bus=RO core=RC in_regf=False
+    .regf_w1_f6_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    // regf_w1_f8_o: bus=RO core=RC in_regf=True
+    .regf_w1_f8_rval_o  (            ), // TODO - Core Read Value
+    .regf_w1_f8_rd_i    (1'b0        ), // TODO - Core Read Strobe
+    // regf_w1_f10_o: bus=RO core=RS in_regf=False
+    .regf_w1_f10_rbus_i (2'h0        ), // TODO - Bus Read Value
+    // regf_w1_f12_o: bus=RO core=RS in_regf=True
+    .regf_w1_f12_rval_o (            ), // TODO - Core Read Value
+    .regf_w1_f12_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w1_f14_o: bus=RO core=WO in_regf=False
+    .regf_w1_f14_rbus_i (2'h0        ), // TODO - Bus Read Value
+    // regf_w1_f16_o: bus=RO core=WO in_regf=True
+    .regf_w1_f16_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w1_f16_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w1_f18_o: bus=RO core=W1C in_regf=False
+    .regf_w1_f18_rbus_i (2'h0        ), // TODO - Bus Read Value
+    // regf_w1_f20_o: bus=RO core=W1C in_regf=True
+    .regf_w1_f20_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w1_f20_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w1_f22_o: bus=RO core=W1S in_regf=False
+    .regf_w1_f22_rbus_i (2'h0        ), // TODO - Bus Read Value
+    // regf_w1_f24_o: bus=RO core=W1S in_regf=True
+    .regf_w1_f24_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w1_f24_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w1_f26_o: bus=RO core=RW in_regf=False
+    .regf_w1_f26_rbus_i (2'h0        ), // TODO - Bus Read Value
+    // regf_w1_f28_o: bus=RO core=RW in_regf=True
+    .regf_w1_f28_rval_o (            ), // TODO - Core Read Value
+    .regf_w1_f28_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w1_f28_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w1_f30_o: bus=RO core=RW1C in_regf=False
+    .regf_w1_f30_rbus_i (2'h0        ), // TODO - Bus Read Value
+    // regf_w2_f0_o: bus=RO core=RW1C in_regf=True
+    .regf_w2_f0_rval_o  (            ), // TODO - Core Read Value
+    .regf_w2_f0_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w2_f0_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w2_f2_o: bus=RO core=RW1S in_regf=False
+    .regf_w2_f2_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    // regf_w2_f4_o: bus=RO core=RW1S in_regf=True
+    .regf_w2_f4_rval_o  (            ), // TODO - Core Read Value
+    .regf_w2_f4_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w2_f4_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w2_f6_o: bus=RC core=RO in_regf=False
+    .regf_w2_f6_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    .regf_w2_f6_rd_o    (            ), // TODO - Bus Read Strobe
+    // regf_w2_f8_o: bus=RC core=RO in_regf=True
+    .regf_w2_f8_rval_o  (            ), // TODO - Core Read Value
+    // regf_w2_f10_o: bus=RC core=RC in_regf=False
+    .regf_w2_f10_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w2_f10_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w2_f12_o: bus=RC core=RC in_regf=True
+    .regf_w2_f12_rval_o (            ), // TODO - Core Read Value
+    .regf_w2_f12_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w2_f14_o: bus=RC core=RS in_regf=False
+    .regf_w2_f14_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w2_f14_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w2_f16_o: bus=RC core=RS in_regf=True
+    .regf_w2_f16_rval_o (            ), // TODO - Core Read Value
+    .regf_w2_f16_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w2_f18_o: bus=RC core=WO in_regf=False
+    .regf_w2_f18_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w2_f18_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w2_f20_o: bus=RC core=WO in_regf=True
+    .regf_w2_f20_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w2_f20_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w2_f22_o: bus=RC core=W1C in_regf=False
+    .regf_w2_f22_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w2_f22_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w2_f24_o: bus=RC core=W1C in_regf=True
+    .regf_w2_f24_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w2_f24_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w2_f26_o: bus=RC core=W1S in_regf=False
+    .regf_w2_f26_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w2_f26_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w2_f28_o: bus=RC core=W1S in_regf=True
+    .regf_w2_f28_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w2_f28_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w2_f30_o: bus=RC core=RW in_regf=False
+    .regf_w2_f30_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w2_f30_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w3_f0_o: bus=RC core=RW in_regf=True
+    .regf_w3_f0_rval_o  (            ), // TODO - Core Read Value
+    .regf_w3_f0_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w3_f0_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w3_f2_o: bus=RC core=RW1C in_regf=False
+    .regf_w3_f2_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    .regf_w3_f2_rd_o    (            ), // TODO - Bus Read Strobe
+    // regf_w3_f4_o: bus=RC core=RW1C in_regf=True
+    .regf_w3_f4_rval_o  (            ), // TODO - Core Read Value
+    .regf_w3_f4_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w3_f4_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w3_f6_o: bus=RC core=RW1S in_regf=False
+    .regf_w3_f6_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    .regf_w3_f6_rd_o    (            ), // TODO - Bus Read Strobe
+    // regf_w3_f8_o: bus=RC core=RW1S in_regf=True
+    .regf_w3_f8_rval_o  (            ), // TODO - Core Read Value
+    .regf_w3_f8_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w3_f8_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w3_f10_o: bus=RS core=RO in_regf=False
+    .regf_w3_f10_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w3_f10_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w3_f12_o: bus=RS core=RO in_regf=True
+    .regf_w3_f12_rval_o (            ), // TODO - Core Read Value
+    // regf_w3_f14_o: bus=RS core=RC in_regf=False
+    .regf_w3_f14_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w3_f14_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w3_f16_o: bus=RS core=RC in_regf=True
+    .regf_w3_f16_rval_o (            ), // TODO - Core Read Value
+    .regf_w3_f16_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w3_f18_o: bus=RS core=RS in_regf=False
+    .regf_w3_f18_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w3_f18_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w3_f20_o: bus=RS core=RS in_regf=True
+    .regf_w3_f20_rval_o (            ), // TODO - Core Read Value
+    .regf_w3_f20_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w3_f22_o: bus=RS core=WO in_regf=False
+    .regf_w3_f22_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w3_f22_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w3_f24_o: bus=RS core=WO in_regf=True
+    .regf_w3_f24_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w3_f24_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w3_f26_o: bus=RS core=W1C in_regf=False
+    .regf_w3_f26_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w3_f26_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w3_f28_o: bus=RS core=W1C in_regf=True
+    .regf_w3_f28_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w3_f28_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w3_f30_o: bus=RS core=W1S in_regf=False
+    .regf_w3_f30_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w3_f30_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w4_f0_o: bus=RS core=W1S in_regf=True
+    .regf_w4_f0_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w4_f0_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w4_f2_o: bus=RS core=RW in_regf=False
+    .regf_w4_f2_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    .regf_w4_f2_rd_o    (            ), // TODO - Bus Read Strobe
+    // regf_w4_f4_o: bus=RS core=RW in_regf=True
+    .regf_w4_f4_rval_o  (            ), // TODO - Core Read Value
+    .regf_w4_f4_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w4_f4_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w4_f6_o: bus=RS core=RW1C in_regf=False
+    .regf_w4_f6_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    .regf_w4_f6_rd_o    (            ), // TODO - Bus Read Strobe
+    // regf_w4_f8_o: bus=RS core=RW1C in_regf=True
+    .regf_w4_f8_rval_o  (            ), // TODO - Core Read Value
+    .regf_w4_f8_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w4_f8_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w4_f10_o: bus=RS core=RW1S in_regf=False
+    .regf_w4_f10_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w4_f10_rd_o   (            ), // TODO - Bus Read Strobe
+    // regf_w4_f12_o: bus=RS core=RW1S in_regf=True
+    .regf_w4_f12_rval_o (            ), // TODO - Core Read Value
+    .regf_w4_f12_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w4_f12_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w4_f14_o: bus=WO core=RO in_regf=False
+    .regf_w4_f14_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w4_f14_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w4_f16_o: bus=WO core=RO in_regf=True
+    .regf_w4_f16_rval_o (            ), // TODO - Core Read Value
+    // regf_w4_f18_o: bus=WO core=RC in_regf=False
+    .regf_w4_f18_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w4_f18_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w4_f20_o: bus=WO core=RC in_regf=True
+    .regf_w4_f20_rval_o (            ), // TODO - Core Read Value
+    .regf_w4_f20_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w4_f22_o: bus=WO core=RS in_regf=False
+    .regf_w4_f22_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w4_f22_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w4_f24_o: bus=WO core=RS in_regf=True
+    .regf_w4_f24_rval_o (            ), // TODO - Core Read Value
+    .regf_w4_f24_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w4_f26_o: bus=WO core=WO in_regf=False
+    .regf_w4_f26_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w4_f26_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w4_f28_o: bus=WO core=WO in_regf=True
+    .regf_w4_f28_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w4_f28_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w4_f30_o: bus=WO core=W1C in_regf=False
+    .regf_w4_f30_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w4_f30_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w5_f0_o: bus=WO core=W1C in_regf=True
+    .regf_w5_f0_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w5_f0_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w5_f2_o: bus=WO core=W1S in_regf=False
+    .regf_w5_f2_wbus_o  (            ), // TODO - Bus Write Value
+    .regf_w5_f2_wr_o    (            ), // TODO - Bus Write Strobe
+    // regf_w5_f4_o: bus=WO core=W1S in_regf=True
+    .regf_w5_f4_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w5_f4_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w5_f6_o: bus=WO core=RW in_regf=False
+    .regf_w5_f6_wbus_o  (            ), // TODO - Bus Write Value
+    .regf_w5_f6_wr_o    (            ), // TODO - Bus Write Strobe
+    // regf_w5_f8_o: bus=WO core=RW in_regf=True
+    .regf_w5_f8_rval_o  (            ), // TODO - Core Read Value
+    .regf_w5_f8_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w5_f8_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w5_f10_o: bus=WO core=RW1C in_regf=False
+    .regf_w5_f10_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w5_f10_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w5_f12_o: bus=WO core=RW1C in_regf=True
+    .regf_w5_f12_rval_o (            ), // TODO - Core Read Value
+    .regf_w5_f12_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w5_f12_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w5_f14_o: bus=WO core=RW1S in_regf=False
+    .regf_w5_f14_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w5_f14_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w5_f16_o: bus=WO core=RW1S in_regf=True
+    .regf_w5_f16_rval_o (            ), // TODO - Core Read Value
+    .regf_w5_f16_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w5_f16_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w5_f18_o: bus=W1C core=RO in_regf=False
+    .regf_w5_f18_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w5_f18_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w5_f20_o: bus=W1C core=RO in_regf=True
+    .regf_w5_f20_rval_o (            ), // TODO - Core Read Value
+    // regf_w5_f22_o: bus=W1C core=RC in_regf=False
+    .regf_w5_f22_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w5_f22_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w5_f24_o: bus=W1C core=RC in_regf=True
+    .regf_w5_f24_rval_o (            ), // TODO - Core Read Value
+    .regf_w5_f24_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w5_f26_o: bus=W1C core=RS in_regf=False
+    .regf_w5_f26_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w5_f26_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w5_f28_o: bus=W1C core=RS in_regf=True
+    .regf_w5_f28_rval_o (            ), // TODO - Core Read Value
+    .regf_w5_f28_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w5_f30_o: bus=W1C core=WO in_regf=False
+    .regf_w5_f30_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w5_f30_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w6_f0_o: bus=W1C core=WO in_regf=True
+    .regf_w6_f0_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w6_f0_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w6_f2_o: bus=W1C core=W1C in_regf=False
+    .regf_w6_f2_wbus_o  (            ), // TODO - Bus Write Value
+    .regf_w6_f2_wr_o    (            ), // TODO - Bus Write Strobe
+    // regf_w6_f4_o: bus=W1C core=W1C in_regf=True
+    .regf_w6_f4_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w6_f4_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w6_f6_o: bus=W1C core=W1S in_regf=False
+    .regf_w6_f6_wbus_o  (            ), // TODO - Bus Write Value
+    .regf_w6_f6_wr_o    (            ), // TODO - Bus Write Strobe
+    // regf_w6_f8_o: bus=W1C core=W1S in_regf=True
+    .regf_w6_f8_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w6_f8_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w6_f10_o: bus=W1C core=RW in_regf=False
+    .regf_w6_f10_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w6_f10_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w6_f12_o: bus=W1C core=RW in_regf=True
+    .regf_w6_f12_rval_o (            ), // TODO - Core Read Value
+    .regf_w6_f12_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w6_f12_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w6_f14_o: bus=W1C core=RW1C in_regf=False
+    .regf_w6_f14_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w6_f14_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w6_f16_o: bus=W1C core=RW1C in_regf=True
+    .regf_w6_f16_rval_o (            ), // TODO - Core Read Value
+    .regf_w6_f16_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w6_f16_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w6_f18_o: bus=W1C core=RW1S in_regf=False
+    .regf_w6_f18_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w6_f18_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w6_f20_o: bus=W1C core=RW1S in_regf=True
+    .regf_w6_f20_rval_o (            ), // TODO - Core Read Value
+    .regf_w6_f20_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w6_f20_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w6_f22_o: bus=W1S core=RO in_regf=False
+    .regf_w6_f22_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w6_f22_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w6_f24_o: bus=W1S core=RO in_regf=True
+    .regf_w6_f24_rval_o (            ), // TODO - Core Read Value
+    // regf_w6_f26_o: bus=W1S core=RC in_regf=False
+    .regf_w6_f26_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w6_f26_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w6_f28_o: bus=W1S core=RC in_regf=True
+    .regf_w6_f28_rval_o (            ), // TODO - Core Read Value
+    .regf_w6_f28_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w6_f30_o: bus=W1S core=RS in_regf=False
+    .regf_w6_f30_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w6_f30_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w7_f0_o: bus=W1S core=RS in_regf=True
+    .regf_w7_f0_rval_o  (            ), // TODO - Core Read Value
+    .regf_w7_f0_rd_i    (1'b0        ), // TODO - Core Read Strobe
+    // regf_w7_f2_o: bus=W1S core=WO in_regf=False
+    .regf_w7_f2_wbus_o  (            ), // TODO - Bus Write Value
+    .regf_w7_f2_wr_o    (            ), // TODO - Bus Write Strobe
+    // regf_w7_f4_o: bus=W1S core=WO in_regf=True
+    .regf_w7_f4_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w7_f4_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w7_f6_o: bus=W1S core=W1C in_regf=False
+    .regf_w7_f6_wbus_o  (            ), // TODO - Bus Write Value
+    .regf_w7_f6_wr_o    (            ), // TODO - Bus Write Strobe
+    // regf_w7_f8_o: bus=W1S core=W1C in_regf=True
+    .regf_w7_f8_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w7_f8_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w7_f10_o: bus=W1S core=W1S in_regf=False
+    .regf_w7_f10_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w7_f10_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w7_f12_o: bus=W1S core=W1S in_regf=True
+    .regf_w7_f12_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w7_f12_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w7_f14_o: bus=W1S core=RW in_regf=False
+    .regf_w7_f14_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w7_f14_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w7_f16_o: bus=W1S core=RW in_regf=True
+    .regf_w7_f16_rval_o (            ), // TODO - Core Read Value
+    .regf_w7_f16_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w7_f16_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w7_f18_o: bus=W1S core=RW1C in_regf=False
+    .regf_w7_f18_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w7_f18_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w7_f20_o: bus=W1S core=RW1C in_regf=True
+    .regf_w7_f20_rval_o (            ), // TODO - Core Read Value
+    .regf_w7_f20_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w7_f20_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w7_f22_o: bus=W1S core=RW1S in_regf=False
+    .regf_w7_f22_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w7_f22_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w7_f24_o: bus=W1S core=RW1S in_regf=True
+    .regf_w7_f24_rval_o (            ), // TODO - Core Read Value
+    .regf_w7_f24_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w7_f24_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w7_f26_o: bus=RW core=RO in_regf=False
+    .regf_w7_f26_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w7_f26_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w7_f26_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w7_f28_o: bus=RW core=RO in_regf=True
+    .regf_w7_f28_rval_o (            ), // TODO - Core Read Value
+    // regf_w7_f30_o: bus=RW core=RC in_regf=False
+    .regf_w7_f30_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w7_f30_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w7_f30_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w8_f0_o: bus=RW core=RC in_regf=True
+    .regf_w8_f0_rval_o  (            ), // TODO - Core Read Value
+    .regf_w8_f0_rd_i    (1'b0        ), // TODO - Core Read Strobe
+    // regf_w8_f2_o: bus=RW core=RS in_regf=False
+    .regf_w8_f2_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    .regf_w8_f2_wbus_o  (            ), // TODO - Bus Write Value
+    .regf_w8_f2_wr_o    (            ), // TODO - Bus Write Strobe
+    // regf_w8_f4_o: bus=RW core=RS in_regf=True
+    .regf_w8_f4_rval_o  (            ), // TODO - Core Read Value
+    .regf_w8_f4_rd_i    (1'b0        ), // TODO - Core Read Strobe
+    // regf_w8_f6_o: bus=RW core=WO in_regf=False
+    .regf_w8_f6_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    .regf_w8_f6_wbus_o  (            ), // TODO - Bus Write Value
+    .regf_w8_f6_wr_o    (            ), // TODO - Bus Write Strobe
+    // regf_w8_f8_o: bus=RW core=WO in_regf=True
+    .regf_w8_f8_wval_i  (2'h0        ), // TODO - Core Write Value
+    .regf_w8_f8_wr_i    (1'b0        ), // TODO - Core Write Strobe
+    // regf_w8_f10_o: bus=RW core=W1C in_regf=False
+    .regf_w8_f10_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w8_f10_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w8_f10_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w8_f12_o: bus=RW core=W1C in_regf=True
+    .regf_w8_f12_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w8_f12_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w8_f14_o: bus=RW core=W1S in_regf=False
+    .regf_w8_f14_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w8_f14_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w8_f14_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w8_f16_o: bus=RW core=W1S in_regf=True
+    .regf_w8_f16_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w8_f16_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w8_f18_o: bus=RW core=RW in_regf=False
+    .regf_w8_f18_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w8_f18_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w8_f18_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w8_f20_o: bus=RW core=RW in_regf=True
+    .regf_w8_f20_rval_o (            ), // TODO - Core Read Value
+    .regf_w8_f20_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w8_f20_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w8_f22_o: bus=RW core=RW1C in_regf=False
+    .regf_w8_f22_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w8_f22_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w8_f22_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w8_f24_o: bus=RW core=RW1C in_regf=True
+    .regf_w8_f24_rval_o (            ), // TODO - Core Read Value
+    .regf_w8_f24_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w8_f24_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w8_f26_o: bus=RW core=RW1S in_regf=False
+    .regf_w8_f26_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w8_f26_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w8_f26_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w8_f28_o: bus=RW core=RW1S in_regf=True
+    .regf_w8_f28_rval_o (            ), // TODO - Core Read Value
+    .regf_w8_f28_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w8_f28_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w8_f30_o: bus=RW1C core=RO in_regf=False
+    .regf_w8_f30_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w8_f30_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w8_f30_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w9_f0_o: bus=RW1C core=RO in_regf=True
+    .regf_w9_f0_rval_o  (            ), // TODO - Core Read Value
+    // regf_w9_f2_o: bus=RW1C core=RC in_regf=False
+    .regf_w9_f2_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    .regf_w9_f2_wbus_o  (            ), // TODO - Bus Write Value
+    .regf_w9_f2_wr_o    (            ), // TODO - Bus Write Strobe
+    // regf_w9_f4_o: bus=RW1C core=RC in_regf=True
+    .regf_w9_f4_rval_o  (            ), // TODO - Core Read Value
+    .regf_w9_f4_rd_i    (1'b0        ), // TODO - Core Read Strobe
+    // regf_w9_f6_o: bus=RW1C core=RS in_regf=False
+    .regf_w9_f6_rbus_i  (2'h0        ), // TODO - Bus Read Value
+    .regf_w9_f6_wbus_o  (            ), // TODO - Bus Write Value
+    .regf_w9_f6_wr_o    (            ), // TODO - Bus Write Strobe
+    // regf_w9_f8_o: bus=RW1C core=RS in_regf=True
+    .regf_w9_f8_rval_o  (            ), // TODO - Core Read Value
+    .regf_w9_f8_rd_i    (1'b0        ), // TODO - Core Read Strobe
+    // regf_w9_f10_o: bus=RW1C core=WO in_regf=False
+    .regf_w9_f10_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w9_f10_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w9_f10_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w9_f12_o: bus=RW1C core=WO in_regf=True
+    .regf_w9_f12_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w9_f12_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w9_f14_o: bus=RW1C core=W1C in_regf=False
+    .regf_w9_f14_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w9_f14_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w9_f14_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w9_f16_o: bus=RW1C core=W1C in_regf=True
+    .regf_w9_f16_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w9_f16_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w9_f18_o: bus=RW1C core=W1S in_regf=False
+    .regf_w9_f18_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w9_f18_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w9_f18_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w9_f20_o: bus=RW1C core=W1S in_regf=True
+    .regf_w9_f20_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w9_f20_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w9_f22_o: bus=RW1C core=RW in_regf=False
+    .regf_w9_f22_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w9_f22_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w9_f22_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w9_f24_o: bus=RW1C core=RW in_regf=True
+    .regf_w9_f24_rval_o (            ), // TODO - Core Read Value
+    .regf_w9_f24_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w9_f24_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w9_f26_o: bus=RW1C core=RW1C in_regf=False
+    .regf_w9_f26_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w9_f26_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w9_f26_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w9_f28_o: bus=RW1C core=RW1C in_regf=True
+    .regf_w9_f28_rval_o (            ), // TODO - Core Read Value
+    .regf_w9_f28_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w9_f28_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w9_f30_o: bus=RW1C core=RW1S in_regf=False
+    .regf_w9_f30_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w9_f30_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w9_f30_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w10_f0_o: bus=RW1C core=RW1S in_regf=True
+    .regf_w10_f0_rval_o (            ), // TODO - Core Read Value
+    .regf_w10_f0_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w10_f0_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w10_f2_o: bus=RW1S core=RO in_regf=False
+    .regf_w10_f2_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w10_f2_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w10_f2_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w10_f4_o: bus=RW1S core=RO in_regf=True
+    .regf_w10_f4_rval_o (            ), // TODO - Core Read Value
+    // regf_w10_f6_o: bus=RW1S core=RC in_regf=False
+    .regf_w10_f6_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w10_f6_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w10_f6_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w10_f8_o: bus=RW1S core=RC in_regf=True
+    .regf_w10_f8_rval_o (            ), // TODO - Core Read Value
+    .regf_w10_f8_rd_i   (1'b0        ), // TODO - Core Read Strobe
+    // regf_w10_f10_o: bus=RW1S core=RS in_regf=False
+    .regf_w10_f10_rbus_i(2'h0        ), // TODO - Bus Read Value
+    .regf_w10_f10_wbus_o(            ), // TODO - Bus Write Value
+    .regf_w10_f10_wr_o  (            ), // TODO - Bus Write Strobe
+    // regf_w10_f12_o: bus=RW1S core=RS in_regf=True
+    .regf_w10_f12_rval_o(            ), // TODO - Core Read Value
+    .regf_w10_f12_rd_i  (1'b0        ), // TODO - Core Read Strobe
+    // regf_w10_f14_o: bus=RW1S core=WO in_regf=False
+    .regf_w10_f14_rbus_i(2'h0        ), // TODO - Bus Read Value
+    .regf_w10_f14_wbus_o(            ), // TODO - Bus Write Value
+    .regf_w10_f14_wr_o  (            ), // TODO - Bus Write Strobe
+    // regf_w10_f16_o: bus=RW1S core=WO in_regf=True
+    .regf_w10_f16_wval_i(2'h0        ), // TODO - Core Write Value
+    .regf_w10_f16_wr_i  (1'b0        ), // TODO - Core Write Strobe
+    // regf_w10_f18_o: bus=RW1S core=W1C in_regf=False
+    .regf_w10_f18_rbus_i(2'h0        ), // TODO - Bus Read Value
+    .regf_w10_f18_wbus_o(            ), // TODO - Bus Write Value
+    .regf_w10_f18_wr_o  (            ), // TODO - Bus Write Strobe
+    // regf_w10_f20_o: bus=RW1S core=W1C in_regf=True
+    .regf_w10_f20_wval_i(2'h0        ), // TODO - Core Write Value
+    .regf_w10_f20_wr_i  (1'b0        ), // TODO - Core Write Strobe
+    // regf_w10_f22_o: bus=RW1S core=W1S in_regf=False
+    .regf_w10_f22_rbus_i(2'h0        ), // TODO - Bus Read Value
+    .regf_w10_f22_wbus_o(            ), // TODO - Bus Write Value
+    .regf_w10_f22_wr_o  (            ), // TODO - Bus Write Strobe
+    // regf_w10_f24_o: bus=RW1S core=W1S in_regf=True
+    .regf_w10_f24_wval_i(2'h0        ), // TODO - Core Write Value
+    .regf_w10_f24_wr_i  (1'b0        ), // TODO - Core Write Strobe
+    // regf_w10_f26_o: bus=RW1S core=RW in_regf=False
+    .regf_w10_f26_rbus_i(2'h0        ), // TODO - Bus Read Value
+    .regf_w10_f26_wbus_o(            ), // TODO - Bus Write Value
+    .regf_w10_f26_wr_o  (            ), // TODO - Bus Write Strobe
+    // regf_w10_f28_o: bus=RW1S core=RW in_regf=True
+    .regf_w10_f28_rval_o(            ), // TODO - Core Read Value
+    .regf_w10_f28_wval_i(2'h0        ), // TODO - Core Write Value
+    .regf_w10_f28_wr_i  (1'b0        ), // TODO - Core Write Strobe
+    // regf_w10_f30_o: bus=RW1S core=RW1C in_regf=False
+    .regf_w10_f30_rbus_i(2'h0        ), // TODO - Bus Read Value
+    .regf_w10_f30_wbus_o(            ), // TODO - Bus Write Value
+    .regf_w10_f30_wr_o  (            ), // TODO - Bus Write Strobe
+    // regf_w11_f0_o: bus=RW1S core=RW1C in_regf=True
+    .regf_w11_f0_rval_o (            ), // TODO - Core Read Value
+    .regf_w11_f0_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w11_f0_wr_i   (1'b0        ), // TODO - Core Write Strobe
+    // regf_w11_f2_o: bus=RW1S core=RW1S in_regf=False
+    .regf_w11_f2_rbus_i (2'h0        ), // TODO - Bus Read Value
+    .regf_w11_f2_wbus_o (            ), // TODO - Bus Write Value
+    .regf_w11_f2_wr_o   (            ), // TODO - Bus Write Strobe
+    // regf_w11_f4_o: bus=RW1S core=RW1S in_regf=True
+    .regf_w11_f4_rval_o (            ), // TODO - Core Read Value
+    .regf_w11_f4_wval_i (2'h0        ), // TODO - Core Write Value
+    .regf_w11_f4_wr_i   (1'b0        )  // TODO - Core Write Strobe
   );
 
 endmodule // full
```

### Comparing `ucdp_regf-0.1.0/tests/refdata/tests.test_svmako/test_top/uart/uart/rtl/uart.sv` & `ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_top/uart/uart/rtl/uart.sv`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 // Data Model: uart.uart.UartMod
 //
 // =============================================================================
 
 
 module uart ( // uart.uart.UartMod
   // main_i
-  input  wire           main_clk_i,
-  input  wire           main_rst_an_i, // Async Reset (Low-Active)
+  input  wire         main_clk_i,
+  input  wire         main_rst_an_i, // Async Reset (Low-Active)
   // uart_o: RX/TX
-  input  wire           uart_rx_i,
-  output logic          uart_tx_o,
+  input  wire         uart_rx_i,
+  output logic        uart_tx_o,
   // bus_i
-  input  wire  [2-1:0]  bus_trans_i,
-  input  wire  [32-1:0] bus_addr_i,
-  input  wire           bus_write_i,
-  input  wire  [32-1:0] bus_wdata_i,
-  output logic          bus_ready_o,
-  output logic          bus_resp_o,
-  output logic [32-1:0] bus_rdata_o
+  input  wire  [1:0]  bus_trans_i,
+  input  wire  [31:0] bus_addr_i,
+  input  wire         bus_write_i,
+  input  wire  [31:0] bus_wdata_i,
+  output logic        bus_ready_o,
+  output logic        bus_resp_o,
+  output logic [31:0] bus_rdata_o
 );
 
 
 
   // ------------------------------------------------------
   //  Signals
   // ------------------------------------------------------
-         logic clk_s;
-  output logic regf_regf_ctrl_ena_rval_o_s;
-  output logic regf_regf_ctrl_busy_rbus_i_s;
+  logic clk_s;
+  logic regf_regf_ctrl_ena_rval_o_s;
+  logic regf_regf_ctrl_busy_rbus_i_s;
 
 
   // ------------------------------------------------------
   //  glbl.clk_gate: u_clk_gate
   // ------------------------------------------------------
   clk_gate u_clk_gate (
     .clk_i(main_clk_i                 ),
@@ -48,19 +48,19 @@
   // ------------------------------------------------------
   uart_regf u_regf (
     // main_i
     .main_clk_i           (main_clk_i                  ),
     .main_rst_an_i        (main_rst_an_i               ), // Async Reset (Low-Active)
     // mem_i
     .mem_ena_i            (1'b0                        ), // TODO
-    .mem_addr_i           (16'h0000                    ), // TODO
+    .mem_addr_i           (13'h0000                    ), // TODO
     .mem_wena_i           (1'b0                        ), // TODO
     .mem_wdata_i          (32'h00000000                ), // TODO
     .mem_rdata_o          (                            ), // TODO
-    .mem_err_i            (1'b0                        ), // TODO
+    .mem_err_o            (                            ), // TODO
     // regf_o
     // regf_ctrl_ena_o: bus=RW core=RO in_regf=True
     .regf_ctrl_ena_rval_o (regf_regf_ctrl_ena_rval_o_s ), // Core Read Value
     // regf_ctrl_busy_o: bus=RO core=RW in_regf=False
     .regf_ctrl_busy_rbus_i(regf_regf_ctrl_busy_rbus_i_s)  // Bus Read Value
   );
```

### Comparing `ucdp_regf-0.1.0/tests/refdata/tests.test_svmako/test_top/uart/uart/rtl/uart_core.sv` & `ucdp_regf-0.2.0/tests/refdata/tests.test_svmako/test_top/uart/uart/rtl/uart_core.sv`

 * *Files identical despite different names*

### Comparing `ucdp_regf-0.1.0/PKG-INFO` & `ucdp_regf-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ucdp-regf
-Version: 0.1.0
+Version: 0.2.0
 Summary: Unified Chip Design Platform - Register File
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/nbiotcloud/ucdp-regf
 Project-URL: Documentation, https://ucdp-regf.readthedocs.io/en/latest/
 Project-URL: Bug tracker, https://github.com/nbiotcloud/ucdp-regf/issues
 Requires-Python: <4.0,>=3.10.0
-Requires-Dist: ucdp-glbl>=0.1.0
-Requires-Dist: ucdp>=0.3.0
+Requires-Dist: ucdp>=0.4.1
+Requires-Dist: ucdp-glbl>=0.2.0
 Description-Content-Type: text/markdown
 
 [![PyPI Version](https://badge.fury.io/py/ucdp-regf.svg)](https://badge.fury.io/py/ucdp-regf)
 [![Python Build](https://github.com/nbiotcloud/ucdp-regf/actions/workflows/main.yml/badge.svg)](https://github.com/nbiotcloud/ucdp-regf/actions/workflows/main.yml)
 [![Documentation](https://readthedocs.org/projects/ucdp-regf/badge/?version=latest)](https://ucdp-regf.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/nbiotcloud/ucdp-regf/badge.svg?branch=main)](https://coveralls.io/github/nbiotcloud/ucdp-regf?branch=main)
 [![python-versions](https://img.shields.io/pypi/pyversions/ucdp-regf.svg)](https://pypi.python.org/pypi/ucdp-regf)
```

