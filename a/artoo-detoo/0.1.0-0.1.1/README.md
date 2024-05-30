# Comparing `tmp/artoo_detoo-0.1.0.tar.gz` & `tmp/artoo_detoo-0.1.1.tar.gz`

## Comparing `artoo_detoo-0.1.0.tar` & `artoo_detoo-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 artoo_detoo-0.1.0/Cargo.toml
--rw-rw-r--   0     1000     1000      695 2024-05-30 20:29:12.000000 artoo_detoo-0.1.0/.gitignore
--rw-rw-r--   0     1000     1000    31474 2024-05-30 20:41:26.000000 artoo_detoo-0.1.0/Cargo.lock
--rw-rw-r--   0     1000     1000      120 2024-05-30 20:38:14.000000 artoo_detoo-0.1.0/README.md
--rw-rw-r--   0     1000     1000       73 2024-05-30 19:59:33.000000 artoo_detoo-0.1.0/r2.example
--rw-rw-r--   0     1000     1000      106 2024-05-30 19:06:27.000000 artoo_detoo-0.1.0/rustfmt.toml
--rw-rw-r--   0     1000     1000     2812 2024-05-30 20:04:20.000000 artoo_detoo-0.1.0/src/main.rs
--rw-rw-r--   0     1000     1000      588 2024-05-30 20:40:33.000000 artoo_detoo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 artoo_detoo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 artoo_detoo-0.1.1/Cargo.toml
+-rw-rw-r--   0     1000     1000      695 2024-05-30 20:29:12.000000 artoo_detoo-0.1.1/.gitignore
+-rw-rw-r--   0     1000     1000      120 2024-05-30 20:38:14.000000 artoo_detoo-0.1.1/README.md
+-rw-rw-r--   0     1000     1000       73 2024-05-30 19:59:33.000000 artoo_detoo-0.1.1/r2.example
+-rw-rw-r--   0     1000     1000      403 2024-05-30 21:19:19.000000 artoo_detoo-0.1.1/r2_d2/__init__.py
+-rw-rw-r--   0     1000     1000      106 2024-05-30 19:06:27.000000 artoo_detoo-0.1.1/rustfmt.toml
+-rw-rw-r--   0     1000     1000     3251 2024-05-30 21:26:09.000000 artoo_detoo-0.1.1/src/lib.rs
+-rw-rw-r--   0     1000     1000    35543 2024-05-30 21:27:30.000000 artoo_detoo-0.1.1/Cargo.lock
+-rw-rw-r--   0     1000     1000      649 2024-05-30 21:20:00.000000 artoo_detoo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 artoo_detoo-0.1.1/PKG-INFO
```

### Comparing `artoo_detoo-0.1.0/Cargo.toml` & `artoo_detoo-0.1.1/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 [package]
 name = "r2-d2"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 readme = "README.md"
 description = "Simple Client for Cloudflare R2 to manage Restic Backups"
 categories = ["development-tools", "command-line-interface", "command-line-utilities"]
 keywords = ["Python", "s3", "r2", "pip", "packaging"]
 repository = "https://github.com/robinvandernoord/uvx2"
 license = "MIT"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
+[lib]
+name = "r2_d2"
+crate-type = ["cdylib"]
+
 [dependencies]
-reqwest = { version = "0.11", features = ["json"] }
+pyo3 = { version = "0.20", features = ["abi3-py38", "extension-module"] }
+pyo3-asyncio = { version = "0.20", features = ["tokio-runtime"] }
 tokio = { version = "1.37", features = ["full"] }
+reqwest = { version = "0.11", features = ["json"] }
+
 dotenvy = "0.15"
 
+
 [lints.clippy]
 # categories:
 pedantic = { level = "warn", priority = -1 }
 nursery = { level = "warn", priority = -1 }
 cargo = { level = "warn", priority = -1 }
 # specific ones:
 module_name_repetitions = "allow"
```

### Comparing `artoo_detoo-0.1.0/.gitignore` & `artoo_detoo-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `artoo_detoo-0.1.0/Cargo.lock` & `artoo_detoo-0.1.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -160,29 +160,73 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
+name = "futures"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
+dependencies = [
+ "futures-channel",
+ "futures-core",
+ "futures-executor",
+ "futures-io",
+ "futures-sink",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
 name = "futures-channel"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
+ "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
+name = "futures-executor"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
+dependencies = [
+ "futures-core",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
+name = "futures-io"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
+
+[[package]]
+name = "futures-macro"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
@@ -192,18 +236,24 @@
 
 [[package]]
 name = "futures-util"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
+ "futures-channel",
  "futures-core",
+ "futures-io",
+ "futures-macro",
+ "futures-sink",
  "futures-task",
+ "memchr",
  "pin-project-lite",
  "pin-utils",
+ "slab",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "40ecd4077b5ae9fd2e9e169b102c6c330d0605168eb0e8bf79952b256dbefffd"
@@ -230,14 +280,20 @@
 [[package]]
 name = "hashbrown"
 version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "hermit-abi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "http"
@@ -327,14 +383,20 @@
 checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
+name = "indoc"
+version = "2.0.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
+
+[[package]]
 name = "ipnet"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
 name = "itoa"
@@ -382,14 +444,23 @@
 [[package]]
 name = "memchr"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
+name = "memoffset"
+version = "0.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "miniz_oxide"
@@ -541,36 +612,120 @@
 [[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "pyo3"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+dependencies = [
+ "cfg-if",
+ "indoc",
+ "libc",
+ "memoffset",
+ "parking_lot",
+ "portable-atomic",
+ "pyo3-build-config",
+ "pyo3-ffi",
+ "pyo3-macros",
+ "unindent",
+]
+
+[[package]]
+name = "pyo3-asyncio"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6ea6b68e93db3622f3bb3bf363246cf948ed5375afe7abff98ccbdd50b184995"
+dependencies = [
+ "futures",
+ "once_cell",
+ "pin-project-lite",
+ "pyo3",
+ "tokio",
+]
+
+[[package]]
+name = "pyo3-build-config"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+dependencies = [
+ "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
+name = "pyo3-ffi"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+dependencies = [
+ "libc",
+ "pyo3-build-config",
+]
+
+[[package]]
+name = "pyo3-macros"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+dependencies = [
+ "proc-macro2",
+ "pyo3-macros-backend",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "pyo3-macros-backend"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "pyo3-build-config",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "r2-d2"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "dotenvy",
+ "pyo3",
+ "pyo3-asyncio",
  "reqwest",
  "tokio",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.5.1"
@@ -804,14 +959,20 @@
 checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
+name = "target-lexicon"
+version = "0.12.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
+
+[[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
@@ -936,14 +1097,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
+name = "unindent"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
+
+[[package]]
 name = "url"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
```

### Comparing `artoo_detoo-0.1.0/src/main.rs` & `artoo_detoo-0.1.1/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use std::collections::BTreeMap;
 use std::path::Path;
-use std::process::exit;
 
 use dotenvy::from_path_iter;
+use pyo3::prelude as pyo;
 use reqwest::Client;
 use reqwest::header::HeaderMap;
 
 struct R2D2Config {
     account_id: String,
     apikey: String,
     bucket: String,
@@ -62,26 +62,27 @@
         let (key, value) = item.ok()?;
         config.insert(key, value);
     }
 
     Some(config)
 }
 
-async fn _main() -> Result<i32, String> {
+
+async fn async_main_rs() -> Result<i32, String> {
     let r2d2 = R2D2Config::from_dot_r2()?;
     let client = Client::new();
     let url = format!("{}/usage?=null", r2d2.base_url());
     let mut request = client.get(url);
     if let Some(headers) = r2d2.headers() {
         request = request.headers(headers);
     }
 
     match request.send().await {
         Ok(resp) => {
-            println!("{}", resp.status().as_u16());
+            println!("{}", resp.status());
             match resp.text().await {
                 Ok(text) => {
                     println!("{text}");
                     Ok(0)
                 }
                 Err(e) => Err(
                     format!("Error reading response text: {e}")
@@ -90,19 +91,31 @@
         }
         Err(e) => Err(
             format!("Request error: {e}")
         ),
     }
 }
 
-#[tokio::main]
-async fn main() {
-    match _main().await {
-        Ok(code) => {
-            exit(code)
-        }
-        Err(msg) => {
-            eprintln!("{msg}");
-            exit(1)
-        }
-    }
+#[pyo::pyfunction]
+/// # Errors
+/// should be handled gracefully?
+pub fn main_rs(py: pyo::Python<'_>) -> pyo::PyResult<&pyo::PyAny> {
+    pyo3_asyncio::tokio::future_into_py(py, async {
+        let exit_code = match async_main_rs().await {
+            Ok(code) => {code}
+            Err(msg) => {
+                eprintln!("{msg}");
+                1
+            }
+        };
+
+        Ok(pyo::Python::with_gil(|_| exit_code))
+    })
+}
+
+#[pyo::pymodule]
+/// # Errors
+/// should be handled gracefully?
+pub fn r2_d2(_py: pyo::Python, m: &pyo::PyModule) -> pyo::PyResult<()> {
+    m.add_function(pyo::wrap_pyfunction!(main_rs, m)?)?;
+    Ok(())
 }
```

### Comparing `artoo_detoo-0.1.0/pyproject.toml` & `artoo_detoo-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 readme = "README.md"
 license = "MIT"
 keywords = []
 authors = [
     { name = "Robin van der Noord", email = "robinvandernoord@gmail.com" },
 ]
 
-
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = ["version"]
 
+
 [tool.maturin]
-bindings = "bin"
+features = ["pyo3/extension-module"]
+
+[project.scripts]
+r2-d2 = "r2_d2:main"
+
```

### Comparing `artoo_detoo-0.1.0/PKG-INFO` & `artoo_detoo-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: artoo-detoo
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Simple Client for Cloudflare R2 to manage Restic Backups
 Keywords: 
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License: MIT
```

