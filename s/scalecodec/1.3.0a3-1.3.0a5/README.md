# Comparing `tmp/scalecodec-1.3.0a3.tar.gz` & `tmp/scalecodec-1.3.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalecodec-1.3.0a3.tar", last modified: Tue Nov 14 13:24:37 2023, max compression
+gzip compressed data, was "scalecodec-1.3.0a5.tar", last modified: Mon Nov 20 10:25:34 2023, max compression
```

## Comparing `scalecodec-1.3.0a3.tar` & `scalecodec-1.3.0a5.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 13:24:37.272842 scalecodec-1.3.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17008 2023-11-14 13:24:37.272842 scalecodec-1.3.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16186 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 13:24:37.264841 scalecodec-1.3.0a3/scalecodec/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36646 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 13:24:37.268841 scalecodec-1.3.0a3/scalecodec/type_registry/
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/acala.json
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/canvas.json
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/contracts-on-rococo.json
--rw-r--r--   0 runner    (1001) docker     (127)    67343 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/core.json
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/crust.json
--rw-r--r--   0 runner    (1001) docker     (127)    16189 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/karura.json
--rw-r--r--   0 runner    (1001) docker     (127)    11820 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/kusama.json
--rw-r--r--   0 runner    (1001) docker     (127)   208220 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/legacy.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/moonbase-alpha.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/moonbeam.json
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/moonriver.json
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/polkadot.json
--rw-r--r--   0 runner    (1001) docker     (127)    47596 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/polymesh-mainnet.json
--rw-r--r--   0 runner    (1001) docker     (127)    47596 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/polymesh-testnet.json
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/rococo.json
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/statemine.json
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/statemint.json
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/substrate-node-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/test.json
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/type_registry/westend.json
--rw-r--r--   0 runner    (1001) docker     (127)   105616 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 13:24:37.268841 scalecodec-1.3.0a3/scalecodec/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     7999 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/scalecodec/utils/ss58.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 13:24:37.264841 scalecodec-1.3.0a3/scalecodec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17008 2023-11-14 13:24:37.000000 scalecodec-1.3.0a3/scalecodec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-11-14 13:24:37.000000 scalecodec-1.3.0a3/scalecodec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 13:24:37.000000 scalecodec-1.3.0a3/scalecodec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-14 13:24:37.000000 scalecodec-1.3.0a3/scalecodec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-14 13:24:37.000000 scalecodec-1.3.0a3/scalecodec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 13:24:37.272842 scalecodec-1.3.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 13:24:37.272842 scalecodec-1.3.0a3/test/
--rw-r--r--   0 runner    (1001) docker     (127)    89166 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/test/test_extrinsic_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/test/test_runtime_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/test/test_runtime_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/test/test_scale_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    36470 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/test/test_scale_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/test/test_scalebytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9509 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/test/test_ss58.py
--rw-r--r--   0 runner    (1001) docker     (127)    17662 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/test/test_type_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)   179798 2023-11-14 13:23:21.000000 scalecodec-1.3.0a3/test/test_type_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 10:25:34.987971 scalecodec-1.3.0a5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17008 2023-11-20 10:25:34.987971 scalecodec-1.3.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16186 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 10:25:34.983971 scalecodec-1.3.0a5/scalecodec/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37878 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 10:25:34.987971 scalecodec-1.3.0a5/scalecodec/type_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/acala.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/canvas.json
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/contracts-on-rococo.json
+-rw-r--r--   0 runner    (1001) docker     (127)    70975 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/crust.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16189 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/karura.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11820 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/kusama.json
+-rw-r--r--   0 runner    (1001) docker     (127)   208220 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/legacy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/moonbase-alpha.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/moonbeam.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/moonriver.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/polkadot.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47596 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/polymesh-mainnet.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47596 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/polymesh-testnet.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/rococo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/statemine.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/statemint.json
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/substrate-node-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/test.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/type_registry/westend.json
+-rw-r--r--   0 runner    (1001) docker     (127)   108210 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 10:25:34.987971 scalecodec-1.3.0a5/scalecodec/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/scalecodec/utils/ss58.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 10:25:34.983971 scalecodec-1.3.0a5/scalecodec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17008 2023-11-20 10:25:34.000000 scalecodec-1.3.0a5/scalecodec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-11-20 10:25:34.000000 scalecodec-1.3.0a5/scalecodec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 10:25:34.000000 scalecodec-1.3.0a5/scalecodec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-20 10:25:34.000000 scalecodec-1.3.0a5/scalecodec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-20 10:25:34.000000 scalecodec-1.3.0a5/scalecodec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 10:25:34.987971 scalecodec-1.3.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 10:25:34.987971 scalecodec-1.3.0a5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    89166 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/test/test_extrinsic_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8394 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/test/test_runtime_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/test/test_scale_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36470 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/test/test_scale_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/test/test_scalebytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/test/test_ss58.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17662 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/test/test_type_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)   179798 2023-11-20 10:24:28.000000 scalecodec-1.3.0a5/test/test_type_registry.py
```

### Comparing `scalecodec-1.3.0a3/LICENSE` & `scalecodec-1.3.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/PKG-INFO` & `scalecodec-1.3.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalecodec
-Version: 1.3.0a3
+Version: 1.3.0a5
 Summary: Python SCALE Codec Library
 Home-page: https://github.com/polkascan/py-scale-codec
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 Keywords: scale codec polkascan polkadot substrate blockchain kusama
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scalecodec-1.3.0a3/README.md` & `scalecodec-1.3.0a5/README.md`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/__init__.py` & `scalecodec-1.3.0a5/scalecodec/__init__.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/base.py` & `scalecodec-1.3.0a5/scalecodec/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -528,50 +528,77 @@
 
         scale_info_types = metadata.portable_registry.value_object['types'].value_object
 
         self.update_from_scale_info_types(scale_info_types, prefix=prefix)
 
         # Process extrinsic type in metadata to register correct Address and ExtrinsicSignature types
         try:
-            # Retrieve Extrinsic using common namespace
-            extrinsic_type = self.get_decoder_class("sp_runtime::generic::unchecked_extrinsic::UncheckedExtrinsic")
 
-            # Try to fall back on extrinsic type in metadata
-            if extrinsic_type is None:
-                extrinsic_type_id = metadata[1][1]['extrinsic']['ty'].value
-                extrinsic_type = self.get_decoder_class(f"{prefix}::{extrinsic_type_id}")
+            if metadata.version >= 15:
 
-            if extrinsic_type is not None:
-                # Extract Address and Signature type and set in type registry
+                extrinsic_dict = metadata[1][1]['extrinsic'].value
 
-                types_dict = {}
+                address_type_string = f"{prefix}::{extrinsic_dict['address_type']}"
 
-                for param in extrinsic_type.scale_info_type.value['params']:
-                    if param['name'] == 'Address':
+                # Update type registry
+                types_dict = {
+                    "Address": address_type_string,
+                    "AccountId": address_type_string,
+                    "LookupSource": address_type_string,
+                    "ExtrinsicSignature": f"{prefix}::{extrinsic_dict['signature_type']}"
+                }
+
+                # Check if Address is MultiAddress
+                addres_type = self.get_decoder_class(address_type_string)
+
+                if addres_type is self.get_decoder_class('sp_runtime::multiaddress::MultiAddress'):
+                    for address_param in addres_type.scale_info_type.value['params']:
+                        if address_param['name'] == 'AccountId':
+                            # Set AccountId
+                            types_dict['AccountId'] = f'{prefix}::{address_param["type"]}'
 
-                        type_string = f'{prefix}::{param["type"]}'
+                self.update_type_registry_types(types_dict)
+            else:
 
-                        types_dict['Address'] = type_string
-                        types_dict['AccountId'] = type_string
-                        types_dict['LookupSource'] = type_string
+                # Retrieve Extrinsic using common namespace
+                extrinsic_type = self.get_decoder_class("sp_runtime::generic::unchecked_extrinsic::UncheckedExtrinsic")
 
-                        # Check if Address is MultiAddress
-                        addres_type = self.get_decoder_class(type_string)
+                # Try to fall back on extrinsic type in metadata
+                if extrinsic_type is None:
+                    extrinsic_type_id = metadata[1][1]['extrinsic']['ty'].value
+                    extrinsic_type = self.get_decoder_class(f"{prefix}::{extrinsic_type_id}")
 
-                        if addres_type is self.get_decoder_class('sp_runtime::multiaddress::MultiAddress'):
-                            for address_param in addres_type.scale_info_type.value['params']:
-                                if address_param['name'] == 'AccountId':
-                                    # Set AccountId
-                                    types_dict['AccountId'] = f'{prefix}::{address_param["type"]}'
+                if extrinsic_type is not None:
+                    # Extract Address and Signature type and set in type registry
 
-                    elif param['name'] == 'Signature':
-                        types_dict['ExtrinsicSignature'] = f'{prefix}::{param["type"]}'
+                    types_dict = {}
 
-                # Update type registry
-                self.update_type_registry_types(types_dict)
+                    for param in extrinsic_type.scale_info_type.value['params']:
+                        if param['name'] == 'Address':
+
+                            type_string = f'{prefix}::{param["type"]}'
+
+                            types_dict['Address'] = type_string
+                            types_dict['AccountId'] = type_string
+                            types_dict['LookupSource'] = type_string
+
+                            # Check if Address is MultiAddress
+                            addres_type = self.get_decoder_class(type_string)
+
+                            if addres_type is self.get_decoder_class('sp_runtime::multiaddress::MultiAddress'):
+                                for address_param in addres_type.scale_info_type.value['params']:
+                                    if address_param['name'] == 'AccountId':
+                                        # Set AccountId
+                                        types_dict['AccountId'] = f'{prefix}::{address_param["type"]}'
+
+                        elif param['name'] == 'Signature':
+                            types_dict['ExtrinsicSignature'] = f'{prefix}::{param["type"]}'
+
+                    # Update type registry
+                    self.update_type_registry_types(types_dict)
         except NotImplementedError:
             pass
 
     def add_contract_metadata_dict_to_type_registry(self, metadata_dict):
         # TODO
         prefix = f"ink::{metadata_dict['source']['hash']}"
         return self.update_from_scale_info_types(metadata_dict['types'], prefix=prefix)
```

### Comparing `scalecodec-1.3.0a3/scalecodec/exceptions.py` & `scalecodec-1.3.0a5/scalecodec/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/__init__.py` & `scalecodec-1.3.0a5/scalecodec/type_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/canvas.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/canvas.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/core.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/core.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9831668169070513%*

 * *Differences: {"'types'": "{'MetadataAll': {'type_mapping': {insert: [(15, ['V15', 'MetadataV15'])]}}, "*

 * *            "'MetadataV15': OrderedDict([('type', 'struct'), ('type_mapping', [['types', "*

 * *            "'PortableRegistry'], ['pallets', 'Vec<PalletMetadataV15>'], ['extrinsic', "*

 * *            "'ExtrinsicMetadataV15'], ['runtime_type', 'SiLookupTypeId'], ['apis', "*

 * *            "'Vec<RuntimeApiMetadataV15>'], ['outer_enums', 'OuterEnums15'], ['custom', "*

 * *            "'Vec<CustomMetadata15>']])]), 'PalletMetadataV15': Or […]*

```diff
@@ -1916,14 +1916,16 @@
                 ],
                 [
                     "events",
                     "Option<Vec<frame_system::eventrecord>>"
                 ]
             ]
         },
+        "CustomMetadata15": "BTreeMap<Text, CustomValueMetadata15>",
+        "CustomValueMetadata15": "Bytes",
         "DoubleMapTypeLatest": "DoubleMapTypeV13",
         "DoubleMapTypeV10": {
             "type": "struct",
             "type_mapping": [
                 [
                     "hasher",
                     "StorageHasherV10"
@@ -2072,14 +2074,43 @@
                 ],
                 [
                     "signed_extensions",
                     "Vec<SignedExtensionMetadataV14>"
                 ]
             ]
         },
+        "ExtrinsicMetadataV15": {
+            "type": "struct",
+            "type_mapping": [
+                [
+                    "version",
+                    "u8"
+                ],
+                [
+                    "address_type",
+                    "SiLookupTypeId"
+                ],
+                [
+                    "call_type",
+                    "SiLookupTypeId"
+                ],
+                [
+                    "signature_type",
+                    "SiLookupTypeId"
+                ],
+                [
+                    "extra_type",
+                    "SiLookupTypeId"
+                ],
+                [
+                    "signed_extensions",
+                    "Vec<SignedExtensionMetadataV14>"
+                ]
+            ]
+        },
         "ExtrinsicPayloadValue": {
             "type": "struct",
             "type_mapping": [
                 [
                     "call",
                     "CallBytes"
                 ],
@@ -2393,14 +2424,18 @@
                 [
                     "V13",
                     "MetadataV13"
                 ],
                 [
                     "V14",
                     "MetadataV14"
+                ],
+                [
+                    "V15",
+                    "MetadataV15"
                 ]
             ]
         },
         "MetadataLatest": "MetadataV13",
         "MetadataV0": "Null",
         "MetadataV1": "Null",
         "MetadataV10": {
@@ -2468,14 +2503,47 @@
                 ],
                 [
                     "runtime_type",
                     "SiLookupTypeId"
                 ]
             ]
         },
+        "MetadataV15": {
+            "type": "struct",
+            "type_mapping": [
+                [
+                    "types",
+                    "PortableRegistry"
+                ],
+                [
+                    "pallets",
+                    "Vec<PalletMetadataV15>"
+                ],
+                [
+                    "extrinsic",
+                    "ExtrinsicMetadataV15"
+                ],
+                [
+                    "runtime_type",
+                    "SiLookupTypeId"
+                ],
+                [
+                    "apis",
+                    "Vec<RuntimeApiMetadataV15>"
+                ],
+                [
+                    "outer_enums",
+                    "OuterEnums15"
+                ],
+                [
+                    "custom",
+                    "Vec<CustomMetadata15>"
+                ]
+            ]
+        },
         "MetadataV2": "Null",
         "MetadataV3": "Null",
         "MetadataV4": "Null",
         "MetadataV5": "Null",
         "MetadataV6": "Null",
         "MetadataV7": "Null",
         "MetadataV8": "Null",
@@ -2714,14 +2782,31 @@
                 ],
                 [
                     "value",
                     "Type"
                 ]
             ]
         },
+        "OuterEnums15": {
+            "type": "struct",
+            "type_mapping": [
+                [
+                    "call_type",
+                    "SiLookupTypeId"
+                ],
+                [
+                    "event_type",
+                    "SiLookupTypeId"
+                ],
+                [
+                    "error_type",
+                    "SiLookupTypeId"
+                ]
+            ]
+        },
         "PalletCallMetadataV14": {
             "base_class": "ScaleInfoCallMetadata",
             "type": "struct",
             "type_mapping": [
                 [
                     "ty",
                     "SiLookupTypeId"
@@ -2800,14 +2885,52 @@
                 ],
                 [
                     "index",
                     "u8"
                 ]
             ]
         },
+        "PalletMetadataV15": {
+            "base_class": "ScaleInfoPalletMetadata",
+            "type": "struct",
+            "type_mapping": [
+                [
+                    "name",
+                    "Text"
+                ],
+                [
+                    "storage",
+                    "Option<StorageMetadataV14>"
+                ],
+                [
+                    "calls",
+                    "Option<PalletCallMetadataV14>"
+                ],
+                [
+                    "event",
+                    "Option<PalletEventMetadataV14>"
+                ],
+                [
+                    "constants",
+                    "Vec<PalletConstantMetadataV14>"
+                ],
+                [
+                    "error",
+                    "Option<PalletErrorMetadataV14>"
+                ],
+                [
+                    "index",
+                    "u8"
+                ],
+                [
+                    "docs",
+                    "Vec<Text>"
+                ]
+            ]
+        },
         "PortableRegistry": {
             "type": "struct",
             "type_mapping": [
                 [
                     "types",
                     "Vec<PortableType>"
                 ]
@@ -2929,50 +3052,117 @@
                 ],
                 [
                     "docs",
                     "Vec<String>"
                 ]
             ]
         },
-        "RuntimeCallDefinition": {
-            "base_class": "GenericRuntimeCallDefinition",
+        "RuntimeApiMetadataV14": {
+            "base_class": "LegacyRuntimeApiMetadata",
             "type": "struct",
             "type_mapping": [
                 [
-                    "api",
-                    "String"
+                    "name",
+                    "Text"
                 ],
                 [
-                    "method",
-                    "String"
+                    "methods",
+                    "Vec<RuntimeApiMethodMetadataV14>"
+                ],
+                [
+                    "docs",
+                    "Vec<Text>"
+                ]
+            ]
+        },
+        "RuntimeApiMetadataV15": {
+            "base_class": "GenericRuntimeApiMetadata",
+            "type": "struct",
+            "type_mapping": [
+                [
+                    "name",
+                    "Text"
+                ],
+                [
+                    "methods",
+                    "Vec<RuntimeApiMethodMetadataV15>"
+                ],
+                [
+                    "docs",
+                    "Vec<Text>"
+                ]
+            ]
+        },
+        "RuntimeApiMethodMetadataV14": {
+            "base_class": "LegacyRuntimeApiMethodMetadata",
+            "type": "struct",
+            "type_mapping": [
+                [
+                    "name",
+                    "Text"
+                ],
+                [
+                    "inputs",
+                    "Vec<RuntimeApiMethodParamMetadataV14>"
                 ],
                 [
-                    "description",
+                    "output",
                     "String"
                 ],
                 [
-                    "params",
-                    "Vec<RuntimeCallDefinitionParam>"
+                    "docs",
+                    "Vec<Text>"
+                ]
+            ]
+        },
+        "RuntimeApiMethodMetadataV15": {
+            "base_class": "GenericRuntimeApiMethodMetadata",
+            "type": "struct",
+            "type_mapping": [
+                [
+                    "name",
+                    "Text"
+                ],
+                [
+                    "inputs",
+                    "Vec<RuntimeApiMethodParamMetadataV15>"
+                ],
+                [
+                    "output",
+                    "SiLookupTypeId"
+                ],
+                [
+                    "docs",
+                    "Vec<Text>"
+                ]
+            ]
+        },
+        "RuntimeApiMethodParamMetadataV14": {
+            "type": "struct",
+            "type_mapping": [
+                [
+                    "name",
+                    "Text"
                 ],
                 [
                     "type",
                     "String"
                 ]
             ]
         },
-        "RuntimeCallDefinitionParam": {
+        "RuntimeApiMethodParamMetadataV15": {
             "type": "struct",
             "type_mapping": [
                 [
                     "name",
-                    "String"
+                    "Text"
                 ],
                 [
                     "type",
-                    "String"
+                    "SiLookupTypeId"
                 ]
             ]
         },
         "SiLookupTypeId": "Compact<u32>",
         "Signature": "H512",
         "SignedExtensionMetadataV14": {
             "type": "struct",
```

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/crust.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/crust.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/karura.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/karura.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/kusama.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/kusama.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/legacy.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/legacy.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/moonriver.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/moonriver.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/polkadot.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/polkadot.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/polymesh-mainnet.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/polymesh-mainnet.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/polymesh-testnet.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/polymesh-testnet.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/rococo.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/rococo.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/substrate-node-template.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/substrate-node-template.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/test.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/test.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/type_registry/westend.json` & `scalecodec-1.3.0a5/scalecodec/type_registry/westend.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/types.py` & `scalecodec-1.3.0a5/scalecodec/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -2188,14 +2188,50 @@
                 if pallet.value['name'] == name:
                     return pallet
         else:
             for pallet in self[1]['modules']:
                 if pallet.value['name'] == name:
                     return pallet
 
+    def get_runtime_apis(self):
+        if self.index >= 15:
+            return self[1]['apis']
+        else:
+            return [self.get_runtime_api(name) for name in self.runtime_config.type_registry.get("runtime_api").keys()]
+
+    def get_runtime_api(self, name: str) -> Optional['GenericRuntimeApiMetadata']:
+
+        if self.index >= 15:
+            for runtime_api in self[1]['apis']:
+                if runtime_api.value['name'] == name:
+                    return runtime_api
+        else:
+            # Legacy: Runtime APIs not included in metadata
+            runtime_api_data = self.runtime_config.type_registry.get("runtime_api", {}).get(name)
+
+            if runtime_api_data:
+                runtime_api = self.runtime_config.create_scale_object("RuntimeApiMetadataV14")
+
+                # Transform data
+                data = {
+                    'name': name,
+                    'methods': [{
+                            'name': m_name, 'inputs': m_data['params'], 'output': m_data['type'],
+                            'docs': [m_data['description']]
+                    } for m_name, m_data in runtime_api_data['methods'].items()],
+                    'docs': []
+                }
+
+                runtime_api.encode(data)
+
+                # Add embedded types to type registry
+                self.runtime_config.update_type_registry_types(runtime_api_data.get("types", {}))
+
+                return runtime_api
+
     def process(self):
         value = super().process()
 
         metadata_obj = self.value_object[1]
 
         if self.index in (12, 13):
             for module in metadata_obj['modules']:
@@ -2268,14 +2304,18 @@
         else:
             return self.value_object[1].error_index.get(f'{module_index}-{error_index}')
 
     def get_metadata(self):
         return self.value_object[1]
 
     @property
+    def version(self) -> int:
+        return self.value_object[1].index
+
+    @property
     def portable_registry(self):
         return self.value_object[1].portable_registry
 
     @property
     def pallets(self):
         return self.value_object[1].pallets
 
@@ -2322,14 +2362,20 @@
                 for se in self.value_object[1][1]['extrinsic']['signed_extensions'].value:
                     if se not in extension_def:
                         extension_def[se] = {'extrinsic': None, 'additional_signed': None}
                     signed_extensions[se] = extension_def[se]
 
         return signed_extensions
 
+    def get_runtime_api(self, name: str):
+        return self.get_metadata().get_runtime_api(name)
+
+    def get_runtime_apis(self):
+        return self.get_metadata().get_runtime_apis()
+
 
 class GenericStringType(String):
     @property
     def name(self):
         return None
 
     @property
@@ -2751,32 +2797,62 @@
         for param_type_string in self.get_params_type_string():
             scale_type = self.runtime_config.create_scale_object(param_type_string)
             param_info.append(scale_type.generate_type_decomposition(max_recursion=max_recursion))
 
         return param_info
 
 
-class GenericRuntimeCallDefinition(Struct):
+class GenericRuntimeApiMetadata(Struct):
+
+    def get_methods(self):
+        return list(self.value_object['methods'])
+
+    def get_method(self, name: str) -> Optional['GenericRuntimeApiMethodMetadata']:
+        for method in self.value_object['methods']:
+            if name == method.value['name']:
+                return method
+
+
+class LegacyRuntimeApiMetadata(GenericRuntimeApiMetadata):
+    pass
+
+
+class GenericRuntimeApiMethodMetadata(Struct):
+
+    def get_params(self):
+        return [{'name': p['name'], 'type': f'scale_info::{p["type"]}'} for p in self.value['inputs']]
+
+    def get_return_type_string(self):
+        return f"scale_info::{self.value['output']}"
 
     def get_param_info(self, max_recursion: int = TYPE_DECOMP_MAX_RECURSIVE) -> list:
         """
         Return a type decomposition how to format parameters for current storage function
 
         Returns
         -------
         list
         """
         param_info = []
-        for param in self.value['params']:
+        for param in self.get_params():
             scale_type = self.runtime_config.create_scale_object(param['type'])
             param_info.append(scale_type.generate_type_decomposition(max_recursion=max_recursion))
 
         return param_info
 
 
+class LegacyRuntimeApiMethodMetadata(GenericRuntimeApiMethodMetadata):
+
+    def get_params(self):
+        return [{'name': p['name'], 'type': p["type"]} for p in self.value['inputs']]
+
+    def get_return_type_string(self):
+        return self.value['output']
+
+
 class GenericEventMetadata(Struct):
 
     @property
     def name(self):
         return self.value['name']
 
     @property
```

### Comparing `scalecodec-1.3.0a3/scalecodec/updater.py` & `scalecodec-1.3.0a5/scalecodec/updater.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/utils/__init__.py` & `scalecodec-1.3.0a5/scalecodec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/utils/math.py` & `scalecodec-1.3.0a5/scalecodec/utils/math.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec/utils/ss58.py` & `scalecodec-1.3.0a5/scalecodec/utils/ss58.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/scalecodec.egg-info/PKG-INFO` & `scalecodec-1.3.0a5/scalecodec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalecodec
-Version: 1.3.0a3
+Version: 1.3.0a5
 Summary: Python SCALE Codec Library
 Home-page: https://github.com/polkascan/py-scale-codec
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 Keywords: scale codec polkascan polkadot substrate blockchain kusama
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scalecodec-1.3.0a3/scalecodec.egg-info/SOURCES.txt` & `scalecodec-1.3.0a5/scalecodec.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 scalecodec/type_registry/test.json
 scalecodec/type_registry/westend.json
 scalecodec/utils/__init__.py
 scalecodec/utils/math.py
 scalecodec/utils/ss58.py
 test/test_extrinsic_payload.py
 test/test_metadata.py
-test/test_runtime_call.py
 test/test_runtime_configuration.py
 test/test_scale_info.py
 test/test_scale_types.py
 test/test_scalebytes.py
 test/test_ss58.py
 test/test_type_encoding.py
 test/test_type_registry.py
```

### Comparing `scalecodec-1.3.0a3/setup.py` & `scalecodec-1.3.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/test/test_extrinsic_payload.py` & `scalecodec-1.3.0a5/test/test_extrinsic_payload.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/test/test_metadata.py` & `scalecodec-1.3.0a5/test/test_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -108,14 +108,38 @@
         self.assertIsNotNone(metadata_obj.portable_registry)
 
         self.assertGreater(len(metadata_obj[1][1]['pallets']), 0)
         self.assertGreater(len(metadata_obj.value[1]['V14']['pallets']), 0)
 
         self.assertGreater(len(metadata_obj.get_signed_extensions().items()), 0)
 
+        # Test runtime api
+        self.assertGreater(len(metadata_obj.get_runtime_apis()), 0)
+        self.assertIsNotNone(metadata_obj.get_runtime_api('Core'))
+
+    def test_metadata_registry_decode_v15(self):
+        metadata_obj = self.runtime_config.create_scale_object(
+            "MetadataVersioned", data=ScaleBytes(self.metadata_fixture_dict['V15'])
+        )
+        metadata_obj.decode()
+        self.assertEqual(metadata_obj.value_object[1].index, 15)
+        self.assertIsNotNone(metadata_obj.portable_registry)
+
+        self.assertGreater(len(metadata_obj[1][1]['pallets']), 0)
+        self.assertGreater(len(metadata_obj.value[1]['V15']['pallets']), 0)
+
+        self.assertGreater(len(metadata_obj.get_signed_extensions().items()), 0)
+
+        # Test runtime api
+        self.assertGreater(len(metadata_obj.get_runtime_apis()), 0)
+        self.assertIsNotNone(metadata_obj.get_runtime_api('Core'))
+
+        self.assertIsNotNone(metadata_obj.get_runtime_api('AccountNonceApi').get_method('account_nonce'))
+
+
     # def test_pickle_test(self):
     #     metadata_obj = self.runtime_config.create_scale_object(
     #         "MetadataVersioned", data=ScaleBytes(self.metadata_fixture_dict['V14'])
     #     )
     #     metadata_obj.decode()
     #
     #     # for name, decoder_class in self.runtime_config.type_registry['types'].items():
```

### Comparing `scalecodec-1.3.0a3/test/test_runtime_configuration.py` & `scalecodec-1.3.0a5/test/test_runtime_configuration.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/test/test_scale_info.py` & `scalecodec-1.3.0a5/test/test_scale_info.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/test/test_scale_types.py` & `scalecodec-1.3.0a5/test/test_scale_types.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/test/test_scalebytes.py` & `scalecodec-1.3.0a5/test/test_scalebytes.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/test/test_ss58.py` & `scalecodec-1.3.0a5/test/test_ss58.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/test/test_type_encoding.py` & `scalecodec-1.3.0a5/test/test_type_encoding.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.3.0a3/test/test_type_registry.py` & `scalecodec-1.3.0a5/test/test_type_registry.py`

 * *Files identical despite different names*

