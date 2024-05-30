# Comparing `tmp/ucdp_glbl-0.1.0.tar.gz` & `tmp/ucdp_glbl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucdp_glbl-0.1.0.tar", last modified: Mon May 20 22:30:17 2024, max compression
+gzip compressed data, was "ucdp_glbl-0.2.0.tar", last modified: Thu May 30 06:53:54 2024, max compression
```

## Comparing `ucdp_glbl-0.1.0.tar` & `ucdp_glbl-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2024-05-20 22:30:04.724147 ucdp_glbl-0.1.0/LICENSE
--rw-r--r--   0        0        0     1030 2024-05-20 22:30:04.724147 ucdp_glbl-0.1.0/README.md
--rw-r--r--   0        0        0     2336 2024-05-20 22:30:17.316099 ucdp_glbl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1154 2024-05-20 22:30:04.724147 ucdp_glbl-0.1.0/src/ucdp_glbl/__init__.py
--rw-r--r--   0        0        0    12697 2024-05-20 22:30:04.724147 ucdp_glbl-0.1.0/src/ucdp_glbl/addrspace.py
--rw-r--r--   0        0        0     4932 2024-05-20 22:30:04.724147 ucdp_glbl-0.1.0/src/ucdp_glbl/mem.py
--rw-r--r--   0        0        0     1122 2024-05-20 22:30:04.724147 ucdp_glbl-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      230 2024-05-20 22:30:04.724147 ucdp_glbl-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-20 22:30:04.724147 ucdp_glbl-0.1.0/tests/refdata/tests.test_addrspace/test_accesses/stderr.txt
--rw-r--r--   0        0        0     1209 2024-05-20 22:30:04.724147 ucdp_glbl-0.1.0/tests/refdata/tests.test_addrspace/test_accesses/stdout.txt
--rw-r--r--   0        0        0     2312 2024-05-20 22:30:04.724147 ucdp_glbl-0.1.0/tests/refdata/tests.test_addrspace/test_volatile/overview.txt
--rw-r--r--   0        0        0     6334 2024-05-20 22:30:04.728147 ucdp_glbl-0.1.0/tests/test_addrspace.py
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 ucdp_glbl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1030 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/README.md
+-rw-r--r--   0        0        0     2336 2024-05-30 06:53:54.754980 ucdp_glbl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1154 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/src/ucdp_glbl/__init__.py
+-rw-r--r--   0        0        0    13409 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/src/ucdp_glbl/addrspace.py
+-rw-r--r--   0        0        0     4951 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/src/ucdp_glbl/mem.py
+-rw-r--r--   0        0        0     1122 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      230 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/tests/refdata/tests.test_addrspace/test_accesses/stderr.txt
+-rw-r--r--   0        0        0     1209 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/tests/refdata/tests.test_addrspace/test_accesses/stdout.txt
+-rw-r--r--   0        0        0     2312 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/tests/refdata/tests.test_addrspace/test_volatile/overview.txt
+-rw-r--r--   0        0        0     6333 2024-05-30 06:53:39.694835 ucdp_glbl-0.2.0/tests/test_addrspace.py
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 ucdp_glbl-0.2.0/PKG-INFO
```

### Comparing `ucdp_glbl-0.1.0/LICENSE` & `ucdp_glbl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ucdp_glbl-0.1.0/README.md` & `ucdp_glbl-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ucdp_glbl-0.1.0/pyproject.toml` & `ucdp_glbl-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "ucdp-glbl"
-version = "0.1.0"
+version = "0.2.0"
 description = "Unified Chip Design Platform - Global"
 readme = "README.md"
 authors = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.10.0,<4.0"
 dependencies = [
-    "ucdp>=0.3.0",
+    "ucdp>=0.4.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/nbiotcloud/ucdp-glbl"
 Documentation = "https://ucdp-glbl.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/nbiotcloud/ucdp-glbl/issues"
```

### Comparing `ucdp_glbl-0.1.0/src/ucdp_glbl/__init__.py` & `ucdp_glbl-0.2.0/src/ucdp_glbl/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp_glbl-0.1.0/src/ucdp_glbl/addrspace.py` & `ucdp_glbl-0.2.0/src/ucdp_glbl/addrspace.py`

 * *Files 3% similar despite different names*

```diff
@@ -237,66 +237,79 @@
 
     type_: u.BaseScalarType
     """Type."""
     bus: Access | None
     """Bus Access."""
     core: Access | None
     """Core Access."""
-    offset: int
+    upd_prio: Literal["bus", "core"] | None
+    """Update Priority: None, 'b'us or 'c'core."""
+    offset: int | u.Expr
     """Rightmost Bit Position."""
     is_volatile: bool = False
     """Volatile."""
     doc: u.Doc = u.Doc()
     """Documentation."""
 
     @property
     def slice(self) -> u.Slice:
         """Slice with Word."""
-        left = self.offset + self.type_.width - 1
-        return u.Slice(right=self.offset, left=left)
+        return u.Slice(width=self.type_.width, right=self.offset)
 
     @property
     def is_const(self) -> bool:
         """Field is Constant."""
         return get_is_const(self.bus, self.core)
 
     @property
     def access(self) -> str:
         """Access."""
         bus = (self.bus and self.bus.name) or "-"
         core = (self.core and self.core.name) or "-"
         return f"{bus}/{core}"
 
+    @property
+    def bus_prio(self) -> bool:
+        """Update prioriy for bus."""
+        if self.upd_prio == "bus":
+            return True
+        if self.upd_prio == "core":
+            return False
+        if self.bus and (self.bus.write or (self.bus.read and self.bus.read.data is not None)):
+            return True
+        return False
+
 
 FieldFilter = Callable[[Field], bool]
 
 
 class Word(u.NamedObject):
     """Word."""
 
     fields: u.Namespace = u.Field(default_factory=u.Namespace, init=False, repr=False)
     """Fields within Word."""
-    offset: int
+    offset: int | u.Expr
     """Rightmost Word Position."""
     width: int
     """Width in Bits."""
-    depth: int | None = None
+    depth: int | u.Expr | None = None
     """Number of words."""
     doc: u.Doc = u.Doc()
     """Documentation"""
 
     def add_field(
         self,
         name: str,
         type_: u.BaseScalarType,
         bus: Access,
         core: Access | None = None,
-        offset: int | None = None,
+        upd_prio: Literal[None, "bus", "core"] | None = None,
+        offset: int | u.Expr | None = None,
         is_volatile: bool | None = None,
-        align: int | None = None,
+        align: int | u.Expr | None = None,
         title: str | None = None,
         descr: str | None = None,
         comment: str | None = None,
         **kwargs,
     ) -> Field:
         """Add field."""
         if bus is not None:
@@ -310,29 +323,38 @@
         else:
             free = 0
         offset = forward(free, offset=offset, align=align)
         doc = u.doc_from_type(type_, title=title, descr=descr, comment=comment)
         if is_volatile is None:
             is_volatile = get_is_volatile(bus, core)
         field = self._create_field(
-            name=name, type_=type_, bus=bus, core=core, offset=offset, is_volatile=is_volatile, doc=doc, **kwargs
+            name=name,
+            type_=type_,
+            bus=bus,
+            core=core,
+            upd_prio=upd_prio,
+            offset=offset,
+            is_volatile=is_volatile,
+            doc=doc,
+            **kwargs,
         )
         if field.slice.left >= self.width:
             raise ValueError(f"Field {field.name!r} exceeds word width of {self.width}")
         self.fields.add(field)
         return field
 
     def _create_field(self, **kwargs) -> Field:
         return Field(**kwargs)
 
     @property
     def slice(self) -> u.Slice:
         """Slice with Address Space."""
-        left = self.offset + (self.depth or 1) - 1
-        return u.Slice(right=self.offset, left=left)
+        if self.depth is None:
+            return u.Slice(left=self.offset, right=self.offset)
+        return u.Slice(width=self.depth, right=self.offset)
 
     def lock(self):
         """Lock For Modification."""
         self.fields.lock()
 
 
 WordFilter = Callable[[Word], bool]
@@ -348,17 +370,17 @@
     """Width in Bits."""
     depth: int = 1024
     """Number of words."""
 
     def add_word(
         self,
         name: str,
-        offset: int | None = None,
-        align: int | None = None,
-        depth: int | None = None,
+        offset: int | u.Expr | None = None,
+        align: int | u.Expr | None = None,
+        depth: int | u.Expr | None = None,
         title: str | None = None,
         descr: str | None = None,
         comment: str | None = None,
         **kwargs,
     ) -> Word:
         """Add Word."""
         if self.words:
@@ -381,15 +403,15 @@
         for word in self.words:
             word.lock()
         self.words.lock()
 
     @property
     def size(self) -> Bytes:
         """Size in Bytes."""
-        return bytes_(self.width * self.depth)
+        return bytes_((self.width * self.depth) // 8)
 
     def get_word_hiername(self, word: Word) -> str:
         """Get Hierarchical Word Name."""
         return f"{self.name}.{word.name}"
 
     def get_field_hiername(self, word: Word, field: Field) -> str:
         """Get Hierarchical Field Name."""
```

### Comparing `ucdp_glbl-0.1.0/src/ucdp_glbl/mem.py` & `ucdp_glbl-0.2.0/src/ucdp_glbl/mem.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         if self.writable:
             self._add("wena", u.EnaType(), title="Memory Write Enable")
             self._add("wdata", datatype, title="Memory Write Data")
         self._add("rdata", datatype, title="Memory Read Data", orientation=u.BWD)
         if self.slicewidths:
             self._add("sel", u.UintType(len(self.slicewidths)), title="Slice Selects")
         if self.err:
-            self._add("err", u.BitType(), title="Memory Access Failed.")
+            self._add("err", u.BitType(), title="Memory Access Failed.", orientation=u.BWD)
 
     @staticmethod
     def with_slicewidth(
         datawidth: int | u.Expr,
         addrwidth: int | u.Expr,
         writable: bool,
         slicewidth: int | u.Expr | None = None,
```

### Comparing `ucdp_glbl-0.1.0/tests/__init__.py` & `ucdp_glbl-0.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp_glbl-0.1.0/tests/refdata/tests.test_addrspace/test_accesses/stdout.txt` & `ucdp_glbl-0.2.0/tests/refdata/tests.test_addrspace/test_accesses/stdout.txt`

 * *Files identical despite different names*

### Comparing `ucdp_glbl-0.1.0/tests/refdata/tests.test_addrspace/test_volatile/overview.txt` & `ucdp_glbl-0.2.0/tests/refdata/tests.test_addrspace/test_volatile/overview.txt`

 * *Files identical despite different names*

### Comparing `ucdp_glbl-0.1.0/tests/test_addrspace.py` & `ucdp_glbl-0.2.0/tests/test_addrspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,25 +137,25 @@
 def test_addrspace():
     """Address Space."""
     addrspace = Addrspace(name="name")
     assert addrspace.name == "name"
     assert addrspace.words == u.Namespace([])
     assert addrspace.width == 32
     assert addrspace.depth == 1024
-    assert addrspace.size == u.Bytes("32 KB")
+    assert addrspace.size == u.Bytes("4 KB")
 
 
 def test_addrspace_custom():
     """Address Space."""
     addrspace = Addrspace(name="name", width=64, depth=128)
     assert addrspace.name == "name"
     assert addrspace.words == u.Namespace([])
     assert addrspace.width == 64
     assert addrspace.depth == 128
-    assert addrspace.size == u.Bytes("8 KB")
+    assert addrspace.size == u.Bytes("1 KB")
 
 
 def test_lock():
     """Lock Mechanism."""
     addrspace = Addrspace(name="name")
     words = []
     for widx in range(3):
```

### Comparing `ucdp_glbl-0.1.0/PKG-INFO` & `ucdp_glbl-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ucdp-glbl
-Version: 0.1.0
+Version: 0.2.0
 Summary: Unified Chip Design Platform - Global
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/nbiotcloud/ucdp-glbl
 Project-URL: Documentation, https://ucdp-glbl.readthedocs.io/en/latest/
 Project-URL: Bug tracker, https://github.com/nbiotcloud/ucdp-glbl/issues
 Requires-Python: <4.0,>=3.10.0
-Requires-Dist: ucdp>=0.3.0
+Requires-Dist: ucdp>=0.4.0
 Description-Content-Type: text/markdown
 
 [![PyPI Version](https://badge.fury.io/py/ucdp-glbl.svg)](https://badge.fury.io/py/ucdp-glbl)
 [![Python Build](https://github.com/nbiotcloud/ucdp-glbl/actions/workflows/main.yml/badge.svg)](https://github.com/nbiotcloud/ucdp-glbl/actions/workflows/main.yml)
 [![Documentation](https://readthedocs.org/projects/ucdp-glbl/badge/?version=latest)](https://ucdp-glbl.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/nbiotcloud/ucdp-glbl/badge.svg?branch=main)](https://coveralls.io/github/nbiotcloud/ucdp-glbl?branch=main)
 [![python-versions](https://img.shields.io/pypi/pyversions/ucdp-glbl.svg)](https://pypi.python.org/pypi/ucdp-glbl)
```

