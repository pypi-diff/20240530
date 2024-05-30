# Comparing `tmp/atlantiscore-9.2.0.tar.gz` & `tmp/atlantiscore-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlantiscore-9.2.0.tar", last modified: Thu May 16 10:17:49 2024, max compression
+gzip compressed data, was "atlantiscore-9.3.0.tar", last modified: Thu May 30 11:45:31 2024, max compression
```

## Comparing `atlantiscore-9.2.0.tar` & `atlantiscore-9.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.721301 atlantiscore-9.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-16 10:17:49.721301 atlantiscore-9.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.705301 atlantiscore-9.2.0/atlantiscore/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.705301 atlantiscore-9.2.0/atlantiscore/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.709301 atlantiscore-9.2.0/atlantiscore/db/types/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/db/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.709301 atlantiscore-9.2.0/atlantiscore/db/types/evm/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/db/types/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/db/types/evm/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/db/types/evm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/db/types/evm/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.709301 atlantiscore-9.2.0/atlantiscore/hash/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/hash/ecdsa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.709301 atlantiscore-9.2.0/atlantiscore/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.713301 atlantiscore-9.2.0/atlantiscore/lib/abi/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/lib/abi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/lib/eth.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/lib/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.713301 atlantiscore-9.2.0/atlantiscore/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.713301 atlantiscore-9.2.0/atlantiscore/middleware/blockchain/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/middleware/blockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/middleware/blockchain/erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/middleware/blockchain/evm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.713301 atlantiscore-9.2.0/atlantiscore/types/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.717301 atlantiscore-9.2.0/atlantiscore/types/evm/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/types/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/types/evm/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/types/evm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/types/evm/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/atlantiscore/types/key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.717301 atlantiscore-9.2.0/atlantiscore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-16 10:17:49.000000 atlantiscore-9.2.0/atlantiscore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-16 10:17:49.000000 atlantiscore-9.2.0/atlantiscore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:17:49.000000 atlantiscore-9.2.0/atlantiscore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-16 10:17:49.000000 atlantiscore-9.2.0/atlantiscore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 10:17:49.000000 atlantiscore-9.2.0/atlantiscore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:17:49.721301 atlantiscore-9.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:17:49.717301 atlantiscore-9.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-16 10:16:51.000000 atlantiscore-9.2.0/tests/test_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.284572 atlantiscore-9.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 11:45:31.284572 atlantiscore-9.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.256572 atlantiscore-9.3.0/atlantiscore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.260572 atlantiscore-9.3.0/atlantiscore/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.260572 atlantiscore-9.3.0/atlantiscore/db/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/db/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.260572 atlantiscore-9.3.0/atlantiscore/db/types/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/db/types/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/db/types/evm/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/db/types/evm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/db/types/evm/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.264572 atlantiscore-9.3.0/atlantiscore/hash/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/hash/ecdsa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.264572 atlantiscore-9.3.0/atlantiscore/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.264572 atlantiscore-9.3.0/atlantiscore/lib/abi/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/lib/abi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/lib/eth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/lib/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.264572 atlantiscore-9.3.0/atlantiscore/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.276572 atlantiscore-9.3.0/atlantiscore/middleware/blockchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/middleware/blockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/middleware/blockchain/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/middleware/blockchain/evm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.280572 atlantiscore-9.3.0/atlantiscore/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.280572 atlantiscore-9.3.0/atlantiscore/types/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/types/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/types/evm/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/types/evm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/types/evm/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/atlantiscore/types/key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.280572 atlantiscore-9.3.0/atlantiscore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 11:45:31.000000 atlantiscore-9.3.0/atlantiscore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-30 11:45:31.000000 atlantiscore-9.3.0/atlantiscore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:45:31.000000 atlantiscore-9.3.0/atlantiscore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 11:45:31.000000 atlantiscore-9.3.0/atlantiscore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 11:45:31.000000 atlantiscore-9.3.0/atlantiscore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:45:31.284572 atlantiscore-9.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:45:31.280572 atlantiscore-9.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-30 11:44:19.000000 atlantiscore-9.3.0/tests/test_finder.py
```

### Comparing `atlantiscore-9.2.0/PKG-INFO` & `atlantiscore-9.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlantiscore
-Version: 9.2.0
+Version: 9.3.0
 Summary: atlantiscore
 Author-email: Atlantis Labs <r00tail@protonmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles~=23.2
 Requires-Dist: codercore~=6.0.1
 Requires-Dist: coincurve~=18.0
 Requires-Dist: eth-hash[pycryptodome]~=0.5
```

### Comparing `atlantiscore-9.2.0/atlantiscore/__init__.py` & `atlantiscore-9.3.0/atlantiscore/__init__.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore/db/types/evm/base.py` & `atlantiscore-9.3.0/atlantiscore/db/types/evm/base.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore/db/types/evm/transaction.py` & `atlantiscore-9.3.0/atlantiscore/db/types/evm/transaction.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore/hash/ecdsa.py` & `atlantiscore-9.3.0/atlantiscore/hash/ecdsa.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore/lib/eth.py` & `atlantiscore-9.3.0/atlantiscore/lib/eth.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore/lib/exceptions.py` & `atlantiscore-9.3.0/atlantiscore/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore/middleware/blockchain/erc20.py` & `atlantiscore-9.3.0/atlantiscore/middleware/blockchain/erc20.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore/middleware/blockchain/evm.py` & `atlantiscore-9.3.0/atlantiscore/middleware/blockchain/evm.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,17 @@
             private_key=self.private_key.to_hex(),
         )
         return self.eth.send_raw_transaction(signed_transaction.rawTransaction).hex()
 
     async def get_nonce(self) -> int:
         return self.eth.get_transaction_count(str(self.private_key.public_address))
 
+    async def get_balance(self) -> int:
+        return self.eth.get_balance(str(self.private_key.public_address))
+
 
 class EVMContractMiddleware(EVMMiddleware, metaclass=ABCMeta):
     address: EVMAddress
 
     def __init__(self, address: EVMAddress, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.address = address
```

### Comparing `atlantiscore-9.2.0/atlantiscore/types/evm/address.py` & `atlantiscore-9.3.0/atlantiscore/types/evm/address.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore/types/evm/base.py` & `atlantiscore-9.3.0/atlantiscore/types/evm/base.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore/types/evm/transaction.py` & `atlantiscore-9.3.0/atlantiscore/types/evm/transaction.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore/types/key.py` & `atlantiscore-9.3.0/atlantiscore/types/key.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/atlantiscore.egg-info/PKG-INFO` & `atlantiscore-9.3.0/atlantiscore.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlantiscore
-Version: 9.2.0
+Version: 9.3.0
 Summary: atlantiscore
 Author-email: Atlantis Labs <r00tail@protonmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles~=23.2
 Requires-Dist: codercore~=6.0.1
 Requires-Dist: coincurve~=18.0
 Requires-Dist: eth-hash[pycryptodome]~=0.5
```

### Comparing `atlantiscore-9.2.0/atlantiscore.egg-info/SOURCES.txt` & `atlantiscore-9.3.0/atlantiscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlantiscore-9.2.0/pyproject.toml` & `atlantiscore-9.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atlantiscore"
-version = "9.2.0"
+version = "9.3.0"
 description = "atlantiscore"
 readme = "README.md"
 authors = [{ name = "Atlantis Labs", email = "r00tail@protonmail.com" }]
 dependencies = [
     "aiofiles ~= 23.2",
     "codercore ~= 6.0.1",
     "coincurve ~= 18.0",
@@ -34,15 +34,15 @@
     "flake8 ~= 6.0",
     "isort ~= 5.12",
     "pre-commit ~= 2.21",
 ]
 
 
 [tool.bumpver]
-current_version = "9.2.0"
+current_version = "9.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `atlantiscore-9.2.0/tests/test_finder.py` & `atlantiscore-9.3.0/tests/test_finder.py`

 * *Files identical despite different names*

