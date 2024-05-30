# Comparing `tmp/llama_index_readers_gcs-0.1.6.tar.gz` & `tmp/llama_index_readers_gcs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_gcs-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_readers_gcs-0.1.7.tar", max compression
```

## Comparing `llama_index_readers_gcs-0.1.6.tar` & `llama_index_readers_gcs-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1535 2024-04-01 21:33:17.092190 llama_index_readers_gcs-0.1.6/README.md
--rw-r--r--   0        0        0       76 2024-04-01 21:33:17.092190 llama_index_readers_gcs-0.1.6/llama_index/readers/gcs/__init__.py
--rw-r--r--   0        0        0     4222 2024-04-01 21:33:17.092190 llama_index_readers_gcs-0.1.6/llama_index/readers/gcs/base.py
--rw-r--r--   0        0        0     1562 2024-04-01 21:33:17.092190 llama_index_readers_gcs-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 llama_index_readers_gcs-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1340 2024-05-30 03:13:06.001119 llama_index_readers_gcs-0.1.7/README.md
+-rw-r--r--   0        0        0       76 2024-05-30 03:13:06.001119 llama_index_readers_gcs-0.1.7/llama_index/readers/gcs/__init__.py
+-rw-r--r--   0        0        0     4582 2024-05-30 03:13:06.001119 llama_index_readers_gcs-0.1.7/llama_index/readers/gcs/base.py
+-rw-r--r--   0        0        0     1562 2024-05-30 03:13:06.001119 llama_index_readers_gcs-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 llama_index_readers_gcs-0.1.7/PKG-INFO
```

### Comparing `llama_index_readers_gcs-0.1.6/README.md` & `llama_index_readers_gcs-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     bucket="scrabble-dictionary",
     key="dictionary.txt",
     service_account_key_json="[SERVICE_ACCOUNT_KEY_JSON]",
 )
 documents = loader.load_data()
 ```
 
-This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
+This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/).
```

### Comparing `llama_index_readers_gcs-0.1.6/llama_index/readers/gcs/base.py` & `llama_index_readers_gcs-0.1.7/llama_index/readers/gcs/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     num_files_limit (Optional[int]): Maximum number of files to read.
         Default is None.
     file_metadata (Optional[Callable[str, Dict]]): A function that takes
         in a filename and returns a Dict of metadata for the Document.
         Default is None.
     service_account_key (Optional[Dict[str, str]]): provide GCP service account key directly.
     service_account_key_json (Optional[str]): provide GCP service account key as a JSON string.
+    service_account_key_path (Optional[str]): provide path to file containing GCP service account key.
     """
 
     is_remote: bool = True
 
     bucket: str
     key: Optional[str] = None
     prefix: Optional[str] = ""
@@ -56,31 +57,36 @@
     )
     required_exts: Optional[List[str]] = None
     filename_as_id: bool = True
     num_files_limit: Optional[int] = None
     file_metadata: Optional[Callable[[str], Dict]] = Field(default=None, exclude=True)
     service_account_key: Optional[Dict[str, str]] = None
     service_account_key_json: Optional[str] = None
+    service_account_key_path: Optional[str] = None
 
     @classmethod
     def class_name(cls) -> str:
         return "GCSReader"
 
     def load_gcs_files_as_docs(self) -> List[Document]:
         """Load file(s) from GCS."""
         from gcsfs import GCSFileSystem
 
         if self.service_account_key is not None:
             creds = service_account.Credentials.from_service_account_info(
                 self.service_account_key, scopes=SCOPES
             )
         elif self.service_account_key_json is not None:
-            creds = service_account.Credentials.from_service_account_file(
+            creds = service_account.Credentials.from_service_account_info(
                 json.loads(self.service_account_key_json), scopes=SCOPES
             )
+        elif self.service_account_key_path is not None:
+            creds = service_account.Credentials.from_service_account_file(
+                self.service_account_key_path, scopes=SCOPES
+            )
         else:
             # Use anonymous access if none are specified
             creds = "anon"
 
         gcsfs = GCSFileSystem(
             token=creds,
         )
```

### Comparing `llama_index_readers_gcs-0.1.6/pyproject.toml` & `llama_index_readers_gcs-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers gcs integration"
 exclude = ["**/BUILD"]
 keywords = ["bucket", "gcp", "gcs", "google cloud storage"]
 license = "MIT"
 maintainers = ["nfiacco"]
 name = "llama-index-readers-gcs"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-readers-file = "^0.1.11"
 gcsfs = "^2024.3.1"
```

### Comparing `llama_index_readers_gcs-0.1.6/PKG-INFO` & `llama_index_readers_gcs-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-gcs
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index readers gcs integration
 License: MIT
 Keywords: bucket,gcp,gcs,google cloud storage
 Author: Your Name
 Author-email: you@example.com
 Maintainer: nfiacco
 Requires-Python: >=3.8.1,<4.0
@@ -35,9 +35,9 @@
     bucket="scrabble-dictionary",
     key="dictionary.txt",
     service_account_key_json="[SERVICE_ACCOUNT_KEY_JSON]",
 )
 documents = loader.load_data()
 ```
 
-This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
+This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/).
```

