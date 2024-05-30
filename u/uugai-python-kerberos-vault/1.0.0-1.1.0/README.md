# Comparing `tmp/uugai_python_kerberos_vault-1.0.0.tar.gz` & `tmp/uugai_python_kerberos_vault-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uugai_python_kerberos_vault-1.0.0.tar", last modified: Thu May 30 10:32:35 2024, max compression
+gzip compressed data, was "uugai_python_kerberos_vault-1.1.0.tar", last modified: Thu May 30 10:45:55 2024, max compression
```

## Comparing `uugai_python_kerberos_vault-1.0.0.tar` & `uugai_python_kerberos_vault-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:32:35.819867 uugai_python_kerberos_vault-1.0.0/
--rw-r--r--   0 glenn      (502) staff       (20)     4846 2024-05-30 10:32:35.819594 uugai_python_kerberos_vault-1.0.0/PKG-INFO
--rw-r--r--   0 glenn      (502) staff       (20)     4554 2024-05-24 13:56:27.000000 uugai_python_kerberos_vault-1.0.0/README.md
--rw-r--r--   0 glenn      (502) staff       (20)       38 2024-05-30 10:32:35.819966 uugai_python_kerberos_vault-1.0.0/setup.cfg
--rw-r--r--   0 glenn      (502) staff       (20)      492 2024-05-24 13:20:21.000000 uugai_python_kerberos_vault-1.0.0/setup.py
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:32:35.817379 uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault/
--rw-r--r--   0 glenn      (502) staff       (20)     4182 2024-05-24 12:35:53.000000 uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault/KerberosVault.py
--rw-r--r--   0 glenn      (502) staff       (20)       63 2024-05-23 07:35:23.000000 uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault/__init__.py
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:32:35.819186 uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault.egg-info/
--rw-r--r--   0 glenn      (502) staff       (20)     4846 2024-05-30 10:32:35.000000 uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault.egg-info/PKG-INFO
--rw-r--r--   0 glenn      (502) staff       (20)      357 2024-05-30 10:32:35.000000 uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault.egg-info/SOURCES.txt
--rw-r--r--   0 glenn      (502) staff       (20)        1 2024-05-30 10:32:35.000000 uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault.egg-info/dependency_links.txt
--rw-r--r--   0 glenn      (502) staff       (20)      309 2024-05-30 10:32:35.000000 uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault.egg-info/requires.txt
--rw-r--r--   0 glenn      (502) staff       (20)       28 2024-05-30 10:32:35.000000 uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault.egg-info/top_level.txt
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:45:55.113991 uugai_python_kerberos_vault-1.1.0/
+-rw-r--r--   0 glenn      (502) staff       (20)     4846 2024-05-30 10:45:55.113713 uugai_python_kerberos_vault-1.1.0/PKG-INFO
+-rw-r--r--   0 glenn      (502) staff       (20)     4554 2024-05-24 13:56:27.000000 uugai_python_kerberos_vault-1.1.0/README.md
+-rw-r--r--   0 glenn      (502) staff       (20)       38 2024-05-30 10:45:55.114088 uugai_python_kerberos_vault-1.1.0/setup.cfg
+-rw-r--r--   0 glenn      (502) staff       (20)      492 2024-05-30 10:45:28.000000 uugai_python_kerberos_vault-1.1.0/setup.py
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:45:55.111747 uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault/
+-rw-r--r--   0 glenn      (502) staff       (20)     4182 2024-05-24 12:35:53.000000 uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault/KerberosVault.py
+-rw-r--r--   0 glenn      (502) staff       (20)       63 2024-05-23 07:35:23.000000 uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault/__init__.py
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:45:55.113337 uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault.egg-info/
+-rw-r--r--   0 glenn      (502) staff       (20)     4846 2024-05-30 10:45:55.000000 uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault.egg-info/PKG-INFO
+-rw-r--r--   0 glenn      (502) staff       (20)      357 2024-05-30 10:45:55.000000 uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 glenn      (502) staff       (20)        1 2024-05-30 10:45:55.000000 uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 glenn      (502) staff       (20)      309 2024-05-30 10:45:55.000000 uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault.egg-info/requires.txt
+-rw-r--r--   0 glenn      (502) staff       (20)       28 2024-05-30 10:45:55.000000 uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault.egg-info/top_level.txt
```

### Comparing `uugai_python_kerberos_vault-1.0.0/PKG-INFO` & `uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uugai_python_kerberos_vault
-Version: 1.0.0
+Name: uugai-python-kerberos-vault
+Version: 1.1.0
 Summary: Kerberos Vault Python library for interacting with the Kerberos Vault.
 Home-page: UNKNOWN
 Author: uug.ai
 Author-email: support@uug.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `uugai_python_kerberos_vault-1.0.0/README.md` & `uugai_python_kerberos_vault-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault/KerberosVault.py` & `uugai_python_kerberos_vault-1.1.0/uugai_python_kerberos_vault/KerberosVault.py`

 * *Files identical despite different names*

### Comparing `uugai_python_kerberos_vault-1.0.0/uugai_python_kerberos_vault.egg-info/PKG-INFO` & `uugai_python_kerberos_vault-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uugai-python-kerberos-vault
-Version: 1.0.0
+Name: uugai_python_kerberos_vault
+Version: 1.1.0
 Summary: Kerberos Vault Python library for interacting with the Kerberos Vault.
 Home-page: UNKNOWN
 Author: uug.ai
 Author-email: support@uug.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

