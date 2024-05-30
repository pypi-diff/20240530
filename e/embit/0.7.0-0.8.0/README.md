# Comparing `tmp/embit-0.7.0.tar.gz` & `tmp/embit-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embit-0.7.0.tar", last modified: Mon Jan  2 22:19:11 2023, max compression
+gzip compressed data, was "embit-0.8.0.tar", last modified: Thu May 30 10:52:26 2024, max compression
```

## Comparing `embit-0.7.0.tar` & `embit-0.8.0.tar`

### file list

```diff
@@ -1,71 +1,76 @@
-drwxrwxr-x   0 ss        (1000) ss        (1000)        0 2023-01-02 22:19:11.342165 embit-0.7.0/
--rw-rw-r--   0 ss        (1000) ss        (1000)      491 2023-01-02 22:19:11.342165 embit-0.7.0/PKG-INFO
--rw-rw-r--   0 ss        (1000) ss        (1000)     2595 2022-11-09 14:10:44.000000 embit-0.7.0/README.md
--rw-rw-r--   0 ss        (1000) ss        (1000)       79 2023-01-02 22:19:11.342165 embit-0.7.0/setup.cfg
--rw-rw-r--   0 ss        (1000) ss        (1000)      726 2023-01-02 22:14:40.000000 embit-0.7.0/setup.py
-drwxrwxr-x   0 ss        (1000) ss        (1000)        0 2023-01-02 22:19:11.330165 embit-0.7.0/src/
-drwxrwxr-x   0 ss        (1000) ss        (1000)        0 2023-01-02 22:19:11.334165 embit-0.7.0/src/embit/
--rw-rw-r--   0 ss        (1000) ss        (1000)        0 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/__init__.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     3164 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/base.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     1910 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/base58.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     5099 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/bech32.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     9942 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/bip32.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     4200 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/bip39.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     1562 2023-01-02 22:13:52.000000 embit-0.7.0/src/embit/bip85.py
--rw-rw-r--   0 ss        (1000) ss        (1000)      918 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/compact.py
-drwxrwxr-x   0 ss        (1000) ss        (1000)        0 2023-01-02 22:19:11.338165 embit-0.7.0/src/embit/descriptor/
--rw-rw-r--   0 ss        (1000) ss        (1000)       87 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/descriptor/__init__.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    14448 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/descriptor/arguments.py
--rw-rw-r--   0 ss        (1000) ss        (1000)      900 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/descriptor/base.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     1194 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/descriptor/checksum.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    10412 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/descriptor/descriptor.py
--rw-rw-r--   0 ss        (1000) ss        (1000)      218 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/descriptor/errors.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    25350 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/descriptor/miniscript.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     7553 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/ec.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     2306 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/finalizer.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     1164 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/hashes.py
-drwxrwxr-x   0 ss        (1000) ss        (1000)        0 2023-01-02 22:19:11.338165 embit-0.7.0/src/embit/liquid/
--rw-rw-r--   0 ss        (1000) ss        (1000)        0 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/__init__.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     3126 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/addresses.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     4522 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/blech32.py
--rw-rw-r--   0 ss        (1000) ss        (1000)      480 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/blip32.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     8265 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/descriptor.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     1954 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/finalizer.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     2234 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/networks.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    24508 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/pset.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     8575 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/psetview.py
--rw-rw-r--   0 ss        (1000) ss        (1000)      450 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/slip77.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    17113 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/liquid/transaction.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     2357 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/networks.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    36258 2022-11-16 10:53:15.000000 embit-0.7.0/src/embit/psbt.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    28747 2022-11-16 12:11:09.000000 embit-0.7.0/src/embit/psbtview.py
--rw-rw-r--   0 ss        (1000) ss        (1000)     6564 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/script.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    14573 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/slip39.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    13652 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/transaction.py
-drwxrwxr-x   0 ss        (1000) ss        (1000)        0 2023-01-02 22:19:11.338165 embit-0.7.0/src/embit/util/
--rw-rw-r--   0 ss        (1000) ss        (1000)       96 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/__init__.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    34192 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/ctypes_secp256k1.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    18967 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/key.py
-drwxrwxr-x   0 ss        (1000) ss        (1000)        0 2023-01-02 22:19:11.342165 embit-0.7.0/src/embit/util/prebuilt/
--rwxrwxr-x   0 ss        (1000) ss        (1000)   194236 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_darwin_arm64.dylib
--rw-rw-r--   0 ss        (1000) ss        (1000)   307184 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_darwin_x86_64.dylib
--rw-rw-r--   0 ss        (1000) ss        (1000)   156376 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_linux_aarch64.so
--rw-rw-r--   0 ss        (1000) ss        (1000)   175208 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_linux_armv6l.so
--rw-rw-r--   0 ss        (1000) ss        (1000)   175208 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_linux_armv7l.so
--rw-rw-r--   0 ss        (1000) ss        (1000)   237992 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_linux_x86_64.so
--rw-rw-r--   0 ss        (1000) ss        (1000)   212992 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_windows_amd64.dll
--rw-rw-r--   0 ss        (1000) ss        (1000)     3960 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/py_ripemd160.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    13041 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/py_secp256k1.py
--rw-rw-r--   0 ss        (1000) ss        (1000)      288 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/util/secp256k1.py
-drwxrwxr-x   0 ss        (1000) ss        (1000)        0 2023-01-02 22:19:11.342165 embit-0.7.0/src/embit/wordlists/
--rw-rw-r--   0 ss        (1000) ss        (1000)        0 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/wordlists/__init__.py
--rw-rw-r--   0 ss        (1000) ss        (1000)      835 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/wordlists/base.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    27466 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/wordlists/bip39.py
--rw-rw-r--   0 ss        (1000) ss        (1000)    14418 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/wordlists/slip39.py
--rw-rw-r--   0 ss        (1000) ss        (1000)      124 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/wordlists/ubip39.py
--rw-rw-r--   0 ss        (1000) ss        (1000)      129 2022-11-09 14:10:44.000000 embit-0.7.0/src/embit/wordlists/uslip39.py
-drwxrwxr-x   0 ss        (1000) ss        (1000)        0 2023-01-02 22:19:11.334165 embit-0.7.0/src/embit.egg-info/
--rw-rw-r--   0 ss        (1000) ss        (1000)      491 2023-01-02 22:19:11.000000 embit-0.7.0/src/embit.egg-info/PKG-INFO
--rw-rw-r--   0 ss        (1000) ss        (1000)     1786 2023-01-02 22:19:11.000000 embit-0.7.0/src/embit.egg-info/SOURCES.txt
--rw-rw-r--   0 ss        (1000) ss        (1000)        1 2023-01-02 22:19:11.000000 embit-0.7.0/src/embit.egg-info/dependency_links.txt
--rw-rw-r--   0 ss        (1000) ss        (1000)        6 2023-01-02 22:19:11.000000 embit-0.7.0/src/embit.egg-info/top_level.txt
+drwxr-xr-x   0 ss        (1000) ss        (1000)        0 2024-05-30 10:52:26.423573 embit-0.8.0/
+-rw-r--r--   0 ss        (1000) ss        (1000)     1072 2024-05-30 10:34:44.000000 embit-0.8.0/LICENSE
+-rw-r--r--   0 ss        (1000) ss        (1000)     3172 2024-05-30 10:52:26.423573 embit-0.8.0/PKG-INFO
+-rw-r--r--   0 ss        (1000) ss        (1000)     2739 2024-05-30 10:34:44.000000 embit-0.8.0/README.md
+-rw-r--r--   0 ss        (1000) ss        (1000)     1325 2024-05-30 10:41:53.000000 embit-0.8.0/pyproject.toml
+-rw-r--r--   0 ss        (1000) ss        (1000)       38 2024-05-30 10:52:26.423573 embit-0.8.0/setup.cfg
+-rw-r--r--   0 ss        (1000) ss        (1000)       63 2024-05-30 10:34:44.000000 embit-0.8.0/setup.py
+drwxr-xr-x   0 ss        (1000) ss        (1000)        0 2024-05-30 10:52:26.419573 embit-0.8.0/src/
+drwxr-xr-x   0 ss        (1000) ss        (1000)        0 2024-05-30 10:52:26.423573 embit-0.8.0/src/embit/
+-rw-r--r--   0 ss        (1000) ss        (1000)        0 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/__init__.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     3472 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/base.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     1978 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/base58.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     5165 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/bech32.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    10157 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/bip32.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     4107 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/bip39.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     1662 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/bip85.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     1135 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/compact.py
+drwxr-xr-x   0 ss        (1000) ss        (1000)        0 2024-05-30 10:52:26.423573 embit-0.8.0/src/embit/descriptor/
+-rw-r--r--   0 ss        (1000) ss        (1000)       87 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/descriptor/__init__.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    16040 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/descriptor/arguments.py
+-rw-r--r--   0 ss        (1000) ss        (1000)      606 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/descriptor/base.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     1424 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/descriptor/checksum.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    12182 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/descriptor/descriptor.py
+-rw-r--r--   0 ss        (1000) ss        (1000)      218 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/descriptor/errors.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    26839 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/descriptor/miniscript.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     4775 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/descriptor/taptree.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     8233 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/ec.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     3339 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/finalizer.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     1222 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/hashes.py
+drwxr-xr-x   0 ss        (1000) ss        (1000)        0 2024-05-30 10:52:26.423573 embit-0.8.0/src/embit/liquid/
+-rw-r--r--   0 ss        (1000) ss        (1000)        0 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/__init__.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     3182 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/addresses.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     4555 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/blech32.py
+-rw-r--r--   0 ss        (1000) ss        (1000)      481 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/blip32.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     8775 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/descriptor.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     2009 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/finalizer.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     2145 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/networks.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    25579 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/pset.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     9065 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/psetview.py
+-rw-r--r--   0 ss        (1000) ss        (1000)      453 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/slip77.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    18054 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/liquid/transaction.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     1763 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/misc.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     2256 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/networks.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    39234 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/psbt.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    32805 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/psbtview.py
+-rw-r--r--   0 ss        (1000) ss        (1000)     6354 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/script.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    13751 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/slip39.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    14415 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/transaction.py
+drwxr-xr-x   0 ss        (1000) ss        (1000)        0 2024-05-30 10:52:26.423573 embit-0.8.0/src/embit/util/
+-rw-r--r--   0 ss        (1000) ss        (1000)       96 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/__init__.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    36766 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/ctypes_secp256k1.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    19186 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/key.py
+drwxr-xr-x   0 ss        (1000) ss        (1000)        0 2024-05-30 10:52:26.423573 embit-0.8.0/src/embit/util/prebuilt/
+-rwxr-xr-x   0 ss        (1000) ss        (1000)   194236 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_darwin_arm64.dylib
+-rw-r--r--   0 ss        (1000) ss        (1000)   307184 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_darwin_x86_64.dylib
+-rw-r--r--   0 ss        (1000) ss        (1000)   156376 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_linux_aarch64.so
+-rw-r--r--   0 ss        (1000) ss        (1000)   175208 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_linux_armv6l.so
+-rw-r--r--   0 ss        (1000) ss        (1000)   175208 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_linux_armv7l.so
+-rw-r--r--   0 ss        (1000) ss        (1000)   237992 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_linux_x86_64.so
+-rw-r--r--   0 ss        (1000) ss        (1000)   212992 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_windows_amd64.dll
+-rw-r--r--   0 ss        (1000) ss        (1000)     5367 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/py_ripemd160.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    13051 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/py_secp256k1.py
+-rw-r--r--   0 ss        (1000) ss        (1000)      288 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/util/secp256k1.py
+drwxr-xr-x   0 ss        (1000) ss        (1000)        0 2024-05-30 10:52:26.423573 embit-0.8.0/src/embit/wordlists/
+-rw-r--r--   0 ss        (1000) ss        (1000)        0 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/wordlists/__init__.py
+-rw-r--r--   0 ss        (1000) ss        (1000)      897 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/wordlists/base.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    27467 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/wordlists/bip39.py
+-rw-r--r--   0 ss        (1000) ss        (1000)    14418 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/wordlists/slip39.py
+-rw-r--r--   0 ss        (1000) ss        (1000)      124 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/wordlists/ubip39.py
+-rw-r--r--   0 ss        (1000) ss        (1000)      129 2024-05-30 10:34:44.000000 embit-0.8.0/src/embit/wordlists/uslip39.py
+drwxr-xr-x   0 ss        (1000) ss        (1000)        0 2024-05-30 10:52:26.423573 embit-0.8.0/src/embit.egg-info/
+-rw-r--r--   0 ss        (1000) ss        (1000)     3172 2024-05-30 10:52:26.000000 embit-0.8.0/src/embit.egg-info/PKG-INFO
+-rw-r--r--   0 ss        (1000) ss        (1000)     1881 2024-05-30 10:52:26.000000 embit-0.8.0/src/embit.egg-info/SOURCES.txt
+-rw-r--r--   0 ss        (1000) ss        (1000)        1 2024-05-30 10:52:26.000000 embit-0.8.0/src/embit.egg-info/dependency_links.txt
+-rw-r--r--   0 ss        (1000) ss        (1000)      100 2024-05-30 10:52:26.000000 embit-0.8.0/src/embit.egg-info/requires.txt
+-rw-r--r--   0 ss        (1000) ss        (1000)        6 2024-05-30 10:52:26.000000 embit-0.8.0/src/embit.egg-info/top_level.txt
```

### Comparing `embit-0.7.0/README.md` & `embit-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -63,14 +63,33 @@
 mnemonic_is_valid(mnemonic, wordlist=spanish_wordlist)
 mnemonic_to_seed(mnemonic, wordlist=spanish_wordlist)
 mnemonic_to_bytes(mnemonic, wordlist=spanish_wordlist)
 mnemonic_from_bytes(bytes_data, wordlist=spanish_wordlist)
 ```
 
 
-# Run the tests
-Clone the repo and complete the development mode `pip3` installation step above.
+# Development
 
+Install in developer mode with dev dependencies:
+
+```sh
+pip install -e .[dev]
+```
+
+Install pre-commit hook:
+
+```sh
+pre-commit install
+```
+
+Run tests with desktop python:
+
+```sh
+pytest
 ```
+
+Run tests with micropython:
+
+```sh
 cd tests
-python3 run_tests.py
-```
+micropython ./run_tests.py
+```
```

### Comparing `embit-0.7.0/src/embit/base.py` & `embit-0.8.0/src/embit/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,93 +5,105 @@
 
 class EmbitError(Exception):
     """Generic Embit error"""
 
     pass
 
 
-def copy(a:bytes) -> bytes:
-    """Ugly copy that works everywhere incl micropython"""
-    if len(a) == 0:
-        return b""
-    return a[:1] + a[1:]
-
 class EmbitBase:
     @classmethod
     def read_from(cls, stream, *args, **kwargs):
         """All classes should be readable from stream"""
         raise NotImplementedError(
-            "%s doesn't implement reading from stream" % type(cls).__name__
+            "%s doesn't implement reading from stream" % cls.__name__
         )
 
     @classmethod
-    def parse(cls, s, *args, **kwargs):
-        """Parses a string or a byte sequence"""
-        if isinstance(s, str):
-            s = s.encode()
+    def parse(cls, s: bytes, *args, **kwargs):
+        """Parse raw bytes"""
         stream = BytesIO(s)
         res = cls.read_from(stream, *args, **kwargs)
         if len(stream.read(1)) > 0:
             raise EmbitError("Unexpected extra bytes")
         return res
 
-    def write_to(self, stream, *args, **kwargs):
+    def write_to(self, stream, *args, **kwargs) -> int:
         """All classes should be writable to stream"""
         raise NotImplementedError(
             "%s doesn't implement writing to stream" % type(self).__name__
         )
 
-    def serialize(self, *args, **kwargs):
+    def serialize(self, *args, **kwargs) -> bytes:
+        """Serialize instance to raw bytes"""
         stream = BytesIO()
         self.write_to(stream, *args, **kwargs)
         return stream.getvalue()
 
-    def to_string(self, *args, **kwargs):
-        """Default string representation is hex of serialized instance or base58 if available"""
+    def to_string(self, *args, **kwargs) -> str:
+        """
+        String representation.
+        If not implemented - uses hex or calls to_base58() method if defined.
+        """
         if hasattr(self, "to_base58"):
-            return self.to_base58(*args, **kwargs)
+            res = self.to_base58(*args, **kwargs)
+            if not isinstance(res, str):
+                raise ValueError("to_base58() must return string")
+            return res
         return hexlify(self.serialize(*args, **kwargs)).decode()
 
     @classmethod
     def from_string(cls, s, *args, **kwargs):
-        """Default string representation is hex of serialized instance or base58 if availabe"""
+        """Create class instance from string"""
         if hasattr(cls, "from_base58"):
             return cls.from_base58(s, *args, **kwargs)
         return cls.parse(unhexlify(s))
 
     def __str__(self):
-        """to_string() can accept kwargs with defaults so str() should work"""
+        """Internally calls `to_string()` method with no arguments"""
         return self.to_string()
 
     def __repr__(self):
         try:
             return type(self).__name__ + "(%s)" % str(self)
         except:
             return type(self).__name__ + "()"
 
     def __eq__(self, other):
+        """Compare two objects by checking their serializations"""
+        if not hasattr(other, "serialize"):
+            return False
         return self.serialize() == other.serialize()
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __hash__(self):
         return hash(self.serialize())
 
 
 class EmbitKey(EmbitBase):
-    def sec(self):
-        """Any EmbitKey should implement sec() method that returns sec-serialized public key"""
+    def sec(self) -> bytes:
+        """
+        Any EmbitKey should implement sec() method that returns
+        a sec-serialized public key
+        """
         raise NotImplementedError(
             "%s doesn't implement sec() method" % type(self).__name__
         )
 
+    def xonly(self) -> bytes:
+        """xonly representation of the key"""
+        return self.sec()[1:33]
+
     @property
     def is_private(self) -> bool:
-        """Any EmbitKey should implement is_private property"""
+        """
+        Any EmbitKey should implement `is_private` property to distinguish
+        between private and public keys.
+        """
         raise NotImplementedError(
             "%s doesn't implement is_private property" % type(self).__name__
         )
 
     def __lt__(self, other):
         # for lexagraphic ordering
         return self.sec() < other.sec()
```

### Comparing `embit-0.7.0/src/embit/base58.py` & `embit-0.8.0/src/embit/base58.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 
 import binascii
 from . import hashes
 
 B58_DIGITS = "123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz"
 
 
-def encode(b):
+def encode(b: bytes) -> str:
     """Encode bytes to a base58-encoded string"""
 
     # Convert big-endian bytes to integer
     n = int("0x0" + binascii.hexlify(b).decode("utf8"), 16)
 
     # Divide that integer into bas58
-    res = []
+    chars = []
     while n > 0:
         n, r = divmod(n, 58)
-        res.append(B58_DIGITS[r])
-    res = "".join(res[::-1])
+        chars.append(B58_DIGITS[r])
+    result = "".join(chars[::-1])
 
     pad = 0
     for c in b:
         if c == 0:
             pad += 1
         else:
             break
-    return B58_DIGITS[0] * pad + res
+    return B58_DIGITS[0] * pad + result
 
 
-def decode(s):
+def decode(s: str) -> bytes:
     """Decode a base58-encoding string, returning bytes"""
     if not s:
         return b""
 
     # Convert the string to an integer
     n = 0
     for c in s:
@@ -57,20 +57,20 @@
         if c == B58_DIGITS[0]:
             pad += 1
         else:
             break
     return b"\x00" * pad + res
 
 
-def encode_check(b):
+def encode_check(b: bytes) -> str:
     """Encode bytes to a base58-encoded string with a checksum"""
     return encode(b + hashes.double_sha256(b)[0:4])
 
 
-def decode_check(s):
+def decode_check(s: str) -> bytes:
     """Decode a base58-encoding string with checksum check.
     Returns bytes without checksum
     """
     b = decode(s)
     checksum = hashes.double_sha256(b[:-4])[:4]
     if b[-4:] != checksum:
         raise ValueError(
```

### Comparing `embit-0.7.0/src/embit/bech32.py` & `embit-0.8.0/src/embit/bech32.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,79 +15,84 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 """Reference implementation for Bech32 and segwit addresses."""
+from .misc import const
 
 CHARSET = "qpzry9x8gf2tvdw0s3jn54khce6mua7l"
-BECH32_CONST = 1
-BECH32M_CONST = 0x2bc830a3
+BECH32_CONST = const(1)
+BECH32M_CONST = const(0x2BC830A3)
+
 
 class Encoding:
     """Enumeration type to list the various supported encodings."""
+
     BECH32 = 1
     BECH32M = 2
 
 
 def bech32_polymod(values):
     """Internal function that computes the Bech32 checksum."""
-    generator = [0x3b6a57b2, 0x26508e6d, 0x1ea119fa, 0x3d4233dd, 0x2a1462b3]
+    generator = [0x3B6A57B2, 0x26508E6D, 0x1EA119FA, 0x3D4233DD, 0x2A1462B3]
     chk = 1
     for value in values:
         top = chk >> 25
-        chk = (chk & 0x1ffffff) << 5 ^ value
+        chk = (chk & 0x1FFFFFF) << 5 ^ value
         for i in range(5):
             chk ^= generator[i] if ((top >> i) & 1) else 0
     return chk
 
 
-def bech32_hrp_expand(hrp):
+def bech32_hrp_expand(hrp: str):
     """Expand the HRP into values for checksum computation."""
     return [ord(x) >> 5 for x in hrp] + [0] + [ord(x) & 31 for x in hrp]
 
 
 def bech32_verify_checksum(hrp, data):
     """Verify a checksum given HRP and converted data characters."""
     check = bech32_polymod(bech32_hrp_expand(hrp) + data)
     if check == BECH32_CONST:
         return Encoding.BECH32
     elif check == BECH32M_CONST:
         return Encoding.BECH32M
     else:
         return None
 
+
 def bech32_create_checksum(encoding, hrp, data):
     """Compute the checksum values given HRP and data."""
     values = bech32_hrp_expand(hrp) + data
     const = BECH32M_CONST if encoding == Encoding.BECH32M else BECH32_CONST
     polymod = bech32_polymod(values + [0, 0, 0, 0, 0, 0]) ^ const
     return [(polymod >> 5 * (5 - i)) & 31 for i in range(6)]
 
 
 def bech32_encode(encoding, hrp, data):
     """Compute a Bech32 or Bech32m string given HRP and data values."""
     combined = data + bech32_create_checksum(encoding, hrp, data)
-    return hrp + '1' + ''.join([CHARSET[d] for d in combined])
+    return hrp + "1" + "".join([CHARSET[d] for d in combined])
 
 
 def bech32_decode(bech):
     """Validate a Bech32/Bech32m string, and determine HRP and data."""
-    if ((any(ord(x) < 33 or ord(x) > 126 for x in bech)) or
-            (bech.lower() != bech and bech.upper() != bech)):
+    if (any(ord(x) < 33 or ord(x) > 126 for x in bech)) or (
+        bech.lower() != bech and bech.upper() != bech
+    ):
         return (None, None, None)
     bech = bech.lower()
-    pos = bech.rfind('1')
+    pos = bech.rfind("1")
     if pos < 1 or pos + 7 > len(bech) or len(bech) > 90:
         return (None, None, None)
-    if not all(x in CHARSET for x in bech[pos+1:]):
+    if not all(x in CHARSET for x in bech[pos + 1 :]):
         return (None, None, None)
     hrp = bech[:pos]
-    data = [CHARSET.find(x) for x in bech[pos+1:]]
+    data = [CHARSET.find(x) for x in bech[pos + 1 :]]
     encoding = bech32_verify_checksum(hrp, data)
     if encoding is None:
         return (None, None, None)
     return (encoding, hrp, data[:-6])
 
 
 def convertbits(data, frombits, tobits, pad=True):
@@ -121,15 +126,17 @@
     decoded = convertbits(data[1:], 5, 8, False)
     if decoded is None or len(decoded) < 2 or len(decoded) > 40:
         return (None, None)
     if data[0] > 16:
         return (None, None)
     if data[0] == 0 and len(decoded) != 20 and len(decoded) != 32:
         return (None, None)
-    if (data[0] == 0 and encoding != Encoding.BECH32) or (data[0] != 0 and encoding != Encoding.BECH32M):
+    if (data[0] == 0 and encoding != Encoding.BECH32) or (
+        data[0] != 0 and encoding != Encoding.BECH32M
+    ):
         return (None, None)
     return (data[0], decoded)
 
 
 def encode(hrp, witver, witprog):
     """Encode a segwit address."""
     encoding = Encoding.BECH32 if witver == 0 else Encoding.BECH32M
```

### Comparing `embit-0.7.0/src/embit/bip32.py` & `embit-0.8.0/src/embit/bip32.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-import sys
-
-if sys.implementation.name == "micropython":
-    import secp256k1
-else:
-    from .util import secp256k1
-import hashlib
 from . import ec
-from .base import EmbitKey, EmbitError, copy
+from .base import EmbitKey, EmbitError
+from .misc import copy, const, secp256k1
 from .networks import NETWORKS
 from . import base58
 from . import hashes
 import hmac
 from binascii import hexlify
-import io
+
+HARDENED_INDEX = const(0x80000000)
+
 
 class HDError(EmbitError):
     pass
 
 
 class HDKey(EmbitKey):
-    """ HD Private or Public key """
+    """HD Private or Public key"""
 
     def __init__(
         self,
-        key,
+        key: EmbitKey,  # more specifically, PrivateKey or PublicKey
         chain_code: bytes,
         version=None,
         depth: int = 0,
         fingerprint: bytes = b"\x00\x00\x00\x00",
         child_number: int = 0,
     ):
         self.key = key
@@ -39,45 +35,45 @@
             if len(key.serialize()) == 32:
                 self.version = NETWORKS["main"]["xprv"]
             else:
                 self.version = NETWORKS["main"]["xpub"]
         self.chain_code = chain_code
         self.depth = depth
         self.fingerprint = fingerprint
-        self._my_fingerprint = None
+        self._my_fingerprint = b""
         self.child_number = child_number
         # check that base58[1:4] is "prv" or "pub"
         if self.is_private and self.to_base58()[1:4] != "prv":
             raise HDError("Invalid version")
         if not self.is_private and self.to_base58()[1:4] != "pub":
             raise HDError("Invalid version")
 
     @classmethod
     def from_seed(cls, seed: bytes, version=NETWORKS["main"]["xprv"]):
         """Creates a root private key from 64-byte seed"""
-        raw = hmac.new(b"Bitcoin seed", seed, digestmod='sha512').digest()
+        raw = hmac.new(b"Bitcoin seed", seed, digestmod="sha512").digest()
         private_key = ec.PrivateKey(raw[:32])
         chain_code = raw[32:]
         return cls(private_key, chain_code, version=version)
 
     @classmethod
     def from_base58(cls, s: str):
         b = base58.decode_check(s)
         return cls.parse(b)
 
     @property
-    def my_fingerprint(self):
-        if self._my_fingerprint is None:
+    def my_fingerprint(self) -> bytes:
+        if not self._my_fingerprint:
             sec = self.sec()
             self._my_fingerprint = hashes.hash160(sec)[:4]
         return self._my_fingerprint
 
     @property
     def is_private(self) -> bool:
-        """ checks if the HDKey is private or public """
+        """checks if the HDKey is private or public"""
         return self.key.is_private
 
     @property
     def secret(self):
         if not self.is_private:
             raise HDError("Key is not private")
         return self.key.secret
@@ -133,14 +129,18 @@
             depth=depth,
             fingerprint=fingerprint,
             child_number=child_number,
         )
         subver = hd.to_base58()[1:4]
         if subver != "prv" and subver != "pub":
             raise HDError("Invalid version")
+        if depth == 0 and child_number != 0:
+            raise HDError("zero depth with non-zero index")
+        if depth == 0 and fingerprint != b"\x00\x00\x00\x00":
+            raise HDError("zero depth with non-zero parent")
         return hd
 
     def to_public(self, version=None):
         if not self.is_private:
             raise HDError("Already public")
         if version is None:
             # detect network
@@ -181,29 +181,29 @@
             child_number=self.child_number,
         )
 
     def child(self, index: int, hardened: bool = False):
         """Derives a child HDKey"""
         if index > 0xFFFFFFFF:
             raise HDError("Index should be less then 2^32")
-        if hardened and index < 0x80000000:
-            index += 0x80000000
-        if index >= 0x80000000:
+        if hardened and index < HARDENED_INDEX:
+            index += HARDENED_INDEX
+        if index >= HARDENED_INDEX:
             hardened = True
         if hardened and not self.is_private:
             raise HDError("Can't do hardened with public key")
 
         # we need pubkey for fingerprint anyways
         sec = self.sec()
         fingerprint = hashes.hash160(sec)[:4]
         if hardened:
             data = b"\x00" + self.key.serialize() + index.to_bytes(4, "big")
         else:
             data = sec + index.to_bytes(4, "big")
-        raw = hmac.new(self.chain_code, data, digestmod='sha512').digest()
+        raw = hmac.new(self.chain_code, data, digestmod="sha512").digest()
         secret = raw[:32]
         chain_code = raw[32:]
         if self.is_private:
             secret = secp256k1.ec_privkey_add(secret, self.key.serialize())
             key = ec.PrivateKey(secret)
         else:
             # copy of internal secp256k1 point structure
@@ -216,15 +216,15 @@
             version=self.version,
             depth=self.depth + 1,
             fingerprint=fingerprint,
             child_number=index,
         )
 
     def derive(self, path):
-        """ path: int array or a string starting with m/ """
+        """path: int array or a string starting with m/"""
         if isinstance(path, str):
             # string of the form m/44h/0'/ind
             path = parse_path(path)
         child = self
         for idx in path:
             child = child.child(idx)
         return child
@@ -263,48 +263,47 @@
     net = network
     if network is None:
         net = NETWORKS["main"]
     if isinstance(path, str):
         path = parse_path(path)
     if len(path) == 0:
         return network[key]
-    if path[0] == 0x80000000 + 84:
+    if path[0] == HARDENED_INDEX + 84:
         key = "z" + default[1:]
-    elif path[0] == 0x80000000 + 49:
+    elif path[0] == HARDENED_INDEX + 49:
         key = "y" + default[1:]
-    elif path[0] == 0x80000000 + 48:
+    elif path[0] == HARDENED_INDEX + 48:
         if len(path) >= 4:
-            if path[3] == 0x80000000 + 1:
+            if path[3] == HARDENED_INDEX + 1:
                 key = "Y" + default[1:]
-            elif path[3] == 0x80000000 + 2:
+            elif path[3] == HARDENED_INDEX + 2:
                 key = "Z" + default[1:]
-    if network is None and len(path) > 1 and path[1] == 0x80000000 + 1:
+    if network is None and len(path) > 1 and path[1] == HARDENED_INDEX + 1:
         net = NETWORKS["test"]
     return net[key]
 
 
+def _parse_der_item(e: str) -> int:
+    if e[-1] in {"h", "H", "'"}:
+        return int(e[:-1]) + HARDENED_INDEX
+    else:
+        return int(e)
+
+
 def parse_path(path: str) -> list:
     """converts derivation path of the form m/44h/1'/0'/0/32 to int array"""
-    arr = path.split("/")
+    arr = path.rstrip("/").split("/")
     if arr[0] == "m":
         arr = arr[1:]
     if len(arr) == 0:
         return []
-    if arr[-1] == "":
-        # trailing slash
-        arr = arr[:-1]
-    for i, e in enumerate(arr):
-        if e[-1] == "h" or e[-1] == "'":
-            arr[i] = int(e[:-1]) + 0x80000000
-        else:
-            arr[i] = int(e)
-    return arr
+    return [_parse_der_item(e) for e in arr]
 
 
 def path_to_str(path: list, fingerprint=None) -> str:
     s = "m" if fingerprint is None else hexlify(fingerprint).decode()
     for el in path:
-        if el >= 0x80000000:
-            s += "/%dh" % (el - 0x80000000)
+        if el >= HARDENED_INDEX:
+            s += "/%dh" % (el - HARDENED_INDEX)
         else:
             s += "/%d" % el
     return s
```

### Comparing `embit-0.7.0/src/embit/bip39.py` & `embit-0.8.0/src/embit/bip39.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 # Mnemonic convertion to seed and to/from bytes
-import sys
 import hashlib
-
-if sys.implementation.name == "micropython":
-    from micropython import const
-else:
-    from .util import const
+from .misc import const
 
 from .wordlists.bip39 import WORDLIST
 
 PBKDF2_ROUNDS = const(2048)
 
 
-def mnemonic_to_bytes(mnemonic: str, ignore_checksum=False, wordlist=WORDLIST):
+def mnemonic_to_bytes(mnemonic: str, ignore_checksum: bool = False, wordlist=WORDLIST):
     # this function is copied from Jimmy Song's HDPrivateKey.from_mnemonic() method
 
     words = mnemonic.strip().split()
     if len(words) % 3 != 0 or len(words) < 12:
         raise ValueError("Invalid recovery phrase")
 
     binary_seed = bytearray()
```

### Comparing `embit-0.7.0/src/embit/bip85.py` & `embit-0.8.0/src/embit/bip85.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 from . import bip32, bip39, ec
+from .bip32 import HARDENED_INDEX
 import hmac
 
 BIP85_MAGIC = b"bip-entropy-from-k"
-H = 0x80000000
+
 
 class LANGUAGES:
     """
     Tuples: (bip85 derivation index, wordlist).
     """
+
     ENGLISH = (0, bip39.WORDLIST)
 
+
 def derive_entropy(root, app_index, path):
     """
     Derive app-specific bip85 entropy using path m/83696968'/app_index'/...path'
     """
-    assert max(path) < H
-    derivation = [ H+83696968 ,H+app_index ] + [ p+H for p in path ]
+    assert max(path) < HARDENED_INDEX
+    derivation = [HARDENED_INDEX + 83696968, HARDENED_INDEX + app_index] + [
+        p + HARDENED_INDEX for p in path
+    ]
     derived = root.derive(derivation)
-    return hmac.new(BIP85_MAGIC, derived.secret, digestmod='sha512').digest()
+    return hmac.new(BIP85_MAGIC, derived.secret, digestmod="sha512").digest()
+
 
 def derive_mnemonic(root, num_words=12, index=0, language=LANGUAGES.ENGLISH):
     """Derive a new mnemonic with num_words using language (code, wordlist)"""
     assert num_words in [12, 18, 24]
     langcode, wordlist = language
     path = [langcode, num_words, index]
     entropy = derive_entropy(root, 39, path)
-    entropy_part = entropy[:num_words*4//3]
+    entropy_part = entropy[: num_words * 4 // 3]
     return bip39.mnemonic_from_bytes(entropy_part, wordlist=wordlist)
 
+
 def derive_wif(root, index=0):
     """Derive ec.PrivateKey"""
     entropy = derive_entropy(root, 2, [index])
     return ec.PrivateKey(entropy[:32])
 
+
 def derive_xprv(root, index=0):
     """Derive bip32.HDKey"""
     entropy = derive_entropy(root, 32, [index])
-    return bip32.HDKey(ec.PrivateKey(entropy[32:]),entropy[:32])
+    return bip32.HDKey(ec.PrivateKey(entropy[32:]), entropy[:32])
+
 
 def derive_hex(root, num_bytes=32, index=0):
     """Derive raw entropy from 16 to 64 bytes long"""
     assert num_bytes <= 64
     assert num_bytes >= 16
     entropy = derive_entropy(root, 128169, [num_bytes, index])
     return entropy[:num_bytes]
```

### Comparing `embit-0.7.0/src/embit/compact.py` & `embit-0.8.0/src/embit/compact.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 """ Compact Int parsing / serialization """
 import io
 
 
-def to_bytes(i: int):
+def to_bytes(i: int) -> bytes:
     """encodes an integer as a compact int"""
     if i < 0:
         raise ValueError("integer can't be negative: {}".format(i))
     order = 0
-    while i >> (8 * (2 ** order)):
+    while i >> (8 * (2**order)):
         order += 1
     if order == 0:
         if i < 0xFD:
             return bytes([i])
         order = 1
     if order > 3:
         raise ValueError("integer too large: {}".format(i))
-    return bytes([0xFC + order]) + i.to_bytes(2 ** order, "little")
+    return bytes([0xFC + order]) + i.to_bytes(2**order, "little")
 
 
-def from_bytes(b: bytes):
+def from_bytes(b: bytes) -> int:
     s = io.BytesIO(b)
     res = read_from(s)
     if len(s.read(1)) > 0:
         raise ValueError("Too many bytes")
     return res
 
 
-def read_from(stream):
+def read_from(stream) -> int:
     """reads a compact integer from a stream"""
-    i = stream.read(1)[0]
+    c = stream.read(1)
+    if not isinstance(c, bytes):
+        raise TypeError("Bytes must be returned from stream.read()")
+    if len(c) != 1:
+        raise RuntimeError("Can't read one byte from the stream")
+    i = c[0]
     if i >= 0xFD:
         bytes_to_read = 2 ** (i - 0xFC)
         return int.from_bytes(stream.read(bytes_to_read), "little")
     else:
         return i
```

### Comparing `embit-0.7.0/src/embit/descriptor/arguments.py` & `embit-0.8.0/src/embit/descriptor/arguments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from binascii import hexlify, unhexlify
-from .base import DescriptorBase, read_until
+from .base import DescriptorBase
 from .errors import ArgumentError
 from .. import bip32, ec, compact, hashes
+from ..bip32 import HARDENED_INDEX
+from ..misc import read_until
 
 
 class KeyOrigin:
     def __init__(self, fingerprint: bytes, derivation: list):
         self.fingerprint = fingerprint
         self.derivation = derivation
 
@@ -20,30 +22,36 @@
         return cls(mfp, derivation)
 
     def __str__(self):
         return bip32.path_to_str(self.derivation, fingerprint=self.fingerprint)
 
 
 class AllowedDerivation(DescriptorBase):
-    # xpub/{0,1}/* - {0,1} is a set of allowed branches, wildcard * is stored as None
+    # xpub/<0;1>/* - <0;1> is a set of allowed branches, wildcard * is stored as None
     def __init__(self, indexes=[[0, 1], None]):
-        # check only one wildcard and only one set is in the derivation
-        if len([i for i in indexes if i is None]) > 1:
+        # check only one wildcard
+        if (
+            len(
+                [i for i in indexes if i is None or (isinstance(i, list) and None in i)]
+            )
+            > 1
+        ):
             raise ArgumentError("Only one wildcard is allowed")
+        # check only one set is in the derivation
         if len([i for i in indexes if isinstance(i, list)]) > 1:
-            raise ArgumentError("Only one wildcard is allowed")
+            raise ArgumentError("Only one set of branches is allowed")
         self.indexes = indexes
 
     @property
     def is_wildcard(self):
         return None in self.indexes
 
     def fill(self, idx, branch_index=None):
         # None is ok
-        if idx is not None and (idx < 0 or idx >= 0x80000000):
+        if idx is not None and (idx < 0 or idx >= HARDENED_INDEX):
             raise ArgumentError("Hardened indexes are not allowed in wildcard")
         arr = [i for i in self.indexes]
         for i, el in enumerate(arr):
             if el is None:
                 arr[i] = idx
             if isinstance(el, list):
                 if branch_index is None:
@@ -92,17 +100,20 @@
             if isinstance(el, list):
                 return el
         return None
 
     @property
     def has_hardend(self):
         for idx in self.indexes:
-            if isinstance(idx, int) and idx >= 0x80000000:
+            if isinstance(idx, int) and idx >= HARDENED_INDEX:
                 return True
-            if isinstance(idx, list) and len([i for i in idx if i >= 0x80000000]) > 0:
+            if (
+                isinstance(idx, list)
+                and len([i for i in idx if i >= HARDENED_INDEX]) > 0
+            ):
                 return True
         return False
 
     @classmethod
     def from_string(cls, der: str, allow_hardened=False, allow_set=True):
         if len(der) == 0:
             return None
@@ -112,66 +123,84 @@
         return cls(indexes)
 
     @classmethod
     def parse_element(cls, d: str, allow_hardened=False, allow_set=True):
         # wildcard
         if d == "*":
             return None
-        # branch set
+        # branch set - legacy `{m,n}`
         if d[0] == "{" and d[-1] == "}":
             if not allow_set:
                 raise ArgumentError("Set is not allowed in derivation %s" % d)
             return [
                 cls.parse_element(dd, allow_hardened, allow_set=False)
                 for dd in d[1:-1].split(",")
             ]
+        # branch set - multipart `<m;n>`
+        if d[0] == "<" and d[-1] == ">":
+            if not allow_set:
+                raise ArgumentError("Set is not allowed in derivation %s" % d)
+            return [
+                cls.parse_element(dd, allow_hardened, allow_set=False)
+                for dd in d[1:-1].split(";")
+            ]
         idx = 0
-        if d[-1] == "h":
+        if d[-1] in ["h", "H", "'"]:
             if not allow_hardened:
                 raise ArgumentError("Hardened derivation is not allowed in %s" % d)
-            idx = 0x80000000
+            idx = HARDENED_INDEX
             d = d[:-1]
         i = int(d)
-        if i < 0 or i >= 0x80000000:
-            raise ArgumentError("Derivation index can be in a range [0, 0x80000000)")
+        if i < 0 or i >= HARDENED_INDEX:
+            raise ArgumentError(
+                "Derivation index can be in a range [0, %d)" % HARDENED_INDEX
+            )
         return idx + i
 
     def __str__(self):
         r = ""
         for idx in self.indexes:
             if idx is None:
                 r += "/*"
             if isinstance(idx, int):
-                if idx >= 0x80000000:
-                    r += "/%dh" % (idx - 0x80000000)
+                if idx >= HARDENED_INDEX:
+                    r += "/%dh" % (idx - HARDENED_INDEX)
                 else:
                     r += "/%d" % idx
             if isinstance(idx, list):
-                r += "/{"
-                r += ",".join(
+                r += "/<"
+                r += ";".join(
                     [
-                        str(i) if i < 0x80000000 else str(i - 0x80000000) + "h"
+                        str(i) if i < HARDENED_INDEX else str(i - HARDENED_INDEX) + "h"
                         for i in idx
                     ]
                 )
-                r += "}"
+                r += ">"
         return r
 
 
 class Key(DescriptorBase):
-    def __init__(self, key, origin=None, derivation=None, taproot=False):
+    def __init__(
+        self,
+        key,
+        origin=None,
+        derivation=None,
+        taproot=False,
+        xonly_repr=False,
+    ):
         self.origin = origin
         self.key = key
         self.taproot = taproot
+        self.xonly_repr = xonly_repr and taproot
         if not hasattr(key, "derive") and derivation:
             raise ArgumentError("Key %s doesn't support derivation" % key)
         self.allowed_derivation = derivation
 
     def __len__(self):
-        return 34 - int(self.taproot) # <33:sec> or <32:xonly>
+        return 34 - int(self.taproot)  # <33:sec> or <32:xonly>
 
     @property
     def my_fingerprint(self):
         if self.is_extended:
             return self.key.my_fingerprint
         return None
 
@@ -185,15 +214,15 @@
         return None
 
     @property
     def derivation(self):
         return [] if self.origin is None else self.origin.derivation
 
     @classmethod
-    def read_from(cls, s, taproot:bool = False):
+    def read_from(cls, s, taproot: bool = False):
         """
         Reads key argument from stream.
         If taproot is set to True - allows both x-only and sec pubkeys.
         If taproot is False - will raise when finds xonly pubkey.
         """
         first = s.read(1)
         origin = None
@@ -204,50 +233,59 @@
             origin = KeyOrigin.from_string(prefix.decode())
         else:
             s.seek(-1, 1)
         k, char = read_until(s, b",)/")
         der = b""
         # there is a following derivation
         if char == b"/":
-            der, char = read_until(s, b"{,)")
-            # we get a set of possible branches: {a,b,c...}
+            der, char = read_until(s, b"<{,)")
+            # legacy branches: {a,b,c...}
             if char == b"{":
                 der += b"{"
                 branch, char = read_until(s, b"}")
                 if char is None:
                     raise ArgumentError("Failed reading the key, missing }")
                 der += branch + b"}"
                 rest, char = read_until(s, b",)")
                 der += rest
+            # multipart descriptor: <a;b;c;...>
+            elif char == b"<":
+                der += b"<"
+                branch, char = read_until(s, b">")
+                if char is None:
+                    raise ArgumentError("Failed reading the key, missing >")
+                der += branch + b">"
+                rest, char = read_until(s, b",)")
+                der += rest
         if char is not None:
             s.seek(-1, 1)
         # parse key
-        k = cls.parse_key(k, taproot)
+        k, xonly_repr = cls.parse_key(k, taproot)
         # parse derivation
         allow_hardened = isinstance(k, bip32.HDKey) and isinstance(k.key, ec.PrivateKey)
         derivation = AllowedDerivation.from_string(
             der.decode(), allow_hardened=allow_hardened
         )
-        return cls(k, origin, derivation, taproot)
+        return cls(k, origin, derivation, taproot, xonly_repr)
 
     @classmethod
-    def parse_key(cls, k: bytes, taproot:bool = False):
+    def parse_key(cls, key: bytes, taproot: bool = False):
         # convert to string
-        k = k.decode()
+        k = key.decode()
         if len(k) in [66, 130] and k[:2] in ["02", "03", "04"]:
             # bare public key
-            return ec.PublicKey.parse(unhexlify(k))
+            return ec.PublicKey.parse(unhexlify(k)), False
         elif taproot and len(k) == 64:
             # x-only pubkey
-            return ec.PublicKey.parse(b"\x02"+unhexlify(k))
+            return ec.PublicKey.parse(b"\x02" + unhexlify(k)), True
         elif k[1:4] in ["pub", "prv"]:
             # bip32 key
-            return bip32.HDKey.from_base58(k)
+            return bip32.HDKey.from_base58(k), False
         else:
-            return ec.PrivateKey.from_wif(k)
+            return ec.PrivateKey.from_wif(k), False
 
     @property
     def is_extended(self):
         return isinstance(self.key, bip32.HDKey)
 
     def check_derivation(self, derivation_path):
         rest = None
@@ -260,15 +298,19 @@
         if self.my_fingerprint == derivation_path.fingerprint:
             rest = derivation_path.derivation
         if self.allowed_derivation is None or rest is None:
             return None
         return self.allowed_derivation.check_derivation(rest)
 
     def get_public_key(self):
-        return self.key.get_public_key() if (self.is_extended or self.is_private) else self.key
+        return (
+            self.key.get_public_key()
+            if (self.is_extended or self.is_private)
+            else self.key
+        )
 
     def sec(self):
         return self.key.sec()
 
     def xonly(self):
         return self.key.xonly()
 
@@ -304,15 +346,19 @@
         return self.allowed_derivation.branches if self.allowed_derivation else None
 
     @property
     def num_branches(self):
         return 1 if self.branches is None else len(self.branches)
 
     def branch(self, branch_index=None):
-        der = self.allowed_derivation.branch(branch_index)
+        der = (
+            self.allowed_derivation.branch(branch_index)
+            if self.allowed_derivation is not None
+            else None
+        )
         return type(self)(self.key, self.origin, der, self.taproot)
 
     @property
     def is_wildcard(self):
         return self.allowed_derivation.is_wildcard if self.allowed_derivation else False
 
     def derive(self, idx, branch_index=None):
@@ -335,32 +381,40 @@
             self.is_extended and self.key.is_private
         )
 
     def to_public(self):
         if not self.is_private:
             return self
         if isinstance(self.key, ec.PrivateKey):
-            return type(self)(self.key.get_public_key(), self.origin, self.allowed_derivation, self.taproot)
+            return type(self)(
+                self.key.get_public_key(),
+                self.origin,
+                self.allowed_derivation,
+                self.taproot,
+            )
         else:
-            return type(self)(self.key.to_public(), self.origin, self.allowed_derivation, self.taproot)
+            return type(self)(
+                self.key.to_public(), self.origin, self.allowed_derivation, self.taproot
+            )
 
     @property
     def private_key(self):
         if not self.is_private:
             raise ArgumentError("Key is not private")
         # either HDKey.key or just the key
         return self.key.key if self.is_extended else self.key
 
     @property
     def secret(self):
         return self.private_key.secret
 
     def to_string(self, version=None):
         if isinstance(self.key, ec.PublicKey):
-            return self.prefix + hexlify(self.key.sec()).decode()
+            k = self.key.sec() if not self.xonly_repr else self.key.xonly()
+            return self.prefix + hexlify(k).decode()
         if isinstance(self.key, bip32.HDKey):
             return self.prefix + self.key.to_base58(version) + self.suffix
         if isinstance(self.key, ec.PrivateKey):
             return self.prefix + self.key.wif()
         return self.prefix + self.key
 
     @classmethod
@@ -371,39 +425,39 @@
 class KeyHash(Key):
     @classmethod
     def parse_key(cls, k: bytes, *args, **kwargs):
         # convert to string
         kd = k.decode()
         # raw 20-byte hash
         if len(kd) == 40:
-            return kd
+            return kd, False
         return super().parse_key(k, *args, **kwargs)
 
     def serialize(self, *args, **kwargs):
         if isinstance(self.key, str):
             return unhexlify(self.key)
         # TODO: should it be xonly?
         if self.taproot:
             return hashes.hash160(self.key.sec()[1:33])
         return hashes.hash160(self.key.sec())
 
     def __len__(self):
-        return 21 # <20:pkh>
+        return 21  # <20:pkh>
 
     def compile(self):
         d = self.serialize()
         return compact.to_bytes(len(d)) + d
 
 
 class Number(DescriptorBase):
     def __init__(self, num):
         self.num = num
 
     @classmethod
-    def read_from(cls, s):
+    def read_from(cls, s, taproot=False):
         num = 0
         char = s.read(1)
         while char in b"0123456789":
             num = 10 * num + int(char.decode())
             char = s.read(1)
         s.seek(-1, 1)
         return cls(num)
@@ -422,34 +476,40 @@
         return len(self.compile())
 
     def __str__(self):
         return "%d" % self.num
 
 
 class Raw(DescriptorBase):
+    LEN = 32
+
     def __init__(self, raw):
         if len(raw) != self.LEN * 2:
             raise ArgumentError("Invalid raw element length: %d" % len(raw))
         self.raw = unhexlify(raw)
 
     @classmethod
-    def read_from(cls, s):
+    def read_from(cls, s, taproot=False):
         return cls(s.read(2 * cls.LEN).decode())
 
     def __str__(self):
         return hexlify(self.raw).decode()
 
     def compile(self):
         return compact.to_bytes(len(self.raw)) + self.raw
 
     def __len__(self):
         return len(compact.to_bytes(self.LEN)) + self.LEN
 
+
 class Raw32(Raw):
     LEN = 32
+
     def __len__(self):
         return 33
 
+
 class Raw20(Raw):
     LEN = 20
+
     def __len__(self):
         return 21
```

### Comparing `embit-0.7.0/src/embit/descriptor/checksum.py` & `embit-0.8.0/src/embit/descriptor/checksum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-def polymod(c, val):
+from .errors import DescriptorError
+
+
+def polymod(c: int, val: int) -> int:
     c0 = c >> 35
     c = ((c & 0x7FFFFFFFF) << 5) ^ val
     if c0 & 1:
         c ^= 0xF5DEE51989
     if c0 & 2:
         c ^= 0xA9FDCA3312
     if c0 & 4:
@@ -10,41 +13,44 @@
     if c0 & 8:
         c ^= 0x3706B1677A
     if c0 & 16:
         c ^= 0x644D626FFD
     return c
 
 
-def checksum(desc):
-    INPUT_CHARSET = "0123456789()[],'/*abcdefgh@:$%{}IJKLMNOPQRSTUVWXYZ&+-.;<=>?!^_|~ijklmnopqrstuvwxyzABCDEFGH`#\"\\ "
+def checksum(desc: str) -> str:
+    """Calculate checksum of desciptor string"""
+    INPUT_CHARSET = (
+        "0123456789()[],'/*abcdefgh@:$%{}IJKLMNOPQRSTUVW"
+        'XYZ&+-.;<=>?!^_|~ijklmnopqrstuvwxyzABCDEFGH`#"\\ '
+    )
     CHECKSUM_CHARSET = "qpzry9x8gf2tvdw0s3jn54khce6mua7l"
 
     c = 1
     cls = 0
     clscount = 0
     for ch in desc:
         pos = INPUT_CHARSET.find(ch)
         if pos == -1:
-            return ""
+            raise DescriptorError("Invalid character '%s' in the input string" % ch)
         c = polymod(c, pos & 31)
         cls = cls * 3 + (pos >> 5)
         clscount += 1
         if clscount == 3:
             c = polymod(c, cls)
             cls = 0
             clscount = 0
     if clscount > 0:
         c = polymod(c, cls)
     for j in range(0, 8):
         c = polymod(c, 0)
     c ^= 1
 
-    ret = [None] * 8
-    for j in range(0, 8):
-        ret[j] = CHECKSUM_CHARSET[(c >> (5 * (7 - j))) & 31]
+    ret = [CHECKSUM_CHARSET[(c >> (5 * (7 - j))) & 31] for j in range(0, 8)]
     return "".join(ret)
 
 
-def add_checksum(desc):
+def add_checksum(desc: str) -> str:
+    """Add checksum to descriptor string"""
     if "#" in desc:
         desc = desc.split("#")[0]
     return desc + "#" + checksum(desc)
```

### Comparing `embit-0.7.0/src/embit/descriptor/descriptor.py` & `embit-0.8.0/src/embit/descriptor/descriptor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,67 @@
-from binascii import hexlify, unhexlify
 from io import BytesIO
-from .. import hashes, compact, ec, bip32, script
+from .. import script
 from ..networks import NETWORKS
 from .errors import DescriptorError
 from .base import DescriptorBase
-from .miniscript import Miniscript
+from .miniscript import Miniscript, Multi, Sortedmulti
 from .arguments import Key
+from .taptree import TapTree
 
 
 class Descriptor(DescriptorBase):
-    def __init__(self, miniscript=None, sh=False, wsh=True, key=None, wpkh=True, taproot=False):
+    def __init__(
+        self,
+        miniscript=None,
+        sh=False,
+        wsh=True,
+        key=None,
+        wpkh=True,
+        taproot=False,
+        taptree=None,
+    ):
         # TODO: add support for taproot scripts
-        if key is None and miniscript is None:
-            raise DescriptorError("Provide either miniscript or a key")
+        # Should:
+        # - accept taptree without a key
+        # - accept key without taptree
+        # - raise if miniscript is not None, but taproot=True
+        # - raise if taptree is not None, but taproot=False
+        if key is None and miniscript is None and taptree is None:
+            raise DescriptorError("Provide a key, miniscript or taptree")
         if miniscript is not None:
             # will raise if can't verify
             miniscript.verify()
             if miniscript.type != "B":
                 raise DescriptorError("Top level miniscript should be 'B'")
-            branches = [k.branches for k in miniscript.keys]
-            branch = None
-            for b in branches:
-                if b is not None:
-                    if branch is None:
-                        branch = b
-                    else:
-                        if len(branch) != len(b):
-                            raise DescriptorError(
-                                "All branches should have the same length"
-                            )
+            # check all branches have the same length
+            branches = {
+                len(k.branches) for k in miniscript.keys if k.branches is not None
+            }
+            if len(branches) > 1:
+                raise DescriptorError("All branches should have the same length")
         self.sh = sh
         self.wsh = wsh
         self.key = key
         self.miniscript = miniscript
         self.wpkh = wpkh
         self.taproot = taproot
+        self.taptree = taptree or TapTree()
         # make sure all keys are either taproot or not
         for k in self.keys:
             k.taproot = taproot
 
     @property
     def script_len(self):
         if self.taproot:
-            return 34 # OP_1 <32:xonly>
+            return 34  # OP_1 <32:xonly>
         if self.miniscript:
             return len(self.miniscript)
         if self.wpkh:
-            return 22 # 00 <20:pkh>
-        return 25 # OP_DUP OP_HASH160 <20:pkh> OP_EQUALVERIFY OP_CHECKSIG
+            return 22  # 00 <20:pkh>
+        return 25  # OP_DUP OP_HASH160 <20:pkh> OP_EQUALVERIFY OP_CHECKSIG
 
     @property
     def num_branches(self):
         return max([k.num_branches for k in self.keys])
 
     def branch(self, branch_index=None):
         if self.miniscript:
@@ -61,50 +71,58 @@
                 self.wsh,
                 None,
                 self.wpkh,
                 self.taproot,
             )
         else:
             return type(self)(
-                None, self.sh, self.wsh, self.key.branch(branch_index), self.wpkh, self.taproot
+                None,
+                self.sh,
+                self.wsh,
+                self.key.branch(branch_index),
+                self.wpkh,
+                self.taproot,
+                self.taptree.branch(branch_index),
             )
 
-
     @property
     def is_wildcard(self):
         return any([key.is_wildcard for key in self.keys])
 
     @property
     def is_wrapped(self):
         return self.sh and self.is_segwit
 
     @property
     def is_legacy(self):
         return not (self.is_segwit or self.is_taproot)
 
     @property
     def is_segwit(self):
-        # TODO: is taproot segwit?
-        return (self.wsh and self.miniscript) or (self.wpkh and self.key) or self.taproot
+        return (
+            (self.wsh and self.miniscript) or (self.wpkh and self.key) or self.taproot
+        )
 
     @property
     def is_pkh(self):
         return self.key is not None and not self.taproot
 
     @property
     def is_taproot(self):
         return self.taproot
 
     @property
-    def is_basic_multisig(self):
-        return self.miniscript and self.miniscript.NAME in ["multi", "sortedmulti"]
+    def is_basic_multisig(self) -> bool:
+        # TODO: should be true for taproot basic multisig with NUMS as internal key
+        # Sortedmulti is subclass of Multi
+        return bool(self.miniscript and isinstance(self.miniscript, Multi))
 
     @property
-    def is_sorted(self):
-        return self.is_basic_multisig and self.miniscript.NAME == "sortedmulti"
+    def is_sorted(self) -> bool:
+        return bool(self.is_basic_multisig and isinstance(self.miniscript, Sortedmulti))
 
     def scriptpubkey_type(self):
         if self.is_taproot:
             return "p2tr"
         if self.sh:
             return "p2sh"
         if self.is_pkh:
@@ -113,31 +131,33 @@
             if self.is_segwit:
                 return "p2wpkh"
         else:
             return "p2wsh"
 
     @property
     def brief_policy(self):
+        if self.taptree:
+            return "taptree"
         if self.key:
             return "single key"
         if self.is_basic_multisig:
             return (
                 str(self.miniscript.args[0])
                 + " of "
                 + str(len(self.keys))
                 + " multisig"
                 + (" (sorted)" if self.is_sorted else "")
             )
         return "miniscript"
 
     @property
     def full_policy(self):
-        if self.key or self.is_basic_multisig:
+        if (self.key and not self.taptree) or self.is_basic_multisig:
             return self.brief_policy
-        s = str(self.miniscript)
+        s = str(self.miniscript or self)
         for i, k in enumerate(self.keys):
             s = s.replace(str(k), chr(65 + i))
         return s
 
     def derive(self, idx, branch_index=None):
         if self.miniscript:
             return type(self)(
@@ -146,33 +166,44 @@
                 self.wsh,
                 None,
                 self.wpkh,
                 self.taproot,
             )
         else:
             return type(self)(
-                None, self.sh, self.wsh, self.key.derive(idx, branch_index), self.wpkh, self.taproot
+                None,
+                self.sh,
+                self.wsh,
+                self.key.derive(idx, branch_index),
+                self.wpkh,
+                self.taproot,
+                self.taptree.derive(idx, branch_index),
             )
 
     def to_public(self):
         if self.miniscript:
             return type(self)(
                 self.miniscript.to_public(),
                 self.sh,
                 self.wsh,
                 None,
                 self.wpkh,
                 self.taproot,
             )
         else:
             return type(self)(
-                None, self.sh, self.wsh, self.key.to_public(), self.wpkh, self.taproot
+                None,
+                self.sh,
+                self.wsh,
+                self.key.to_public(),
+                self.wpkh,
+                self.taproot,
+                self.taptree.to_public(),
             )
 
-
     def owns(self, psbt_scope):
         """Checks if psbt input or output belongs to this descriptor"""
         # we can't check if we don't know script_pubkey
         if psbt_scope.script_pubkey is None:
             return False
         # quick check of script_pubkey type
         if psbt_scope.script_pubkey.script_type() != self.scriptpubkey_type():
@@ -183,26 +214,26 @@
                 if not k.is_extended:
                     continue
                 res = k.check_derivation(der)
                 if res:
                     idx, branch_idx = res
                     sc = self.derive(idx, branch_index=branch_idx).script_pubkey()
                     # if derivation is found but scriptpubkey doesn't match - fail
-                    return (sc == psbt_scope.script_pubkey)
+                    return sc == psbt_scope.script_pubkey
         for pub, (leafs, der) in psbt_scope.taproot_bip32_derivations.items():
             # check of the fingerprints
             for k in self.keys:
                 if not k.is_extended:
                     continue
                 res = k.check_derivation(der)
                 if res:
                     idx, branch_idx = res
                     sc = self.derive(idx, branch_index=branch_idx).script_pubkey()
                     # if derivation is found but scriptpubkey doesn't match - fail
-                    return (sc == psbt_scope.script_pubkey)
+                    return sc == psbt_scope.script_pubkey
         return False
 
     def check_derivation(self, derivation_path):
         for k in self.keys:
             # returns a tuple branch_idx, idx
             der = k.check_derivation(derivation_path)
             if der is not None:
@@ -223,15 +254,15 @@
                 return script.p2wsh(script.Script(self.miniscript.compile()))
         else:
             return script.p2wpkh(self.key)
 
     def script_pubkey(self):
         # covers sh-wpkh, sh and sh-wsh
         if self.taproot:
-            return script.p2tr(self.key)
+            return script.p2tr(self.key, self.taptree)
         if self.sh:
             return script.p2sh(self.redeem_script())
         if self.wsh:
             return script.p2wsh(self.witness_script())
         if self.miniscript:
             return script.Script(self.miniscript.compile())
         if self.wpkh:
@@ -239,15 +270,19 @@
         return script.p2pkh(self.key)
 
     def address(self, network=NETWORKS["main"]):
         return self.script_pubkey().address(network)
 
     @property
     def keys(self):
-        if self.key:
+        if self.taptree and self.key:
+            return [self.key] + self.taptree.keys
+        elif self.taptree:
+            return self.taptree.keys
+        elif self.key:
             return [self.key]
         return self.miniscript.keys
 
     @classmethod
     def from_string(cls, desc):
         s = BytesIO(desc.encode())
         res = cls.read_from(s)
@@ -261,17 +296,17 @@
         # starts with sh(wsh()), sh() or wsh()
         start = s.read(7)
         sh = False
         wsh = False
         wpkh = False
         is_miniscript = True
         taproot = False
+        taptree = TapTree()
         if start.startswith(b"tr("):
             taproot = True
-            is_miniscript = False
             s.seek(-4, 1)
         elif start.startswith(b"sh(wsh("):
             sh = True
             wsh = True
         elif start.startswith(b"wsh("):
             sh = False
             wsh = True
@@ -289,30 +324,55 @@
             is_miniscript = False
             s.seek(-3, 1)
         elif start.startswith(b"sh("):
             sh = True
             wsh = False
             s.seek(-4, 1)
         else:
-            raise ValueError("Invalid descriptor")
-        if is_miniscript:
+            raise ValueError("Invalid descriptor (starts with '%s')" % start.decode())
+        # taproot always has a key, and may have taptree miniscript
+        if taproot:
+            miniscript = None
+            key = Key.read_from(s, taproot=True)
+            nbrackets = 1
+            c = s.read(1)
+            # TODO: should it be ok to pass just taptree without a key?
+            # check if we have taptree after the key
+            if c != b",":
+                s.seek(-1, 1)
+            else:
+                taptree = TapTree.read_from(s)
+        elif is_miniscript:
             miniscript = Miniscript.read_from(s)
             key = None
             nbrackets = int(sh) + int(wsh)
+        # single key for sure
         else:
             miniscript = None
             key = Key.read_from(s, taproot=taproot)
             nbrackets = 1 + int(sh)
         end = s.read(nbrackets)
         if end != b")" * nbrackets:
-            raise ValueError("Invalid descriptor")
-        return cls(miniscript, sh=sh, wsh=wsh, key=key, wpkh=wpkh, taproot=taproot)
+            raise ValueError(
+                "Invalid descriptor (expected ')' but ends with '%s')" % end.decode()
+            )
+        return cls(
+            miniscript,
+            sh=sh,
+            wsh=wsh,
+            key=key,
+            wpkh=wpkh,
+            taproot=taproot,
+            taptree=taptree,
+        )
 
     def to_string(self):
         if self.taproot:
+            if self.taptree:
+                return "tr(%s,%s)" % (self.key, self.taptree)
             return "tr(%s)" % self.key
         if self.miniscript is not None:
             res = str(self.miniscript)
             if self.wsh:
                 res = "wsh(%s)" % res
         else:
             if self.wpkh:
```

### Comparing `embit-0.7.0/src/embit/descriptor/miniscript.py` & `embit-0.8.0/src/embit/descriptor/miniscript.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from binascii import hexlify, unhexlify
-from io import BytesIO
-from .. import hashes, compact, ec, bip32, script
-from ..networks import NETWORKS
+from ..misc import read_until
 from .errors import MiniscriptError
 from .base import DescriptorBase
-from .arguments import *
+from .arguments import Key, KeyHash, Number, Raw32, Raw20
 
 
 class Miniscript(DescriptorBase):
-    def __init__(self, *args):
+    def __init__(self, *args, **kwargs):
         self.args = args
+        self.taproot = kwargs.get("taproot", False)
 
     def compile(self):
         return self.inner_compile()
 
     def verify(self):
         for arg in self.args:
             if isinstance(arg, Miniscript):
@@ -27,82 +25,81 @@
         )
 
     def derive(self, idx, branch_index=None):
         args = [
             arg.derive(idx, branch_index) if hasattr(arg, "derive") else arg
             for arg in self.args
         ]
-        return type(self)(*args)
+        return type(self)(*args, taproot=self.taproot)
 
     def to_public(self):
         args = [
-            arg.to_public() if hasattr(arg, "to_public") else arg
-            for arg in self.args
+            arg.to_public() if hasattr(arg, "to_public") else arg for arg in self.args
         ]
-        return type(self)(*args)
+        return type(self)(*args, taproot=self.taproot)
 
     def branch(self, branch_index):
         args = [
             arg.branch(branch_index) if hasattr(arg, "branch") else arg
             for arg in self.args
         ]
-        return type(self)(*args)
+        return type(self)(*args, taproot=self.taproot)
 
     @property
     def properties(self):
         return self.PROPS
 
     @property
     def type(self):
         return self.TYPE
 
     @classmethod
-    def read_from(cls, s):
+    def read_from(cls, s, taproot=False):
         op, char = read_until(s, b"(")
         op = op.decode()
         wrappers = ""
         if ":" in op:
             wrappers, op = op.split(":")
         if char != b"(":
             raise MiniscriptError("Missing operator")
         if op not in OPERATOR_NAMES:
             raise MiniscriptError("Unknown operator '%s'" % op)
-        # number of arguments, classes of arguments, compile function, type, validity checker
+        # number of arguments, classes of args, compile fn, type, validity checker
         MiniscriptCls = OPERATORS[OPERATOR_NAMES.index(op)]
-        args = MiniscriptCls.read_arguments(s)
-        miniscript = MiniscriptCls(*args)
+        args = MiniscriptCls.read_arguments(s, taproot=taproot)
+        miniscript = MiniscriptCls(*args, taproot=taproot)
         for w in reversed(wrappers):
             if w not in WRAPPER_NAMES:
                 raise MiniscriptError("Unknown wrapper")
             WrapperCls = WRAPPERS[WRAPPER_NAMES.index(w)]
-            miniscript = WrapperCls(miniscript)
+            miniscript = WrapperCls(miniscript, taproot=taproot)
         return miniscript
 
     @classmethod
-    def read_arguments(cls, s):
+    def read_arguments(cls, s, taproot=False):
         args = []
         if cls.NARGS is None:
             if type(cls.ARGCLS) == tuple:
                 firstcls, nextcls = cls.ARGCLS
             else:
                 firstcls, nextcls = cls.ARGCLS, cls.ARGCLS
-            args.append(firstcls.read_from(s))
+            args.append(firstcls.read_from(s, taproot=taproot))
             while True:
                 char = s.read(1)
                 if char == b",":
-                    args.append(nextcls.read_from(s))
+                    args.append(nextcls.read_from(s, taproot=taproot))
                 elif char == b")":
                     break
                 else:
                     raise MiniscriptError(
                         "Expected , or ), got: %s" % (char + s.read())
                     )
         else:
             for i in range(cls.NARGS):
-                args.append(cls.ARGCLS.read_from(s))
+                args.append(cls.ARGCLS.read_from(s, taproot=taproot))
                 if i < cls.NARGS - 1:
                     char = s.read(1)
                     if char != b",":
                         raise MiniscriptError("Missing arguments, %s" % char)
             char = s.read(1)
             if char != b")":
                 raise MiniscriptError("Expected ) got %s" % (char + s.read()))
@@ -114,19 +111,21 @@
     def __len__(self):
         """Length of the compiled script, override this if you know the length"""
         return len(self.compile())
 
     def len_args(self):
         return sum([len(arg) for arg in self.args])
 
+
 ########### Known fragments (miniscript operators) ##############
 
 
 class OneArg(Miniscript):
     NARGS = 1
+
     # small handy functions
     @property
     def arg(self):
         return self.args[0]
 
     @property
     def carg(self):
@@ -156,14 +155,15 @@
 
     def inner_compile(self):
         return b"\x76\xa9" + self.carg + b"\x88"
 
     def __len__(self):
         return self.len_args() + 3
 
+
 class Older(OneArg):
     # <n> CHECKSEQUENCEVERIFY
     NAME = "older"
     ARGCLS = Number
     TYPE = "B"
     PROPS = "z"
 
@@ -176,14 +176,15 @@
             raise MiniscriptError(
                 "%s should have an argument in range [1, 0x80000000)" % self.NAME
             )
 
     def __len__(self):
         return self.len_args() + 1
 
+
 class After(Older):
     # <n> CHECKLOCKTIMEVERIFY
     NAME = "after"
 
     def inner_compile(self):
         return self.carg + b"\xb1"
 
@@ -197,14 +198,15 @@
 
     def inner_compile(self):
         return b"\x82" + Number(32).compile() + b"\x88\xa8" + self.carg + b"\x87"
 
     def __len__(self):
         return self.len_args() + 6
 
+
 class Hash256(Sha256):
     # SIZE <32> EQUALVERIFY HASH256 <h> EQUAL
     NAME = "hash256"
 
     def inner_compile(self):
         return b"\x82" + Number(32).compile() + b"\x88\xaa" + self.carg + b"\x87"
 
@@ -230,15 +232,15 @@
     # [X] NOTIF [Z] ELSE [Y] ENDIF
     NAME = "andor"
     NARGS = 3
     ARGCLS = Miniscript
 
     @property
     def type(self):
-        # type: same as Y/Z
+        # same as Y/Z
         return self.args[1].type
 
     def verify(self):
         # requires: X is Bdu; Y and Z are both B, K, or V
         super().verify()
         if self.args[0].type != "B":
             raise MiniscriptError("andor: X should be 'B'")
@@ -276,14 +278,15 @@
             + self.args[1].compile()
             + b"\x68"
         )
 
     def __len__(self):
         return self.len_args() + 3
 
+
 class AndV(Miniscript):
     # [X] [Y]
     NAME = "and_v"
     NARGS = 2
     ARGCLS = Miniscript
 
     def inner_compile(self):
@@ -377,15 +380,15 @@
         )
 
     def __len__(self):
         return self.len_args() + 4
 
     @property
     def type(self):
-        # type: same as Y/Z
+        # same as Y/Z
         return self.args[1].type
 
     def verify(self):
         # requires: X is Bdu; Y and Z are both B, K, or V
         super().verify()
         if self.args[0].type != "B":
             raise MiniscriptError("and_n: X should be 'B'")
@@ -578,15 +581,15 @@
     NARGS = None
     ARGCLS = (Number, Miniscript)
     TYPE = "B"
 
     def inner_compile(self):
         return (
             self.args[1].compile()
-            + b"".join([arg.compile()+b"\x93" for arg in self.args[2:]])
+            + b"".join([arg.compile() + b"\x93" for arg in self.args[2:]])
             + self.args[0].compile()
             + b"\x87"
         )
 
     def __len__(self):
         return self.len_args() + len(self.args) - 1
 
@@ -628,14 +631,22 @@
 class Multi(Miniscript):
     # <k> <key1> ... <keyn> <n> CHECKMULTISIG
     NAME = "multi"
     NARGS = None
     ARGCLS = (Number, Key)
     TYPE = "B"
     PROPS = "ndu"
+    _expected_taproot = False
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if self.taproot is not self._expected_taproot:
+            raise MiniscriptError(
+                "%s can't be used if taproot is %s" % (self.NAME, self.taproot)
+            )
 
     def inner_compile(self):
         return (
             b"".join([arg.compile() for arg in self.args])
             + Number(len(self.args) - 1).compile()
             + b"\xae"
         )
@@ -660,14 +671,47 @@
             self.args[0].compile()
             + b"".join(sorted([arg.compile() for arg in self.args[1:]]))
             + Number(len(self.args) - 1).compile()
             + b"\xae"
         )
 
 
+class MultiA(Multi):
+    # <key1> CHECKSIG <key2> CHECKSIGADD ... <keyN> CHECKSIGNADD <k> NUMEQUAL
+    NAME = "multi_a"
+    _expected_taproot = True
+
+    def inner_compile(self):
+        return (
+            self.args[1].compile()
+            + b"\xac"
+            + b"".join([arg.compile() + b"\xba" for arg in self.args[2:]])
+            + self.args[0].compile()
+            + b"\x9c"
+        )
+
+    def __len__(self):
+        return self.len_args() + len(self.args)
+
+
+class SortedmultiA(MultiA):
+    # <key1> CHECKSIG <key2> CHECKSIGADD ... <keyN> CHECKSIGNADD <k> NUMEQUAL
+    NAME = "sortedmulti_a"
+
+    def inner_compile(self):
+        keys = list(sorted([k.compile() for k in self.args[1:]]))
+        return (
+            keys[0]
+            + b"\xac"
+            + b"".join([k + b"\xba" for k in keys[1:]])
+            + self.args[0].compile()
+            + b"\x9c"
+        )
+
+
 class Pk(OneArg):
     # <key> CHECKSIG
     NAME = "pk"
     ARGCLS = Key
     TYPE = "B"
     PROPS = "ondu"
 
@@ -710,14 +754,16 @@
     OrB,
     OrC,
     OrD,
     OrI,
     Thresh,
     Multi,
     Sortedmulti,
+    MultiA,
+    SortedmultiA,
     Pk,
     Pkh,
 ]
 OPERATOR_NAMES = [cls.NAME for cls in OPERATORS]
 
 
 class Wrapper(OneArg):
@@ -857,15 +903,19 @@
         if self.arg.type != "V":
             raise MiniscriptError("d: X should be V")
         if "z" not in self.arg.properties:
             raise MiniscriptError("d: X should be z")
 
     @property
     def properties(self):
-        props = "ndu"
+        # https://github.com/bitcoin/bitcoin/pull/24906
+        if self.taproot:
+            props = "ndu"
+        else:
+            props = "nd"
         px = self.arg.properties
         if "z" in px:
             props += "o"
         return props
 
 
 class V(Wrapper):
```

### Comparing `embit-0.7.0/src/embit/ec.py` & `embit-0.8.0/src/embit/ec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,46 @@
-import sys
-
-if sys.implementation.name == "micropython":
-    import secp256k1
-else:
-    from .util import secp256k1
 from . import base58
 from . import hashes
+from .misc import secp256k1
 from .networks import NETWORKS
 from .base import EmbitBase, EmbitError, EmbitKey
 from binascii import hexlify, unhexlify
 
 
 class ECError(EmbitError):
     pass
 
+
 class Signature(EmbitBase):
     def __init__(self, sig):
         self._sig = sig
 
     def write_to(self, stream) -> int:
         return stream.write(secp256k1.ecdsa_signature_serialize_der(self._sig))
 
     @classmethod
     def read_from(cls, stream):
         der = stream.read(2)
         der += stream.read(der[1])
         return cls(secp256k1.ecdsa_signature_parse_der(der))
 
+
 class SchnorrSig(EmbitBase):
     def __init__(self, sig):
         assert len(sig) == 64
         self._sig = sig
 
     def write_to(self, stream) -> int:
         return stream.write(self._sig)
 
     @classmethod
     def read_from(cls, stream):
         return cls(stream.read(64))
 
+
 class PublicKey(EmbitKey):
     def __init__(self, point: bytes, compressed: bool = True):
         self._point = point
         self.compressed = compressed
 
     @classmethod
     def read_from(cls, stream):
@@ -90,17 +88,17 @@
 
     def _xonly(self):
         """Returns internal representation of the xonly-pubkey (64 bytes)"""
         pub, _ = secp256k1.xonly_pubkey_from_pubkey(self._point)
         return pub
 
     @classmethod
-    def from_xonly(cls, data:bytes):
+    def from_xonly(cls, data: bytes):
         assert len(data) == 32
-        return cls.parse(b"\x02"+data)
+        return cls.parse(b"\x02" + data)
 
     def schnorr_verify(self, sig, msg_hash) -> bool:
         return bool(secp256k1.schnorrsig_verify(sig._sig, msg_hash, self._xonly()))
 
     @classmethod
     def from_string(cls, s):
         return cls.parse(unhexlify(s))
@@ -161,15 +159,15 @@
 
     def xonly(self) -> bytes:
         return self.sec()[1:]
 
     def taproot_tweak(self, h=b""):
         """Returns a tweaked private key"""
         sec = self.sec()
-        negate = (sec[0] != 0x02)
+        negate = sec[0] != 0x02
         x = sec[1:33]
         tweak = hashes.tagged_hash("TapTweak", x + h)
         if not secp256k1.ec_seckey_verify(tweak):
             raise EmbitError("Tweak is too large")
         if negate:
             secret = secp256k1.ec_privkey_negate(self._secret)
         else:
@@ -204,43 +202,62 @@
     def to_base58(self, network=None) -> str:
         return self.wif(network)
 
     @classmethod
     def from_base58(cls, s):
         return cls.from_wif(s)
 
-    def get_public_key(self):
+    def get_public_key(self) -> PublicKey:
         return PublicKey(secp256k1.ec_pubkey_create(self._secret), self.compressed)
 
-    def sign(self, msg_hash, grind=True):
+    def to_public(self) -> PublicKey:
+        """Alias to get_public_key for API consistency"""
+        return self.get_public_key()
+
+    def sign(self, msg_hash, grind=True) -> Signature:
         sig = Signature(secp256k1.ecdsa_sign(msg_hash, self._secret))
         if grind:
             counter = 1
             while len(sig.serialize()) > 70:
-                sig = Signature(secp256k1.ecdsa_sign(msg_hash, self._secret, None, counter.to_bytes(32, 'little')))
+                sig = Signature(
+                    secp256k1.ecdsa_sign(
+                        msg_hash, self._secret, None, counter.to_bytes(32, "little")
+                    )
+                )
                 counter += 1
                 # just in case we get in infinite loop for some reason
                 if counter > 200:
                     break
         return sig
 
-    def schnorr_sign(self, msg_hash):
+    def schnorr_sign(self, msg_hash) -> SchnorrSig:
         return SchnorrSig(secp256k1.schnorrsig_sign(msg_hash, self._secret))
 
-    def verify(self, sig, msg_hash):
+    def verify(self, sig, msg_hash) -> bool:
         return self.get_public_key().verify(sig, msg_hash)
 
     def schnorr_verify(self, sig, msg_hash) -> bool:
         return self.get_public_key().schnorr_verify(sig, msg_hash)
 
     def write_to(self, stream) -> int:
         # return a copy of the secret
         return stream.write(self._secret)
 
+    def ecdh(self, public_key: PublicKey, hashfn=None, data=None) -> bytes:
+        pubkey_point = secp256k1.ec_pubkey_parse(public_key.sec())
+        return secp256k1.ecdh(pubkey_point, self._secret, hashfn, data)
+
     @classmethod
     def read_from(cls, stream):
         # just to unify the API
         return cls(stream.read(32))
 
     @property
     def is_private(self) -> bool:
         return True
+
+
+# Nothing up my sleeve point for no-internal-key taproot
+# see https://github.com/bitcoin/bips/blob/master/bip-0341.mediawiki#constructing-and-spending-taproot-outputs
+NUMS_PUBKEY = PublicKey.from_string(
+    "0250929b74c1a04954b78b4b6035e97a5e078a5a0f28ec96d547bfee9ace803ac0"
+)
```

### Comparing `embit-0.7.0/src/embit/finalizer.py` & `embit-0.8.0/src/embit/liquid/finalizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,57 @@
-from . import ec
-from .script import Witness, Script
-from .transaction import Transaction
+from .. import ec
+from ..script import Witness, Script
+from .transaction import TxOutWitness, Proof, LTransaction
+
 
 def parse_multisig(sc):
     d = sc.data
-    if d[-1] != 0xae:
+    if d[-1] != 0xAE:
         raise RuntimeError("Not multisig")
-    m = d[0]-80
-    n = d[-2]-80
+    m = d[0] - 80
+    n = d[-2] - 80
     if m > n or m < 1 or n < 1 or m > 16 or n > 16:
         raise RuntimeError("Invalid m or n in multisig script")
     pubs = d[1:-2]
     if len(pubs) % 34 != 0:
         raise RuntimeError("Pubkeys of strange length")
-    if len(pubs) != 34*n:
+    if len(pubs) != 34 * n:
         raise RuntimeError("Not enough pubkeys")
-    pubkeys = [ec.PublicKey.parse(pubs[i*34+1:(i+1)*34]) for i in range(n)]
+    pubkeys = [ec.PublicKey.parse(pubs[i * 34 + 1 : (i + 1) * 34]) for i in range(n)]
     return m, pubkeys
 
+
 def finalize_psbt(tx, ignore_missing=False):
     # ugly copy
-    ttx = Transaction.parse(tx.tx.serialize())
+    ttx = LTransaction.parse(tx.blinded_tx.serialize())
     done = 0
     for i, inp in enumerate(ttx.vin):
-        if tx.utxo(i).script_pubkey.script_type() == "p2pkh":
-            d = b""
-            # meh, ugly, doesn't check pubkeys
-            for k in tx.inputs[i].partial_sigs:
-                v = tx.inputs[i].partial_sigs[k]
-                d += bytes([len(v)]) + v + bytes([len(k.sec())]) + k.sec()
-            ttx.vin[i].script_sig = Script(d)
-            done += 1
-            continue
-
         if tx.inputs[i].redeem_script is not None:
             ttx.vin[i].script_sig = Script(tx.inputs[i].redeem_script.serialize())
 
         # if multisig
         if tx.inputs[i].witness_script is not None:
             m, pubs = parse_multisig(tx.inputs[i].witness_script)
             sigs = []
             for pub in pubs:
                 if pub in tx.inputs[i].partial_sigs:
                     sigs.append(tx.inputs[i].partial_sigs[pub])
                 if len(sigs) == m:
                     break
             if len(sigs) == m or ignore_missing:
-                inp.witness = Witness([b""] + sigs + [tx.inputs[i].witness_script.data])
+                inp.witness.script_witness = Witness(
+                    [b""] + sigs + [tx.inputs[i].witness_script.data]
+                )
                 done += 1
             continue
 
         # meh, ugly, doesn't check pubkeys
         for k in tx.inputs[i].partial_sigs:
             v = tx.inputs[i].partial_sigs[k]
             arr = [v, k.sec()]
             # if tx.inputs[i].redeem_script:
             #     arr = [tx.inputs[i].redeem_script.data] + arr
-            inp.witness = Witness(arr)
+            inp.witness.script_witness = Witness(arr)
             done += 1
-
-        # TODO: legacy
     if not ignore_missing and done < len(ttx.vin):
         return None
     return ttx
-
```

### Comparing `embit-0.7.0/src/embit/liquid/addresses.py` & `embit-0.8.0/src/embit/liquid/addresses.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from .. import bech32, ec, script, base58
 from . import blech32
 from .networks import NETWORKS
 
-def address(script, blinding_key=None, network=NETWORKS['liquidv1']):
+
+def address(script, blinding_key=None, network=NETWORKS["liquidv1"]):
     """
     Returns liquid address from scriptpubkey and blinding key.
     Confidential if blinding key is set, unconfidential otherwise.
     """
     if script.data == b"":
         return "Fee"
     if script.script_type() == "p2sh":
         data = script.data[2:-1]
         if blinding_key is None:
-            return base58.encode_check(network["p2sh"]+data)
+            return base58.encode_check(network["p2sh"] + data)
         else:
-            return base58.encode_check(network["bp2sh"]+blinding_key.sec()+data)
+            return base58.encode_check(network["bp2sh"] + blinding_key.sec() + data)
     else:
         data = script.data
         ver = data[0]
         # FIXME: should be one of OP_N
         if ver > 0:
             ver = ver % 0x50
         if blinding_key is None:
             return bech32.encode(network["bech32"], ver, data[2:])
         else:
-            return blech32.encode(network["blech32"], ver, blinding_key.sec() + data[2:])
+            return blech32.encode(
+                network["blech32"], ver, blinding_key.sec() + data[2:]
+            )
+
 
 def addr_decode(addr):
     """
     Decodes a liquid address and returns scriptpubkey and blinding pubkey.
     If unconfidential address is used - blinding pubkey will be None
     """
     if addr == "Fee":
@@ -37,46 +41,48 @@
     if addr.split("1")[0].lower() in [net.get("blech32") for net in NETWORKS.values()]:
         addr = addr.lower()
         hrp = addr.split("1")[0]
         ver, data = blech32.decode(hrp, addr)
         data = bytes(data)
         pub = ec.PublicKey.parse(data[:33])
         pubhash = data[33:]
-        sc = script.Script(b"\x00"+bytes([len(pubhash)])+pubhash)
+        sc = script.Script(b"\x00" + bytes([len(pubhash)]) + pubhash)
     elif addr.split("1")[0].lower() in [net.get("bech32") for net in NETWORKS.values()]:
         hrp = addr.split("1")[0]
         ver, data = bech32.decode(hrp, addr)
         pub = None
-        sc = script.Script(b"\x00"+bytes([len(data)])+bytes(data))
+        sc = script.Script(b"\x00" + bytes([len(data)]) + bytes(data))
     else:
         data = base58.decode_check(addr)
         if data[:2] in [net.get("bp2sh") for net in NETWORKS.values()]:
             pub = ec.PublicKey.parse(data[2:35])
-            sc = script.Script(b"\xa9\x14"+data[35:]+b"\x87")
+            sc = script.Script(b"\xa9\x14" + data[35:] + b"\x87")
         elif data[:1] in [net.get("p2sh") for net in NETWORKS.values()]:
             pub = None
-            sc = script.Script(b"\xa9\x14"+data[1:]+b"\x87")
+            sc = script.Script(b"\xa9\x14" + data[1:] + b"\x87")
         else:
             raise RuntimeError("Invalid address")
     return sc, pub
 
+
 def detect_network(addr):
     """Detects what networks the address belongs to"""
     # check if it's bech32
     for net in NETWORKS.values():
         if addr.lower().startswith(net.get("bech32")):
             return net
         if "blech32" in net and addr.lower().startswith(net.get("blech32")):
             return net
     # if not - it's base58
     data = base58.decode_check(addr)
     for net in NETWORKS.values():
         if data[:2] in [net.get("bp2sh"), net.get("p2sh")]:
             return net
 
+
 def to_unconfidential(addr):
     """
     Converts address from confidential to unconfidential.
     Returns the same address if already unconfidential.
     """
     sc, pub = addr_decode(addr)
     if pub is None:
```

### Comparing `embit-0.7.0/src/embit/liquid/blech32.py` & `embit-0.8.0/src/embit/liquid/blech32.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,28 +18,31 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 """Reference implementation for Bech32 and segwit addresses."""
 
 CHARSET = "qpzry9x8gf2tvdw0s3jn54khce6mua7l"
 
+
 def bech32_polymod(values):
     """Internal function that computes the Bech32 checksum."""
     generator = [
         # ELEMENTS
-        0x7d52fba40bd886,
-        0x5e8dbf1a03950c,
-        0x1c3a3c74072a18,
-        0x385d72fa0e5139,
-        0x7093e5a608865b,
+        0x7D52FBA40BD886,
+        0x5E8DBF1A03950C,
+        0x1C3A3C74072A18,
+        0x385D72FA0E5139,
+        0x7093E5A608865B,
     ]
     chk = 1
     for value in values:
-        top = chk >> 55 # ELEMENTS: 25->55
-        chk = (chk & 0x7fffffffffffff) << 5 ^ value # ELEMENTS 0x1ffffff->0x7fffffffffffff
+        top = chk >> 55  # ELEMENTS: 25->55
+        chk = (
+            chk & 0x7FFFFFFFFFFFFF
+        ) << 5 ^ value  # ELEMENTS 0x1ffffff->0x7fffffffffffff
         for i in range(5):
             chk ^= generator[i] if ((top >> i) & 1) else 0
     return chk
 
 
 def bech32_hrp_expand(hrp):
     """Expand the HRP into values for checksum computation."""
@@ -50,37 +53,38 @@
     """Verify a checksum given HRP and converted data characters."""
     return bech32_polymod(bech32_hrp_expand(hrp) + data) == 1
 
 
 def bech32_create_checksum(hrp, data):
     """Compute the checksum values given HRP and data."""
     values = bech32_hrp_expand(hrp) + data
-    polymod = bech32_polymod(values + [0]*12) ^ 1
-    return [(polymod >> 5 * (11 - i)) & 0x1f for i in range(12)]
+    polymod = bech32_polymod(values + [0] * 12) ^ 1
+    return [(polymod >> 5 * (11 - i)) & 0x1F for i in range(12)]
 
 
 def bech32_encode(hrp, data):
     """Compute a Bech32 string given HRP and data values."""
     combined = data + bech32_create_checksum(hrp, data)
-    return hrp + '1' + ''.join([CHARSET[d] for d in combined])
+    return hrp + "1" + "".join([CHARSET[d] for d in combined])
 
 
 def bech32_decode(bech):
     """Validate a Bech32 string, and determine HRP and data."""
-    if ((any(ord(x) < 33 or ord(x) > 126 for x in bech)) or
-            (bech.lower() != bech and bech.upper() != bech)):
+    if (any(ord(x) < 33 or ord(x) > 126 for x in bech)) or (
+        bech.lower() != bech and bech.upper() != bech
+    ):
         return (None, None)
     bech = bech.lower()
-    pos = bech.rfind('1')
+    pos = bech.rfind("1")
     if pos < 1 or pos + 7 > len(bech):
         return (None, None)
-    if not all(x in CHARSET for x in bech[pos+1:]):
+    if not all(x in CHARSET for x in bech[pos + 1 :]):
         return (None, None)
     hrp = bech[:pos]
-    data = [CHARSET.find(x) for x in bech[pos+1:]]
+    data = [CHARSET.find(x) for x in bech[pos + 1 :]]
     if not bech32_verify_checksum(hrp, data):
         return (None, None)
     return (hrp, data[:-12])
 
 
 def convertbits(data, frombits, tobits, pad=True):
     """General power-of-2 base conversion."""
```

### Comparing `embit-0.7.0/src/embit/liquid/descriptor.py` & `embit-0.8.0/src/embit/liquid/descriptor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from ..descriptor.descriptor import *
+from .. import ec
+from ..descriptor.descriptor import Descriptor
+from ..descriptor.base import DescriptorBase
+from ..descriptor.errors import DescriptorError
+from ..descriptor.arguments import Key
 from .networks import NETWORKS
 from .addresses import address
 from . import slip77
 from ..hashes import tagged_hash, sha256
-from ..ec import PrivateKey, PublicKey, secp256k1
+from ..misc import secp256k1
+
 
 class LDescriptor(Descriptor):
     """Liquid descriptor that supports blinded() wrapper"""
+
     def __init__(self, *args, blinding_key=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.blinding_key = blinding_key
 
     @property
     def is_blinded(self):
         return self.blinding_key is not None
@@ -48,35 +54,54 @@
     @classmethod
     def read_from(cls, s):
         # starts with blinded(K,...) or directly with sh(wsh()), sh() or wsh()
         start = s.read(8)
         if not start.startswith(b"blinded("):
             s.seek(-8, 1)
             d = Descriptor.read_from(s)
-            return cls(d.miniscript, sh=d.sh, wsh=d.wsh, key=d.key, wpkh=d.wpkh, blinding_key=None, taproot=d.taproot)
+            return cls(
+                d.miniscript,
+                sh=d.sh,
+                wsh=d.wsh,
+                key=d.key,
+                wpkh=d.wpkh,
+                blinding_key=None,
+                taproot=d.taproot,
+            )
 
         blinding_key = BlindingKey.read_from(s)
         if s.read(1) != b",":
             raise DescriptorError("Missing bitcoin descriptor")
         d = Descriptor.read_from(s)
         if s.read(1) != b")":
             raise DescriptorError("Missing ending bracket")
         if not blinding_key.slip77:
             if blinding_key.is_wildcard != d.is_wildcard:
-                raise DescriptorError("Wildcards mismatch in blinded key and descriptor")
+                raise DescriptorError(
+                    "Wildcards mismatch in blinded key and descriptor"
+                )
             if blinding_key.num_branches != d.num_branches:
                 raise DescriptorError("Branches mismatch in blinded key and descriptor")
-        return cls(d.miniscript, sh=d.sh, wsh=d.wsh, key=d.key, wpkh=d.wpkh, blinding_key=blinding_key, taproot=d.taproot)
+        return cls(
+            d.miniscript,
+            sh=d.sh,
+            wsh=d.wsh,
+            key=d.key,
+            wpkh=d.wpkh,
+            blinding_key=blinding_key,
+            taproot=d.taproot,
+        )
 
     def to_string(self, blinded=True):
         res = super().to_string()
         if self.is_blinded and blinded:
             res = "blinded(%s,%s)" % (self.blinding_key, res)
         return res
 
+
 class BlindingKey(DescriptorBase):
     def __init__(self, key, slip77=False):
         self.key = key
         self.slip77 = slip77
 
     def derive(self, idx, branch_index=None):
         if self.slip77:
@@ -105,18 +130,20 @@
             return slip77.blinding_key(self.key.private_key, sc)
         # if not slip77 - make a script tweak to the key
         tweak = tagged_hash("elements/blindingkey", sc.data)
         if self.key.is_private:
             secret = secp256k1.ec_privkey_add(self.key.secret, tweak)
             # negate if it's odd
             if ec.PrivateKey(secret).sec()[0] == 0x03:
-                 secp256k1.ec_privkey_negate(secret)
+                secp256k1.ec_privkey_negate(secret)
             return ec.PrivateKey(secret)
         else:
-            pub = secp256k1.ec_pubkey_add(secp256k1.ec_pubkey_parse(self.key.sec()), tweak)
+            pub = secp256k1.ec_pubkey_add(
+                secp256k1.ec_pubkey_parse(self.key.sec()), tweak
+            )
             if secp256k1.ec_pubkey_serialize(pub)[0] == 0x03:
                 secp256k1.ec_pubkey_negate(pub)
             return ec.PublicKey(pub)
 
     @classmethod
     def read_from(cls, s):
         start = s.read(7)
@@ -138,14 +165,15 @@
 
     def to_string(self):
         if self.slip77:
             return "slip77(%s)" % self.key
         else:
             return str(self.key)
 
+
 class MuSigKey(DescriptorBase):
     def __init__(self, keys):
         self.keys = keys
         self._secret = None
         self._pubkey = None
 
     def derive(self, idx, branch_index=None):
@@ -187,52 +215,63 @@
             self._secret = musig_combine_privs([k.secret for k in self.keys])
         return self._secret
 
     def sec(self):
         if self._pubkey is None:
             pubs = [secp256k1.ec_pubkey_parse(k.sec()) for k in self.keys]
             pub = musig_combine_pubs(pubs)
-            self._pubkey = PublicKey(pub)
+            self._pubkey = ec.PublicKey(pub)
         return self._pubkey.sec()
 
+
 def musig_combine_privs(privs, sort=True):
-    keys = [[b""+prv, secp256k1.ec_pubkey_serialize(secp256k1.ec_pubkey_create(prv))] for prv in privs]
+    keys = [
+        [b"" + prv, secp256k1.ec_pubkey_serialize(secp256k1.ec_pubkey_create(prv))]
+        for prv in privs
+    ]
     for karr in keys:
         if karr[1][0] == 0x03:
             secp256k1.ec_privkey_negate(karr[0])
         # x only
         karr[1] = karr[1][1:]
     if sort:
         keys = list(sorted(keys, key=lambda k: k[1]))
     secs = [k[1] for k in keys]
     ll = sha256(b"".join(secs))
-    coefs = [tagged_hash("MuSig coefficient", ll+i.to_bytes(4,'little')) for i in range(len(keys))]
+    coefs = [
+        tagged_hash("MuSig coefficient", ll + i.to_bytes(4, "little"))
+        for i in range(len(keys))
+    ]
     # tweak them all
     for i in range(len(keys)):
         secp256k1.ec_privkey_tweak_mul(coefs[i], keys[i][0])
     s = coefs[0]
     for c in coefs[1:]:
         s = secp256k1.ec_privkey_add(s, c)
     pub = secp256k1.ec_pubkey_create(s)
     if secp256k1.ec_pubkey_serialize(pub)[0] == 0x03:
         secp256k1.ec_privkey_negate(s)
     return s
 
+
 def musig_combine_pubs(pubs, sort=True):
     keys = [[pub, secp256k1.ec_pubkey_serialize(pub)] for pub in pubs]
     for karr in keys:
         if karr[1][0] == 0x03:
             secp256k1.ec_pubkey_negate(karr[0])
         # x only
         karr[1] = karr[1][1:]
     if sort:
         keys = list(sorted(keys, key=lambda k: k[1]))
     secs = [k[1] for k in keys]
     ll = sha256(b"".join(secs))
-    coefs = [tagged_hash("MuSig coefficient", ll+i.to_bytes(4,'little')) for i in range(len(keys))]
+    coefs = [
+        tagged_hash("MuSig coefficient", ll + i.to_bytes(4, "little"))
+        for i in range(len(keys))
+    ]
     # tweak them all
     pubs = [k[0] for k in keys]
     for i in range(len(keys)):
         secp256k1.ec_pubkey_tweak_mul(pubs[i], coefs[i])
     pub = secp256k1.ec_pubkey_combine(*pubs)
     if secp256k1.ec_pubkey_serialize(pub)[0] == 0x03:
         pub = secp256k1.ec_pubkey_negate(pub)
```

### Comparing `embit-0.7.0/src/embit/liquid/pset.py` & `embit-0.8.0/src/embit/liquid/pset.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,30 @@
 else:
     from ..util import secp256k1
 
 from .. import compact, hashes
 from ..psbt import *
 from collections import OrderedDict
 from io import BytesIO
-from .transaction import LTransaction, LTransactionOutput, LTransactionInput, TxOutWitness, TxInWitness, AssetIssuance, Proof, RangeProof, LSIGHASH, unblind
+from .transaction import (
+    LTransaction,
+    LTransactionOutput,
+    LTransactionInput,
+    TxOutWitness,
+    TxInWitness,
+    AssetIssuance,
+    Proof,
+    RangeProof,
+    LSIGHASH,
+    unblind,
+)
 from . import slip77
 import hashlib, gc
 
+
 class LInputScope(InputScope):
     TX_CLS = LTransaction
     TXOUT_CLS = LTransactionOutput
 
     def __init__(self, unknown: dict = {}, **kwargs):
         # liquid-specific fields:
         self.value = None
@@ -24,15 +36,15 @@
         self.asset = None
         self.asset_blinding_factor = None
         self.range_proof = None
         # issuance stuff
         self.issue_value = None
         self.issue_commitment = None
         self.issue_rangeproof = None
-        self.issue_proof = None # Explicit value proof
+        self.issue_proof = None  # Explicit value proof
         self.issue_nonce = None
         self.issue_entropy = None
         # reissuance token stuff
         self.token_value = None
         self.token_commitment = None
         self.token_rangeproof = None
         self.token_proof = None
@@ -49,15 +61,15 @@
         self.asset_blinding_factor = None
         self.value = None
         self.asset = None
         # issuance stuff
         self.issue_value = None
         self.issue_commitment = None
         self.issue_rangeproof = None
-        self.issue_proof = None # Explicit value proof
+        self.issue_proof = None  # Explicit value proof
         self.issue_nonce = None
         self.issue_entropy = None
         # reissuance token stuff
         self.token_value = None
         self.token_commitment = None
         self.token_rangeproof = None
         self.token_proof = None
@@ -68,15 +80,20 @@
     def unblind(self, blinding_key):
         if self.range_proof is None:
             return
 
         pk = slip77.blinding_key(blinding_key, self.utxo.script_pubkey)
         try:
             value, asset, vbf, in_abf, extra, min_value, max_value = unblind(
-                self.utxo.ecdh_pubkey, pk.secret, self.range_proof, self.utxo.value, self.utxo.asset, self.utxo.script_pubkey
+                self.utxo.ecdh_pubkey,
+                pk.secret,
+                self.range_proof,
+                self.utxo.value,
+                self.utxo.asset,
+                self.utxo.script_pubkey,
             )
         # failed to unblind
         except:
             return
         # verify
         gen = secp256k1.generator_generate_blinded(asset, in_abf)
         assert gen == secp256k1.generator_parse(self.utxo.asset)
@@ -91,123 +108,138 @@
     @property
     def has_issuance(self):
         return bool(self.issue_value or self.issue_commitment)
 
     @property
     def asset_issuance(self):
         if self.has_issuance:
-            return AssetIssuance(self.issue_nonce, self.issue_entropy, self.issue_commitment or self.issue_value, self.token_commitment or self.token_value)
+            return AssetIssuance(
+                self.issue_nonce,
+                self.issue_entropy,
+                self.issue_commitment or self.issue_value,
+                self.token_commitment or self.token_value,
+            )
 
     @property
     def vin(self):
-        return LTransactionInput(self.txid, self.vout, sequence=(self.sequence or 0xFFFFFFFF), asset_issuance=self.asset_issuance)
+        return LTransactionInput(
+            self.txid,
+            self.vout,
+            sequence=(self.sequence or 0xFFFFFFFF),
+            asset_issuance=self.asset_issuance,
+        )
 
     @property
     def blinded_vin(self):
-        return LTransactionInput(self.txid, self.vout, sequence=(self.sequence or 0xFFFFFFFF),
-                            asset_issuance=self.asset_issuance, witness=TxInWitness(self.issue_rangeproof, self.token_rangeproof))
+        return LTransactionInput(
+            self.txid,
+            self.vout,
+            sequence=(self.sequence or 0xFFFFFFFF),
+            asset_issuance=self.asset_issuance,
+            witness=TxInWitness(self.issue_rangeproof, self.token_rangeproof),
+        )
 
     def read_value(self, stream, k):
         # standard bitcoin stuff
-        if (b'\xfc\x08elements' not in k) and (b"\xfc\x04pset" not in k):
+        if (b"\xfc\x08elements" not in k) and (b"\xfc\x04pset" not in k):
             super().read_value(stream, k)
-        elif k == b'\xfc\x04pset\x0e':
+        elif k == b"\xfc\x04pset\x0e":
             # range proof is very large,
             # so we don't load it if compress flag is set.
             if self.compress:
                 skip_string(stream)
             else:
                 self.range_proof = read_string(stream)
-        elif k == b'\xfc\x04pset\x02':
+        elif k == b"\xfc\x04pset\x02":
             if self.compress:
                 skip_string(stream)
             else:
                 self.issue_rangeproof = read_string(stream)
-        elif k == b'\xfc\x04pset\x03':
+        elif k == b"\xfc\x04pset\x03":
             if self.compress:
                 skip_string(stream)
             else:
                 self.token_rangeproof = read_string(stream)
         else:
             v = read_string(stream)
             # liquid-specific fields
-            if k == b'\xfc\x08elements\x00':
-                self.value = int.from_bytes(v, 'little')
-            elif k == b'\xfc\x08elements\x01':
+            if k == b"\xfc\x08elements\x00":
+                self.value = int.from_bytes(v, "little")
+            elif k == b"\xfc\x08elements\x01":
                 self.value_blinding_factor = v
-            elif k == b'\xfc\x08elements\x02':
+            elif k == b"\xfc\x08elements\x02":
                 self.asset = v
-            elif k == b'\xfc\x08elements\x03':
+            elif k == b"\xfc\x08elements\x03":
                 self.asset_blinding_factor = v
-            elif k == b'\xfc\x04pset\x00':
-                self.issue_value = int.from_bytes(v, 'little')
-            elif k == b'\xfc\x04pset\x01':
+            elif k == b"\xfc\x04pset\x00":
+                self.issue_value = int.from_bytes(v, "little")
+            elif k == b"\xfc\x04pset\x01":
                 self.issue_commitment = v
-            elif k == b'\xfc\x04pset\x0f':
+            elif k == b"\xfc\x04pset\x0f":
                 self.issue_proof = v
-            elif k == b'\xfc\x04pset\x0a':
-                self.token_value = int.from_bytes(v, 'little')
-            elif k == b'\xfc\x04pset\x0b':
+            elif k == b"\xfc\x04pset\x0a":
+                self.token_value = int.from_bytes(v, "little")
+            elif k == b"\xfc\x04pset\x0b":
                 self.token_commitment = v
-            elif k == b'\xfc\x04pset\x0c':
+            elif k == b"\xfc\x04pset\x0c":
                 self.issue_nonce = v
-            elif k == b'\xfc\x04pset\x0d':
+            elif k == b"\xfc\x04pset\x0d":
                 self.issue_entropy = v
-            elif k == b'\xfc\x04pset\x10':
+            elif k == b"\xfc\x04pset\x10":
                 self.token_proof = v
             else:
                 self.unknown[k] = v
 
     def write_to(self, stream, skip_separator=False, **kwargs) -> int:
         r = super().write_to(stream, skip_separator=True, **kwargs)
         # liquid-specific keys
         if self.value is not None:
-            r += ser_string(stream, b'\xfc\x08elements\x00')
-            r += ser_string(stream, self.value.to_bytes(8, 'little'))
+            r += ser_string(stream, b"\xfc\x08elements\x00")
+            r += ser_string(stream, self.value.to_bytes(8, "little"))
         if self.value_blinding_factor is not None:
-            r += ser_string(stream, b'\xfc\x08elements\x01')
+            r += ser_string(stream, b"\xfc\x08elements\x01")
             r += ser_string(stream, self.value_blinding_factor)
         if self.asset is not None:
-            r += ser_string(stream, b'\xfc\x08elements\x02')
+            r += ser_string(stream, b"\xfc\x08elements\x02")
             r += ser_string(stream, self.asset)
         if self.asset_blinding_factor is not None:
-            r += ser_string(stream, b'\xfc\x08elements\x03')
+            r += ser_string(stream, b"\xfc\x08elements\x03")
             r += ser_string(stream, self.asset_blinding_factor)
         if self.range_proof is not None:
-            r += ser_string(stream, b'\xfc\x04pset\x0e')
+            r += ser_string(stream, b"\xfc\x04pset\x0e")
             r += ser_string(stream, self.range_proof)
         if self.issue_value:
-            r += ser_string(stream, b'\xfc\x04pset\x00')
-            r += ser_string(stream, self.issue_value.to_bytes(8, 'little'))
+            r += ser_string(stream, b"\xfc\x04pset\x00")
+            r += ser_string(stream, self.issue_value.to_bytes(8, "little"))
         if self.token_value:
-            r += ser_string(stream, b'\xfc\x04pset\x0a')
-            r += ser_string(stream, self.token_value.to_bytes(8, 'little'))
+            r += ser_string(stream, b"\xfc\x04pset\x0a")
+            r += ser_string(stream, self.token_value.to_bytes(8, "little"))
         if self.issue_commitment:
-            r += ser_string(stream, b'\xfc\x04pset\x01')
+            r += ser_string(stream, b"\xfc\x04pset\x01")
             r += ser_string(stream, self.issue_commitment)
         if self.issue_proof:
-            r += ser_string(stream, b'\xfc\x04pset\x0f')
+            r += ser_string(stream, b"\xfc\x04pset\x0f")
             r += ser_string(stream, self.issue_proof)
         if self.issue_rangeproof:
-            r += ser_string(stream, b'\xfc\x04pset\x02')
+            r += ser_string(stream, b"\xfc\x04pset\x02")
             r += ser_string(stream, self.issue_rangeproof)
         if self.token_commitment:
-            r += ser_string(stream, b'\xfc\x04pset\x0b')
+            r += ser_string(stream, b"\xfc\x04pset\x0b")
             r += ser_string(stream, self.token_commitment)
         if self.issue_nonce:
-            r += ser_string(stream, b'\xfc\x04pset\x0c')
+            r += ser_string(stream, b"\xfc\x04pset\x0c")
             r += ser_string(stream, self.issue_nonce)
         if self.issue_entropy:
-            r += ser_string(stream, b'\xfc\x04pset\x0d')
+            r += ser_string(stream, b"\xfc\x04pset\x0d")
             r += ser_string(stream, self.issue_entropy)
         if self.token_proof:
-            r += ser_string(stream, b'\xfc\x04pset\x10')
+            r += ser_string(stream, b"\xfc\x04pset\x10")
             r += ser_string(stream, self.token_proof)
         if self.token_rangeproof:
-            r += ser_string(stream, b'\xfc\x04pset\x03')
+            r += ser_string(stream, b"\xfc\x04pset\x03")
             r += ser_string(stream, self.token_rangeproof)
         # separator
         if not skip_separator:
             r += stream.write(b"\x00")
         return r
 
 
@@ -243,34 +275,42 @@
         if self.asset and self.asset_commitment:
             # we can't verify asset
             if not self.asset_blinding_factor and not self.asset_proof:
                 raise e
             gen = secp256k1.generator_parse(self.asset_commitment)
             # we have blinding factor
             if self.asset_blinding_factor:
-                if gen != secp256k1.generator_generate_blinded(self.asset, self.asset_blinding_factor):
+                if gen != secp256k1.generator_generate_blinded(
+                    self.asset, self.asset_blinding_factor
+                ):
                     raise e
             # otherwise use asset proof
             else:
                 surj_proof = secp256k1.surjectionproof_parse(self.asset_proof)
                 gen_asset = secp256k1.generator_generate(self.asset)
                 if not secp256k1.surjectionproof_verify(surj_proof, [gen_asset], gen):
                     raise e
 
         if self.value and self.value_commitment:
             if not gen or not (self.value_blinding_factor or self.value_proof):
                 raise e
             # we have blinding factor
             if self.value_blinding_factor:
-                value_commitment = secp256k1.pedersen_commit(self.value_blinding_factor, self.value, gen)
-                if self.value_commitment != secp256k1.pedersen_commitment_serialize(value_commitment):
+                value_commitment = secp256k1.pedersen_commit(
+                    self.value_blinding_factor, self.value, gen
+                )
+                if self.value_commitment != secp256k1.pedersen_commitment_serialize(
+                    value_commitment
+                ):
                     raise e
             # otherwise use value proof
             else:
-                value_commitment = secp256k1.pedersen_commitment_parse(self.value_commitment)
+                value_commitment = secp256k1.pedersen_commitment_parse(
+                    self.value_commitment
+                )
                 min_value, max_value = secp256k1.rangeproof_verify(
                     self.value_proof,
                     value_commitment,
                     b"",
                     gen,
                 )
                 if (min_value != max_value) or (self.value != min_value):
@@ -292,27 +332,32 @@
         if self.asset_commitment:
             self.asset = None
         self.blinder_index = None
 
     @property
     def vout(self):
         return LTransactionOutput(
-                    self.asset or self.asset_commitment,
-                    self.value if self.value is not None else self.value_commitment,
-                    self.script_pubkey,
-                    None if self.asset else self.ecdh_pubkey)
+            self.asset or self.asset_commitment,
+            self.value if self.value is not None else self.value_commitment,
+            self.script_pubkey,
+            None if self.asset else self.ecdh_pubkey,
+        )
 
     @property
     def blinded_vout(self):
         return LTransactionOutput(
-                    self.asset_commitment or self.asset,
-                    self.value_commitment or self.value,
-                    self.script_pubkey,
-                    self.ecdh_pubkey,
-                    None if not self.surjection_proof else TxOutWitness(Proof(self.surjection_proof), RangeProof(self.range_proof))
+            self.asset_commitment or self.asset,
+            self.value_commitment or self.value,
+            self.script_pubkey,
+            self.ecdh_pubkey,
+            None
+            if not self.surjection_proof
+            else TxOutWitness(
+                Proof(self.surjection_proof), RangeProof(self.range_proof)
+            ),
         )
 
     def reblind(self, nonce, blinding_pubkey=None, extra_message=b""):
         """
         Re-generates range-proof with particular nonce
         and includes extra message in the range proof.
         This message can contain some useful info like a label or whatever else.
@@ -326,159 +371,170 @@
         pub = secp256k1.ec_pubkey_parse(blinding_pubkey)
         self.ecdh_pubkey = ec.PrivateKey(nonce).sec()
         secp256k1.ec_pubkey_tweak_mul(pub, nonce)
         sec = secp256k1.ec_pubkey_serialize(pub)
         ecdh_nonce = hashlib.sha256(hashlib.sha256(sec).digest()).digest()
         msg = self.asset[-32:] + self.asset_blinding_factor + extra_message
         self.range_proof = secp256k1.rangeproof_sign(
-            ecdh_nonce, self.value, secp256k1.pedersen_commitment_parse(self.value_commitment),
-            self.value_blinding_factor, msg,
-            self.script_pubkey.data, secp256k1.generator_parse(self.asset_commitment))
-
+            ecdh_nonce,
+            self.value,
+            secp256k1.pedersen_commitment_parse(self.value_commitment),
+            self.value_blinding_factor,
+            msg,
+            self.script_pubkey.data,
+            secp256k1.generator_parse(self.asset_commitment),
+        )
 
     def read_value(self, stream, k):
-        if (b'\xfc\x08elements' not in k) and (b"\xfc\x04pset" not in k):
+        if (b"\xfc\x08elements" not in k) and (b"\xfc\x04pset" not in k):
             super().read_value(stream, k)
         # range proof and surjection proof are very large,
         # so we don't load them if compress flag is set.
-        elif k in [b'\xfc\x08elements\x04', b'\xfc\x04pset\x04']:
+        elif k in [b"\xfc\x08elements\x04", b"\xfc\x04pset\x04"]:
             if self.compress:
                 skip_string(stream)
             else:
                 self.range_proof = read_string(stream)
-        elif k in [b'\xfc\x08elements\x05', b'\xfc\x04pset\x05']:
+        elif k in [b"\xfc\x08elements\x05", b"\xfc\x04pset\x05"]:
             if self.compress:
                 skip_string(stream)
             else:
                 self.surjection_proof = read_string(stream)
         else:
             v = read_string(stream)
             # liquid-specific fields
-            if k in [b'\xfc\x08elements\x00', b'\xfc\x04pset\x01']:
+            if k in [b"\xfc\x08elements\x00", b"\xfc\x04pset\x01"]:
                 self.value_commitment = v
-            elif k == b'\xfc\x08elements\x01':
+            elif k == b"\xfc\x08elements\x01":
                 self.value_blinding_factor = v
-            elif k == b'\xfc\x04pset\x02':
+            elif k == b"\xfc\x04pset\x02":
                 self.asset = v
-            elif k in [b'\xfc\x08elements\x02', b'\xfc\x04pset\x03']:
+            elif k in [b"\xfc\x08elements\x02", b"\xfc\x04pset\x03"]:
                 self.asset_commitment = v
-            elif k == b'\xfc\x08elements\x03':
+            elif k == b"\xfc\x08elements\x03":
                 self.asset_blinding_factor = v
-            elif k in [b'\xfc\x08elements\x06', b'\xfc\x04pset\x06']:
+            elif k in [b"\xfc\x08elements\x06", b"\xfc\x04pset\x06"]:
                 self.blinding_pubkey = v
-            elif k in [b'\xfc\x08elements\x07', b'\xfc\x04pset\x07']:
+            elif k in [b"\xfc\x08elements\x07", b"\xfc\x04pset\x07"]:
                 self.ecdh_pubkey = v
             elif k == b"\xfc\x04pset\x08":
-                self.blinder_index = int.from_bytes(v, 'little')
-            elif k == b'\xfc\x04pset\x09':
+                self.blinder_index = int.from_bytes(v, "little")
+            elif k == b"\xfc\x04pset\x09":
                 self.value_proof = v
-            elif k == b'\xfc\x04pset\x0a':
+            elif k == b"\xfc\x04pset\x0a":
                 self.asset_proof = v
             else:
                 self.unknown[k] = v
 
     @property
     def is_blinded(self):
         # TODO: not great
         return self.value_commitment and self.asset_commitment
 
     def write_to(self, stream, skip_separator=False, version=None, **kwargs) -> int:
         # TODO: super.write_to()
         r = super().write_to(stream, skip_separator=True, version=version, **kwargs)
         # liquid-specific keys
         if self.asset is not None and version == 2:
-            r += ser_string(stream, b'\xfc\x04pset\x02')
+            r += ser_string(stream, b"\xfc\x04pset\x02")
             r += ser_string(stream, self.asset)
         if self.value_commitment is not None:
             if version == 2:
-                r += ser_string(stream, b'\xfc\x04pset\x01')
+                r += ser_string(stream, b"\xfc\x04pset\x01")
             else:
-                r += ser_string(stream, b'\xfc\x08elements\x00')
+                r += ser_string(stream, b"\xfc\x08elements\x00")
             r += ser_string(stream, self.value_commitment)
         if self.value_blinding_factor is not None:
-            r += ser_string(stream, b'\xfc\x08elements\x01')
+            r += ser_string(stream, b"\xfc\x08elements\x01")
             r += ser_string(stream, self.value_blinding_factor)
         if self.asset_commitment is not None:
             if version == 2:
-                r += ser_string(stream, b'\xfc\x04pset\x03')
+                r += ser_string(stream, b"\xfc\x04pset\x03")
             else:
-                r += ser_string(stream, b'\xfc\x08elements\x02')
+                r += ser_string(stream, b"\xfc\x08elements\x02")
             r += ser_string(stream, self.asset_commitment)
         if self.asset_blinding_factor is not None:
-            r += ser_string(stream, b'\xfc\x08elements\x03')
+            r += ser_string(stream, b"\xfc\x08elements\x03")
             r += ser_string(stream, self.asset_blinding_factor)
         if self.blinding_pubkey is not None:
             if version == 2:
-                r += ser_string(stream, b'\xfc\x04pset\x06')
+                r += ser_string(stream, b"\xfc\x04pset\x06")
             else:
-                r += ser_string(stream, b'\xfc\x08elements\x06')
+                r += ser_string(stream, b"\xfc\x08elements\x06")
             r += ser_string(stream, self.blinding_pubkey)
         if self.ecdh_pubkey is not None:
             if version == 2:
-                r += ser_string(stream, b'\xfc\x04pset\x07')
+                r += ser_string(stream, b"\xfc\x04pset\x07")
             else:
-                r += ser_string(stream, b'\xfc\x08elements\x07')
+                r += ser_string(stream, b"\xfc\x08elements\x07")
             r += ser_string(stream, self.ecdh_pubkey)
         # for some reason keys 04 and 05 are serialized after 07
         if self.range_proof is not None:
             if version == 2:
-                r += ser_string(stream, b'\xfc\x04pset\x04')
+                r += ser_string(stream, b"\xfc\x04pset\x04")
             else:
-                r += ser_string(stream, b'\xfc\x08elements\x04')
+                r += ser_string(stream, b"\xfc\x08elements\x04")
             r += ser_string(stream, self.range_proof)
         if self.surjection_proof is not None:
             if version == 2:
-                r += ser_string(stream, b'\xfc\x04pset\x05')
+                r += ser_string(stream, b"\xfc\x04pset\x05")
             else:
-                r += ser_string(stream, b'\xfc\x08elements\x05')
+                r += ser_string(stream, b"\xfc\x08elements\x05")
             r += ser_string(stream, self.surjection_proof)
         if self.blinder_index is not None:
             r += ser_string(stream, b"\xfc\x04pset\x08")
-            r += ser_string(stream, self.blinder_index.to_bytes(4, 'little'))
+            r += ser_string(stream, self.blinder_index.to_bytes(4, "little"))
         if self.value_proof is not None:
             r += ser_string(stream, b"\xfc\x04pset\x09")
             r += ser_string(stream, self.value_proof)
         if self.asset_proof is not None:
             r += ser_string(stream, b"\xfc\x04pset\x0a")
             r += ser_string(stream, self.asset_proof)
         # separator
         if not skip_separator:
             r += stream.write(b"\x00")
         return r
 
+
 class PSET(PSBT):
     MAGIC = b"pset\xff"
     PSBTIN_CLS = LInputScope
     PSBTOUT_CLS = LOutputScope
     TX_CLS = LTransaction
 
     def unblind(self, blinding_key):
         for inp in self.inputs:
             inp.unblind(blinding_key)
 
-    def txseed(self, seed:bytes):
+    def txseed(self, seed: bytes):
         assert len(seed) == 32
         # get unique seed for this tx:
         # we use seed + txid:vout + scriptpubkey as unique data for tagged hash
-        data = b"".join([
-            bytes(reversed(inp.txid))+inp.vout.to_bytes(4,'little')
-            for inp in self.inputs
-        ]) + b"".join([out.script_pubkey.serialize() for out in self.outputs])
-        return hashes.tagged_hash("liquid/txseed", seed+data)
+        data = b"".join(
+            [
+                bytes(reversed(inp.txid)) + inp.vout.to_bytes(4, "little")
+                for inp in self.inputs
+            ]
+        ) + b"".join([out.script_pubkey.serialize() for out in self.outputs])
+        return hashes.tagged_hash("liquid/txseed", seed + data)
 
-    def blind(self, seed:bytes):
+    def blind(self, seed: bytes):
         txseed = self.txseed(seed)
         # assign blinding factors to all outputs
         blinding_outs = []
         for i, out in enumerate(self.outputs):
             # skip ones where we don't need blinding
             if out.blinding_pubkey is None or out.value is None:
                 continue
-            out.asset_blinding_factor = hashes.tagged_hash("liquid/abf", txseed+i.to_bytes(4,'little'))
-            out.value_blinding_factor = hashes.tagged_hash("liquid/vbf", txseed+i.to_bytes(4,'little'))
+            out.asset_blinding_factor = hashes.tagged_hash(
+                "liquid/abf", txseed + i.to_bytes(4, "little")
+            )
+            out.value_blinding_factor = hashes.tagged_hash(
+                "liquid/vbf", txseed + i.to_bytes(4, "little")
+            )
             blinding_outs.append(out)
         if len(blinding_outs) == 0:
             raise PSBTError("Nothing to blind")
         # calculate last vbf
         vals = []
         abfs = []
         vbfs = []
@@ -486,15 +542,17 @@
             value = sc.value if sc.value is not None else sc.utxo.value
             asset = sc.asset or sc.utxo.asset
             if not (isinstance(value, int) and len(asset) == 32):
                 continue
             vals.append(value)
             abfs.append(sc.asset_blinding_factor or b"\x00" * 32)
             vbfs.append(sc.value_blinding_factor or b"\x00" * 32)
-        last_vbf = secp256k1.pedersen_blind_generator_blind_sum(vals, abfs, vbfs, len(vals)-len(blinding_outs))
+        last_vbf = secp256k1.pedersen_blind_generator_blind_sum(
+            vals, abfs, vbfs, len(vals) - len(blinding_outs)
+        )
         blinding_outs[-1].value_blinding_factor = last_vbf
 
         # calculate commitments (surj proof etc)
 
         in_tags = []
         in_gens = []
         for inp in self.inputs:
@@ -505,64 +563,97 @@
             elif len(inp.utxo.asset) == 32:
                 in_tags.append(inp.utxo.asset)
                 in_gens.append(secp256k1.generator_generate(inp.utxo.asset))
 
         for i, out in enumerate(self.outputs):
             if None in [out.blinding_pubkey, out.value, out.asset_blinding_factor]:
                 continue
-            gen = secp256k1.generator_generate_blinded(out.asset, out.asset_blinding_factor)
+            gen = secp256k1.generator_generate_blinded(
+                out.asset, out.asset_blinding_factor
+            )
             out.asset_commitment = secp256k1.generator_serialize(gen)
-            value_commitment = secp256k1.pedersen_commit(out.value_blinding_factor, out.value, gen)
-            out.value_commitment = secp256k1.pedersen_commitment_serialize(value_commitment)
+            value_commitment = secp256k1.pedersen_commit(
+                out.value_blinding_factor, out.value, gen
+            )
+            out.value_commitment = secp256k1.pedersen_commitment_serialize(
+                value_commitment
+            )
 
-            proof_seed = hashes.tagged_hash("liquid/surjection_proof", txseed+i.to_bytes(4,'little'))
-            proof, in_idx = secp256k1.surjectionproof_initialize(in_tags, out.asset, proof_seed)
-            secp256k1.surjectionproof_generate(proof, in_idx, in_gens, gen, abfs[in_idx], out.asset_blinding_factor)
+            proof_seed = hashes.tagged_hash(
+                "liquid/surjection_proof", txseed + i.to_bytes(4, "little")
+            )
+            proof, in_idx = secp256k1.surjectionproof_initialize(
+                in_tags, out.asset, proof_seed
+            )
+            secp256k1.surjectionproof_generate(
+                proof, in_idx, in_gens, gen, abfs[in_idx], out.asset_blinding_factor
+            )
             out.surjection_proof = secp256k1.surjectionproof_serialize(proof)
             del proof
             gc.collect()
 
             # generate range proof
-            rangeproof_nonce = hashes.tagged_hash("liquid/range_proof", txseed+i.to_bytes(4,'little'))
+            rangeproof_nonce = hashes.tagged_hash(
+                "liquid/range_proof", txseed + i.to_bytes(4, "little")
+            )
             out.reblind(rangeproof_nonce)
 
             # generate asset proof
             gen_asset = secp256k1.generator_generate(out.asset)
-            proof, idx = secp256k1.surjectionproof_initialize([out.asset], out.asset, b"\x00"*32, 1, 1)
-            proof = secp256k1.surjectionproof_generate(proof, idx, [gen_asset], gen, b"\x00"*32, out.asset_blinding_factor)
+            proof, idx = secp256k1.surjectionproof_initialize(
+                [out.asset], out.asset, b"\x00" * 32, 1, 1
+            )
+            proof = secp256k1.surjectionproof_generate(
+                proof, idx, [gen_asset], gen, b"\x00" * 32, out.asset_blinding_factor
+            )
             out.asset_proof = secp256k1.surjectionproof_serialize(proof)
 
             # generate value proof
-            value_proof_nonce = hashes.tagged_hash("liquid/value_proof", txseed+i.to_bytes(4,'little'))
+            value_proof_nonce = hashes.tagged_hash(
+                "liquid/value_proof", txseed + i.to_bytes(4, "little")
+            )
             out.value_proof = secp256k1.rangeproof_sign(
-                value_proof_nonce, out.value, value_commitment,
-                out.value_blinding_factor, b"",
-                b"", gen,
-                out.value, # min_value
-                -1, # exp
-                0, # min bits
+                value_proof_nonce,
+                out.value,
+                value_commitment,
+                out.value_blinding_factor,
+                b"",
+                b"",
+                gen,
+                out.value,  # min_value
+                -1,  # exp
+                0,  # min bits
             )
 
-
     def fee(self):
         fee = 0
         for out in self.tx.vout:
             if out.script_pubkey.data == b"":
                 fee += out.value
         return fee
 
     @property
     def blinded_tx(self):
-        return self.TX_CLS(version=self.tx_version or 2,
-                           locktime=self.locktime or 0,
-                           vin=[inp.blinded_vin for inp in self.inputs],
-                           vout=[out.blinded_vout for out in self.outputs])
+        return self.TX_CLS(
+            version=self.tx_version or 2,
+            locktime=self.locktime or 0,
+            vin=[inp.blinded_vin for inp in self.inputs],
+            vout=[out.blinded_vout for out in self.outputs],
+        )
 
-    def sighash_segwit(self, input_index, script_pubkey, value, sighash=(LSIGHASH.ALL | LSIGHASH.RANGEPROOF)):
-        return self.blinded_tx.sighash_segwit(input_index, script_pubkey, value, sighash)
+    def sighash_segwit(
+        self,
+        input_index,
+        script_pubkey,
+        value,
+        sighash=(LSIGHASH.ALL | LSIGHASH.RANGEPROOF),
+    ):
+        return self.blinded_tx.sighash_segwit(
+            input_index, script_pubkey, value, sighash
+        )
 
     def sighash_legacy(self, *args, **kwargs):
         return self.blinded_tx.sighash_legacy(*args, **kwargs)
 
     # def sign_with(self, root, sighash=(LSIGHASH.ALL | LSIGHASH.RANGEPROOF)) -> int:
     # TODO: change back to sighash rangeproof when deployed
     def sign_with(self, root, sighash=LSIGHASH.ALL) -> int:
@@ -573,8 +664,8 @@
         return all([sc.is_verified for sc in self.inputs + self.outputs])
 
     def verify(self, *args, **kwargs):
         """Checks that all commitments, values and assets are consistent"""
         super().verify(*args, **kwargs)
         for out in self.outputs:
             out.verify()
-        return self.is_verified
+        return self.is_verified
```

### Comparing `embit-0.7.0/src/embit/liquid/psetview.py` & `embit-0.8.0/src/embit/liquid/psetview.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from ..psbtview import *
 from .pset import *
 import hashlib
 
+
 def skip_commitment(stream):
     c = stream.read(1)
     assert len(c) == 1
-    if c == b"\x00": # None
+    if c == b"\x00":  # None
         return 1
-    if c == b"\x01": # unconfidential
+    if c == b"\x01":  # unconfidential
         r = stream.seek(8, 1)
         return 9
     # confidential
     r = stream.seek(32, 1)
     return 33
 
+
 class GlobalLTransactionView(GlobalTransactionView):
     """
     Global liquid transaction in PSET is
     - unsigned (with empty scriptsigs)
     - doesn't have witness
     """
-    NUM_VIN_OFFSET = 5 # version + marker
+
+    NUM_VIN_OFFSET = 5  # version + marker
 
     def __init__(self, *args, **kwargs):
         self._num_vout_offset = None
         super().__init__(*args, **kwargs)
 
     @property
     def num_vout_offset(self):
@@ -43,70 +46,74 @@
             self.stream.seek(self.num_vout_offset)
             self._num_vout = compact.read_from(self.stream)
         return self._num_vout
 
     @property
     def vout0_offset(self):
         if self._vout0_offset is None:
-            self._vout0_offset = self.num_vout_offset + len(compact.to_bytes(self.num_vout))
+            self._vout0_offset = self.num_vout_offset + len(
+                compact.to_bytes(self.num_vout)
+            )
         return self._vout0_offset
 
     def vin(self, i):
         if i < 0 or i >= self.num_vin:
             raise PSBTError("Invalid input index")
         self.stream.seek(self.vin0_offset)
         for j in range(i):
             self._skip_input()
         return LTransactionInput.read_from(self.stream)
 
     def _skip_input(self):
         off = 32 + 4 + 5
-        self.stream.seek(32, 1) # txid
+        self.stream.seek(32, 1)  # txid
         vout = int.from_bytes(self.stream.read(4), "little")
-        self.stream.seek(5, 1) # scriptsig, sequence
+        self.stream.seek(5, 1)  # scriptsig, sequence
         is_pegin = False
         if vout != 0xFFFFFFFF:
             is_pegin = vout & (1 << 30) != 0
             has_issuance = vout & (1 << 31) != 0
             if has_issuance:
-                self.stream.seek(32+32, 1) # nonce, entropy
+                self.stream.seek(32 + 32, 1)  # nonce, entropy
                 off += 64
-                off += skip_commitment(self.stream) # amount commitment
-                off += skip_commitment(self.stream) # token commitment
+                off += skip_commitment(self.stream)  # amount commitment
+                off += skip_commitment(self.stream)  # token commitment
         return off
 
     def _skip_output(self):
         """Seeks over one output"""
-        self.stream.seek(33, 1) # asset
+        self.stream.seek(33, 1)  # asset
         c = self.stream.read(1)
         if c != b"\x01":
-            self.stream.seek(32, 1) # confidential
+            self.stream.seek(32, 1)  # confidential
         else:
-            self.stream.seek(8, 1) # unconfidential
+            self.stream.seek(8, 1)  # unconfidential
         c = self.stream.read(1)
         if c != b"\x00":
-            self.stream.seek(32, 1) # ecdh_pubkey
+            self.stream.seek(32, 1)  # ecdh_pubkey
         l = compact.read_from(self.stream)
-        self.stream.seek(l, 1) # scriptpubkey
+        self.stream.seek(l, 1)  # scriptpubkey
 
     def vout(self, i):
         if i < 0 or i >= self.num_vout:
             raise PSBTError("Invalid input index")
         self.stream.seek(self.vout0_offset)
         n = i
         while n:
             self._skip_output()
             n -= 1
         return LTransactionOutput.read_from(self.stream)
 
+
 class PSETView(PSBTView):
     """
     Constructor shouldn't be used directly. PSBTView.view_from(stream) should be used instead.
     Either version should be 2 or tx_offset should be int, otherwise you get an error
     """
+
     MAGIC = b"pset\xff"
     PSBTIN_CLS = LInputScope
     PSBTOUT_CLS = LOutputScope
     TX_CLS = GlobalLTransactionView
 
     def clear_cache(self):
         # cache for digests
@@ -145,30 +152,38 @@
         h.update(self.stream.read(l))
 
     def hash_rangeproofs(self):
         if self._hash_rangeproofs is None:
             h = hashlib.sha256()
             for i in range(self.num_outputs):
                 off = self.seek_to_scope(self.num_inputs + i)
-                rangeproof_offset = self.seek_to_value(b'\xfc\x04pset\x04', from_current=True)
+                rangeproof_offset = self.seek_to_value(
+                    b"\xfc\x04pset\x04", from_current=True
+                )
                 if not rangeproof_offset:
                     self.stream.seek(off)
-                    rangeproof_offset = self.seek_to_value(b'\xfc\x08elements\x04', from_current=True)
+                    rangeproof_offset = self.seek_to_value(
+                        b"\xfc\x08elements\x04", from_current=True
+                    )
                 if not rangeproof_offset:
                     h.update(b"\x00")
                 else:
                     l = compact.read_from(self.stream)
                     h.update(compact.to_bytes(l))
                     self._hash_to(h, l)
 
                 self.stream.seek(off)
-                surj_proof_offset = self.seek_to_value(b'\xfc\x04pset\x05', from_current=True)
+                surj_proof_offset = self.seek_to_value(
+                    b"\xfc\x04pset\x05", from_current=True
+                )
                 if not surj_proof_offset:
                     self.stream.seek(off)
-                    surj_proof_offset = self.seek_to_value(b'\xfc\x08elements\x05', from_current=True)
+                    surj_proof_offset = self.seek_to_value(
+                        b"\xfc\x08elements\x05", from_current=True
+                    )
                 if not surj_proof_offset:
                     h.update(b"\x00")
                 else:
                     l = compact.read_from(self.stream)
                     h.update(compact.to_bytes(l))
                     self._hash_to(h, l)
             self._hash_rangeproofs = h.digest()
@@ -179,20 +194,26 @@
             h = hashlib.sha256()
             for i in range(self.num_outputs):
                 out = self.blinded_vout(i)
                 h.update(out.serialize())
             self._hash_outputs = h.digest()
         return self._hash_outputs
 
-    def sighash_segwit(self, input_index, script_pubkey, value, sighash=(LSIGHASH.ALL | LSIGHASH.RANGEPROOF)):
+    def sighash_segwit(
+        self,
+        input_index,
+        script_pubkey,
+        value,
+        sighash=(LSIGHASH.ALL | LSIGHASH.RANGEPROOF),
+    ):
         if input_index < 0 or input_index >= self.num_inputs:
             raise PSBTError("Invalid input index")
         sh, anyonecanpay, hash_rangeproofs = LSIGHASH.check(sighash)
         inp = self.blinded_vin(input_index, compress=True)
-        zero = b"\x00"*32 # for sighashes
+        zero = b"\x00" * 32  # for sighashes
         h = hashlib.sha256()
         h.update(self.tx_version.to_bytes(4, "little"))
         if anyonecanpay:
             h.update(zero)
         else:
             h.update(hashlib.sha256(self.hash_prevouts()).digest())
         if anyonecanpay or sh in [SIGHASH.NONE, SIGHASH.SINGLE]:
@@ -200,33 +221,45 @@
         else:
             h.update(hashlib.sha256(self.hash_sequence()).digest())
         h.update(hashlib.sha256(self.hash_issuances()).digest())
         h.update(bytes(reversed(inp.txid)))
         h.update(inp.vout.to_bytes(4, "little"))
         h.update(script_pubkey.serialize())
         if isinstance(value, int):
-            h.update(b"\x01"+value.to_bytes(8, 'big'))
+            h.update(b"\x01" + value.to_bytes(8, "big"))
         else:
             h.update(value)
         h.update(inp.sequence.to_bytes(4, "little"))
         if inp.has_issuance:
             inp.asset_issuance.hash_to(h)
         if not (sh in [SIGHASH.NONE, SIGHASH.SINGLE]):
             h.update(hashlib.sha256(self.hash_outputs()).digest())
             if hash_rangeproofs:
                 h.update(hashlib.sha256(self.hash_rangeproofs()).digest())
         elif sh == SIGHASH.SINGLE and input_index < self.num_outputs:
-            h.update(hashlib.sha256(hashlib.sha256(self.blinded_vout(input_index).serialize()).digest()).digest())
+            h.update(
+                hashlib.sha256(
+                    hashlib.sha256(self.blinded_vout(input_index).serialize()).digest()
+                ).digest()
+            )
             if hash_rangeproofs:
-                h.update(hashlib.sha256(hashlib.sha256(self.blinded_vout(input_index).witness.serialize()).digest()).digest())
+                h.update(
+                    hashlib.sha256(
+                        hashlib.sha256(
+                            self.blinded_vout(input_index).witness.serialize()
+                        ).digest()
+                    ).digest()
+                )
         else:
             h.update(zero)
         h.update(self.locktime.to_bytes(4, "little"))
         h.update(sighash.to_bytes(4, "little"))
         return hashlib.sha256(h.digest()).digest()
 
     def sighash_legacy(self, input_index, script_pubkey, sighash=SIGHASH.ALL):
         raise NotImplementedError()
 
-    def sighash_taproot(self, input_index, script_pubkeys, values, sighash=SIGHASH.DEFAULT):
+    def sighash_taproot(
+        self, input_index, script_pubkeys, values, sighash=SIGHASH.DEFAULT
+    ):
         """check out bip-341"""
         raise NotImplementedError()
```

### Comparing `embit-0.7.0/src/embit/liquid/transaction.py` & `embit-0.8.0/src/embit/liquid/transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import sys
 import io
 from .. import compact
 from ..script import Script, Witness
 from .. import hashes
 from ..transaction import *
 from ..base import EmbitBase
 import hashlib
+
 if sys.implementation.name == "micropython":
     import secp256k1
 else:
     from ..util import secp256k1
 
+
 class LSIGHASH(SIGHASH):
     # ALL and others are defined in SIGHASH
     RANGEPROOF = 0x40
 
     @classmethod
     def check(cls, sighash: int):
         anyonecanpay = False
@@ -26,61 +29,76 @@
             # remove RANGEPROOF flag
             sighash = sighash ^ cls.RANGEPROOF
             rangeproof = True
         if sighash not in [cls.ALL, cls.NONE, cls.SINGLE]:
             raise TransactionError("Invalid SIGHASH type")
         return sighash, anyonecanpay, rangeproof
 
+
 class LTransactionError(TransactionError):
     pass
 
+
 def read_commitment(stream):
     c = stream.read(1)
     assert len(c) == 1
-    if c == b"\x00": # None
+    if c == b"\x00":  # None
         return None
-    if c == b"\x01": # unconfidential
+    if c == b"\x01":  # unconfidential
         r = stream.read(8)
         assert len(r) == 8
         return int.from_bytes(r, "big")
     # confidential
     r = stream.read(32)
     assert len(r) == 32
-    return c+r
+    return c + r
+
 
 def write_commitment(c):
     if c is None:
         return b"\x00"
     if isinstance(c, int):
-        return b"\x01"+c.to_bytes(8, 'big')
+        return b"\x01" + c.to_bytes(8, "big")
     return c
 
-def unblind(pubkey:bytes, blinding_key:bytes, range_proof:bytes, value_commitment:bytes, asset_commitment:bytes, script_pubkey, message_length=64) -> tuple:
+
+def unblind(
+    pubkey: bytes,
+    blinding_key: bytes,
+    range_proof: bytes,
+    value_commitment: bytes,
+    asset_commitment: bytes,
+    script_pubkey,
+    message_length=64,
+) -> tuple:
     """Unblinds a range proof and returns value, asset, value blinding factor, asset blinding factor, extra data, min and max values"""
     assert len(pubkey) in [33, 65]
     assert len(blinding_key) == 32
     assert len(value_commitment) == 33
     assert len(asset_commitment) == 33
     pub = secp256k1.ec_pubkey_parse(pubkey)
     secp256k1.ec_pubkey_tweak_mul(pub, blinding_key)
     sec = secp256k1.ec_pubkey_serialize(pub)
     nonce = hashlib.sha256(hashlib.sha256(sec).digest()).digest()
 
     commit = secp256k1.pedersen_commitment_parse(value_commitment)
     gen = secp256k1.generator_parse(asset_commitment)
 
-    value, vbf, msg, min_value, max_value = secp256k1.rangeproof_rewind(range_proof, nonce, commit, script_pubkey.data, gen, message_length)
+    value, vbf, msg, min_value, max_value = secp256k1.rangeproof_rewind(
+        range_proof, nonce, commit, script_pubkey.data, gen, message_length
+    )
     if len(msg) < 64:
         raise TransactionError("Rangeproof message is too small")
     asset = msg[:32]
     abf = msg[32:64]
     extra = msg[64:]
     # vbf[:16]+vbf[16:] is an ugly copy that works both in micropython and python3
     # not sure why rewind() changes previous values after a fresh new call, but this is a fix...
-    return value, asset, vbf[:16]+vbf[16:], abf, extra, min_value, max_value
+    return value, asset, vbf[:16] + vbf[16:], abf, extra, min_value, max_value
+
 
 class Proof(EmbitBase):
     def __init__(self, data=b""):
         self.data = data
 
     @property
     def is_empty(self):
@@ -95,46 +113,76 @@
     def read_from(cls, stream):
         l = compact.read_from(stream)
         data = stream.read(l)
         return cls(data)
 
 
 class RangeProof(Proof):
-
-    def unblind(self, ecdh_pubkey, blinding_key, value, asset, script_pubkey, message_length=64):
+    def unblind(
+        self, ecdh_pubkey, blinding_key, value, asset, script_pubkey, message_length=64
+    ):
         if not self.data:
             raise TransactionError("Rangeproof is empty")
-        return unblind(ecdh_pubkey, blinding_key, self.data, value, asset, script_pubkey, message_length)
+        return unblind(
+            ecdh_pubkey,
+            blinding_key,
+            self.data,
+            value,
+            asset,
+            script_pubkey,
+            message_length,
+        )
 
 
 class TxInWitness(EmbitBase):
-    def __init__(self, amount_proof=None, token_proof=None, script_witness=None, pegin_witness=None):
+    def __init__(
+        self,
+        amount_proof=None,
+        token_proof=None,
+        script_witness=None,
+        pegin_witness=None,
+    ):
         self.amount_proof = amount_proof if amount_proof is not None else Proof()
         self.token_proof = token_proof if token_proof is not None else Proof()
-        self.script_witness = script_witness if script_witness is not None else Witness([])
+        self.script_witness = (
+            script_witness if script_witness is not None else Witness([])
+        )
         self.pegin_witness = pegin_witness if pegin_witness is not None else Witness([])
 
     def write_to(self, stream):
         res = self.amount_proof.write_to(stream)
         res += self.token_proof.write_to(stream)
         res += self.script_witness.write_to(stream)
         res += self.pegin_witness.write_to(stream)
         return res
 
     @property
     def is_empty(self):
-        return self.amount_proof.is_empty and self.token_proof.is_empty and len(self.script_witness.items)==0 and len(self.pegin_witness.items)==0
+        return (
+            self.amount_proof.is_empty
+            and self.token_proof.is_empty
+            and len(self.script_witness.items) == 0
+            and len(self.pegin_witness.items) == 0
+        )
 
     @classmethod
     def read_from(cls, stream):
-        return cls(Proof.read_from(stream), Proof.read_from(stream), Witness.read_from(stream), Witness.read_from(stream))
+        return cls(
+            Proof.read_from(stream),
+            Proof.read_from(stream),
+            Witness.read_from(stream),
+            Witness.read_from(stream),
+        )
+
 
 class TxOutWitness(EmbitBase):
     def __init__(self, surjection_proof=None, range_proof=None):
-        self.surjection_proof = surjection_proof if surjection_proof is not None else Proof()
+        self.surjection_proof = (
+            surjection_proof if surjection_proof is not None else Proof()
+        )
         self.range_proof = range_proof if range_proof is not None else RangeProof()
 
     def write_to(self, stream):
         res = self.surjection_proof.write_to(stream)
         res += self.range_proof.write_to(stream)
         return res
 
@@ -144,15 +192,14 @@
 
     @classmethod
     def read_from(cls, stream):
         return cls(Proof.read_from(stream), RangeProof.read_from(stream))
 
 
 class LTransaction(Transaction):
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._hash_rangeproofs = None
         self._hash_issuance = None
 
     @property
     def has_witness(self):
@@ -211,15 +258,17 @@
         h.update(compact.to_bytes(num_vin))
         for i in range(num_vin):
             txin = LTransactionInput.read_from(stream)
             h.update(txin.serialize())
         num_vout = compact.read_from(stream)
         h.update(compact.to_bytes(num_vout))
         if idx >= num_vout or idx < 0:
-            raise TransactionError("Invalid vout index %d, max is %d"  % (idx, num_vout-1))
+            raise TransactionError(
+                "Invalid vout index %d, max is %d" % (idx, num_vout - 1)
+            )
         res = None
         for i in range(num_vout):
             vout = LTransactionOutput.read_from(stream)
             if idx == i:
                 res = vout
             h.update(vout.serialize())
         h.update(stream.read(4))
@@ -276,20 +325,26 @@
         if self._hash_outputs is None:
             h = hashlib.sha256()
             for out in self.vout:
                 h.update(out.serialize())
             self._hash_outputs = h.digest()
         return self._hash_outputs
 
-    def sighash_segwit(self, input_index, script_pubkey, value, sighash=(LSIGHASH.ALL | LSIGHASH.RANGEPROOF)):
+    def sighash_segwit(
+        self,
+        input_index,
+        script_pubkey,
+        value,
+        sighash=(LSIGHASH.ALL | LSIGHASH.RANGEPROOF),
+    ):
         if input_index < 0 or input_index >= len(self.vin):
             raise LTransactionError("Invalid input index")
         sh, anyonecanpay, hash_rangeproofs = LSIGHASH.check(sighash)
         inp = self.vin[input_index]
-        zero = b"\x00"*32 # for sighashes
+        zero = b"\x00" * 32  # for sighashes
         h = hashlib.sha256()
         h.update(self.version.to_bytes(4, "little"))
         if anyonecanpay:
             h.update(zero)
         else:
             h.update(hashlib.sha256(self.hash_prevouts()).digest())
         if anyonecanpay or sh in [SIGHASH.NONE, SIGHASH.SINGLE]:
@@ -297,38 +352,49 @@
         else:
             h.update(hashlib.sha256(self.hash_sequence()).digest())
         h.update(hashlib.sha256(self.hash_issuances()).digest())
         h.update(bytes(reversed(inp.txid)))
         h.update(inp.vout.to_bytes(4, "little"))
         h.update(script_pubkey.serialize())
         if isinstance(value, int):
-            h.update(b"\x01"+value.to_bytes(8, 'big'))
+            h.update(b"\x01" + value.to_bytes(8, "big"))
         else:
             h.update(value)
         h.update(inp.sequence.to_bytes(4, "little"))
         if inp.has_issuance:
             inp.asset_issuance.hash_to(h)
         if not (sh in [SIGHASH.NONE, SIGHASH.SINGLE]):
             h.update(hashlib.sha256(self.hash_outputs()).digest())
             if hash_rangeproofs:
                 h.update(hashlib.sha256(self.hash_rangeproofs()).digest())
         elif sh == SIGHASH.SINGLE and input_index < len(self.vout):
-            h.update(hashlib.sha256(hashlib.sha256(self.vout[input_index].serialize()).digest()).digest())
+            h.update(
+                hashlib.sha256(
+                    hashlib.sha256(self.vout[input_index].serialize()).digest()
+                ).digest()
+            )
             if hash_rangeproofs:
-                h.update(hashlib.sha256(hashlib.sha256(self.vout[input_index].witness.serialize()).digest()).digest())
+                h.update(
+                    hashlib.sha256(
+                        hashlib.sha256(
+                            self.vout[input_index].witness.serialize()
+                        ).digest()
+                    ).digest()
+                )
         else:
             h.update(zero)
         h.update(self.locktime.to_bytes(4, "little"))
         h.update(sighash.to_bytes(4, "little"))
         return hashlib.sha256(h.digest()).digest()
 
+
 class AssetIssuance(EmbitBase):
     def __init__(self, nonce, entropy, amount_commitment, token_commitment=None):
-        self.nonce = nonce or b"\x00"*32
-        self.entropy = entropy or b"\x00"*32
+        self.nonce = nonce or b"\x00" * 32
+        self.entropy = entropy or b"\x00" * 32
         self.amount_commitment = amount_commitment
         self.token_commitment = token_commitment
 
     @classmethod
     def read_from(cls, stream):
         nonce = stream.read(32)
         assert len(nonce) == 32
@@ -347,29 +413,39 @@
     def write_to(self, stream):
         res = stream.write(self.nonce)
         res += stream.write(self.entropy)
         res += stream.write(write_commitment(self.amount_commitment))
         res += stream.write(write_commitment(self.token_commitment))
         return res
 
+
 class LTransactionInput(TransactionInput):
-    def __init__(self, txid, vout, script_sig=None, sequence=0xFFFFFFFF, witness=None, is_pegin=False, asset_issuance=None):
+    def __init__(
+        self,
+        txid,
+        vout,
+        script_sig=None,
+        sequence=0xFFFFFFFF,
+        witness=None,
+        is_pegin=False,
+        asset_issuance=None,
+    ):
         super().__init__(txid, vout, script_sig, sequence, witness)
         self.is_pegin = is_pegin
         self.asset_issuance = asset_issuance
         self.witness = witness if witness is not None else TxInWitness()
 
     def write_to(self, stream, script_sig=None):
         if script_sig is None:
             script_sig = self.script_sig
         vout = self.vout
         if self.has_issuance:
-            vout += (1<<31)
+            vout += 1 << 31
         if self.is_pegin:
-            vout += (1<<30)
+            vout += 1 << 30
         res = stream.write(bytes(reversed(self.txid)))
         res += stream.write(vout.to_bytes(4, "little"))
         res += script_sig.write_to(stream)
         res += stream.write(self.sequence.to_bytes(4, "little"))
         if self.has_issuance:
             res += self.asset_issuance.write_to(stream)
         return res
@@ -383,22 +459,29 @@
         is_pegin = False
         asset_issuance = None
         if vout != 0xFFFFFFFF:
             is_pegin = vout & (1 << 30) != 0
             has_issuance = vout & (1 << 31) != 0
             if has_issuance:
                 asset_issuance = AssetIssuance.read_from(stream)
-            # remove issue and pegin flags 
+            # remove issue and pegin flags
             vout &= 0x3FFFFFFF
-        return cls(txid, vout, script_sig, sequence, is_pegin=is_pegin, asset_issuance=asset_issuance)
+        return cls(
+            txid,
+            vout,
+            script_sig,
+            sequence,
+            is_pegin=is_pegin,
+            asset_issuance=asset_issuance,
+        )
 
     @property
     def has_issuance(self):
         return self.asset_issuance is not None
-    
+
 
 class LTransactionOutput(TransactionOutput):
     def __init__(self, asset, value, script_pubkey, ecdh_pubkey=None, witness=None):
         if asset and len(asset) == 33 and asset[0] == 0x01:
             asset = asset[1:]
         self.asset = asset
         self.value = value
@@ -431,15 +514,23 @@
         """
         Unblinds the output and returns a tuple:
         (value, asset, value_blinding_factor, asset_blinding_factor, min_value, max_value)
         """
         if not self.is_blinded:
             return self.value, self.asset, None, None, None, None
 
-        return unblind(self.ecdh_pubkey, blinding_key, self.witness.range_proof.data, self.value, self.asset, self.script_pubkey, message_length)
+        return unblind(
+            self.ecdh_pubkey,
+            blinding_key,
+            self.witness.range_proof.data,
+            self.value,
+            self.asset,
+            self.script_pubkey,
+            message_length,
+        )
 
     @classmethod
     def read_from(cls, stream):
         asset = stream.read(33)
         blinded = False
         ecdh_pubkey = None
         c = stream.read(1)
```

### Comparing `embit-0.7.0/src/embit/networks.py` & `embit-0.8.0/src/embit/networks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-import sys
-
-if sys.implementation.name == "micropython":
-    from micropython import const
-else:
-    from .util import const
+from .misc import const
 
 NETWORKS = {
     "main": {
         "name": "Mainnet",
         "wif": b"\x80",
         "p2pkh": b"\x00",
         "p2sh": b"\x05",
```

### Comparing `embit-0.7.0/src/embit/psbt.py` & `embit-0.8.0/src/embit/psbt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from collections import OrderedDict
 from .transaction import Transaction, TransactionOutput, TransactionInput, SIGHASH
 from . import compact
 from . import bip32
 from . import ec
 from . import hashes
-from .script import Script, Witness
 from . import script
+from .script import Script, Witness
 from .base import EmbitBase, EmbitError
 
 from binascii import b2a_base64, a2b_base64, hexlify, unhexlify
 from io import BytesIO
 
+
 class PSBTError(EmbitError):
     pass
 
+
 class CompressMode:
     KEEP_ALL = 0
     CLEAR_ALL = 1
     PARTIAL = 2
 
+
 def ser_string(stream, s: bytes) -> int:
     return stream.write(compact.to_bytes(len(s))) + stream.write(s)
 
 
 def read_string(stream) -> bytes:
     l = compact.read_from(stream)
     s = stream.read(l)
@@ -134,14 +137,17 @@
         self.redeem_script = None
         self.witness_script = None
         self.bip32_derivations = OrderedDict()
 
         # tuples of ([leaf_hashes], DerivationPath)
         self.taproot_bip32_derivations = OrderedDict()
         self.taproot_internal_key = None
+        self.taproot_merkle_root = None
+        self.taproot_sigs = OrderedDict()
+        self.taproot_scripts = OrderedDict()
 
         self.final_scriptsig = None
         self.final_scriptwitness = None
         self.parse_unknowns()
 
     def clear_metadata(self, compress=CompressMode.CLEAR_ALL):
         """Removes metadata like derivations, utxos etc except final or partial sigs"""
@@ -156,40 +162,55 @@
             self.witness_script = None
         else:
             if self.witness_utxo is not None:
                 self.non_witness_utxo = None
         self.bip32_derivations = OrderedDict()
         self.taproot_bip32_derivations = OrderedDict()
         self.taproot_internal_key = None
+        self.taproot_merkle_root = None
+        self.taproot_scripts = OrderedDict()
 
     def update(self, other):
         self.txid = other.txid or self.txid
         self.vout = other.vout if other.vout is not None else self.vout
         self.sequence = other.sequence if other.sequence is not None else self.sequence
         self.unknown.update(other.unknown)
         self.non_witness_utxo = other.non_witness_utxo or self.non_witness_utxo
         self.witness_utxo = other.witness_utxo or self.witness_utxo
         self._utxo = other._utxo or self._utxo
         self.partial_sigs.update(other.partial_sigs)
-        self.sighash_type = other.sighash_type if other.sighash_type is not None else self.sighash_type
+        self.sighash_type = (
+            other.sighash_type if other.sighash_type is not None else self.sighash_type
+        )
         self.redeem_script = other.redeem_script or self.redeem_script
         self.witness_script = other.witness_script or self.witness_script
         self.bip32_derivations.update(other.bip32_derivations)
         self.taproot_bip32_derivations.update(other.taproot_bip32_derivations)
         self.taproot_internal_key = other.taproot_internal_key
+        self.taproot_merkle_root = other.taproot_merkle_root or self.taproot_merkle_root
+        self.taproot_sigs.update(other.taproot_sigs)
+        self.taproot_scripts.update(other.taproot_scripts)
         self.final_scriptsig = other.final_scriptsig or self.final_scriptsig
         self.final_scriptwitness = other.final_scriptwitness or self.final_scriptwitness
 
     @property
     def vin(self):
-        return TransactionInput(self.txid, self.vout, sequence=(self.sequence or 0xFFFFFFFF))
+        return TransactionInput(
+            self.txid, self.vout, sequence=(self.sequence or 0xFFFFFFFF)
+        )
 
     @property
     def utxo(self):
-        return self._utxo or self.witness_utxo or (self.non_witness_utxo.vout[self.vout] if self.non_witness_utxo else None)
+        return (
+            self._utxo
+            or self.witness_utxo
+            or (
+                self.non_witness_utxo.vout[self.vout] if self.non_witness_utxo else None
+            )
+        )
 
     @property
     def script_pubkey(self):
         return self.utxo.script_pubkey if self.utxo else None
 
     @property
     def is_verified(self):
@@ -204,15 +225,19 @@
         """Verifies the hash of previous transaction provided in non_witness_utxo.
         We must verify on a hardware wallet even on segwit transactions to avoid
         miner fee attack described here:
         https://blog.trezor.io/details-of-firmware-updates-for-trezor-one-version-1-9-1-and-trezor-model-t-version-2-3-1-1eba8f60f2dd
         For legacy txs we need to verify it to calculate fee.
         """
         if self.non_witness_utxo or self._txhash:
-            txid = bytes(reversed(self._txhash)) if self._txhash else self.non_witness_utxo.txid()
+            txid = (
+                bytes(reversed(self._txhash))
+                if self._txhash
+                else self.non_witness_utxo.txid()
+            )
             if self.txid == txid:
                 self._verified = True
                 return True
             else:
                 raise PSBTError("Previous txid doesn't match non_witness_utxo txid")
         if not ignore_missing:
             raise PSBTError("Missing non_witness_utxo")
@@ -313,38 +338,60 @@
                 return
             if len(k) != 1:
                 raise PSBTError("Invalid final scriptwitness key")
             elif self.final_scriptwitness is None:
                 self.final_scriptwitness = Witness.parse(v)
             else:
                 raise PSBTError("Duplicated final scriptwitness")
-        
+
         elif k == b"\x0e":
             self.txid = bytes(reversed(v))
         elif k == b"\x0f":
-            self.vout = int.from_bytes(v, 'little')
+            self.vout = int.from_bytes(v, "little")
         elif k == b"\x10":
-            self.sequence = int.from_bytes(v, 'little')
+            self.sequence = int.from_bytes(v, "little")
+
+        # TODO: 0x13 - tap key signature
+        # PSBT_IN_TAP_SCRIPT_SIG
+        elif k[0] == 0x14:
+            if len(k) != 65:
+                raise PSBTError("Invalid key length")
+            pub = ec.PublicKey.from_xonly(k[1:33])
+            leaf = k[33:]
+            if (pub, leaf) in self.taproot_sigs:
+                raise PSBTError("Duplicated taproot sig")
+            self.taproot_sigs[(pub, leaf)] = v
+
+        # PSBT_IN_TAP_LEAF_SCRIPT
+        elif k[0] == 0x15:
+            control_block = k[1:]
+            if control_block in self.taproot_scripts:
+                raise PSBTError("Duplicated taproot script")
+            self.taproot_scripts[control_block] = v
 
         # PSBT_IN_TAP_BIP32_DERIVATION
         elif k[0] == 0x16:
             pub = ec.PublicKey.from_xonly(k[1:])
             if pub not in self.taproot_bip32_derivations:
                 b = BytesIO(v)
                 num_leaf_hashes = compact.read_from(b)
                 leaf_hashes = [b.read(32) for i in range(num_leaf_hashes)]
-                if not all([len(leaf)==32 for leaf in leaf_hashes]):
+                if not all([len(leaf) == 32 for leaf in leaf_hashes]):
                     raise PSBTError("Invalid length of taproot leaf hashes")
                 der = DerivationPath.read_from(b)
                 self.taproot_bip32_derivations[pub] = (leaf_hashes, der)
-        
+
         # PSBT_IN_TAP_INTERNAL_KEY
         elif k[0] == 0x17:
             self.taproot_internal_key = ec.PublicKey.from_xonly(v)
 
+        # PSBT_IN_TAP_MERKLE_ROOT
+        elif k[0] == 0x18:
+            self.taproot_merkle_root = v
+
         else:
             if k in self.unknown:
                 raise PSBTError("Duplicated key")
             self.unknown[k] = v
 
     def write_to(self, stream, skip_separator=False, version=None, **kwargs) -> int:
         r = 0
@@ -378,30 +425,50 @@
 
         if version == 2:
             if self.txid is not None:
                 r += ser_string(stream, b"\x0e")
                 r += ser_string(stream, bytes(reversed(self.txid)))
             if self.vout is not None:
                 r += ser_string(stream, b"\x0f")
-                r += ser_string(stream, self.vout.to_bytes(4, 'little'))
+                r += ser_string(stream, self.vout.to_bytes(4, "little"))
             if self.sequence is not None:
                 r += ser_string(stream, b"\x10")
-                r += ser_string(stream, self.sequence.to_bytes(4, 'little'))
+                r += ser_string(stream, self.sequence.to_bytes(4, "little"))
+
+        # PSBT_IN_TAP_SCRIPT_SIG
+        for pub, leaf in self.taproot_sigs:
+            r += ser_string(stream, b"\x14" + pub.xonly() + leaf)
+            r += ser_string(stream, self.taproot_sigs[(pub, leaf)])
+
+        # PSBT_IN_TAP_LEAF_SCRIPT
+        for control_block in self.taproot_scripts:
+            r += ser_string(stream, b"\x15" + control_block)
+            r += ser_string(stream, self.taproot_scripts[control_block])
 
         # PSBT_IN_TAP_BIP32_DERIVATION
         for pub in self.taproot_bip32_derivations:
             r += ser_string(stream, b"\x16" + pub.xonly())
             leaf_hashes, derivation = self.taproot_bip32_derivations[pub]
-            r += ser_string(stream, compact.to_bytes(len(leaf_hashes)) + b"".join(leaf_hashes) + derivation.serialize())
+            r += ser_string(
+                stream,
+                compact.to_bytes(len(leaf_hashes))
+                + b"".join(leaf_hashes)
+                + derivation.serialize(),
+            )
 
         # PSBT_IN_TAP_INTERNAL_KEY
         if self.taproot_internal_key is not None:
             r += ser_string(stream, b"\x17")
             r += ser_string(stream, self.taproot_internal_key.xonly())
 
+        # PSBT_IN_TAP_MERKLE_ROOT
+        if self.taproot_merkle_root is not None:
+            r += ser_string(stream, b"\x18")
+            r += ser_string(stream, self.taproot_merkle_root)
+
         # unknown
         for key in self.unknown:
             r += ser_string(stream, key)
             r += ser_string(stream, self.unknown[key])
         # separator
         if not skip_separator:
             r += stream.write(b"\x00")
@@ -477,40 +544,39 @@
             pub = ec.PublicKey.parse(k[1:])
             if pub in self.bip32_derivations:
                 raise PSBTError("Duplicated derivation path")
             else:
                 self.bip32_derivations[pub] = DerivationPath.parse(v)
 
         elif k == b"\x03":
-            self.value = int.from_bytes(v, 'little')
+            self.value = int.from_bytes(v, "little")
         elif k == b"\x04":
             self.script_pubkey = Script(v)
 
         # PSBT_OUT_TAP_INTERNAL_KEY
         elif k[0] == 0x05:
             self.taproot_internal_key = ec.PublicKey.from_xonly(v)
 
         # PSBT_OUT_TAP_BIP32_DERIVATION
         elif k[0] == 0x07:
             pub = ec.PublicKey.from_xonly(k[1:])
             if pub not in self.taproot_bip32_derivations:
                 b = BytesIO(v)
                 num_leaf_hashes = compact.read_from(b)
                 leaf_hashes = [b.read(32) for i in range(num_leaf_hashes)]
-                if not all([len(leaf)==32 for leaf in leaf_hashes]):
+                if not all([len(leaf) == 32 for leaf in leaf_hashes]):
                     raise PSBTError("Invalid length of taproot leaf hashes")
                 der = DerivationPath.read_from(b)
                 self.taproot_bip32_derivations[pub] = (leaf_hashes, der)
 
         else:
             if k in self.unknown:
                 raise PSBTError("Duplicated key")
             self.unknown[k] = v
 
-
     def write_to(self, stream, skip_separator=False, version=None, **kwargs) -> int:
         r = 0
         if self.redeem_script is not None:
             r += stream.write(b"\x01\x00")
             r += self.redeem_script.write_to(stream)  # script serialization has length
         if self.witness_script is not None:
             r += stream.write(b"\x01\x01")
@@ -518,48 +584,54 @@
         for pub in self.bip32_derivations:
             r += ser_string(stream, b"\x02" + pub.serialize())
             r += ser_string(stream, self.bip32_derivations[pub].serialize())
 
         if version == 2:
             if self.value is not None:
                 r += ser_string(stream, b"\x03")
-                r += ser_string(stream, self.value.to_bytes(8, 'little'))
+                r += ser_string(stream, self.value.to_bytes(8, "little"))
             if self.script_pubkey is not None:
                 r += ser_string(stream, b"\x04")
                 r += self.script_pubkey.write_to(stream)
 
         # PSBT_OUT_TAP_INTERNAL_KEY
         if self.taproot_internal_key is not None:
             r += ser_string(stream, b"\x05")
             r += ser_string(stream, self.taproot_internal_key.xonly())
 
         # PSBT_OUT_TAP_BIP32_DERIVATION
         for pub in self.taproot_bip32_derivations:
             r += ser_string(stream, b"\x07" + pub.xonly())
             leaf_hashes, derivation = self.taproot_bip32_derivations[pub]
-            r += ser_string(stream, compact.to_bytes(len(leaf_hashes)) + b"".join(leaf_hashes) + derivation.serialize())
+            r += ser_string(
+                stream,
+                compact.to_bytes(len(leaf_hashes))
+                + b"".join(leaf_hashes)
+                + derivation.serialize(),
+            )
 
         # unknown
         for key in self.unknown:
             r += ser_string(stream, key)
             r += ser_string(stream, self.unknown[key])
         # separator
         if not skip_separator:
             r += stream.write(b"\x00")
         return r
 
+
 class PSBT(EmbitBase):
     MAGIC = b"psbt\xff"
     # for subclasses
     PSBTIN_CLS = InputScope
     PSBTOUT_CLS = OutputScope
     TX_CLS = Transaction
 
     def __init__(self, tx=None, unknown={}, version=None):
-        self.version = version # None for v0
+        self.version = version  # None for v0
         self.inputs = []
         self.outputs = []
         self.tx_version = None
         self.locktime = None
 
         if tx is not None:
             self.parse_tx(tx)
@@ -572,18 +644,20 @@
         self.tx_version = tx.version
         self.locktime = tx.locktime
         self.inputs = [self.PSBTIN_CLS(vin=vin) for vin in tx.vin]
         self.outputs = [self.PSBTOUT_CLS(vout=vout) for vout in tx.vout]
 
     @property
     def tx(self):
-        return self.TX_CLS(version=self.tx_version or 2,
-                           locktime=self.locktime or 0,
-                           vin=[inp.vin for inp in self.inputs],
-                           vout=[out.vout for out in self.outputs])
+        return self.TX_CLS(
+            version=self.tx_version or 2,
+            locktime=self.locktime or 0,
+            vin=[inp.vin for inp in self.inputs],
+            vout=[out.vout for out in self.outputs],
+        )
 
     def sighash_segwit(self, *args, **kwargs):
         return self.tx.sighash_segwit(*args, **kwargs)
 
     def sighash_legacy(self, *args, **kwargs):
         return self.tx.sighash_legacy(*args, **kwargs)
 
@@ -600,15 +674,18 @@
         return self.is_verified
 
     def utxo(self, i):
         if self.inputs[i].is_verified:
             return self.inputs[i].utxo
         if not (self.inputs[i].witness_utxo or self.inputs[i].non_witness_utxo):
             raise PSBTError("Missing previous utxo on input %d" % i)
-        return self.inputs[i].witness_utxo or self.inputs[i].non_witness_utxo.vout[self.inputs[i].vout]
+        return (
+            self.inputs[i].witness_utxo
+            or self.inputs[i].non_witness_utxo.vout[self.inputs[i].vout]
+        )
 
     def fee(self):
         fee = sum([self.utxo(i).value for i in range(len(self.inputs))])
         fee -= sum([out.value for out in self.tx.vout])
         return fee
 
     def write_to(self, stream) -> int:
@@ -624,24 +701,24 @@
         for xpub in self.xpubs:
             r += ser_string(stream, b"\x01" + xpub.serialize())
             r += ser_string(stream, self.xpubs[xpub].serialize())
 
         if self.version == 2:
             if self.tx_version is not None:
                 r += ser_string(stream, b"\x02")
-                r += ser_string(stream, self.tx_version.to_bytes(4, 'little'))
+                r += ser_string(stream, self.tx_version.to_bytes(4, "little"))
             if self.locktime is not None:
                 r += ser_string(stream, b"\x03")
-                r += ser_string(stream, self.locktime.to_bytes(4, 'little'))
+                r += ser_string(stream, self.locktime.to_bytes(4, "little"))
             r += ser_string(stream, b"\x04")
             r += ser_string(stream, compact.to_bytes(len(self.inputs)))
             r += ser_string(stream, b"\x05")
             r += ser_string(stream, compact.to_bytes(len(self.outputs)))
             r += ser_string(stream, b"\xfb")
-            r += ser_string(stream, self.version.to_bytes(4, 'little'))
+            r += ser_string(stream, self.version.to_bytes(4, "little"))
         # unknown
         for key in self.unknown:
             r += ser_string(stream, key)
             r += ser_string(stream, self.unknown[key])
         # separator
         r += stream.write(b"\x00")
         # inputs
@@ -697,220 +774,276 @@
                 if tx is None:
                     tx = cls.TX_CLS.parse(value)
                 else:
                     raise PSBTError(
                         "Failed to parse PSBT - duplicated transaction field"
                     )
             elif key == b"\xfb":
-                version = int.from_bytes(value, 'little')
+                version = int.from_bytes(value, "little")
             else:
                 if key in unknown:
                     raise PSBTError("Duplicated key")
                 unknown[key] = value
 
         if tx and version == 2:
             raise PSBTError("Global TX field is not allowed in PSBTv2")
         psbt = cls(tx, unknown, version=version)
         # input scopes
         for i, vin in enumerate(psbt.tx.vin):
-            psbt.inputs[i] = cls.PSBTIN_CLS.read_from(stream, compress=compress, vin=vin)
+            psbt.inputs[i] = cls.PSBTIN_CLS.read_from(
+                stream, compress=compress, vin=vin
+            )
         # output scopes
         for i, vout in enumerate(psbt.tx.vout):
-            psbt.outputs[i] = cls.PSBTOUT_CLS.read_from(stream, compress=compress, vout=vout)
+            psbt.outputs[i] = cls.PSBTOUT_CLS.read_from(
+                stream, compress=compress, vout=vout
+            )
         return psbt
 
     def parse_unknowns(self):
         for k in list(self.unknown):
             # xpub field
             if k[0] == 0x01:
                 xpub = bip32.HDKey.parse(k[1:])
                 self.xpubs[xpub] = DerivationPath.parse(self.unknown.pop(k))
             elif k == b"\x02":
-                self.tx_version = int.from_bytes(self.unknown.pop(k), 'little')
+                self.tx_version = int.from_bytes(self.unknown.pop(k), "little")
             elif k == b"\x03":
-                self.locktime = int.from_bytes(self.unknown.pop(k), 'little')
+                self.locktime = int.from_bytes(self.unknown.pop(k), "little")
             elif k == b"\x04":
                 if len(self.inputs) > 0:
                     raise PSBTError("Inputs already initialized")
-                self.inputs = [self.PSBTIN_CLS() for _ in range(compact.from_bytes(self.unknown.pop(k)))]
+                self.inputs = [
+                    self.PSBTIN_CLS()
+                    for _ in range(compact.from_bytes(self.unknown.pop(k)))
+                ]
             elif k == b"\x05":
                 if len(self.outputs) > 0:
                     raise PSBTError("Outputs already initialized")
-                self.outputs = [self.PSBTOUT_CLS() for _ in range(compact.from_bytes(self.unknown.pop(k)))]
+                self.outputs = [
+                    self.PSBTOUT_CLS()
+                    for _ in range(compact.from_bytes(self.unknown.pop(k)))
+                ]
 
-    def sighash(self, i, sighash=SIGHASH.ALL):
+    def sighash(self, i, sighash=SIGHASH.ALL, **kwargs):
         inp = self.inputs[i]
 
         if inp.is_taproot:
             values = [inp.utxo.value for inp in self.inputs]
             scripts = [inp.utxo.script_pubkey for inp in self.inputs]
-            return self.sighash_taproot(i, script_pubkeys=scripts, values=values, sighash=sighash)
+            return self.sighash_taproot(
+                i,
+                script_pubkeys=scripts,
+                values=values,
+                sighash=sighash,
+                **kwargs,
+            )
 
         value = inp.utxo.value
         sc = inp.witness_script or inp.redeem_script or inp.utxo.script_pubkey
 
         # detect if it is a segwit input
-        is_segwit = (inp.witness_script
-                    or inp.witness_utxo
-                    or inp.utxo.script_pubkey.script_type() in {"p2wpkh", "p2wsh"}
-                    or (
-                        inp.redeem_script
-                        and inp.redeem_script.script_type() in {"p2wpkh", "p2wsh"}
-                    )
+        is_segwit = (
+            inp.witness_script
+            or inp.witness_utxo
+            or inp.utxo.script_pubkey.script_type() in {"p2wpkh", "p2wsh"}
+            or (
+                inp.redeem_script
+                and inp.redeem_script.script_type() in {"p2wpkh", "p2wsh"}
+            )
         )
         # convert to p2pkh according to bip143
         if sc.script_type() == "p2wpkh":
             sc = script.p2pkh_from_p2wpkh(sc)
 
         if is_segwit:
             h = self.sighash_segwit(i, sc, value, sighash=sighash)
         else:
             h = self.sighash_legacy(i, sc, sighash=sighash)
         return h
 
+    def sign_input_with_tapkey(
+        self,
+        key: ec.PrivateKey,
+        input_index: int,
+        inp=None,
+        sighash=SIGHASH.DEFAULT,
+    ) -> int:
+        """Sign taproot input with key. Signs with internal or leaf key."""
+        # get input ourselves if not provided
+        inp = inp or self.inputs[input_index]
+        if not inp.is_taproot:
+            return 0
+        # check if key is internal key
+        pk = key.taproot_tweak(inp.taproot_merkle_root or b"")
+        if pk.xonly() in inp.utxo.script_pubkey.data:
+            h = self.sighash(
+                input_index,
+                sighash=sighash,
+            )
+            sig = pk.schnorr_sign(h)
+            wit = sig.serialize()
+            if sighash != SIGHASH.DEFAULT:
+                wit += bytes([sighash])
+            # TODO: maybe better to put into internal key sig field
+            inp.final_scriptwitness = Witness([wit])
+            # no need to sign anything else
+            return 1
+        counter = 0
+        # negate if necessary
+        pub = ec.PublicKey.from_xonly(key.xonly())
+        # iterate over leafs and sign
+        for ctrl, sc in inp.taproot_scripts.items():
+            if pub.xonly() not in sc:
+                continue
+            leaf_version = sc[-1]
+            script = Script(sc[:-1])
+            h = self.sighash(
+                input_index,
+                sighash=sighash,
+                ext_flag=1,
+                script=script,
+                leaf_version=leaf_version,
+            )
+            sig = key.schnorr_sign(h)
+            leaf = hashes.tagged_hash(
+                "TapLeaf", bytes([leaf_version]) + script.serialize()
+            )
+            sigdata = sig.serialize()
+            # append sighash if necessary
+            if sighash != SIGHASH.DEFAULT:
+                sigdata += bytes([sighash])
+            inp.taproot_sigs[(pub, leaf)] = sigdata
+            counter += 1
+        return counter
+
     def sign_with(self, root, sighash=SIGHASH.DEFAULT) -> int:
         """
         Signs psbt with root key (HDKey or similar).
         Returns number of signatures added to PSBT.
-        Sighash kwarg is set to SIGHASH.DEFAULT, for segwit and legacy it's replaced to SIGHASH.ALL
+        Sighash kwarg is set to SIGHASH.DEFAULT,
+        for segwit and legacy it's replaced to SIGHASH.ALL
         so if PSBT is asking to sign with a different sighash this function won't sign.
         If you want to sign with sighashes provided in the PSBT - set sighash=None.
         """
-        # check if it's a descriptor
+        counter = 0  # sigs counter
+        # check if it's a descriptor, and sign with all private keys in this descriptor
         if hasattr(root, "keys"):
-            counter = 0
             for k in root.keys:
                 if hasattr(k, "is_private") and k.is_private:
                     counter += self.sign_with(k, sighash)
             return counter
 
         # if WIF - fingerprint is None
         fingerprint = None
         # if descriptor key
         if hasattr(root, "origin"):
-            if not root.is_private: # pubkey can't sign
+            if not root.is_private:  # pubkey can't sign
                 return 0
-            if root.is_extended: # use fingerprint only for HDKey
+            if root.is_extended:  # use fingerprint only for HDKey
                 fingerprint = root.fingerprint
             else:
-                root = root.key # WIF key
+                root = root.key  # WIF key
         # if HDKey
         if not fingerprint and hasattr(root, "my_fingerprint"):
             fingerprint = root.my_fingerprint
-        if not fingerprint:
-            pub = root.get_public_key()
-            sec = pub.sec()
-            pkh = hashes.hash160(sec)
+
+        rootpub = root.get_public_key()
+        sec = rootpub.sec()
+        pkh = hashes.hash160(sec)
 
         counter = 0
         for i, inp in enumerate(self.inputs):
-            # SIGHASH.DEFAULT is only for taproot, fallback to SIGHASH.ALL for other inputs
+            # SIGHASH.DEFAULT is only for taproot, fallback
+            # to SIGHASH.ALL for other inputs
             required_sighash = sighash
             if not inp.is_taproot and required_sighash == SIGHASH.DEFAULT:
                 required_sighash = SIGHASH.ALL
 
             # check which sighash to use
-            inp_sighash = inp.sighash_type or required_sighash or SIGHASH.DEFAULT
+            inp_sighash = inp.sighash_type
+            if inp_sighash is None:
+                inp_sighash = required_sighash or SIGHASH.DEFAULT
             if not inp.is_taproot and inp_sighash == SIGHASH.DEFAULT:
                 inp_sighash = SIGHASH.ALL
 
-            # if input sighash is set and is different from kwarg - don't sign this input
+            # if input sighash is set and is different from required sighash
+            # we don't sign this input
+            # except DEFAULT is functionally the same as ALL
             if required_sighash is not None and inp_sighash != required_sighash:
-                continue
-
-            h = self.sighash(i, sighash=inp_sighash)
+                if inp_sighash not in {
+                    SIGHASH.DEFAULT,
+                    SIGHASH.ALL,
+                } or required_sighash not in {SIGHASH.DEFAULT, SIGHASH.ALL}:
+                    continue
+
+            # get all possible derivations with matching fingerprint
+            bip32_derivations = set()
+            if fingerprint:
+                # if taproot derivations are present add them
+                for pub in inp.taproot_bip32_derivations:
+                    (_leafs, derivation) = inp.taproot_bip32_derivations[pub]
+                    if derivation.fingerprint == fingerprint:
+                        bip32_derivations.add((pub, derivation))
+
+                # segwit and legacy derivations
+                for pub in inp.bip32_derivations:
+                    derivation = inp.bip32_derivations[pub]
+                    if derivation.fingerprint == fingerprint:
+                        bip32_derivations.add((pub, derivation))
+
+            # get derived keys for signing
+            derived_keypairs = set()  # (prv, pub)
+            for pub, derivation in bip32_derivations:
+                der = derivation.derivation
+                # descriptor key has origin derivation that we take into account
+                if hasattr(root, "origin"):
+                    if root.origin:
+                        if root.origin.derivation != der[: len(root.origin.derivation)]:
+                            # derivation doesn't match - go to next input
+                            continue
+                        der = der[len(root.origin.derivation) :]
+                    hdkey = root.key.derive(der)
+                else:
+                    hdkey = root.derive(der)
 
-            sc = inp.witness_script or inp.redeem_script or inp.utxo.script_pubkey
+                if hdkey.xonly() != pub.xonly():
+                    raise PSBTError("Derivation path doesn't look right")
+                derived_keypairs.add((hdkey.key, pub))
 
-            # taproot is special
-            # currently works only for single key
+            # sign with taproot key
             if inp.is_taproot:
-                # individual private key
-                if not fingerprint:
-                    # TODO: tweak using taproot psbt fields
-                    pk = root.taproot_tweak(b"")
-                    if pk.xonly() in sc.data:
-                        sig = pk.schnorr_sign(h)
-                        wit = sig.serialize()
-                        if inp_sighash != SIGHASH.DEFAULT:
-                            wit += bytes([inp_sighash])
-                        inp.final_scriptwitness = Witness([wit])
-                        counter += 1
-                # if we use HDKey
-                else:
-                    bip32_derivations = []
-                    for pub in inp.taproot_bip32_derivations:
-                        leaf_hashes, derivation = inp.taproot_bip32_derivations[pub]
-                        # TODO: also sign with leaf_hashes
-                        if derivation.fingerprint == fingerprint and len(leaf_hashes) == 0:
-                            bip32_derivations.append((pub, derivation))
-                    
-                    # "Legacy" support for workaround when BIP-371 Taproot psbt fields aren't available.
-                    # TODO: Remove this (and refactor above) when workaround has been phased out.
-                    for pub in inp.bip32_derivations:
-                        derivation = inp.bip32_derivations[pub]
-                        if derivation.fingerprint == fingerprint:
-                            bip32_derivations.append((pub, derivation))
-
-                    for pub, derivation in bip32_derivations:
-                        der = derivation.derivation
-                        if hasattr(root, "origin"):
-                            # for descriptor key remove origin part
-                            if root.origin:
-                                if root.origin.derivation != der[:len(root.origin.derivation)]:
-                                    continue
-                                der = der[len(root.origin.derivation):]
-                            hdkey = root.key.derive(der)
-                        else:
-                            hdkey = root.derive(der)
-                        
-                        # Taproot BIP32 derivations use X-only pubkeys
-                        xonly_pub = hdkey.key.xonly()
-                        mypub = ec.PublicKey.from_xonly(xonly_pub)
-
-                        if mypub != pub:
-                            raise PSBTError("Derivation path doesn't look right")
-                        
-                        # TODO: Support signing for keys within leaves
-                        pk = hdkey.taproot_tweak(b"")
-                        if pk.xonly() in sc.data:
-                            sig = pk.schnorr_sign(h)
-                            # sig plus sighash flag
-                            wit = sig.serialize()
-                            if inp_sighash != SIGHASH.DEFAULT:
-                                wit += bytes([inp_sighash])
-                            inp.final_scriptwitness = Witness([wit])
-                            counter += 1
+                # try to sign with individual private key (WIF)
+                # or with root without derivations
+                counter += self.sign_input_with_tapkey(
+                    root,
+                    i,
+                    inp,
+                    sighash=inp_sighash,
+                )
+                # sign with all derived keys
+                for prv, pub in derived_keypairs:
+                    counter += self.sign_input_with_tapkey(
+                        prv,
+                        i,
+                        inp,
+                        sighash=inp_sighash,
+                    )
                 continue
 
-            # if we have individual private key
-            if not fingerprint:
-                # check if we are included in the script
-                if sec in sc.data or pkh in sc.data:
-                    sig = root.sign(h)
-                    # sig plus sighash flag
-                    inp.partial_sigs[pub] = sig.serialize() + bytes([inp_sighash])
-                    counter += 1
-                continue
+            # hash can be reused
+            h = self.sighash(i, sighash=inp_sighash)
+            sc = inp.witness_script or inp.redeem_script or inp.utxo.script_pubkey
 
-            # if we use HDKey
-            for pub in inp.bip32_derivations:
-                # check if it is root key
-                if inp.bip32_derivations[pub].fingerprint == fingerprint:
-                    der = inp.bip32_derivations[pub].derivation
-                    if hasattr(root, "origin"):
-                        # for descriptor key remove origin part
-                        if root.origin:
-                            if root.origin.derivation != der[:len(root.origin.derivation)]:
-                                continue
-                            der = der[len(root.origin.derivation):]
-                        hdkey = root.key.derive(der)
-                    else:
-                        hdkey = root.derive(der)
-                    mypub = hdkey.key.get_public_key()
-                    if mypub != pub:
-                        raise PSBTError("Derivation path doesn't look right")
-                    sig = hdkey.key.sign(h)
-                    # sig plus sighash flag
-                    inp.partial_sigs[mypub] = sig.serialize() + bytes([inp_sighash])
-                    counter += 1
-        return counter
+            # check if root itself is included in the script
+            if sec in sc.data or pkh in sc.data:
+                sig = root.sign(h)
+                # sig plus sighash flag
+                inp.partial_sigs[rootpub] = sig.serialize() + bytes([inp_sighash])
+                counter += 1
+
+            for prv, pub in derived_keypairs:
+                sig = prv.sign(h)
+                # sig plus sighash flag
+                inp.partial_sigs[pub] = sig.serialize() + bytes([inp_sighash])
+                counter += 1
+        return counter
```

### Comparing `embit-0.7.0/src/embit/psbtview.py` & `embit-0.8.0/src/embit/psbtview.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,82 @@
 """
-PSBTView class is RAM-friendly implementation of PSBT that reads required data from a stream on request.
-The PSBT transaction itself passed to the class is a readable stream - it can be a file stream or a BytesIO object.
-When using files make sure they are in trusted storage - when using SD card or other untrusted source make sure
-to copy the file to a trusted media (flash, QSPI or SPIRAM for example).
-Otherwise you expose yourself to time-of-check-time-of-use style of attacks where SD card MCU can trick you
-to sign a wrong transactions.
+PSBTView class is RAM-friendly implementation of PSBT
+that reads required data from a stream on request.
+
+The PSBT transaction itself passed to the class
+is a readable stream - it can be a file stream or a BytesIO object.
+When using files make sure they are in trusted storage - when using SD card
+or other untrusted source make sure to copy the file to a trusted media
+(flash, QSPI or SPIRAM for example).
+
+Otherwise you expose yourself to time-of-check-time-of-use style of attacks
+where SD card MCU can trick you to sign a wrong transactions.
+
 Makes sense to run gc.collect() after processing of each scope to free memory.
 """
-from .psbt import *
-from .transaction import hash_amounts, hash_script_pubkeys
+# TODO: refactor, a lot of code is duplicated here from transaction.py
 import hashlib
+from . import compact
+from . import ec
+from . import script
+from .script import Script, Witness
+from . import hashes
+from .psbt import (
+    PSBTError,
+    CompressMode,
+    InputScope,
+    OutputScope,
+    read_string,
+    ser_string,
+    skip_string,
+)
+from .transaction import (
+    TransactionOutput,
+    TransactionInput,
+    SIGHASH,
+    hash_amounts,
+    hash_script_pubkeys,
+)
 
-def read_write(sin, sout, l=None, chunk_size=32) -> int:
+
+def read_write(sin, sout, sz=None, chunk_size=32) -> int:
     """Reads l or all bytes from sin and writes to sout"""
     # number of bytes written
     res = 0
     barr = bytearray(chunk_size)
     while True:
-        if l == 0: # nothing else to read
+        if sz == 0:  # nothing else to read
             return res
-        elif l and l < chunk_size: # read less than full chunk
-            r = sin.read(l)
+        elif sz and sz < chunk_size:  # read less than full chunk
+            r = sin.read(sz)
             sout.write(r)
             return res + len(r)
-        else: # reading full chunk
-            r = sin.readinto(barr)
-            if r == 0:
-                return res
-            res += r
-            if r == chunk_size:
-                sout.write(barr)
-            else:
-                sout.write(barr[:r])
-            if l:
-                l -= r
-    return res
+        # reading full chunk
+        r = sin.readinto(barr)
+        if r == 0:
+            return res
+        res += r
+        if r == chunk_size:
+            sout.write(barr)
+        else:
+            sout.write(barr[:r])
+        if sz:
+            sz -= r
+
 
 class GlobalTransactionView:
     """
     Global transaction in PSBT is
     - unsigned (with empty scriptsigs)
     - doesn't have witness
     """
-    LEN_VIN = 32 + 4 + 1 + 4 # txid, vout, scriptsig, sequence
-    NUM_VIN_OFFSET = 4 # version
+
+    LEN_VIN = 32 + 4 + 1 + 4  # txid, vout, scriptsig, sequence
+    NUM_VIN_OFFSET = 4  # version
+
     def __init__(self, stream, offset):
         self.stream = stream
         self.offset = offset
         self._num_vin = None
         self._vin0_offset = None
         self._num_vout = None
         self._vout0_offset = None
@@ -75,21 +104,27 @@
             self.stream.seek(self.vin0_offset + self.LEN_VIN * self.num_vin)
             self._num_vout = compact.read_from(self.stream)
         return self._num_vout
 
     @property
     def vin0_offset(self):
         if self._vin0_offset is None:
-            self._vin0_offset = self.offset + self.NUM_VIN_OFFSET + len(compact.to_bytes(self.num_vin))
+            self._vin0_offset = (
+                self.offset + self.NUM_VIN_OFFSET + len(compact.to_bytes(self.num_vin))
+            )
         return self._vin0_offset
 
     @property
     def vout0_offset(self):
         if self._vout0_offset is None:
-            self._vout0_offset = self.vin0_offset + self.LEN_VIN * self.num_vin + len(compact.to_bytes(self.num_vout))
+            self._vout0_offset = (
+                self.vin0_offset
+                + self.LEN_VIN * self.num_vin
+                + len(compact.to_bytes(self.num_vout))
+            )
         return self._vout0_offset
 
     @property
     def locktime(self):
         if self._locktime is None:
             self.stream.seek(self.vout0_offset)
             n = self.num_vout
@@ -117,31 +152,38 @@
         self.stream.seek(self.vout0_offset)
         n = i
         while n:
             self._skip_output()
             n -= 1
         return TransactionOutput.read_from(self.stream)
 
+
 class PSBTView:
     """
     Constructor shouldn't be used directly. PSBTView.view_from(stream) should be used instead.
     Either version should be 2 or tx_offset should be int, otherwise you get an error
     """
+
     # for subclasses like PSET
     MAGIC = b"psbt\xff"
     PSBTIN_CLS = InputScope
     PSBTOUT_CLS = OutputScope
     TX_CLS = GlobalTransactionView
 
-    def __init__(self, stream,
-            num_inputs, num_outputs,
-            offset, first_scope,
-            version=None, tx_offset=None,
-            compress=CompressMode.KEEP_ALL,
-        ):
+    def __init__(
+        self,
+        stream,
+        num_inputs,
+        num_outputs,
+        offset,
+        first_scope,
+        version=None,
+        tx_offset=None,
+        compress=CompressMode.KEEP_ALL,
+    ):
         if version != 2 and tx_offset is None:
             raise PSBTError("Global tx is not found, but PSBT version is %d" % version)
         self.version = version
         self.stream = stream
         # by default we use provided offset, tell() or 0 as default value
         self.offset = offset or 0
         self.num_inputs = num_inputs
@@ -161,15 +203,15 @@
         self._hash_sequence = None
         self._hash_outputs = None
         self._hash_amounts = None
         self._hash_script_pubkeys = None
 
     @classmethod
     def view(cls, stream, offset=None, compress=CompressMode.KEEP_ALL):
-        if offset is None and hasattr(stream, 'tell'):
+        if offset is None and hasattr(stream, "tell"):
             offset = stream.tell()
         offset = offset or 0
         # current offset
         cur = offset
         # check magic
         if stream.read(len(cls.MAGIC)) != cls.MAGIC:
             raise PSBTError("Invalid PSBT magic")
@@ -186,15 +228,15 @@
             # separator
             if len(key) == 0:
                 break
             if key in [b"\xfb", b"\x04", b"\x05"]:
                 value = read_string(stream)
                 cur += len(value) + len(compact.to_bytes(len(value)))
                 if key == b"\xfb":
-                    version = int.from_bytes(value, 'little')
+                    version = int.from_bytes(value, "little")
                 elif key == b"\x04":
                     num_inputs = compact.from_bytes(value)
                 elif key == b"\x05":
                     num_outputs = compact.from_bytes(value)
             elif key == b"\x00":
                 # we found global transaction
                 assert version != 2
@@ -209,16 +251,24 @@
                 stream.seek(tx_offset + tx_len)
                 cur += tx_len
             else:
                 cur += skip_string(stream)
         first_scope = cur
         if None in [version or tx_offset, num_inputs, num_outputs]:
             raise PSBTError("Missing something important in PSBT")
-        return cls(stream, num_inputs, num_outputs, offset,
-                   first_scope, version, tx_offset, compress)
+        return cls(
+            stream,
+            num_inputs,
+            num_outputs,
+            offset,
+            first_scope,
+            version,
+            tx_offset,
+            compress,
+        )
 
     def _skip_scope(self):
         off = 0
         while True:
             # read key and update cursor
             keylen = skip_string(self.stream)
             off += keylen
@@ -235,15 +285,15 @@
         n can be from 0 to num_inputs+num_outputs or None.
         If n = None it seeks to global scope.
         If n = num_inputs + num_outputs it seeks to the end of PSBT.
         This can be useful to check that nothing is left in the stream (i.e. for tests).
         Returns an offset at this scope.
         """
         if n is None:
-            off = self.offset+len(self.MAGIC)
+            off = self.offset + len(self.MAGIC)
             self.stream.seek(off)
             return off
         if n > self.num_inputs + self.num_outputs:
             raise PSBTError("Invalid scope number")
         # seek to first scope
         self.stream.seek(self.first_scope)
         off = self.first_scope
@@ -281,51 +331,51 @@
 
         self.seek_to_scope(i)
         v = self.get_value(b"\x0e", from_current=True)
         txid = bytes(reversed(v))
 
         self.seek_to_scope(i)
         v = self.get_value(b"\x0f", from_current=True)
-        vout = int.from_bytes(v, 'little')
+        vout = int.from_bytes(v, "little")
 
         self.seek_to_scope(i)
         v = self.get_value(b"\x10", from_current=True) or b"\xFF\xFF\xFF\xFF"
-        sequence = int.from_bytes(v, 'little')
+        sequence = int.from_bytes(v, "little")
 
         return TransactionInput(txid, vout, sequence=sequence)
 
     # compress is not used here, but may be used by subclasses (liquid)
     def vout(self, i, compress=None):
         if i < 0 or i >= self.num_outputs:
             raise PSBTError("Invalid output index")
         if self.tx:
             return self.tx.vout(i)
 
         self.seek_to_scope(self.num_inputs + i)
         v = self.get_value(b"\x03", from_current=True)
-        value = int.from_bytes(v, 'little')
+        value = int.from_bytes(v, "little")
 
         self.seek_to_scope(self.num_inputs + i)
         v = self.get_value(b"\x04", from_current=True)
         script_pubkey = Script(v)
 
         return TransactionOutput(value, script_pubkey)
 
     @property
     def locktime(self):
         if self._locktime is None:
             v = self.get_value(b"\x03")
-            self._locktime = int.from_bytes(v, 'little') if v is not None else 0
+            self._locktime = int.from_bytes(v, "little") if v is not None else 0
         return self._locktime
 
     @property
     def tx_version(self):
         if self._tx_version is None:
             v = self.get_value(b"\x02")
-            self._tx_version = int.from_bytes(v, 'little') if v is not None else 0
+            self._tx_version = int.from_bytes(v, "little") if v is not None else 0
         return self._tx_version
 
     def seek_to_value(self, key_start, from_current=False):
         """
         Seeks to value with key starting with key_start.
         Returns offset - relative if from_current=True, absolute otherwise.
         If key is not found - returns None.
@@ -386,16 +436,28 @@
         return self._hash_amounts
 
     def hash_script_pubkeys(self, script_pubkeys):
         if self._hash_script_pubkeys is None:
             self._hash_script_pubkeys = hash_script_pubkeys(script_pubkeys)
         return self._hash_script_pubkeys
 
-    def sighash_taproot(self, input_index, script_pubkeys, values, sighash=SIGHASH.DEFAULT):
+    def sighash_taproot(
+        self,
+        input_index,
+        script_pubkeys,
+        values,
+        sighash=SIGHASH.DEFAULT,
+        ext_flag=0,
+        annex=None,
+        script=None,
+        leaf_version=0xC0,
+        codeseparator_pos=None,
+    ):
         """check out bip-341"""
+        # TODO: refactor, it's almost a complete copy of tx.sighash_taproot
         if input_index < 0 or input_index >= self.num_inputs:
             raise PSBTError("Invalid input index")
         if len(values) != self.num_inputs:
             raise PSBTError("All spent amounts are required")
         sh, anyonecanpay = SIGHASH.check(sighash)
         h = hashes.tagged_hash_init("TapSighash", b"\x00")
         h.update(bytes([sighash]))
@@ -405,38 +467,51 @@
             h.update(self.hash_prevouts())
             h.update(self.hash_amounts(values))
             h.update(self.hash_script_pubkeys(script_pubkeys))
             h.update(self.hash_sequence())
         if sh not in [SIGHASH.SINGLE, SIGHASH.NONE]:
             h.update(self.hash_outputs())
         # data about this input
-        h.update(b"\x00") # ext_flags and annex are not supported
+        h.update(bytes([2 * ext_flag + int(annex is not None)]))
         if anyonecanpay:
             vin = self.vin(input_index)
             h.update(vin.serialize())
             h.update(values[input_index].to_bytes(8, "little"))
             h.update(script_pubkeys[input_index].serialize())
             h.update(vin.sequence.to_bytes(4, "little"))
         else:
             h.update(input_index.to_bytes(4, "little"))
-        # annex is not supported
+        if annex is not None:
+            h.update(hashes.sha256(compact.to_bytes(len(annex)) + annex))
         if sh == SIGHASH.SINGLE:
             h.update(self.vout(input_index).serialize())
+        if script is not None:
+            h.update(
+                hashes.tagged_hash(
+                    "TapLeaf", bytes([leaf_version]) + script.serialize()
+                )
+            )
+            h.update(b"\x00")
+            h.update(
+                b"\xff\xff\xff\xff"
+                if codeseparator_pos is None
+                else codeseparator_pos.to_bytes(4, "little")
+            )
         return h.digest()
 
     def sighash_segwit(self, input_index, script_pubkey, value, sighash=SIGHASH.ALL):
         """check out bip-143"""
         if input_index < 0 or input_index >= self.num_inputs:
             raise PSBTError("Invalid input index")
         sh, anyonecanpay = SIGHASH.check(sighash)
         # default sighash is used only in taproot
         if sh == SIGHASH.DEFAULT:
             sh = SIGHASH.ALL
         inp = self.vin(input_index)
-        zero = b"\x00"*32 # for sighashes
+        zero = b"\x00" * 32  # for sighashes
         h = hashlib.sha256()
         h.update(self.tx_version.to_bytes(4, "little"))
         if anyonecanpay:
             h.update(zero)
         else:
             h.update(hashlib.sha256(self.hash_prevouts()).digest())
         if anyonecanpay or sh in [SIGHASH.NONE, SIGHASH.SINGLE]:
@@ -444,20 +519,22 @@
         else:
             h.update(hashlib.sha256(self.hash_sequence()).digest())
         h.update(bytes(reversed(inp.txid)))
         h.update(inp.vout.to_bytes(4, "little"))
         h.update(script_pubkey.serialize())
         h.update(int(value).to_bytes(8, "little"))
         h.update(inp.sequence.to_bytes(4, "little"))
-        if not (sh in [SIGHASH.NONE, SIGHASH.SINGLE]):
+        if sh not in {SIGHASH.NONE, SIGHASH.SINGLE}:
             h.update(hashlib.sha256(self.hash_outputs()).digest())
         elif sh == SIGHASH.SINGLE and input_index < self.num_outputs:
-            h.update(hashlib.sha256(
-                hashlib.sha256(self.vout(input_index).serialize()).digest()
-            ).digest())
+            h.update(
+                hashlib.sha256(
+                    hashlib.sha256(self.vout(input_index).serialize()).digest()
+                ).digest()
+            )
         else:
             h.update(zero)
         h.update(self.locktime.to_bytes(4, "little"))
         h.update(sighash.to_bytes(4, "little"))
         return hashlib.sha256(h.digest()).digest()
 
     def sighash_legacy(self, input_index, script_pubkey, sighash=SIGHASH.ALL):
@@ -465,15 +542,15 @@
             raise PSBTError("Invalid input index")
         sh, anyonecanpay = SIGHASH.check(sighash)
         # default sighash is used only in taproot
         if sh == SIGHASH.DEFAULT:
             sh = SIGHASH.ALL
         # no corresponding output for this input, we sign 00...01
         if sh == SIGHASH.SINGLE and input_index >= self.num_outputs:
-            return b"\x00"*31+b"\x01"
+            return b"\x00" * 31 + b"\x01"
 
         h = hashlib.sha256()
         h.update(self.tx_version.to_bytes(4, "little"))
         # ANYONECANPAY - only one input is serialized
         if anyonecanpay:
             h.update(compact.to_bytes(1))
             h.update(self.vin(input_index).serialize(script_pubkey))
@@ -486,15 +563,15 @@
                 else:
                     h.update(inp.serialize(Script(b""), sighash))
         # no outputs
         if sh == SIGHASH.NONE:
             h.update(compact.to_bytes(0))
         # one output on the same index, others are empty
         elif sh == SIGHASH.SINGLE:
-            h.update(compact.to_bytes(input_index+1))
+            h.update(compact.to_bytes(input_index + 1))
             empty = TransactionOutput(0xFFFFFFFF, Script(b"")).serialize()
             # this way we commit to input index
             for i in range(input_index):
                 h.update(empty)
             # last is ours
             h.update(self.vout(input_index).serialize())
         elif sh == SIGHASH.ALL:
@@ -505,186 +582,280 @@
         else:
             # shouldn't happen
             raise PSBTError("Invalid sighash")
         h.update(self.locktime.to_bytes(4, "little"))
         h.update(sighash.to_bytes(4, "little"))
         return hashlib.sha256(h.digest()).digest()
 
-    def sighash(self, i, sighash=SIGHASH.ALL, input_scope=None):
+    def sighash(self, i, sighash=SIGHASH.ALL, input_scope=None, **kwargs):
         inp = self.input(i) if input_scope is None else input_scope
 
         if inp.is_taproot:
-            # TODO: not very optimal. Maybe use build_cache() or something?
             values = []
             scripts = []
+            # TODO: not very optimal. Maybe use build_cache() or something?
             for idx in range(self.num_inputs):
                 inp = self.input(idx)
                 values.append(inp.utxo.value)
                 scripts.append(inp.utxo.script_pubkey)
-            return self.sighash_taproot(i, script_pubkeys=scripts, values=values, sighash=sighash)
+            return self.sighash_taproot(
+                i,
+                script_pubkeys=scripts,
+                values=values,
+                sighash=sighash,
+                **kwargs,
+            )
 
         value = inp.utxo.value
         sc = inp.witness_script or inp.redeem_script or inp.utxo.script_pubkey
 
         # detect if it is a segwit input
-        is_segwit = (inp.witness_script
-                    or inp.witness_utxo
-                    or inp.utxo.script_pubkey.script_type() in {"p2wpkh", "p2wsh"}
-                    or (
-                        inp.redeem_script
-                        and inp.redeem_script.script_type() in {"p2wpkh", "p2wsh"}
-                    )
+        is_segwit = (
+            inp.witness_script
+            or inp.witness_utxo
+            or inp.utxo.script_pubkey.script_type() in {"p2wpkh", "p2wsh"}
+            or (
+                inp.redeem_script
+                and inp.redeem_script.script_type() in {"p2wpkh", "p2wsh"}
+            )
         )
         # convert to p2pkh according to bip143
         if sc.script_type() == "p2wpkh":
             sc = script.p2pkh_from_p2wpkh(sc)
 
         if is_segwit:
             h = self.sighash_segwit(i, sc, value, sighash=sighash)
         else:
             h = self.sighash_legacy(i, sc, sighash=sighash)
         return h
 
-    def sign_input(self, i, root, sig_stream, sighash=SIGHASH.DEFAULT, extra_scope_data=None) -> int:
+    def sign_input_with_tapkey(
+        self,
+        key: ec.PrivateKey,
+        input_index: int,
+        inp=None,
+        sighash=SIGHASH.DEFAULT,
+    ) -> int:
+        """Sign taproot input with key. Signs with internal or leaf key."""
+        # get input ourselves if not provided
+        inp = inp or self.input(input_index)
+        if not inp.is_taproot:
+            return 0
+        # check if key is internal key
+        pk = key.taproot_tweak(inp.taproot_merkle_root or b"")
+        if pk.xonly() in inp.utxo.script_pubkey.data:
+            h = self.sighash(
+                input_index,
+                sighash=sighash,
+            )
+            sig = pk.schnorr_sign(h)
+            wit = sig.serialize()
+            if sighash != SIGHASH.DEFAULT:
+                wit += bytes([sighash])
+            # TODO: maybe better to put into internal key sig field
+            inp.final_scriptwitness = Witness([wit])
+            # no need to sign anything else
+            return 1
+        counter = 0
+        # negate if necessary
+        pub = ec.PublicKey.from_xonly(key.xonly())
+        # iterate over leafs and sign
+        for ctrl, sc in inp.taproot_scripts.items():
+            if pub.xonly() not in sc:
+                continue
+            leaf_version = sc[-1]
+            script = Script(sc[:-1])
+            h = self.sighash(
+                input_index,
+                sighash=sighash,
+                ext_flag=1,
+                script=script,
+                leaf_version=leaf_version,
+            )
+            sig = key.schnorr_sign(h)
+            leaf = hashes.tagged_hash(
+                "TapLeaf", bytes([leaf_version]) + script.serialize()
+            )
+            sigdata = sig.serialize()
+            # append sighash if necessary
+            if sighash != SIGHASH.DEFAULT:
+                sigdata += bytes([sighash])
+            inp.taproot_sigs[(pub, leaf)] = sigdata
+            counter += 1
+        return counter
+
+    def sign_input(
+        self, i, root, sig_stream, sighash=SIGHASH.DEFAULT, extra_scope_data=None
+    ) -> int:
         """
-        Signs input taking into account additional derivation information for this input.
+        Signs input taking into account additional
+        derivation information for this input.
+
         It's helpful if your wallet knows more than provided in PSBT.
-        As PSBTView is read-only it can't change anything in PSBT, that's why you may need extra_scope_data
+        As PSBTView is read-only it can't change anything in PSBT,
+        that's why you may need extra_scope_data.
         """
         if i < 0 or i >= self.num_inputs:
             raise PSBTError("Invalid input number")
 
         # if WIF - fingerprint is None
-        fingerprint = None if not hasattr(root, "my_fingerprint") else root.my_fingerprint
-        if not fingerprint:
-            pub = root.get_public_key()
-            sec = pub.sec()
-            pkh = hashes.hash160(sec)
+        fingerprint = None
+        # if descriptor key
+        if hasattr(root, "origin"):
+            if not root.is_private:  # pubkey can't sign
+                return 0
+            if root.is_extended:  # use fingerprint only for HDKey
+                fingerprint = root.fingerprint
+            else:
+                root = root.key  # WIF key
+        # if HDKey
+        if not fingerprint and hasattr(root, "my_fingerprint"):
+            fingerprint = root.my_fingerprint
+
+        rootpub = root.get_public_key()
+        sec = rootpub.sec()
+        pkh = hashes.hash160(sec)
 
         inp = self.input(i)
         if extra_scope_data is not None:
             inp.update(extra_scope_data)
 
         # SIGHASH.DEFAULT is only for taproot, fallback to SIGHASH.ALL for other inputs
         required_sighash = sighash
         if not inp.is_taproot and required_sighash == SIGHASH.DEFAULT:
             required_sighash = SIGHASH.ALL
 
         # check which sighash to use
-        inp_sighash = inp.sighash_type or required_sighash or SIGHASH.DEFAULT
+        inp_sighash = inp.sighash_type
+        if inp_sighash is None:
+            inp_sighash = required_sighash or SIGHASH.DEFAULT
         if not inp.is_taproot and inp_sighash == SIGHASH.DEFAULT:
             inp_sighash = SIGHASH.ALL
 
-        # if input sighash is set and is different from kwarg - don't sign this input
+        # if input sighash is set and is different from required sighash
+        # we don't sign this input
+        # except DEFAULT is functionally the same as ALL
         if required_sighash is not None and inp_sighash != required_sighash:
-            return 0
+            if inp_sighash not in {
+                SIGHASH.DEFAULT,
+                SIGHASH.ALL,
+            } or required_sighash not in {SIGHASH.DEFAULT, SIGHASH.ALL}:
+                return 0
+
+        # get all possible derivations with matching fingerprint
+        bip32_derivations = set()
+        if fingerprint:
+            # if taproot derivations are present add them
+            for pub in inp.taproot_bip32_derivations:
+                (_leafs, derivation) = inp.taproot_bip32_derivations[pub]
+                if derivation.fingerprint == fingerprint:
+                    bip32_derivations.add((pub, derivation))
 
-        h = self.sighash(i, sighash=inp_sighash, input_scope=inp)
+            # segwit and legacy derivations
+            for pub in inp.bip32_derivations:
+                derivation = inp.bip32_derivations[pub]
+                if derivation.fingerprint == fingerprint:
+                    bip32_derivations.add((pub, derivation))
+
+        # get derived keys for signing
+        derived_keypairs = set()  # (prv, pub)
+        for pub, derivation in bip32_derivations:
+            der = derivation.derivation
+            # descriptor key has origin derivation that we take into account
+            if hasattr(root, "origin"):
+                if root.origin:
+                    if root.origin.derivation != der[: len(root.origin.derivation)]:
+                        # derivation doesn't match - go to next input
+                        continue
+                    der = der[len(root.origin.derivation) :]
+                hdkey = root.key.derive(der)
+            else:
+                hdkey = root.derive(der)
 
-        sc = inp.witness_script or inp.redeem_script or inp.utxo.script_pubkey
+            if hdkey.xonly() != pub.xonly():
+                raise PSBTError("Derivation path doesn't look right")
+            derived_keypairs.add((hdkey.key, pub))
 
         counter = 0
-        partial_sigs = OrderedDict()
-
-        # taproot is special
-        # currently works only for single key
+        # sign with taproot key
         if inp.is_taproot:
-            # individual private key
-            if not fingerprint:
-                # TODO: tweak using taproot psbt fields
-                pk = root.taproot_tweak(b"")
-                if pk.xonly() in sc.data:
-                    sig = pk.schnorr_sign(h)
-                    wit = sig.serialize()
-                    if inp_sighash != SIGHASH.DEFAULT:
-                        wit += bytes([inp_sighash])
-                    inp.final_scriptwitness = Witness([wit])
-                    counter = 1
-            # if we use HDKey
-            else:
-                bip32_derivations = []
-                for pub in inp.taproot_bip32_derivations:
-                    leaf_hashes, derivation = inp.taproot_bip32_derivations[pub]
-                    if derivation.fingerprint == fingerprint:
-                        bip32_derivations.append((pub, derivation))
-
-                # "Legacy" support for workaround when BIP-371 Taproot psbt fields aren't available
-                for pub in inp.bip32_derivations:
-                    derivation = inp.bip32_derivations[pub]
-                    if derivation.fingerprint == fingerprint:
-                        bip32_derivations.append((pub, derivation))
-
-                for pub, derivation in bip32_derivations:
-                    hdkey = root.derive(derivation.derivation)
-
-                    # Taproot BIP32 derivations use X-only pubkeys
-                    xonly_pub = hdkey.key.xonly()
-                    mypub = ec.PublicKey.from_xonly(xonly_pub)
-
-                    if mypub != pub:
-                        raise PSBTError("Derivation path doesn't look right")
-                    pk = hdkey.taproot_tweak(b"")
-                    if pk.xonly() in sc.data:
-                        sig = pk.schnorr_sign(h)
-                        # sig plus sighash flag
-                        wit = sig.serialize()
-                        if inp_sighash != SIGHASH.DEFAULT:
-                            wit += bytes([inp_sighash])
-                        inp.final_scriptwitness = Witness([wit])
-                        counter = 1
-            if counter:
+            # try to sign with individual private key (WIF)
+            # or with root without derivations
+            counter += self.sign_input_with_tapkey(
+                root,
+                i,
+                inp,
+                sighash=inp_sighash,
+            )
+            # sign with all derived keys
+            for prv, pub in derived_keypairs:
+                counter += self.sign_input_with_tapkey(
+                    prv,
+                    i,
+                    inp,
+                    sighash=inp_sighash,
+                )
+            if inp.final_scriptwitness:
                 ser_string(sig_stream, b"\x08")
                 ser_string(sig_stream, inp.final_scriptwitness.serialize())
+
+            for pub, leaf in inp.taproot_sigs:
+                ser_string(sig_stream, b"\x14" + pub.xonly() + leaf)
+                ser_string(sig_stream, inp.taproot_sigs[(pub, leaf)])
             return counter
 
-        # if we have individual private key
-        if not fingerprint:
-            # check if we are included in the script
-            if sec in sc.data or pkh in sc.data:
-                sig = root.sign(h)
-                # sig plus sighash flag
-                partial_sigs[pub] = sig.serialize() + bytes([inp_sighash])
-                counter += 1
-        # if we use HDKey
-        else:
-            for pub in inp.bip32_derivations:
-                # check if it is root key
-                if inp.bip32_derivations[pub].fingerprint == fingerprint:
-                    hdkey = root.derive(inp.bip32_derivations[pub].derivation)
-                    mypub = hdkey.key.get_public_key()
-                    if mypub != pub:
-                        raise PSBTError("Derivation path doesn't look right")
-                    sig = hdkey.key.sign(h)
-                    # sig plus sighash flag
-                    partial_sigs[mypub] = sig.serialize() + bytes([inp_sighash])
-                    counter += 1
-        for pub in partial_sigs:
+        h = self.sighash(i, sighash=inp_sighash, input_scope=inp)
+        sc = inp.witness_script or inp.redeem_script or inp.utxo.script_pubkey
+
+        # check if root is included in the script
+        if sec in sc.data or pkh in sc.data:
+            sig = root.sign(h)
+            # sig plus sighash flag
+            inp.partial_sigs[rootpub] = sig.serialize() + bytes([inp_sighash])
+            counter += 1
+        for prv, pub in derived_keypairs:
+            sig = prv.sign(h)
+            # sig plus sighash flag
+            inp.partial_sigs[pub] = sig.serialize() + bytes([inp_sighash])
+            counter += 1
+        for pub in inp.partial_sigs:
             ser_string(sig_stream, b"\x02" + pub.serialize())
-            ser_string(sig_stream, partial_sigs[pub])
+            ser_string(sig_stream, inp.partial_sigs[pub])
         return counter
 
     def sign_with(self, root, sig_stream, sighash=SIGHASH.DEFAULT) -> int:
         """
         Signs psbtview with root key (HDKey or similar) and writes per-input signatures to the sig_stream.
         It can be either a simple BytesIO object or a file stream open for writing.
         Returns number of signatures added to PSBT.
         Sighash kwarg is set to SIGHASH.DEFAULT, for segwit and legacy it's replaced to SIGHASH.ALL
         so if PSBT is asking to sign with a different sighash this function won't sign.
         If you want to sign with sighashes provided in the PSBT - set sighash=None.
         """
         counter = 0
         for i in range(self.num_inputs):
-            counter += self.sign_input(i, root, sig_stream, sighash=sighash)
+            # check if it's a descriptor, and sign with
+            # all private keys in this descriptor
+            if hasattr(root, "keys"):
+                for k in root.keys:
+                    if hasattr(k, "is_private") and k.is_private:
+                        counter += self.sign_input(i, k, sig_stream, sighash=sighash)
+            else:
+                # just sign with the key
+                counter += self.sign_input(i, root, sig_stream, sighash=sighash)
             # add separator
             sig_stream.write(b"\x00")
         return counter
 
-    def write_to(self, writable_stream, compress=None,
-            extra_input_streams=[],
-            extra_output_streams=[],
+    def write_to(
+        self,
+        writable_stream,
+        compress=None,
+        extra_input_streams=[],
+        extra_output_streams=[],
     ):
         """
         Writes PSBTView to stream.
         extra_input_streams and extra_output_streams
         are streams with extra per-input and per-output data that should be written to stream as well.
         For example they can contain signatures or extra derivations.
 
@@ -693,15 +864,15 @@
         For psbtv2 it will have version, tx_version, locktime, per-vin data, per-vout data and partial sigs
         """
         if compress is None:
             compress = self.compress
 
         # first we write global scope
         self.stream.seek(self.offset)
-        res = read_write(self.stream, writable_stream, self.first_scope-self.offset)
+        res = read_write(self.stream, writable_stream, self.first_scope - self.offset)
 
         # write all inputs
         for i in range(self.num_inputs):
             inp = self.input(i)
             # add extra data from extra input streams
             for s in extra_input_streams:
                 extra = InputScope.read_from(s)
```

### Comparing `embit-0.7.0/src/embit/script.py` & `embit-0.8.0/src/embit/script.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from .networks import NETWORKS
 from . import base58
 from . import bech32
 from . import hashes
 from . import compact
 from .base import EmbitBase, EmbitError
-import sys
-if sys.implementation.name == "micropython":
-    import secp256k1
-else:
-    from .util import secp256k1
 
 SIGHASH_ALL = 1
 
 
 class Script(EmbitBase):
     def __init__(self, data=b""):
         self.data = data
@@ -75,15 +70,15 @@
         l = compact.read_from(stream)
         data = stream.read(l)
         if len(data) != l:
             raise ValueError("Cant read %d bytes" % l)
         return cls(data)
 
     @classmethod
-    def from_address(cls, addr:str):
+    def from_address(cls, addr: str):
         """
         Decodes a bitcoin address and returns corresponding scriptpubkey.
         """
         return address_to_scriptpubkey(addr)
 
     def __eq__(self, other):
         return self.data == other.data
@@ -147,16 +142,15 @@
 
 
 def p2tr(pubkey, script_tree=None):
     """Return Pay-To-Taproot ScriptPubkey"""
     if script_tree is None:
         h = b""
     else:
-        raise NotImplementedError("Taproot script trees are not supported yet")
-        _, h = taproot_tree_helper(script_tree)
+        h = script_tree.tweak()
     output_pubkey = pubkey.taproot_tweak(h)
     return Script(b"\x51\x20" + output_pubkey.xonly())
 
 
 def p2pkh_from_p2wpkh(script):
     """Convert p2wpkh to p2pkh script"""
     return Script(b"\x76\xa9" + script.serialize()[2:] + b"\x88\xac")
```

### Comparing `embit-0.7.0/src/embit/slip39.py` & `embit-0.8.0/src/embit/slip39.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,13 @@
 import hmac
-import sys
 import hashlib
 from .bip39 import mnemonic_from_bytes, mnemonic_to_bytes
-
+from .misc import secure_randint
 from .wordlists.slip39 import SLIP39_WORDS
 
-try:
-    # if urandom is available from os module:
-    from os import urandom as _urandom
-except:
-    # otherwise - try reading from /dev/urandom
-    def _urandom(n):
-        with open("/dev/urandom", "rb") as f:
-            return f.read(n)
-
-def _getrandbits(k):
-    b = _urandom(k//8+1)
-    return int.from_bytes(b,'big') % (2**k)
-
-def secure_randint(vmin:int, vmax:int) -> int:
-    """
-    Normal random.randint uses PRNG that is not suitable
-    for cryptographic applications.
-    This one uses os.urandom for randomness.
-    """
-    import math
-    assert vmax > vmin
-    delta = vmax - vmin
-    nbits = math.ceil(math.log2(delta+1))
-    randn = _getrandbits(nbits)
-    while randn > delta:
-        randn = _getrandbits(nbits)
-    return vmin + randn
 
 # functions for SLIP39 checksum
 def rs1024_polymod(values):
     GEN = [
         0xE0E040,
         0x1C1C080,
         0x3838100,
@@ -101,37 +73,29 @@
         value,
     ):
         self.share_bit_length = share_bit_length
         self.id = id
         self.exponent = exponent
         self.group_index = group_index
         if group_index < 0 or group_index > 15:
-            raise ValueError(
-                "Group index should be between 0 and 15 inclusive"
-            )
+            raise ValueError("Group index should be between 0 and 15 inclusive")
         self.group_threshold = group_threshold
         if group_threshold < 1 or group_threshold > group_count:
             raise ValueError(
                 "Group threshold should be between 1 and %d inclusive" % group_count
             )
         self.group_count = group_count
         if group_count < 1 or group_count > 16:
-            raise ValueError(
-                "Group count should be between 1 and 16 inclusive"
-            )
+            raise ValueError("Group count should be between 1 and 16 inclusive")
         self.member_index = member_index
         if member_index < 0 or member_index > 15:
-            raise ValueError(
-                "Member index should be between 0 and 15 inclusive"
-            )
+            raise ValueError("Member index should be between 0 and 15 inclusive")
         self.member_threshold = member_threshold
         if member_threshold < 1 or member_threshold > 16:
-            raise ValueError(
-                "Member threshold should be between 1 and 16 inclusive"
-            )
+            raise ValueError("Member threshold should be between 1 and 16 inclusive")
         self.value = value
         self.bytes = value.to_bytes(share_bit_length // 8, "big")
 
     @classmethod
     def parse(cls, mnemonic):
         # convert mnemonic into bits
         words = mnemonic.split()
@@ -185,19 +149,20 @@
             (all_bits >> 10 * (num_words - i - 1)) & 1023 for i in range(num_words)
         ]
         checksum = rs1024_create_checksum(b"shamir", indices)
         return " ".join([SLIP39_WORDS[index] for index in indices + checksum])
 
 
 class ShareSet:
+    exp = bytearray(255)
+    log2 = bytearray(256)
+
     @classmethod
     def _load(cls):
         """Pre-computes the exponent/log for LaGrange calculation"""
-        cls.exp = [0] * 255
-        cls.log2 = [0] * 256
         cur = 1
         for i in range(255):
             cls.exp[i] = cur
             cls.log2[cur] = i
             cur = (cur << 1) ^ cur
             if cur > 255:
                 cur ^= 0x11B
@@ -337,27 +302,31 @@
         if k == 1:
             return [(0, secret)]
         else:
             r = bytes(randint(0, 255) for _ in range(num_bytes - 4))
             digest = cls.digest(r, secret)
             digest_share = digest + r
             share_data = [
-                (i, bytes(randint(0, 255) for _ in range(num_bytes))) for i in range(k - 2)
+                (i, bytes(randint(0, 255) for _ in range(num_bytes)))
+                for i in range(k - 2)
             ]
             more_data = share_data.copy()
             share_data.append((254, digest_share))
             share_data.append((255, secret))
             for i in range(k - 2, n):
                 more_data.append((i, cls.interpolate(i, share_data)))
         return more_data
 
     @classmethod
-    def generate_shares(cls, mnemonic, k, n, passphrase=b"", exponent=0, randint=secure_randint):
+    def generate_shares(
+        cls, mnemonic, k, n, passphrase=b"", exponent=0, randint=secure_randint
+    ):
         """Takes a BIP39 mnemonic along with k, n, passphrase and exponent.
-        Returns a list of SLIP39 mnemonics, any k of of which, along with the passphrase, recover the secret"""
+        Returns a list of SLIP39 mnemonics, any k of of which, along with the passphrase, recover the secret
+        """
         # convert mnemonic to a shared secret
         secret = mnemonic_to_bytes(mnemonic)
         num_bits = len(secret) * 8
         if num_bits not in (128, 256):
             raise ValueError("mnemonic must be 12 or 24 words")
         # generate id
         id = randint(0, 32767)
```

### Comparing `embit-0.7.0/src/embit/transaction.py` & `embit-0.8.0/src/embit/transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,56 @@
-import sys
-import io
 import hashlib
 from . import compact
-from .script import Script, Witness
 from . import hashes
 from .base import EmbitBase, EmbitError
+from .script import Script, Witness
+from .misc import const
+
 
 class TransactionError(EmbitError):
     pass
 
+
 # micropython doesn't support typing and Enum
 class SIGHASH:
-    DEFAULT = 0
-    ALL = 1
-    NONE = 2
-    SINGLE = 3
-    ANYONECANPAY = 0x80
+    DEFAULT = const(0)
+    ALL = const(1)
+    NONE = const(2)
+    SINGLE = const(3)
+    ANYONECANPAY = const(0x80)
 
     @classmethod
     def check(cls, sighash: int):
         anyonecanpay = False
         if sighash & cls.ANYONECANPAY:
             # remove ANYONECANPAY flag
             sighash = sighash ^ cls.ANYONECANPAY
             anyonecanpay = True
         if sighash not in [cls.DEFAULT, cls.ALL, cls.NONE, cls.SINGLE]:
             raise TransactionError("Invalid SIGHASH type")
         return sighash, anyonecanpay
 
+
 # util functions
 
+
 def hash_amounts(amounts):
     h = hashlib.sha256()
     for a in amounts:
         h.update(a.to_bytes(8, "little"))
     return h.digest()
 
+
 def hash_script_pubkeys(script_pubkeys):
     h = hashlib.sha256()
     for sc in script_pubkeys:
         h.update(sc.serialize())
     return h.digest()
 
+
 # API similar to bitcoin-cli decoderawtransaction
 
 
 class Transaction(EmbitBase):
     def __init__(self, version=2, vin=[], vout=[], locktime=0):
         self.version = version
         self.locktime = locktime
@@ -118,15 +123,17 @@
         h.update(compact.to_bytes(num_vin))
         for i in range(num_vin):
             txin = TransactionInput.read_from(stream)
             h.update(txin.serialize())
         num_vout = compact.read_from(stream)
         h.update(compact.to_bytes(num_vout))
         if idx >= num_vout or idx < 0:
-            raise TransactionError("Invalid vout index %d, max is %d" % (idx, num_vout-1))
+            raise TransactionError(
+                "Invalid vout index %d, max is %d" % (idx, num_vout - 1)
+            )
         res = None
         for i in range(num_vout):
             vout = TransactionOutput.read_from(stream)
             if idx == i:
                 res = vout
             h.update(vout.serialize())
         if is_segwit:
@@ -190,15 +197,26 @@
         return self._hash_amounts
 
     def hash_script_pubkeys(self, script_pubkeys):
         if self._hash_script_pubkeys is None:
             self._hash_script_pubkeys = hash_script_pubkeys(script_pubkeys)
         return self._hash_script_pubkeys
 
-    def sighash_taproot(self, input_index, script_pubkeys, values, sighash=SIGHASH.DEFAULT):
+    def sighash_taproot(
+        self,
+        input_index,
+        script_pubkeys,
+        values,
+        sighash=SIGHASH.DEFAULT,
+        ext_flag=0,
+        annex=None,
+        script=None,
+        leaf_version=0xC0,
+        codeseparator_pos=None,
+    ):
         """check out bip-341"""
         if input_index < 0 or input_index >= len(self.vin):
             raise TransactionError("Invalid input index")
         if len(values) != len(self.vin):
             raise TransactionError("All spent amounts are required")
         sh, anyonecanpay = SIGHASH.check(sighash)
         h = hashes.tagged_hash_init("TapSighash", b"\x00")
@@ -209,37 +227,50 @@
             h.update(self.hash_prevouts())
             h.update(self.hash_amounts(values))
             h.update(self.hash_script_pubkeys(script_pubkeys))
             h.update(self.hash_sequence())
         if sh not in [SIGHASH.SINGLE, SIGHASH.NONE]:
             h.update(self.hash_outputs())
         # data about this input
-        h.update(b"\x00") # ext_flags and annex are not supported
+        h.update(bytes([2 * ext_flag + int(annex is not None)]))
         if anyonecanpay:
             h.update(self.vin[input_index].serialize())
             h.update(values[input_index].to_bytes(8, "little"))
             h.update(script_pubkeys[input_index].serialize())
             h.update(self.vin[input_index].sequence.to_bytes(4, "little"))
         else:
             h.update(input_index.to_bytes(4, "little"))
-        # annex is not supported
+        if annex is not None:
+            h.update(hashes.sha256(compact.to_bytes(len(annex)) + annex))
         if sh == SIGHASH.SINGLE:
             h.update(self.vout[input_index].serialize())
+        if script is not None:
+            h.update(
+                hashes.tagged_hash(
+                    "TapLeaf", bytes([leaf_version]) + script.serialize()
+                )
+            )
+            h.update(b"\x00")
+            h.update(
+                b"\xff\xff\xff\xff"
+                if codeseparator_pos is None
+                else codeseparator_pos.to_bytes(4, "little")
+            )
         return h.digest()
 
     def sighash_segwit(self, input_index, script_pubkey, value, sighash=SIGHASH.ALL):
         """check out bip-143"""
         if input_index < 0 or input_index >= len(self.vin):
             raise TransactionError("Invalid input index")
         sh, anyonecanpay = SIGHASH.check(sighash)
         # default sighash is used only in taproot
         if sh == SIGHASH.DEFAULT:
             sh = SIGHASH.ALL
         inp = self.vin[input_index]
-        zero = b"\x00"*32 # for sighashes
+        zero = b"\x00" * 32  # for sighashes
         h = hashlib.sha256()
         h.update(self.version.to_bytes(4, "little"))
         if anyonecanpay:
             h.update(zero)
         else:
             h.update(hashlib.sha256(self.hash_prevouts()).digest())
         if anyonecanpay or sh in [SIGHASH.NONE, SIGHASH.SINGLE]:
@@ -250,32 +281,34 @@
         h.update(inp.vout.to_bytes(4, "little"))
         h.update(script_pubkey.serialize())
         h.update(int(value).to_bytes(8, "little"))
         h.update(inp.sequence.to_bytes(4, "little"))
         if not (sh in [SIGHASH.NONE, SIGHASH.SINGLE]):
             h.update(hashlib.sha256(self.hash_outputs()).digest())
         elif sh == SIGHASH.SINGLE and input_index < len(self.vout):
-            h.update(hashlib.sha256(
-                hashlib.sha256(self.vout[input_index].serialize()).digest()
-            ).digest())
+            h.update(
+                hashlib.sha256(
+                    hashlib.sha256(self.vout[input_index].serialize()).digest()
+                ).digest()
+            )
         else:
             h.update(zero)
         h.update(self.locktime.to_bytes(4, "little"))
         h.update(sighash.to_bytes(4, "little"))
         return hashlib.sha256(h.digest()).digest()
 
     def sighash_legacy(self, input_index, script_pubkey, sighash=SIGHASH.ALL):
         if input_index < 0 or input_index >= len(self.vin):
             raise TransactionError("Invalid input index")
         sh, anyonecanpay = SIGHASH.check(sighash)
         if sh == SIGHASH.DEFAULT:
             sh = SIGHASH.ALL
         # no corresponding output for this input, we sign 00...01
         if sh == SIGHASH.SINGLE and input_index >= len(self.vout):
-            return b"\x00"*31+b"\x01"
+            return b"\x00" * 31 + b"\x01"
 
         h = hashlib.sha256()
         h.update(self.version.to_bytes(4, "little"))
         # ANYONECANPAY - only one input is serialized
         if anyonecanpay:
             h.update(compact.to_bytes(1))
             h.update(self.vin[input_index].serialize(script_pubkey))
@@ -287,15 +320,15 @@
                 else:
                     h.update(inp.serialize(Script(b""), sighash))
         # no outputs
         if sh == SIGHASH.NONE:
             h.update(compact.to_bytes(0))
         # one output on the same index, others are empty
         elif sh == SIGHASH.SINGLE:
-            h.update(compact.to_bytes(input_index+1))
+            h.update(compact.to_bytes(input_index + 1))
             empty = TransactionOutput(0xFFFFFFFF, Script(b"")).serialize()
             # this way we commit to input index
             for i in range(input_index):
                 h.update(empty)
             # last is ours
             h.update(self.vout[input_index].serialize())
         elif sh == SIGHASH.ALL:
```

### Comparing `embit-0.7.0/src/embit/util/ctypes_secp256k1.py` & `embit-0.8.0/src/embit/util/ctypes_secp256k1.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,36 +16,42 @@
     c_uint64,
     create_string_buffer,
     CFUNCTYPE,
     POINTER,
 )
 
 _lock = threading.Lock()
+
+
 # @locked decorator
 def locked(func):
     def wrapper(*args, **kwargs):
         with _lock:
             return func(*args, **kwargs)
+
     return wrapper
 
+
 # Flags to pass to context_create.
 CONTEXT_VERIFY = 0b0100000001
 CONTEXT_SIGN = 0b1000000001
 CONTEXT_NONE = 0b0000000001
 
 # Flags to pass to ec_pubkey_serialize
 EC_COMPRESSED = 0b0100000010
 EC_UNCOMPRESSED = 0b0000000010
 
-def _copy(a:bytes) -> bytes:
+
+def _copy(a: bytes) -> bytes:
     """Ugly copy that works everywhere incl micropython"""
     if len(a) == 0:
         return b""
     return a[:1] + a[1:]
 
+
 def _find_library():
     library_path = None
     extension = ""
     if platform.system() == "Darwin":
         extension = ".dylib"
     elif platform.system() == "Linux":
         extension = ".so"
@@ -68,14 +74,15 @@
     if not library_path:
         if platform.system() == "Linux" and os.path.isfile(
             "/usr/local/lib/libsecp256k1.so.0"
         ):
             library_path = "/usr/local/lib/libsecp256k1.so.0"
     return library_path
 
+
 @locked
 def _init(flags=(CONTEXT_SIGN | CONTEXT_VERIFY)):
     library_path = _find_library()
     # meh, can't find library
     if not library_path:
         raise RuntimeError(
             "Can't find libsecp256k1 library. Make sure to compile and install it."
@@ -172,46 +179,60 @@
         c_void_p,
         c_char_p,
         c_void_p,
         c_size_t,
     ]
     secp256k1.secp256k1_ec_pubkey_combine.restype = c_int
 
+    # ecdh
+    try:
+        secp256k1.secp256k1_ecdh.argtypes = [
+            c_void_p,  # ctx
+            c_char_p,  # output
+            c_char_p,  # point
+            c_char_p,  # scalar
+            CFUNCTYPE,  # hashfp
+            c_void_p,  # data
+        ]
+        secp256k1.secp256k1_ecdh.restype = c_int
+    except:
+        pass
+
     # schnorr sig
     try:
         secp256k1.secp256k1_xonly_pubkey_from_pubkey.argtypes = [
-            c_void_p, # ctx
-            c_char_p, # xonly pubkey
-            POINTER(c_int), # parity
-            c_char_p, # pubkey
+            c_void_p,  # ctx
+            c_char_p,  # xonly pubkey
+            POINTER(c_int),  # parity
+            c_char_p,  # pubkey
         ]
         secp256k1.secp256k1_xonly_pubkey_from_pubkey.restype = c_int
 
         secp256k1.secp256k1_schnorrsig_verify.argtypes = [
-            c_void_p, # ctx
-            c_char_p, # sig
-            c_char_p, # msg
-            c_char_p, # pubkey
+            c_void_p,  # ctx
+            c_char_p,  # sig
+            c_char_p,  # msg
+            c_char_p,  # pubkey
         ]
         secp256k1.secp256k1_schnorrsig_verify.restype = c_int
 
         secp256k1.secp256k1_schnorrsig_sign.argtypes = [
-            c_void_p, # ctx
-            c_char_p, # sig
-            c_char_p, # msg
-            c_char_p, # keypair
-            c_void_p, # nonce_function
-            c_char_p, # extra data
+            c_void_p,  # ctx
+            c_char_p,  # sig
+            c_char_p,  # msg
+            c_char_p,  # keypair
+            c_void_p,  # nonce_function
+            c_char_p,  # extra data
         ]
         secp256k1.secp256k1_schnorrsig_sign.restype = c_int
 
         secp256k1.secp256k1_keypair_create.argtypes = [
-            c_void_p, # ctx
-            c_char_p, # keypair
-            c_char_p, # secret
+            c_void_p,  # ctx
+            c_char_p,  # keypair
+            c_char_p,  # secret
         ]
         secp256k1.secp256k1_keypair_create.restype = c_int
     except:
         pass
 
     # recoverable module
     try:
@@ -235,15 +256,17 @@
 
         secp256k1.secp256k1_ecdsa_recoverable_signature_serialize_compact.argtypes = [
             c_void_p,
             c_char_p,
             c_char_p,
             c_char_p,
         ]
-        secp256k1.secp256k1_ecdsa_recoverable_signature_serialize_compact.restype = c_int
+        secp256k1.secp256k1_ecdsa_recoverable_signature_serialize_compact.restype = (
+            c_int
+        )
 
         secp256k1.secp256k1_ecdsa_recoverable_signature_convert.argtypes = [
             c_void_p,
             c_char_p,
             c_char_p,
         ]
         secp256k1.secp256k1_ecdsa_recoverable_signature_convert.restype = c_int
@@ -260,165 +283,207 @@
 
     # zkp modules
     try:
         # generator module
         secp256k1.secp256k1_generator_parse.argtypes = [c_void_p, c_char_p, c_char_p]
         secp256k1.secp256k1_generator_parse.restype = c_int
 
-        secp256k1.secp256k1_generator_serialize.argtypes = [c_void_p, c_char_p, c_char_p]
+        secp256k1.secp256k1_generator_serialize.argtypes = [
+            c_void_p,
+            c_char_p,
+            c_char_p,
+        ]
         secp256k1.secp256k1_generator_serialize.restype = c_int
 
         secp256k1.secp256k1_generator_generate.argtypes = [c_void_p, c_char_p, c_char_p]
         secp256k1.secp256k1_generator_generate.restype = c_int
 
-        secp256k1.secp256k1_generator_generate_blinded.argtypes = [c_void_p, c_char_p, c_char_p, c_char_p]
+        secp256k1.secp256k1_generator_generate_blinded.argtypes = [
+            c_void_p,
+            c_char_p,
+            c_char_p,
+            c_char_p,
+        ]
         secp256k1.secp256k1_generator_generate_blinded.restype = c_int
-        
+
         # pederson commitments
-        secp256k1.secp256k1_pedersen_commitment_parse.argtypes = [c_void_p, c_char_p, c_char_p]
+        secp256k1.secp256k1_pedersen_commitment_parse.argtypes = [
+            c_void_p,
+            c_char_p,
+            c_char_p,
+        ]
         secp256k1.secp256k1_pedersen_commitment_parse.restype = c_int
 
-        secp256k1.secp256k1_pedersen_commitment_serialize.argtypes = [c_void_p, c_char_p, c_char_p]
+        secp256k1.secp256k1_pedersen_commitment_serialize.argtypes = [
+            c_void_p,
+            c_char_p,
+            c_char_p,
+        ]
         secp256k1.secp256k1_pedersen_commitment_serialize.restype = c_int
 
-        secp256k1.secp256k1_pedersen_commit.argtypes = [c_void_p, c_char_p, c_char_p, c_uint64, c_char_p]
+        secp256k1.secp256k1_pedersen_commit.argtypes = [
+            c_void_p,
+            c_char_p,
+            c_char_p,
+            c_uint64,
+            c_char_p,
+        ]
         secp256k1.secp256k1_pedersen_commit.restype = c_int
 
         secp256k1.secp256k1_pedersen_blind_generator_blind_sum.argtypes = [
-            c_void_p, # const secp256k1_context* ctx,
-            POINTER(c_uint64), # const uint64_t *value,
-            c_void_p, # const unsigned char* const* generator_blind,
-            c_void_p, # unsigned char* const* blinding_factor,
-            c_size_t, # size_t n_total,
-            c_size_t, # size_t n_inputs
+            c_void_p,  # const secp256k1_context* ctx,
+            POINTER(c_uint64),  # const uint64_t *value,
+            c_void_p,  # const unsigned char* const* generator_blind,
+            c_void_p,  # unsigned char* const* blinding_factor,
+            c_size_t,  # size_t n_total,
+            c_size_t,  # size_t n_inputs
         ]
         secp256k1.secp256k1_pedersen_blind_generator_blind_sum.restype = c_int
 
-        secp256k1.secp256k1_pedersen_verify_tally.argtypes = [c_void_p, c_void_p, c_size_t, c_void_p, c_size_t]
+        secp256k1.secp256k1_pedersen_verify_tally.argtypes = [
+            c_void_p,
+            c_void_p,
+            c_size_t,
+            c_void_p,
+            c_size_t,
+        ]
         secp256k1.secp256k1_pedersen_verify_tally.restype = c_int
 
         # rangeproof
         secp256k1.secp256k1_rangeproof_rewind.argtypes = [
-            c_void_p, # ctx
-            c_char_p, # vbf out
-            POINTER(c_uint64), # value out
-            c_char_p, # message out
-            POINTER(c_uint64), # msg out len
-            c_char_p, # nonce
-            POINTER(c_uint64), # min value
-            POINTER(c_uint64), # max value
-            c_char_p, # pedersen commitment
-            c_char_p, # range proof
-            c_uint64, # proof len
-            c_char_p, # extra commitment (scriptpubkey)
-            c_uint64, # extra len
-            c_char_p, # generator
+            c_void_p,  # ctx
+            c_char_p,  # vbf out
+            POINTER(c_uint64),  # value out
+            c_char_p,  # message out
+            POINTER(c_uint64),  # msg out len
+            c_char_p,  # nonce
+            POINTER(c_uint64),  # min value
+            POINTER(c_uint64),  # max value
+            c_char_p,  # pedersen commitment
+            c_char_p,  # range proof
+            c_uint64,  # proof len
+            c_char_p,  # extra commitment (scriptpubkey)
+            c_uint64,  # extra len
+            c_char_p,  # generator
         ]
         secp256k1.secp256k1_rangeproof_rewind.restype = c_int
 
         secp256k1.secp256k1_rangeproof_verify.argtypes = [
-            c_void_p, # ctx
-            POINTER(c_uint64), # min value
-            POINTER(c_uint64), # max value
-            c_char_p, # pedersen commitment
-            c_char_p, # proof
-            c_uint64, # proof len
-            c_char_p, # extra
-            c_uint64, # extra len
-            c_char_p, # generator
+            c_void_p,  # ctx
+            POINTER(c_uint64),  # min value
+            POINTER(c_uint64),  # max value
+            c_char_p,  # pedersen commitment
+            c_char_p,  # proof
+            c_uint64,  # proof len
+            c_char_p,  # extra
+            c_uint64,  # extra len
+            c_char_p,  # generator
         ]
         secp256k1.secp256k1_rangeproof_verify.restype = c_int
 
         secp256k1.secp256k1_rangeproof_sign.argtypes = [
-          c_void_p, # ctx
-          c_char_p, # proof
-          POINTER(c_uint64), # plen
-          c_uint64, # min_value
-          c_char_p, # commit
-          c_char_p, # blind
-          c_char_p, # nonce
-          c_int,    # exp
-          c_int,    # min_bits
-          c_uint64, # value
-          c_char_p, # message
-          c_uint64, # msg_len
-          c_char_p, # extra_commit
-          c_uint64, # extra_commit_len
-          c_char_p, # gen
+            c_void_p,  # ctx
+            c_char_p,  # proof
+            POINTER(c_uint64),  # plen
+            c_uint64,  # min_value
+            c_char_p,  # commit
+            c_char_p,  # blind
+            c_char_p,  # nonce
+            c_int,  # exp
+            c_int,  # min_bits
+            c_uint64,  # value
+            c_char_p,  # message
+            c_uint64,  # msg_len
+            c_char_p,  # extra_commit
+            c_uint64,  # extra_commit_len
+            c_char_p,  # gen
         ]
         secp256k1.secp256k1_rangeproof_sign.restype = c_int
 
         # musig
-        secp256k1.secp256k1_musig_pubkey_combine.argtypes = [c_void_p, c_void_p, c_char_p, c_void_p, c_void_p, c_size_t]
+        secp256k1.secp256k1_musig_pubkey_combine.argtypes = [
+            c_void_p,
+            c_void_p,
+            c_char_p,
+            c_void_p,
+            c_void_p,
+            c_size_t,
+        ]
         secp256k1.secp256k1_musig_pubkey_combine.restype = c_int
 
         # surjection proofs
         secp256k1.secp256k1_surjectionproof_initialize.argtypes = [
-            c_void_p, # const secp256k1_context* ctx,
-            c_char_p, # secp256k1_surjectionproof* proof,
-            POINTER(c_size_t), # size_t *input_index,
-            c_void_p, # c_char_p, # const secp256k1_fixed_asset_tag* fixed_input_tags,
-            c_size_t, # const size_t n_input_tags,
-            c_size_t, # const size_t n_input_tags_to_use,
-            c_char_p, # const secp256k1_fixed_asset_tag* fixed_output_tag,
-            c_size_t, # const size_t n_max_iterations,
-            c_char_p, # const unsigned char *random_seed32
+            c_void_p,  # const secp256k1_context* ctx,
+            c_char_p,  # secp256k1_surjectionproof* proof,
+            POINTER(c_size_t),  # size_t *input_index,
+            c_void_p,  # c_char_p, # const secp256k1_fixed_asset_tag* fixed_input_tags,
+            c_size_t,  # const size_t n_input_tags,
+            c_size_t,  # const size_t n_input_tags_to_use,
+            c_char_p,  # const secp256k1_fixed_asset_tag* fixed_output_tag,
+            c_size_t,  # const size_t n_max_iterations,
+            c_char_p,  # const unsigned char *random_seed32
         ]
         secp256k1.secp256k1_surjectionproof_initialize.restype = c_int
 
         secp256k1.secp256k1_surjectionproof_generate.argtypes = [
-            c_void_p, # const secp256k1_context* ctx,
-            c_char_p, # secp256k1_surjectionproof* proof,
-            c_char_p, # const secp256k1_generator* ephemeral_input_tags,
-            c_size_t, # size_t n_ephemeral_input_tags,
-            c_char_p, # const secp256k1_generator* ephemeral_output_tag,
-            c_size_t, # size_t input_index,
-            c_char_p, # const unsigned char *input_blinding_key,
-            c_char_p, # const unsigned char *output_blinding_key
+            c_void_p,  # const secp256k1_context* ctx,
+            c_char_p,  # secp256k1_surjectionproof* proof,
+            c_char_p,  # const secp256k1_generator* ephemeral_input_tags,
+            c_size_t,  # size_t n_ephemeral_input_tags,
+            c_char_p,  # const secp256k1_generator* ephemeral_output_tag,
+            c_size_t,  # size_t input_index,
+            c_char_p,  # const unsigned char *input_blinding_key,
+            c_char_p,  # const unsigned char *output_blinding_key
         ]
         secp256k1.secp256k1_surjectionproof_generate.restype = c_int
 
         secp256k1.secp256k1_surjectionproof_verify.argtypes = [
-            c_void_p, # const secp256k1_context* ctx,
-            c_char_p, # const secp256k1_surjectionproof* proof,
-            c_char_p, # const secp256k1_generator* ephemeral_input_tags,
-            c_size_t, # size_t n_ephemeral_input_tags,
-            c_char_p, # const secp256k1_generator* ephemeral_output_tag
+            c_void_p,  # const secp256k1_context* ctx,
+            c_char_p,  # const secp256k1_surjectionproof* proof,
+            c_char_p,  # const secp256k1_generator* ephemeral_input_tags,
+            c_size_t,  # size_t n_ephemeral_input_tags,
+            c_char_p,  # const secp256k1_generator* ephemeral_output_tag
         ]
         secp256k1.secp256k1_surjectionproof_verify.restype = c_int
 
         secp256k1.secp256k1_surjectionproof_serialize.argtypes = [
-            c_void_p, # const secp256k1_context* ctx,
-            c_char_p, # unsigned char *output,
-            POINTER(c_size_t), # size_t *outputlen,
-            c_char_p, # const secp256k1_surjectionproof *proof
+            c_void_p,  # const secp256k1_context* ctx,
+            c_char_p,  # unsigned char *output,
+            POINTER(c_size_t),  # size_t *outputlen,
+            c_char_p,  # const secp256k1_surjectionproof *proof
         ]
         secp256k1.secp256k1_surjectionproof_serialize.restype = c_int
 
         secp256k1.secp256k1_surjectionproof_serialized_size.argtypes = [
-            c_void_p, # const secp256k1_context* ctx,
-            c_char_p, # const secp256k1_surjectionproof* proof
+            c_void_p,  # const secp256k1_context* ctx,
+            c_char_p,  # const secp256k1_surjectionproof* proof
         ]
         secp256k1.secp256k1_surjectionproof_serialized_size.restype = c_size_t
 
-        secp256k1.secp256k1_surjectionproof_parse.argtypes = [c_void_p, c_char_p, c_char_p, c_size_t]
+        secp256k1.secp256k1_surjectionproof_parse.argtypes = [
+            c_void_p,
+            c_char_p,
+            c_char_p,
+            c_size_t,
+        ]
         secp256k1.secp256k1_surjectionproof_parse.restype = c_int
 
     except:
         pass
 
     secp256k1.ctx = secp256k1.secp256k1_context_create(flags)
 
     r = secp256k1.secp256k1_context_randomize(secp256k1.ctx, os.urandom(32))
 
     return secp256k1
 
 
 _secp = _init()
 
+
 # bindings equal to ones in micropython
 @locked
 def context_randomize(seed, context=_secp.ctx):
     if len(seed) != 32:
         raise ValueError("Seed should be 32 bytes long")
     if _secp.secp256k1_context_randomize(context, seed) == 0:
         raise RuntimeError("Failed to randomize context")
@@ -535,15 +600,17 @@
     if len(msg) != 32:
         raise ValueError("Message should be 32 bytes long")
     if len(secret) != 32:
         raise ValueError("Secret key should be 32 bytes long")
     if extra_data and len(extra_data) != 32:
         raise ValueError("Extra data should be 32 bytes long")
     sig = bytes(64)
-    r = _secp.secp256k1_ecdsa_sign(context, sig, msg, secret, nonce_function, extra_data)
+    r = _secp.secp256k1_ecdsa_sign(
+        context, sig, msg, secret, nonce_function, extra_data
+    )
     if r == 0:
         raise ValueError("Failed to sign")
     return sig
 
 
 @locked
 def ec_seckey_verify(secret, context=_secp.ctx):
@@ -577,14 +644,15 @@
     if len(secret) != 32 or len(tweak) != 32:
         raise ValueError("Secret and tweak should both be 32 bytes long")
     t = _copy(tweak)
     if _secp.secp256k1_ec_privkey_tweak_add(context, secret, tweak) == 0:
         raise ValueError("Failed to tweak the secret")
     return None
 
+
 @locked
 def ec_pubkey_tweak_add(pub, tweak, context=_secp.ctx):
     if len(pub) != 64:
         raise ValueError("Public key should be 64 bytes long")
     if len(tweak) != 32:
         raise ValueError("Tweak should be 32 bytes long")
     t = _copy(tweak)
@@ -640,57 +708,98 @@
     pub = bytes(64)
     pubkeys = (c_char_p * len(args))(*args)
     r = _secp.secp256k1_ec_pubkey_combine(context, pub, pubkeys, len(args))
     if r == 0:
         raise ValueError("Failed to combine pubkeys")
     return pub
 
+
+# ecdh
+@locked
+def ecdh(pubkey, scalar, hashfn=None, data=None, context=_secp.ctx):
+    if not len(pubkey) == 64:
+        raise ValueError("Pubkey should be 64 bytes long")
+    if not len(scalar) == 32:
+        raise ValueError("Scalar should be 32 bytes long")
+    secret = bytes(32)
+    if hashfn is None:
+        res = _secp.secp256k1_ecdh(context, secret, pubkey, scalar, None, None)
+    else:
+
+        def _hashfn(out, x, y):
+            x = ctypes.string_at(x, 32)
+            y = ctypes.string_at(y, 32)
+            try:
+                res = hashfn(x, y, data)
+            except Exception as e:
+                return 0
+            out = cast(out, POINTER(c_char * 32))
+            out.contents.value = res
+            return 1
+
+        HASHFN = CFUNCTYPE(c_int, c_void_p, c_void_p, c_void_p)
+        res = _secp.secp256k1_ecdh(
+            context, secret, pubkey, scalar, HASHFN(_hashfn), data
+        )
+    if res != 1:
+        raise RuntimeError("Failed to compute the shared secret")
+    return secret
+
+
 # schnorrsig
 @locked
 def xonly_pubkey_from_pubkey(pubkey, context=_secp.ctx):
-    if len(pubkey)!=64:
+    if len(pubkey) != 64:
         raise ValueError("Pubkey should be 64 bytes long")
     pointer = POINTER(c_int)
     parity = pointer(c_int(0))
     xonly_pub = bytes(64)
     res = _secp.secp256k1_xonly_pubkey_from_pubkey(context, xonly_pub, parity, pubkey)
     if res != 1:
         raise RuntimeError("Failed to convert the pubkey")
     return xonly_pub, bool(parity.contents.value)
 
+
 @locked
 def schnorrsig_verify(sig, msg, pubkey, context=_secp.ctx):
     assert len(sig) == 64
     assert len(msg) == 32
     assert len(pubkey) == 64
     res = _secp.secp256k1_schnorrsig_verify(context, sig, msg, pubkey)
     return bool(res)
 
+
 @locked
 def keypair_create(secret, context=_secp.ctx):
     assert len(secret) == 32
     keypair = bytes(96)
     r = _secp.secp256k1_keypair_create(context, keypair, secret)
     if r == 0:
         raise ValueError("Failed to create keypair")
     return keypair
 
+
 # not @locked because it uses keypair_create inside
-def schnorrsig_sign(msg, keypair, nonce_function=None, extra_data=None, context=_secp.ctx):
+def schnorrsig_sign(
+    msg, keypair, nonce_function=None, extra_data=None, context=_secp.ctx
+):
     assert len(msg) == 32
     if len(keypair) == 32:
         keypair = keypair_create(keypair, context=context)
     with _lock:
         assert len(keypair) == 96
         sig = bytes(64)
-        r = _secp.secp256k1_schnorrsig_sign(context, sig, msg, keypair, nonce_function, extra_data)
+        r = _secp.secp256k1_schnorrsig_sign(
+            context, sig, msg, keypair, nonce_function, extra_data
+        )
         if r == 0:
             raise ValueError("Failed to sign")
         return sig
 
+
 # recoverable
 @locked
 def ecdsa_sign_recoverable(msg, secret, context=_secp.ctx):
     if len(msg) != 32:
         raise ValueError("Message should be 32 bytes long")
     if len(secret) != 32:
         raise ValueError("Secret key should be 32 bytes long")
@@ -747,238 +856,347 @@
         raise ValueError("Message should be 32 bytes long")
     pub = bytes(64)
     r = _secp.secp256k1_ecdsa_recover(context, pub, sig, msghash)
     if r == 0:
         raise ValueError("Failed to recover public key")
     return pub
 
+
 # zkp modules
 
+
 @locked
 def pedersen_commitment_parse(inp, context=_secp.ctx):
-    if len(inp)!=33:
+    if len(inp) != 33:
         raise ValueError("Serialized commitment should be 33 bytes long")
     commit = bytes(64)
     r = _secp.secp256k1_pedersen_commitment_parse(context, commit, inp)
     if r == 0:
         raise ValueError("Failed to parse commitment")
     return commit
 
+
 @locked
 def pedersen_commitment_serialize(commit, context=_secp.ctx):
-    if len(commit)!=64:
+    if len(commit) != 64:
         raise ValueError("Commitment should be 64 bytes long")
     sec = bytes(33)
     r = _secp.secp256k1_pedersen_commitment_serialize(context, sec, commit)
     if r == 0:
         raise ValueError("Failed to serialize commitment")
     return sec
 
+
 @locked
 def pedersen_commit(vbf, value, gen, context=_secp.ctx):
-    if len(gen)!=64:
+    if len(gen) != 64:
         raise ValueError("Generator should be 64 bytes long")
-    if len(vbf)!=32:
+    if len(vbf) != 32:
         raise ValueError(f"Blinding factor should be 32 bytes long, not {len(vbf)}")
     commit = bytes(64)
     r = _secp.secp256k1_pedersen_commit(context, commit, vbf, value, gen)
     if r == 0:
         raise ValueError("Failed to create commitment")
     return commit
 
+
 @locked
-def pedersen_blind_generator_blind_sum(values, gens, vbfs, num_inputs, context=_secp.ctx):
+def pedersen_blind_generator_blind_sum(
+    values, gens, vbfs, num_inputs, context=_secp.ctx
+):
     vals = (c_uint64 * len(values))(*values)
     vbf = bytes(vbfs[-1])
-    p = c_char_p(vbf) # obtain a pointer of various types
-    address = cast(p,c_void_p).value
+    p = c_char_p(vbf)  # obtain a pointer of various types
+    address = cast(p, c_void_p).value
 
     vbfs_joined = (c_char_p * len(vbfs))(*vbfs[:-1], address)
     gens_joined = (c_char_p * len(gens))(*gens)
-    res = _secp.secp256k1_pedersen_blind_generator_blind_sum(context, vals, gens_joined, vbfs_joined, len(values), num_inputs)
+    res = _secp.secp256k1_pedersen_blind_generator_blind_sum(
+        context, vals, gens_joined, vbfs_joined, len(values), num_inputs
+    )
     if res == 0:
         raise ValueError("Failed to get the last blinding factor.")
     res = (c_char * 32).from_address(address).raw
     assert len(res) == 32
     return res
 
+
 @locked
 def pedersen_verify_tally(ins, outs, context=_secp.ctx):
     in_ptr = (c_char_p * len(ins))(*ins)
     out_ptr = (c_char_p * len(outs))(*outs)
-    res = _secp.secp256k1_pedersen_verify_tally(context, in_ptr, len(in_ptr), out_ptr, len(out_ptr))
+    res = _secp.secp256k1_pedersen_verify_tally(
+        context, in_ptr, len(in_ptr), out_ptr, len(out_ptr)
+    )
     return bool(res)
 
+
 # generator
 @locked
 def generator_parse(inp, context=_secp.ctx):
-    if len(inp)!=33:
+    if len(inp) != 33:
         raise ValueError("Serialized generator should be 33 bytes long")
     gen = bytes(64)
     r = _secp.secp256k1_generator_parse(context, gen, inp)
     if r == 0:
         raise ValueError("Failed to parse generator")
     return gen
 
+
 @locked
 def generator_generate(asset, context=_secp.ctx):
-    if len(asset)!=32:
+    if len(asset) != 32:
         raise ValueError("Asset should be 32 bytes long")
     gen = bytes(64)
     r = _secp.secp256k1_generator_generate(context, gen, asset)
     if r == 0:
         raise ValueError("Failed to generate generator")
     return gen
 
+
 @locked
 def generator_generate_blinded(asset, abf, context=_secp.ctx):
-    if len(asset)!=32:
+    if len(asset) != 32:
         raise ValueError("Asset should be 32 bytes long")
-    if len(abf)!=32:
+    if len(abf) != 32:
         raise ValueError("Asset blinding factor should be 32 bytes long")
     gen = bytes(64)
     r = _secp.secp256k1_generator_generate_blinded(context, gen, asset, abf)
     if r == 0:
         raise ValueError("Failed to generate generator")
     return gen
 
+
 @locked
 def generator_serialize(generator, context=_secp.ctx):
-    if len(generator)!=64:
+    if len(generator) != 64:
         raise ValueError("Generator should be 64 bytes long")
     sec = bytes(33)
     if _secp.secp256k1_generator_serialize(context, sec, generator) == 0:
         raise RuntimeError("Failed to serialize generator")
     return sec
 
+
 # rangeproof
 @locked
-def rangeproof_rewind(proof, nonce, value_commitment, script_pubkey, generator, message_length=64, context=_secp.ctx):
-    if len(generator)!=64:
+def rangeproof_rewind(
+    proof,
+    nonce,
+    value_commitment,
+    script_pubkey,
+    generator,
+    message_length=64,
+    context=_secp.ctx,
+):
+    if len(generator) != 64:
         raise ValueError("Generator should be 64 bytes long")
-    if len(nonce)!=32:
+    if len(nonce) != 32:
         raise ValueError("Nonce should be 32 bytes long")
-    if len(value_commitment)!=64:
+    if len(value_commitment) != 64:
         raise ValueError("Value commitment should be 64 bytes long")
 
     pointer = POINTER(c_uint64)
 
-    msg = b"\x00"*message_length
+    msg = b"\x00" * message_length
     msglen = pointer(c_uint64(len(msg)))
 
-    vbf_out = b"\x00"*32
+    vbf_out = b"\x00" * 32
     value_out = pointer(c_uint64(0))
     min_value = pointer(c_uint64(0))
     max_value = pointer(c_uint64(0))
-    res = _secp.secp256k1_rangeproof_rewind(context, vbf_out, value_out,
-                            msg, msglen,
-                            nonce, min_value, max_value,
-                            value_commitment, proof, len(proof),
-                            script_pubkey, len(script_pubkey),
-                            generator)
+    res = _secp.secp256k1_rangeproof_rewind(
+        context,
+        vbf_out,
+        value_out,
+        msg,
+        msglen,
+        nonce,
+        min_value,
+        max_value,
+        value_commitment,
+        proof,
+        len(proof),
+        script_pubkey,
+        len(script_pubkey),
+        generator,
+    )
     if res != 1:
         raise RuntimeError("Failed to rewind the proof")
-    return value_out.contents.value, vbf_out, msg[:msglen.contents.value], min_value.contents.value, max_value.contents.value
+    return (
+        value_out.contents.value,
+        vbf_out,
+        msg[: msglen.contents.value],
+        min_value.contents.value,
+        max_value.contents.value,
+    )
+
 
 # rangeproof
 
+
 @locked
-def rangeproof_verify(proof, value_commitment, script_pubkey, generator, context=_secp.ctx):
-    if len(generator)!=64:
+def rangeproof_verify(
+    proof, value_commitment, script_pubkey, generator, context=_secp.ctx
+):
+    if len(generator) != 64:
         raise ValueError("Generator should be 64 bytes long")
-    if len(value_commitment)!=64:
+    if len(value_commitment) != 64:
         raise ValueError("Value commitment should be 64 bytes long")
 
     pointer = POINTER(c_uint64)
     min_value = pointer(c_uint64(0))
     max_value = pointer(c_uint64(0))
     res = _secp.secp256k1_rangeproof_verify(
         context,
         min_value,
         max_value,
         value_commitment,
-        proof, len(proof),
-        script_pubkey, len(script_pubkey),
+        proof,
+        len(proof),
+        script_pubkey,
+        len(script_pubkey),
         generator,
     )
     if res != 1:
         raise RuntimeError("Failed to verify the proof")
     return min_value.contents.value, max_value.contents.value
 
+
 @locked
-def rangeproof_sign(nonce, value, value_commitment, vbf, message, extra, gen, min_value=1, exp=0, min_bits=52, context=_secp.ctx):
+def rangeproof_sign(
+    nonce,
+    value,
+    value_commitment,
+    vbf,
+    message,
+    extra,
+    gen,
+    min_value=1,
+    exp=0,
+    min_bits=52,
+    context=_secp.ctx,
+):
     if value == 0:
         min_value = 0
-    if len(gen)!=64:
+    if len(gen) != 64:
         raise ValueError("Generator should be 64 bytes long")
-    if len(nonce)!=32:
+    if len(nonce) != 32:
         raise ValueError("Nonce should be 32 bytes long")
-    if len(value_commitment)!=64:
+    if len(value_commitment) != 64:
         raise ValueError("Value commitment should be 64 bytes long")
-    if len(vbf)!=32:
+    if len(vbf) != 32:
         raise ValueError("Value blinding factor should be 32 bytes long")
     proof = bytes(5134)
     pointer = POINTER(c_uint64)
     prooflen = pointer(c_uint64(len(proof)))
-    res = _secp.secp256k1_rangeproof_sign(context, proof, prooflen,
-                min_value, value_commitment, vbf, nonce,
-                exp, min_bits, value, message, len(message), extra, len(extra), gen)
+    res = _secp.secp256k1_rangeproof_sign(
+        context,
+        proof,
+        prooflen,
+        min_value,
+        value_commitment,
+        vbf,
+        nonce,
+        exp,
+        min_bits,
+        value,
+        message,
+        len(message),
+        extra,
+        len(extra),
+        gen,
+    )
     if res != 1:
         raise RuntimeError("Failed to generate the proof")
-    return bytes(proof[:prooflen.contents.value])
+    return bytes(proof[: prooflen.contents.value])
+
 
 @locked
 def musig_pubkey_combine(*args, context=_secp.ctx):
     pub = bytes(64)
     # TODO: strange that behaviour is different from pubkey_combine...
-    pubkeys = b"".join(args) # (c_char_p * len(args))(*args)
-    res = _secp.secp256k1_musig_pubkey_combine(context, None, pub, None, pubkeys, len(args))
+    pubkeys = b"".join(args)  # (c_char_p * len(args))(*args)
+    res = _secp.secp256k1_musig_pubkey_combine(
+        context, None, pub, None, pubkeys, len(args)
+    )
     if res == 0:
         raise ValueError("Failed to combine pubkeys")
     return pub
 
+
 # surjection proof
 @locked
-def surjectionproof_initialize(in_tags, out_tag, seed, tags_to_use=None, iterations=100, context=_secp.ctx):
+def surjectionproof_initialize(
+    in_tags, out_tag, seed, tags_to_use=None, iterations=100, context=_secp.ctx
+):
     if tags_to_use is None:
         tags_to_use = min(3, len(in_tags))
     if seed is None:
         seed = os.urandom(32)
-    proof = bytes(4+8+256//8+32*257)
+    proof = bytes(4 + 8 + 256 // 8 + 32 * 257)
     pointer = POINTER(c_size_t)
     input_index = pointer(c_size_t(0))
     input_tags = b"".join(in_tags)
-    res = _secp.secp256k1_surjectionproof_initialize(context, proof, input_index, input_tags, len(in_tags), tags_to_use, out_tag, iterations, seed)
+    res = _secp.secp256k1_surjectionproof_initialize(
+        context,
+        proof,
+        input_index,
+        input_tags,
+        len(in_tags),
+        tags_to_use,
+        out_tag,
+        iterations,
+        seed,
+    )
     if res == 0:
         raise RuntimeError("Failed to initialize the proof")
     return proof, input_index.contents.value
 
+
 @locked
-def surjectionproof_generate(proof, in_idx, in_tags, out_tag, in_abf, out_abf, context=_secp.ctx):
-    res = _secp.secp256k1_surjectionproof_generate(context, proof, b"".join(in_tags), len(in_tags), out_tag, in_idx, in_abf, out_abf)
+def surjectionproof_generate(
+    proof, in_idx, in_tags, out_tag, in_abf, out_abf, context=_secp.ctx
+):
+    res = _secp.secp256k1_surjectionproof_generate(
+        context,
+        proof,
+        b"".join(in_tags),
+        len(in_tags),
+        out_tag,
+        in_idx,
+        in_abf,
+        out_abf,
+    )
     if not res:
         raise RuntimeError("Failed to generate surjection proof")
     return proof
 
+
 @locked
 def surjectionproof_verify(proof, in_tags, out_tag, context=_secp.ctx):
-    res = _secp.secp256k1_surjectionproof_verify(context, proof, b"".join(in_tags), len(in_tags), out_tag)
+    res = _secp.secp256k1_surjectionproof_verify(
+        context, proof, b"".join(in_tags), len(in_tags), out_tag
+    )
     return bool(res)
 
+
 @locked
 def surjectionproof_serialize(proof, context=_secp.ctx):
     s = _secp.secp256k1_surjectionproof_serialized_size(context, proof)
     b = bytes(s)
     pointer = POINTER(c_size_t)
     sz = pointer(c_size_t(s))
     _secp.secp256k1_surjectionproof_serialize(context, b, sz, proof)
     if s != sz.contents.value:
         raise RuntimeError("Failed to serialize surjection proof - size mismatch")
     return b
 
+
 @locked
 def surjectionproof_parse(proof, context=_secp.ctx):
-    parsed_proof = bytes(4+8+256//8+32*257)
-    res = _secp.secp256k1_surjectionproof_parse(context, parsed_proof, proof, len(proof))
+    parsed_proof = bytes(4 + 8 + 256 // 8 + 32 * 257)
+    res = _secp.secp256k1_surjectionproof_parse(
+        context, parsed_proof, proof, len(proof)
+    )
     if res == 0:
         raise RuntimeError("Failed to parse surjection proof")
     return parsed_proof
```

### Comparing `embit-0.7.0/src/embit/util/key.py` & `embit-0.8.0/src/embit/util/key.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 Copy-paste from key.py in bitcoin test_framework.
 This is a fallback option if the library can't do ctypes bindings to secp256k1 library.
 """
 import random
 import hmac
 import hashlib
 
+
 def TaggedHash(tag, data):
-    ss = hashlib.sha256(tag.encode('utf-8')).digest()
+    ss = hashlib.sha256(tag.encode("utf-8")).digest()
     ss += ss
     ss += data
     return hashlib.sha256(ss).digest()
 
+
 def modinv(a, n):
     """Compute the modular inverse of a modulo n using the extended Euclidean
     Algorithm. See https://en.wikipedia.org/wiki/Extended_Euclidean_algorithm#Modular_integers.
     """
     # TODO: Change to pow(a, -1, n) available in Python 3.8
     t1, t2 = 0, 1
     r1, r2 = n, a
@@ -35,15 +37,16 @@
 
 
 def jacobi_symbol(n, k):
     """Compute the Jacobi symbol of n modulo k
 
     See http://en.wikipedia.org/wiki/Jacobi_symbol
 
-    For our application k is always prime, so this is the same as the Legendre symbol."""
+    For our application k is always prime, so this is the same as the Legendre symbol.
+    """
     assert k > 0 and k & 1, "jacobi symbol is only defined for positive odd k"
     n %= k
     t = 0
     while n != 0:
         while n & 1 == 0:
             n >>= 1
             r = k & 7
@@ -86,15 +89,15 @@
         """Convert a Jacobian point tuple p1 to affine form, or None if at infinity.
 
         An affine point is represented as the Jacobian (x, y, 1)"""
         x1, y1, z1 = p1
         if z1 == 0:
             return None
         inv = modinv(z1, self.p)
-        inv_2 = (inv ** 2) % self.p
+        inv_2 = (inv**2) % self.p
         inv_3 = (inv_2 * inv) % self.p
         return ((inv_2 * x1) % self.p, (inv_3 * y1) % self.p, 1)
 
     def has_even_y(self, p1):
         """Whether the point p1 has an even Y coordinate when expressed in affine coordinates."""
         return not (p1[2] == 0 or self.affine(p1)[1] & 1)
 
@@ -133,116 +136,119 @@
         if y is None:
             return None
         return (x, self.p - y if y & 1 else y, 1)
 
     def double(self, p1):
         """Double a Jacobian tuple p1
 
-        See https://en.wikibooks.org/wiki/Cryptography/Prime_Curve/Jacobian_Coordinates - Point Doubling"""
+        See https://en.wikibooks.org/wiki/Cryptography/Prime_Curve/Jacobian_Coordinates - Point Doubling
+        """
         x1, y1, z1 = p1
         if z1 == 0:
             return (0, 1, 0)
-        y1_2 = (y1 ** 2) % self.p
-        y1_4 = (y1_2 ** 2) % self.p
-        x1_2 = (x1 ** 2) % self.p
+        y1_2 = (y1**2) % self.p
+        y1_4 = (y1_2**2) % self.p
+        x1_2 = (x1**2) % self.p
         s = (4 * x1 * y1_2) % self.p
         m = 3 * x1_2
         if self.a:
             m += self.a * pow(z1, 4, self.p)
         m = m % self.p
-        x2 = (m ** 2 - 2 * s) % self.p
+        x2 = (m**2 - 2 * s) % self.p
         y2 = (m * (s - x2) - 8 * y1_4) % self.p
         z2 = (2 * y1 * z1) % self.p
         return (x2, y2, z2)
 
     def add_mixed(self, p1, p2):
         """Add a Jacobian tuple p1 and an affine tuple p2
 
-        See https://en.wikibooks.org/wiki/Cryptography/Prime_Curve/Jacobian_Coordinates - Point Addition (with affine point)"""
+        See https://en.wikibooks.org/wiki/Cryptography/Prime_Curve/Jacobian_Coordinates - Point Addition (with affine point)
+        """
         x1, y1, z1 = p1
         x2, y2, z2 = p2
         assert z2 == 1
         # Adding to the point at infinity is a no-op
         if z1 == 0:
             return p2
-        z1_2 = (z1 ** 2) % self.p
+        z1_2 = (z1**2) % self.p
         z1_3 = (z1_2 * z1) % self.p
         u2 = (x2 * z1_2) % self.p
         s2 = (y2 * z1_3) % self.p
         if x1 == u2:
             if y1 != s2:
                 # p1 and p2 are inverses. Return the point at infinity.
                 return (0, 1, 0)
             # p1 == p2. The formulas below fail when the two points are equal.
             return self.double(p1)
         h = u2 - x1
         r = s2 - y1
-        h_2 = (h ** 2) % self.p
+        h_2 = (h**2) % self.p
         h_3 = (h_2 * h) % self.p
         u1_h_2 = (x1 * h_2) % self.p
-        x3 = (r ** 2 - h_3 - 2 * u1_h_2) % self.p
+        x3 = (r**2 - h_3 - 2 * u1_h_2) % self.p
         y3 = (r * (u1_h_2 - x3) - y1 * h_3) % self.p
         z3 = (h * z1) % self.p
         return (x3, y3, z3)
 
     def add(self, p1, p2):
         """Add two Jacobian tuples p1 and p2
 
-        See https://en.wikibooks.org/wiki/Cryptography/Prime_Curve/Jacobian_Coordinates - Point Addition"""
+        See https://en.wikibooks.org/wiki/Cryptography/Prime_Curve/Jacobian_Coordinates - Point Addition
+        """
         x1, y1, z1 = p1
         x2, y2, z2 = p2
         # Adding the point at infinity is a no-op
         if z1 == 0:
             return p2
         if z2 == 0:
             return p1
         # Adding an Affine to a Jacobian is more efficient since we save field multiplications and squarings when z = 1
         if z1 == 1:
             return self.add_mixed(p2, p1)
         if z2 == 1:
             return self.add_mixed(p1, p2)
-        z1_2 = (z1 ** 2) % self.p
+        z1_2 = (z1**2) % self.p
         z1_3 = (z1_2 * z1) % self.p
-        z2_2 = (z2 ** 2) % self.p
+        z2_2 = (z2**2) % self.p
         z2_3 = (z2_2 * z2) % self.p
         u1 = (x1 * z2_2) % self.p
         u2 = (x2 * z1_2) % self.p
         s1 = (y1 * z2_3) % self.p
         s2 = (y2 * z1_3) % self.p
         if u1 == u2:
             if s1 != s2:
                 # p1 and p2 are inverses. Return the point at infinity.
                 return (0, 1, 0)
             # p1 == p2. The formulas below fail when the two points are equal.
             return self.double(p1)
         h = u2 - u1
         r = s2 - s1
-        h_2 = (h ** 2) % self.p
+        h_2 = (h**2) % self.p
         h_3 = (h_2 * h) % self.p
         u1_h_2 = (u1 * h_2) % self.p
-        x3 = (r ** 2 - h_3 - 2 * u1_h_2) % self.p
+        x3 = (r**2 - h_3 - 2 * u1_h_2) % self.p
         y3 = (r * (u1_h_2 - x3) - s1 * h_3) % self.p
         z3 = (h * z1 * z2) % self.p
         return (x3, y3, z3)
 
     def mul(self, ps):
         """Compute a (multi) point multiplication
 
         ps is a list of (Jacobian tuple, scalar) pairs.
         """
         r = (0, 1, 0)
         for i in range(255, -1, -1):
             r = self.double(r)
-            for (p, n) in ps:
+            for p, n in ps:
                 if (n >> i) & 1:
                     r = self.add(r, p)
         return r
 
 
-SECP256K1_FIELD_SIZE = 2 ** 256 - 2 ** 32 - 977
+SECP256K1_FIELD_SIZE = 2**256 - 2**32 - 977
 SECP256K1 = EllipticCurve(SECP256K1_FIELD_SIZE, 0, 7)
 SECP256K1_G = (
     0x79BE667EF9DCBBAC55A06295CE870B07029BFCDB2DCE28D959F2815B16F81798,
     0x483ADA7726A3C4655DA4FBFC0E1108A8FD17B448A68554199C47D08FFB10D4B8,
     1,
 )
 SECP256K1_ORDER = 0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFEBAAEDCE6AF48A03BBFD25E8CD0364141
@@ -508,61 +514,84 @@
     if t >= SECP256K1_ORDER:
         return None
     Q = SECP256K1.affine(SECP256K1.mul([(SECP256K1_G, t), (P, 1)]))
     if Q is None:
         return None
     return (Q[0].to_bytes(32, "big"), not SECP256K1.has_even_y(Q))
 
+
 def verify_schnorr(key, sig, msg):
     """Verify a Schnorr signature (see BIP 340).
     - key is a 32-byte xonly pubkey (computed using compute_xonly_pubkey).
     - sig is a 64-byte Schnorr signature
     - msg is a 32-byte message
     """
     assert len(key) == 32
     assert len(msg) == 32
     assert len(sig) == 64
 
-    x_coord = int.from_bytes(key, 'big')
+    x_coord = int.from_bytes(key, "big")
     if x_coord == 0 or x_coord >= SECP256K1_FIELD_SIZE:
         return False
     P = SECP256K1.lift_x(x_coord)
     if P is None:
         return False
-    r = int.from_bytes(sig[0:32], 'big')
+    r = int.from_bytes(sig[0:32], "big")
     if r >= SECP256K1_FIELD_SIZE:
         return False
-    s = int.from_bytes(sig[32:64], 'big')
+    s = int.from_bytes(sig[32:64], "big")
     if s >= SECP256K1_ORDER:
         return False
-    e = int.from_bytes(TaggedHash("BIP0340/challenge", sig[0:32] + key + msg), 'big') % SECP256K1_ORDER
+    e = (
+        int.from_bytes(TaggedHash("BIP0340/challenge", sig[0:32] + key + msg), "big")
+        % SECP256K1_ORDER
+    )
     R = SECP256K1.mul([(SECP256K1_G, s), (P, SECP256K1_ORDER - e)])
     if not SECP256K1.has_even_y(R):
         return False
     if ((r * R[2] * R[2]) % SECP256K1_FIELD_SIZE) != R[0]:
         return False
     return True
 
+
 def sign_schnorr(key, msg, aux=None, flip_p=False, flip_r=False):
     """Create a Schnorr signature (see BIP 340)."""
 
     assert len(key) == 32
     assert len(msg) == 32
     if aux is not None:
         assert len(aux) == 32
 
-    sec = int.from_bytes(key, 'big')
+    sec = int.from_bytes(key, "big")
     if sec == 0 or sec >= SECP256K1_ORDER:
         return None
     P = SECP256K1.affine(SECP256K1.mul([(SECP256K1_G, sec)]))
     if SECP256K1.has_even_y(P) == flip_p:
         sec = SECP256K1_ORDER - sec
     if aux is not None:
-        t = (sec ^ int.from_bytes(TaggedHash("BIP0340/aux", aux), 'big')).to_bytes(32, 'big')
+        t = (sec ^ int.from_bytes(TaggedHash("BIP0340/aux", aux), "big")).to_bytes(
+            32, "big"
+        )
     else:
-        t = sec.to_bytes(32, 'big')
-    kp = int.from_bytes(TaggedHash("BIP0340/nonce", t + P[0].to_bytes(32, 'big') + msg), 'big') % SECP256K1_ORDER
+        t = sec.to_bytes(32, "big")
+    kp = (
+        int.from_bytes(
+            TaggedHash("BIP0340/nonce", t + P[0].to_bytes(32, "big") + msg), "big"
+        )
+        % SECP256K1_ORDER
+    )
     assert kp != 0
     R = SECP256K1.affine(SECP256K1.mul([(SECP256K1_G, kp)]))
     k = kp if SECP256K1.has_even_y(R) != flip_r else SECP256K1_ORDER - kp
-    e = int.from_bytes(TaggedHash("BIP0340/challenge", R[0].to_bytes(32, 'big') + P[0].to_bytes(32, 'big') + msg), 'big') % SECP256K1_ORDER
-    return R[0].to_bytes(32, 'big') + ((k + e * sec) % SECP256K1_ORDER).to_bytes(32, 'big')
+    e = (
+        int.from_bytes(
+            TaggedHash(
+                "BIP0340/challenge",
+                R[0].to_bytes(32, "big") + P[0].to_bytes(32, "big") + msg,
+            ),
+            "big",
+        )
+        % SECP256K1_ORDER
+    )
+    return R[0].to_bytes(32, "big") + ((k + e * sec) % SECP256K1_ORDER).to_bytes(
+        32, "big"
+    )
```

### Comparing `embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_darwin_arm64.dylib` & `embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_darwin_arm64.dylib`

 * *Files identical despite different names*

### Comparing `embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_darwin_x86_64.dylib` & `embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_darwin_x86_64.dylib`

 * *Files identical despite different names*

### Comparing `embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_linux_aarch64.so` & `embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_linux_aarch64.so`

 * *Files identical despite different names*

### Comparing `embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_linux_armv6l.so` & `embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_linux_armv6l.so`

 * *Files identical despite different names*

### Comparing `embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_linux_armv7l.so` & `embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_linux_armv7l.so`

 * *Files identical despite different names*

### Comparing `embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_linux_x86_64.so` & `embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_linux_x86_64.so`

 * *Files identical despite different names*

### Comparing `embit-0.7.0/src/embit/util/prebuilt/libsecp256k1_windows_amd64.dll` & `embit-0.8.0/src/embit/util/prebuilt/libsecp256k1_windows_amd64.dll`

 * *Files identical despite different names*

### Comparing `embit-0.7.0/src/embit/util/py_secp256k1.py` & `embit-0.8.0/src/embit/util/py_secp256k1.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     return s2.to_bytes(32, "big")
 
 
 def ec_pubkey_negate(pubkey, context=None):
     if len(pubkey) != 64:
         raise ValueError("Pubkey should be a 64-byte structure")
     sec = ec_pubkey_serialize(pubkey)
-    return ec_pubkey_parse(bytes([0x05-sec[0]]) + sec[1:])
+    return ec_pubkey_parse(bytes([0x05 - sec[0]]) + sec[1:])
 
 
 def ec_privkey_tweak_add(secret, tweak, context=None):
     res = ec_privkey_add(secret, tweak)
     for i in range(len(secret)):
         secret[i] = res[i]
 
@@ -268,44 +268,50 @@
 #     r = _secp.secp256k1_ec_pubkey_combine(context, pub, pubkeys, len(args))
 #     if r == 0:
 #         raise ValueError("Failed to negate pubkey")
 #     return pub
 
 # schnorrsig
 
+
 def xonly_pubkey_from_pubkey(pubkey, context=None):
-    if len(pubkey)!=64:
+    if len(pubkey) != 64:
         raise ValueError("Pubkey should be 64 bytes long")
     sec = ec_pubkey_serialize(pubkey)
-    parity = (sec[0] == 0x03)
-    pub = ec_pubkey_parse(b"\x02"+sec[1:33])
+    parity = sec[0] == 0x03
+    pub = ec_pubkey_parse(b"\x02" + sec[1:33])
     return pub, parity
 
+
 def schnorrsig_verify(sig, msg, pubkey, context=None):
     assert len(sig) == 64
     assert len(msg) == 32
     assert len(pubkey) == 64
     sec = ec_pubkey_serialize(pubkey)
     return _key.verify_schnorr(sec[1:33], sig, msg)
 
+
 def keypair_create(secret, context=None):
     pub = ec_pubkey_create(secret)
     pub2, parity = xonly_pubkey_from_pubkey(pub)
     keypair = secret + pub
     return keypair
 
+
 def schnorrsig_sign(msg, keypair, nonce_function=None, extra_data=None, context=None):
     assert len(msg) == 32
     if len(keypair) == 32:
         keypair = keypair_create(keypair, context=context)
     assert len(keypair) == 96
     return _key.sign_schnorr(keypair[:32], msg, extra_data)
 
+
 # recoverable
 
+
 def ecdsa_sign_recoverable(msg, secret, context=None):
     sig = ecdsa_sign(msg, secret)
     pub = ec_pubkey_create(secret)
     # Search for correct index. Not efficient but I am lazy.
     # For efficiency use c-bindings to libsecp256k1
     for i in range(4):
         if ecdsa_recover(sig + bytes([i]), msg) == pub:
```

### Comparing `embit-0.7.0/src/embit/wordlists/base.py` & `embit-0.8.0/src/embit/wordlists/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 class WordlistBase:
     def __init__(self, mod):
         self._mod = mod
 
     def __getitem__(self, n):
         if isinstance(n, slice):
-            (start, stop, step) = (n.start or 0, n.stop if n.stop is not None else len(self), n.step or 1)
+            (start, stop, step) = (
+                n.start or 0,
+                n.stop if n.stop is not None else len(self),
+                n.step or 1,
+            )
             if start < 0:
                 start += len(self)
             if stop < 0:
                 stop += len(self)
             return [self._mod.get(i) for i in range(start, stop, step)]
         if n < 0:
             n = len(self) + n
@@ -22,8 +26,8 @@
     def index(self, word):
         idx = self._mod.index(word)
         if idx < 0:
             raise ValueError
         return idx
 
     def __contains__(self, word):
-        return (self._mod.index(word) >= 0)
+        return self._mod.index(word) >= 0
```

### Comparing `embit-0.7.0/src/embit/wordlists/bip39.py` & `embit-0.8.0/src/embit/wordlists/bip39.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2043,8 +2043,8 @@
     "you",
     "young",
     "youth",
     "zebra",
     "zero",
     "zone",
     "zoo",
-]
+]
```

### Comparing `embit-0.7.0/src/embit/wordlists/slip39.py` & `embit-0.8.0/src/embit/wordlists/slip39.py`

 * *Files identical despite different names*

### Comparing `embit-0.7.0/src/embit.egg-info/SOURCES.txt` & `embit-0.8.0/src/embit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,42 @@
+LICENSE
 README.md
-setup.cfg
+pyproject.toml
 setup.py
 src/embit/__init__.py
 src/embit/base.py
 src/embit/base58.py
 src/embit/bech32.py
 src/embit/bip32.py
 src/embit/bip39.py
 src/embit/bip85.py
 src/embit/compact.py
 src/embit/ec.py
 src/embit/finalizer.py
 src/embit/hashes.py
+src/embit/misc.py
 src/embit/networks.py
 src/embit/psbt.py
 src/embit/psbtview.py
 src/embit/script.py
 src/embit/slip39.py
 src/embit/transaction.py
 src/embit.egg-info/PKG-INFO
 src/embit.egg-info/SOURCES.txt
 src/embit.egg-info/dependency_links.txt
+src/embit.egg-info/requires.txt
 src/embit.egg-info/top_level.txt
 src/embit/descriptor/__init__.py
 src/embit/descriptor/arguments.py
 src/embit/descriptor/base.py
 src/embit/descriptor/checksum.py
 src/embit/descriptor/descriptor.py
 src/embit/descriptor/errors.py
 src/embit/descriptor/miniscript.py
+src/embit/descriptor/taptree.py
 src/embit/liquid/__init__.py
 src/embit/liquid/addresses.py
 src/embit/liquid/blech32.py
 src/embit/liquid/blip32.py
 src/embit/liquid/descriptor.py
 src/embit/liquid/finalizer.py
 src/embit/liquid/networks.py
```

