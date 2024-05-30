# Comparing `tmp/imspy_connector-0.2.8.tar.gz` & `tmp/imspy_connector-0.2.9.tar.gz`

## Comparing `imspy_connector-0.2.8.tar` & `imspy_connector-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0     1001      127      417 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/Cargo.toml
--rw-r--r--   0     1001      127        0 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/README.md
--rw-r--r--   0     1001      127      975 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/src/data/dataset.rs
--rw-r--r--   0     1001      127     2941 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/src/data/dda.rs
--rw-r--r--   0     1001      127      990 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/src/data/dia.rs
--rw-r--r--   0     1001      127    15764 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/src/data/handle.rs
--rw-r--r--   0     1001      127     8314 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/src/data/meta.rs
--rw-r--r--   0     1001      127       85 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/src/data/mod.rs
--rw-r--r--   0     1001      127     3720 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/src/data/raw.rs
--rw-r--r--   0     1001      127      141 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/src/lib.rs
--rw-r--r--   0     1001      127      449 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/rustdf/src/main.rs
--rw-r--r--   0     1001      127      275 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/mscore/Cargo.toml
--rw-r--r--   0     1001      127        0 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/mscore/README.md
--rw-r--r--   0     1001      127     2015 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/mscore/src/chemistry.rs
--rw-r--r--   0     1001      127      764 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/mscore/src/lib.rs
--rw-r--r--   0     1001      127       44 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/mscore/src/main.rs
--rw-r--r--   0     1001      127    23639 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/mscore/src/mz_spectrum.rs
--rw-r--r--   0     1001      127    16144 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/mscore/src/tims_frame.rs
--rw-r--r--   0     1001      127    13856 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/mscore/src/tims_slice.rs
--rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 imspy_connector-0.2.8/imspy_connector/Cargo.toml
--rw-r--r--   0     1001      127        0 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/imspy_connector/README.md
--rw-r--r--   0     1001      127     1082 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/imspy_connector/src/lib.rs
--rw-r--r--   0     1001      127     1196 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/imspy_connector/src/py_dataset.rs
--rw-r--r--   0     1001      127     2174 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/imspy_connector/src/py_dda.rs
--rw-r--r--   0     1001      127     1124 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/imspy_connector/src/py_dia.rs
--rw-r--r--   0     1001      127     7158 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/imspy_connector/src/py_mz_spectrum.rs
--rw-r--r--   0     1001      127     9354 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/imspy_connector/src/py_tims_frame.rs
--rw-r--r--   0     1001      127     8816 2023-11-24 18:04:18.000000 imspy_connector-0.2.8/imspy_connector/src/py_tims_slice.rs
--rw-r--r--   0     1001      127    23086 2023-11-24 18:04:30.000000 imspy_connector-0.2.8/imspy_connector/Cargo.lock
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 imspy_connector-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      380 1970-01-01 00:00:00.000000 imspy_connector-0.2.8/PKG-INFO
+-rw-r--r--   0     1001      127      275 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/mscore/Cargo.toml
+-rw-r--r--   0     1001      127        0 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/mscore/README.md
+-rw-r--r--   0     1001      127     2015 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/mscore/src/chemistry.rs
+-rw-r--r--   0     1001      127      764 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/mscore/src/lib.rs
+-rw-r--r--   0     1001      127       44 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/mscore/src/main.rs
+-rw-r--r--   0     1001      127    23639 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/mscore/src/mz_spectrum.rs
+-rw-r--r--   0     1001      127    16144 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/mscore/src/tims_frame.rs
+-rw-r--r--   0     1001      127    13856 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/mscore/src/tims_slice.rs
+-rw-r--r--   0     1001      127      417 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/Cargo.toml
+-rw-r--r--   0     1001      127        0 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/README.md
+-rw-r--r--   0     1001      127      975 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/src/data/dataset.rs
+-rw-r--r--   0     1001      127     2941 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/src/data/dda.rs
+-rw-r--r--   0     1001      127      990 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/src/data/dia.rs
+-rw-r--r--   0     1001      127    15764 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/src/data/handle.rs
+-rw-r--r--   0     1001      127     8314 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/src/data/meta.rs
+-rw-r--r--   0     1001      127       85 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/src/data/mod.rs
+-rw-r--r--   0     1001      127     3720 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/src/data/raw.rs
+-rw-r--r--   0     1001      127      141 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/src/lib.rs
+-rw-r--r--   0     1001      127      449 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/rustdf/src/main.rs
+-rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 imspy_connector-0.2.9/imspy_connector/Cargo.toml
+-rw-r--r--   0     1001      127        0 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/imspy_connector/README.md
+-rw-r--r--   0     1001      127     1082 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/imspy_connector/src/lib.rs
+-rw-r--r--   0     1001      127     1196 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/imspy_connector/src/py_dataset.rs
+-rw-r--r--   0     1001      127     2174 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/imspy_connector/src/py_dda.rs
+-rw-r--r--   0     1001      127     1124 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/imspy_connector/src/py_dia.rs
+-rw-r--r--   0     1001      127     7158 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/imspy_connector/src/py_mz_spectrum.rs
+-rw-r--r--   0     1001      127     9354 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/imspy_connector/src/py_tims_frame.rs
+-rw-r--r--   0     1001      127     8816 2023-11-24 18:34:59.000000 imspy_connector-0.2.9/imspy_connector/src/py_tims_slice.rs
+-rw-r--r--   0     1001      127    23086 2023-11-24 18:35:11.000000 imspy_connector-0.2.9/imspy_connector/Cargo.lock
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 imspy_connector-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      380 1970-01-01 00:00:00.000000 imspy_connector-0.2.9/PKG-INFO
```

### Comparing `imspy_connector-0.2.8/rustdf/src/data/dataset.rs` & `imspy_connector-0.2.9/rustdf/src/data/dataset.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/rustdf/src/data/dda.rs` & `imspy_connector-0.2.9/rustdf/src/data/dda.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/rustdf/src/data/dia.rs` & `imspy_connector-0.2.9/rustdf/src/data/dia.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/rustdf/src/data/handle.rs` & `imspy_connector-0.2.9/rustdf/src/data/handle.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/rustdf/src/data/meta.rs` & `imspy_connector-0.2.9/rustdf/src/data/meta.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/rustdf/src/data/raw.rs` & `imspy_connector-0.2.9/rustdf/src/data/raw.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/mscore/src/chemistry.rs` & `imspy_connector-0.2.9/mscore/src/chemistry.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/mscore/src/lib.rs` & `imspy_connector-0.2.9/mscore/src/lib.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/mscore/src/mz_spectrum.rs` & `imspy_connector-0.2.9/mscore/src/mz_spectrum.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/mscore/src/tims_frame.rs` & `imspy_connector-0.2.9/mscore/src/tims_frame.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/mscore/src/tims_slice.rs` & `imspy_connector-0.2.9/mscore/src/tims_slice.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/imspy_connector/src/lib.rs` & `imspy_connector-0.2.9/imspy_connector/src/lib.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/imspy_connector/src/py_dataset.rs` & `imspy_connector-0.2.9/imspy_connector/src/py_dataset.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/imspy_connector/src/py_dda.rs` & `imspy_connector-0.2.9/imspy_connector/src/py_dda.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/imspy_connector/src/py_dia.rs` & `imspy_connector-0.2.9/imspy_connector/src/py_dia.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/imspy_connector/src/py_mz_spectrum.rs` & `imspy_connector-0.2.9/imspy_connector/src/py_mz_spectrum.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/imspy_connector/src/py_tims_frame.rs` & `imspy_connector-0.2.9/imspy_connector/src/py_tims_frame.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/imspy_connector/src/py_tims_slice.rs` & `imspy_connector-0.2.9/imspy_connector/src/py_tims_slice.rs`

 * *Files identical despite different names*

### Comparing `imspy_connector-0.2.8/imspy_connector/Cargo.lock` & `imspy_connector-0.2.9/imspy_connector/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 name = "hermit-abi"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
 
 [[package]]
 name = "imspy-connector"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "mscore",
  "numpy",
  "pyo3",
  "rustdf",
 ]
```

