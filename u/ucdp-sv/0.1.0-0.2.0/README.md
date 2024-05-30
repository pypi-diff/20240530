# Comparing `tmp/ucdp_sv-0.1.0.tar.gz` & `tmp/ucdp_sv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucdp_sv-0.1.0.tar", last modified: Mon May 20 22:11:28 2024, max compression
+gzip compressed data, was "ucdp_sv-0.2.0.tar", last modified: Thu May 30 06:54:35 2024, max compression
```

## Comparing `ucdp_sv-0.1.0.tar` & `ucdp_sv-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2024-05-20 22:11:16.133225 ucdp_sv-0.1.0/LICENSE
--rw-r--r--   0        0        0     1000 2024-05-20 22:11:16.133225 ucdp_sv-0.1.0/README.md
--rw-r--r--   0        0        0     2394 2024-05-20 22:11:28.329111 ucdp_sv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    14628 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/src/ucdpsv/__init__.py
--rw-r--r--   0        0        0     6704 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/src/ucdpsv/templates/sv.mako
--rw-r--r--   0        0        0       13 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      313 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1188 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/refdata/tests.test_svmako/test_top/glbl/clk_gate.sv
--rw-r--r--   0        0        0     1936 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/refdata/tests.test_svmako/test_top/top/top.sv
--rw-r--r--   0        0        0      679 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/refdata/tests.test_svmako/test_top/top/top_core.sv
--rw-r--r--   0        0        0     2476 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/test_svexprresolver.py
--rw-r--r--   0        0        0     1530 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/test_svmako.py
--rw-r--r--   0        0        0     1635 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/testdata/example/fileliststandard.py
--rw-r--r--   0        0        0     1140 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/testdata/example/glbl/__init__.py
--rw-r--r--   0        0        0     2696 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/testdata/example/glbl/bus.py
--rw-r--r--   0        0        0     1518 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/testdata/example/glbl/clk_gate.py
--rw-r--r--   0        0        0      419 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/testdata/example/src/glbl/clk_gate.sv
--rw-r--r--   0        0        0     1132 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/testdata/example/top/__init__.py
--rw-r--r--   0        0        0     2757 2024-05-20 22:11:16.137225 ucdp_sv-0.1.0/tests/testdata/example/top/top.py
--rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 ucdp_sv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-30 06:54:23.126046 ucdp_sv-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1000 2024-05-30 06:54:23.126046 ucdp_sv-0.2.0/README.md
+-rw-r--r--   0        0        0     2394 2024-05-30 06:54:35.390122 ucdp_sv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    15894 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/src/ucdpsv/__init__.py
+-rw-r--r--   0        0        0     6711 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/src/ucdpsv/templates/sv.mako
+-rw-r--r--   0        0        0       13 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1188 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/refdata/tests.test_svmako/test_top/glbl/clk_gate.sv
+-rw-r--r--   0        0        0     2418 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/refdata/tests.test_svmako/test_top/top/top.sv
+-rw-r--r--   0        0        0      935 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/refdata/tests.test_svmako/test_top/top/top_core.sv
+-rw-r--r--   0        0        0     2476 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/test_svexprresolver.py
+-rw-r--r--   0        0        0     1530 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/test_svmako.py
+-rw-r--r--   0        0        0     1635 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/testdata/example/fileliststandard.py
+-rw-r--r--   0        0        0     1140 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/testdata/example/glbl/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/testdata/example/glbl/bus.py
+-rw-r--r--   0        0        0     1518 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/testdata/example/glbl/clk_gate.py
+-rw-r--r--   0        0        0      419 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/testdata/example/src/glbl/clk_gate.sv
+-rw-r--r--   0        0        0     1132 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/testdata/example/top/__init__.py
+-rw-r--r--   0        0        0     3358 2024-05-30 06:54:23.130046 ucdp_sv-0.2.0/tests/testdata/example/top/top.py
+-rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 ucdp_sv-0.2.0/PKG-INFO
```

### Comparing `ucdp_sv-0.1.0/LICENSE` & `ucdp_sv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ucdp_sv-0.1.0/README.md` & `ucdp_sv-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ucdp_sv-0.1.0/pyproject.toml` & `ucdp_sv-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "ucdp-sv"
-version = "0.1.0"
+version = "0.2.0"
 description = "Unified Chip Design Platform"
 readme = "README.md"
 authors = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 packages = [
     "src/ucdpsv/",
 ]
 requires-python = ">=3.10.0,<4.0"
 dependencies = [
     "aligntext>=1.0.0",
-    "ucdp>=0.3.0",
+    "ucdp>=0.4.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/nbiotcloud/ucdp-sv"
 Documentation = "https://ucdp-sv.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/nbiotcloud/ucdp-sv/issues"
```

### Comparing `ucdp_sv-0.1.0/src/ucdpsv/__init__.py` & `ucdp_sv-0.2.0/src/ucdpsv/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """Unified Chip Design Platform - SystemVerilog."""
 
 from collections.abc import Iterable, Iterator
-from typing import Literal
+from typing import ClassVar, Literal
 
 import ucdp as u
 from aligntext import Align
 from matchor import matchs
 
 DIRKEYWORDS = {
     u.IN: "input",
@@ -69,33 +69,55 @@
     >>> resolver = usv.SvExprResolver()
     >>> resolver.resolve(u.ConstExpr(u.UintType(18, default=5)))
     "18'h00005"
     >>> resolver.resolve(u.ConstExpr(u.SintType(18, default=-5)))
     "18'sh3FFFB"
     """
 
+    ff_dly: str = ""
+    _opremap: ClassVar[dict[str, str]] = {"//": "/"}
+
     @staticmethod
     def _get_rail_value(value: int) -> str:
         return f"1'b{value}"
 
     @staticmethod
     def _get_bit_value(value: int) -> str:
         return f"1'b{value}"
 
-    @staticmethod
-    def _get_uint_value(value: int, width: int) -> str:
-        hexstr = f"{value:X}".zfill((width + 3) // 4)
-        return f"{width}'h{hexstr}"
+    def _get_uint_value(self, value: int, width: int | u.Expr) -> str:
+        if isinstance(width, int):
+            hexstr = f"{value:X}".zfill((width + 3) // 4)
+            return f"{width}'h{hexstr}"
+
+        # parameterized width
+        width = self.resolve(width)
+        if value != 0:
+            # This is not the best, but all we can do - or?
+            return f"{width}'d{value}"
+
+        return f"{{{width} {{1'b0}}}}"
+
+    def _get_sint_value(self, value: int, width: int | u.Expr) -> str:
+        if isinstance(width, int):
+            wrap = 1 << width
+            value = (value + wrap) % wrap
+            hexstr = f"{value:X}".zfill((width + 3) // 4)
+            return f"{width}'sh{hexstr}"
+
+        # parameterized width
+        width = self.resolve(width)
+
+        # This is not the best, but all we can do - or?
+        if value > 0:
+            return f"{width}'d{value}"
+        if value < 0:
+            return f"-({width}'d{-value})"
 
-    @staticmethod
-    def _get_sint_value(value: int, width: int) -> str:
-        wrap = 1 << width
-        value = (value + wrap) % wrap
-        hexstr = f"{value:X}".zfill((width + 3) // 4)
-        return f"{width}'sh{hexstr}"
+        return f"{{{width} {{1'sb0}}}}"
 
     @staticmethod
     def _get_integer_value(value: int) -> str:
         return str(value)
 
     @staticmethod
     def _get_bool_value(value: bool) -> str:
@@ -131,15 +153,17 @@
             align.add_row((keyword, *svdecl, name, svdims, "=", svdefault, svcomment))
         return align
 
     def get_portdecls(
         self, ports: u.Idents, is_last: bool = True, indent: int = 0, wirenames: u.Names | None = None
     ) -> Align:
         """Return `Align` With Port Declarations."""
-        return self._get_signaldecls(ports.iter(), ",", is_last=is_last, indent=indent, wirenames=wirenames)
+        return self._get_signaldecls(
+            ports.iter(), ",", is_last=is_last, indent=indent, wirenames=wirenames, is4ports=True
+        )
 
     def get_signaldecls(self, signals: u.Idents, indent: int = 0, wirenames: u.Names | None = None) -> Align:
         """Return `Align` With Signal Declarations."""
 
         def stop(signal):
             return isinstance(signal, u.Port)
 
@@ -148,33 +172,37 @@
     def _get_signaldecls(
         self,
         iterator: Iterable[u.Ident],
         sep: str,
         is_last: bool,
         indent: int,
         wirenames: u.Names | None = None,
+        is4ports: bool = False,
     ) -> Align:
         align = Align(rtrim=True, strip_empty_cols=True)
         pre = " " * indent
         align.set_separators(" ", first=pre)
         wirenames = u.split(wirenames)
         for ident, svdecl, svsep in self._iter_idents(align, pre, iterator, sep, is_last):
             name = ident.name
             svdims = self.get_dims(ident.type_)
             if svdims:
                 svdims = f"{svdims}{svsep}"
             else:
                 name = f"{name}{svsep}"
             svcomment = _get_comment(ident.doc.comment)
-            dirkeyword = DIRKEYWORDS.get(ident.direction)
-            if isinstance(ident.type_, u.BaseScalarType):
+            if isinstance(ident.type_, (u.BaseScalarType, u.ArrayType)):
                 logickeyword = "wire" if matchs(ident.name, wirenames) else LOGICKEYWORDS.get(ident.direction)
             else:
                 logickeyword = ""
-            align.add_row((dirkeyword, logickeyword, *svdecl, name, svdims, svcomment))
+            if is4ports:
+                dirkeyword = DIRKEYWORDS.get(ident.direction)
+                align.add_row((dirkeyword, logickeyword, *svdecl, name, svdims, svcomment))
+            else:
+                align.add_row((logickeyword, *svdecl, name, svdims, svcomment))
         return align
 
     def get_instparams(self, mod: u.BaseMod, is_last: bool = True, indent: int = 0) -> Align:
         """Return `Align` With Parameter Declarations."""
         align = Align(rtrim=True)
         pre = " " * indent
         align.set_separators("(", ")", "", first=pre)
@@ -278,21 +306,21 @@
         if isinstance(type_, u.SintType):
             return "signed", self._resolve_slice(type_.slice_).replace(" ", "")
 
         if isinstance(type_, u.BaseStructType):
             return None
 
         if isinstance(type_, u.IntegerType):
-            return "", "integer"
+            return "integer", ""
 
         if isinstance(type_, u.BoolType):
-            return "", "bool"
+            return "bool", ""
 
         if isinstance(type_, u.StringType):
-            return "", "string"
+            return "string", ""
 
         raise ValueError(type_)
 
     def get_dims(self, type_: u.BaseType) -> str:
         """Get SV Dimensions."""
         dims = []
         while isinstance(type_, u.ArrayType):
@@ -340,14 +368,20 @@
             return None
         if op == 0:
             return self._resolve_value(type_, value=0)
         if op == 1:
             return self._resolve_value(type_, value=type_.max_)
         return f"{op}{name}"
 
+    def _get_array_value(self, itemvalue: str, slice_: u.Slice) -> str:
+        width = slice_.width
+        if not isinstance(width, int):
+            width = self._resolve(width)
+        return f"'{{{width}{{{itemvalue}}}}}"
+
 
 def _get_comment(comment, level=0, pre="") -> str:
     """Return Systemverilog Comment."""
     if comment:
         comment = comment.split("\n", maxsplit=1)[0]
         fill = "  " * level
         return f"{pre}// {fill}{comment}"
@@ -385,10 +419,12 @@
         else:
             comment = f"{name}{comment}"
         align.add_spacer(_get_comment(comment, pre=pre))
         return 0
     return None
 
 
-def get_resolver(mod: u.BaseMod) -> SvExprResolver:
+def get_resolver(mod: u.BaseMod, inst: u.BaseMod | None = None) -> SvExprResolver:
     """Get SvExprResolver for `mod`."""
+    if inst is not None:
+        return SvExprResolver(namespace=mod.namespace, remap=inst.params)
     return SvExprResolver(namespace=mod.namespace)
```

### Comparing `ucdp_sv-0.1.0/src/ucdpsv/templates/sv.mako` & `ucdp_sv-0.2.0/src/ucdpsv/templates/sv.mako`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 
 
 <%def name="inst(inst, indent=0)">\
 <%
   inst = mod.get_inst(inst)
   pre = " " * indent
   comment = inst.doc.comment or f"{inst.libname}.{inst.modname}: {inst.name}"
-  rslvr = usv.get_resolver(mod)
+  rslvr = usv.get_resolver(mod, inst=inst)
   params = rslvr.get_instparams(inst, indent=indent+2)
   ports = rslvr.get_instcons(mod.get_instcons(inst), indent=indent+2)
 %>\
 ${pre}// ------------------------------------------------------
 % for line in comment.split("\n"):
 ${pre}//  ${line}
 % endfor
@@ -235,18 +235,18 @@
 ${pre}//  Flip-Flops
 ${pre}// ------------------------------------------------------
 % endif
 % for idx, flipflop in enumerate(flipflops):
 
 ${pre}always_ff @(posedge ${flipflop.clk.name} or negedge ${flipflop.rst_an.name}) begin: proc_seq_${idx}
 ${pre}  if (${flipflop.rst_an.name} == 1'b0) begin
-${rslvr.get_defaults(flipflop.defaults(), indent=indent+4, oper="<= #1").get()}
+${rslvr.get_defaults(flipflop.defaults(), indent=indent+4, oper="<= ").get()}
 % if flipflop.rst is not None:
 ${pre}  end else if (${rslvr.resolve(flipflop.rst)}) begin
-${rslvr.get_defaults(flipflop.defaults(), indent=indent+4, oper="<= #1").get()}
+${rslvr.get_defaults(flipflop.defaults(), indent=indent+4, oper="<= ").get()}
 % endif
 % if flipflop.ena is not None:
 ${pre}  end else if (${rslvr.resolve(flipflop.ena)}) begin
 % else:
 ${pre}  end else begin
 % endif
 ${rslvr.get_assigns(flipflop, indent=indent+4, oper="<= #1").get()}
```

### Comparing `ucdp_sv-0.1.0/tests/refdata/tests.test_svmako/test_top/glbl/clk_gate.sv` & `ucdp_sv-0.2.0/tests/refdata/tests.test_svmako/test_top/glbl/clk_gate.sv`

 * *Files identical despite different names*

### Comparing `ucdp_sv-0.1.0/tests/refdata/tests.test_svmako/test_top/top/top.sv` & `ucdp_sv-0.2.0/tests/refdata/tests.test_svmako/test_top/top/top.sv`

 * *Files 10% similar despite different names*

```diff
@@ -3,45 +3,49 @@
 // Module:     top.top
 // Data Model: top.top.TopMod
 //
 // =============================================================================
 
 
 module top #( // top.top.TopMod
-  parameter integer width_p = 10,
-  parameter integer sub_p   = (width_p / 2)
+  parameter integer               param_p   = 10,
+  parameter integer               width_p   = $clog2(param_p + 1),
+  parameter         [param_p-1:0] default_p = {param_p {1'b0}}
 ) (
   // main_i
-  input  wire           main_clk_i,
-  input  wire           main_rst_an_i, // Async Reset (Low-Active)
+  input  wire                main_clk_i,
+  input  wire                main_rst_an_i, // Async Reset (Low-Active)
   // intf_i: RX/TX
-  output logic          intf_rx_o,
-  input  wire           intf_tx_i,
+  output logic               intf_rx_o,
+  input  wire                intf_tx_i,
   // bus_i
-  input  wire  [2-1:0]  bus_trans_i,
-  input  wire  [32-1:0] bus_addr_i,
-  input  wire           bus_write_i,
-  input  wire  [32-1:0] bus_wdata_i,
-  output logic          bus_ready_o,
-  output logic          bus_resp_o,
-  output logic [32-1:0] bus_rdata_o
+  input  wire  [1:0]         bus_trans_i,
+  input  wire  [31:0]        bus_addr_i,
+  input  wire                bus_write_i,
+  input  wire  [31:0]        bus_wdata_i,
+  output logic               bus_ready_o,
+  output logic               bus_resp_o,
+  output logic [31:0]        bus_rdata_o,
+  input  wire  [param_p-1:0] data_i,
+  output logic [width_p-1:0] cnt_o
 );
 
 
 
   // ------------------------------------------------------
   //  Local Parameter
   // ------------------------------------------------------
-  localparam integer cntwidth_p = $clog2((width_p + 1));
+  localparam [param_p-1:0] const_c = default_p / param_p'd2;
 
 
   // ------------------------------------------------------
   //  Signals
   // ------------------------------------------------------
-  logic clk_s;
+  logic       clk_s;
+  logic [7:0] array_s [0:0+(param_p-1)];
 
 
   // ------------------------------------------------------
   //  glbl.clk_gate: u_clk_gate
   // ------------------------------------------------------
   clk_gate u_clk_gate (
     .clk_i(main_clk_i),
@@ -50,20 +54,25 @@
   );
 
 
   // ------------------------------------------------------
   //  top.top_core: u_core
   // ------------------------------------------------------
   top_core #(
-    .width_p(width_p)
+    .param_p(10            ),
+    .width_p($clog2(10 + 1))
   ) u_core (
     // main_i
     .main_clk_i   (clk_s        ),
     .main_rst_an_i(main_rst_an_i), // Async Reset (Low-Active)
-    .data_i       (10'h000      ), // TODO
+    .p_i          ({10 {1'b0}}  ), // TODO
+    .p_o          (             ), // TODO
+    .data_i       ({8 {1'b0}}   ), // TODO
     .data_o       (             ), // TODO
+    .array_i      (array_s      ),
+    .array_open_i ('{8{8'h00}}  ), // TODO
     // intf_i: RX/TX
     .intf_rx_o    (intf_rx_o    ),
     .intf_tx_i    (intf_tx_i    )
   );
 
 endmodule // top
```

### Comparing `ucdp_sv-0.1.0/tests/test_svexprresolver.py` & `ucdp_sv-0.2.0/tests/test_svexprresolver.py`

 * *Files identical despite different names*

### Comparing `ucdp_sv-0.1.0/tests/test_svmako.py` & `ucdp_sv-0.2.0/tests/test_svmako.py`

 * *Files identical despite different names*

### Comparing `ucdp_sv-0.1.0/tests/testdata/example/fileliststandard.py` & `ucdp_sv-0.2.0/tests/testdata/example/fileliststandard.py`

 * *Files identical despite different names*

### Comparing `ucdp_sv-0.1.0/tests/testdata/example/glbl/__init__.py` & `ucdp_sv-0.2.0/tests/testdata/example/glbl/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp_sv-0.1.0/tests/testdata/example/glbl/bus.py` & `ucdp_sv-0.2.0/tests/testdata/example/glbl/bus.py`

 * *Files identical despite different names*

### Comparing `ucdp_sv-0.1.0/tests/testdata/example/glbl/clk_gate.py` & `ucdp_sv-0.2.0/tests/testdata/example/glbl/clk_gate.py`

 * *Files identical despite different names*

### Comparing `ucdp_sv-0.1.0/tests/testdata/example/top/__init__.py` & `ucdp_sv-0.2.0/tests/testdata/example/top/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp_sv-0.1.0/tests/testdata/example/top/top.py` & `ucdp_sv-0.2.0/tests/testdata/example/top/top.py`

 * *Files 19% similar despite different names*

```diff
@@ -45,34 +45,47 @@
 class TopMod(u.AMod):
     """Top Module."""
 
     filelists: ClassVar[u.ModFileLists] = (HdlFileList(gen="full"),)
 
     def _build(self) -> None:
         parser = self.parser
+
+        param_p = self.add_param(u.IntegerType(default=10), "param_p")
+        width_p = self.add_param(u.IntegerType(default=parser.log2(param_p + 1)), "width_p")
+        default_p = self.add_param(u.UintType(param_p), "default_p")
+
         self.add_port(u.ClkRstAnType(), "main_i")
         self.add_port(IoType(), "intf_i", route="create(u_core/intf_i)")
         self.add_port(BusType(), "bus_i")
 
-        width_p = self.add_param(u.IntegerType(default=10), "width_p")
-        self.add_param(u.IntegerType(default=width_p // 2), "sub_p")
-        self.add_const(u.IntegerType(default=parser.log2(width_p + 1)), "cntwidth_p")
+        self.add_port(u.UintType(param_p), "data_i")
+        self.add_port(u.UintType(width_p), "cnt_o")
+
+        self.add_const(u.UintType(param_p, default=default_p // 2), "const_c")
 
         clkgate = ClkGateMod(self, "u_clk_gate")
         clkgate.con("clk_i", "main_clk_i")
         clkgate.con("clk_o", "create(clk_s)")
 
-        core = TopCoreMod(self, "u_core", paramdict={"width_p": width_p})
-        width_p = core.add_param(width_p)
-        core.add_param(u.IntegerType(default=4), "depth_p")
+        core = TopCoreMod(self, "u_core", paramdict={"width_p": width_p, "param_p": param_p})
+        param_p = core.add_param(u.IntegerType(default=10), "param_p")
+        width_p = core.add_param(u.IntegerType(default=8), "width_p")
+        core.add_param(u.SintType(8, default=-3), "other_p")
 
         core.add_port(u.ClkRstAnType(), "main_i")
+        core.add_port(u.UintType(param_p), "p_i")
+        core.add_port(u.UintType(param_p), "p_o")
         core.add_port(u.UintType(width_p), "data_i")
         core.add_port(u.UintType(width_p), "data_o")
 
+        core.add_port(u.ArrayType(u.UintType(8), param_p), "array_i")
+        core.add_port(u.ArrayType(u.UintType(8), 8), "array_open_i")
+        core.con("array_i", "create(array_s)")
+
         core.con("main_clk_i", "clk_s")
         core.con("main_rst_an_i", "main_rst_an_i")
 
 
 class TopCoreMod(u.ACoreMod):
     """Core Module."""
```

### Comparing `ucdp_sv-0.1.0/PKG-INFO` & `ucdp_sv-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ucdp-sv
-Version: 0.1.0
+Version: 0.2.0
 Summary: Unified Chip Design Platform
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/nbiotcloud/ucdp-sv
 Project-URL: Documentation, https://ucdp-sv.readthedocs.io/en/latest/
 Project-URL: Bug tracker, https://github.com/nbiotcloud/ucdp-sv/issues
 Requires-Python: <4.0,>=3.10.0
 Requires-Dist: aligntext>=1.0.0
-Requires-Dist: ucdp>=0.3.0
+Requires-Dist: ucdp>=0.4.0
 Description-Content-Type: text/markdown
 
 [![PyPI Version](https://badge.fury.io/py/ucdp-sv.svg)](https://badge.fury.io/py/ucdp-sv)
 [![Python Build](https://github.com/nbiotcloud/ucdp-sv/actions/workflows/main.yml/badge.svg)](https://github.com/nbiotcloud/ucdp-sv/actions/workflows/main.yml)
 [![Documentation](https://readthedocs.org/projects/ucdp-sv/badge/?version=latest)](https://ucdp-sv.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/nbiotcloud/ucdp-sv/badge.svg?branch=main)](https://coveralls.io/github/nbiotcloud/ucdp-sv?branch=main)
 [![python-versions](https://img.shields.io/pypi/pyversions/ucdp-sv.svg)](https://pypi.python.org/pypi/ucdp-sv)
```

