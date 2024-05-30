# Comparing `tmp/unfuncaptcha_bda-0.0.3.tar.gz` & `tmp/unfuncaptcha_bda-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfuncaptcha_bda-0.0.3.tar", last modified: Mon May 20 06:28:28 2024, max compression
+gzip compressed data, was "unfuncaptcha_bda-0.0.4.tar", last modified: Thu May 30 19:05:36 2024, max compression
```

## Comparing `unfuncaptcha_bda-0.0.3.tar` & `unfuncaptcha_bda-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-20 06:28:28.325940 unfuncaptcha_bda-0.0.3/
--rw-r--r--   0 camel      (501) staff       (20)    34888 2024-05-17 19:39:57.000000 unfuncaptcha_bda-0.0.3/LICENSE
--rw-r--r--   0 camel      (501) staff       (20)     1357 2024-05-20 06:28:28.325733 unfuncaptcha_bda-0.0.3/PKG-INFO
--rw-r--r--   0 camel      (501) staff       (20)      835 2024-05-17 19:39:57.000000 unfuncaptcha_bda-0.0.3/README.md
--rw-r--r--   0 camel      (501) staff       (20)      591 2024-05-20 06:27:57.000000 unfuncaptcha_bda-0.0.3/pyproject.toml
--rw-r--r--   0 camel      (501) staff       (20)       38 2024-05-20 06:28:28.326021 unfuncaptcha_bda-0.0.3/setup.cfg
-drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-20 06:28:28.324018 unfuncaptcha_bda-0.0.3/src/
-drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-20 06:28:28.324802 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/
--rw-r--r--   0 camel      (501) staff       (20)       49 2024-05-17 19:39:57.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/__init__.py
--rw-r--r--   0 camel      (501) staff       (20)     1580 2024-05-18 07:16:49.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/crypto.py
--rw-r--r--   0 camel      (501) staff       (20)     3040 2024-05-17 21:11:50.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/fingerprint.py
-drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-20 06:28:28.325528 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/
--rw-r--r--   0 camel      (501) staff       (20)     1357 2024-05-20 06:28:28.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/PKG-INFO
--rw-r--r--   0 camel      (501) staff       (20)      308 2024-05-20 06:28:28.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/SOURCES.txt
--rw-r--r--   0 camel      (501) staff       (20)        1 2024-05-20 06:28:28.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/dependency_links.txt
--rw-r--r--   0 camel      (501) staff       (20)       17 2024-05-20 06:28:28.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/top_level.txt
+drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-30 19:05:36.258216 unfuncaptcha_bda-0.0.4/
+-rw-r--r--   0 camel      (501) staff       (20)    34888 2024-05-30 19:01:20.000000 unfuncaptcha_bda-0.0.4/LICENSE
+-rw-r--r--   0 camel      (501) staff       (20)     1357 2024-05-30 19:05:36.258015 unfuncaptcha_bda-0.0.4/PKG-INFO
+-rw-r--r--   0 camel      (501) staff       (20)      835 2024-05-30 19:01:20.000000 unfuncaptcha_bda-0.0.4/README.md
+-rw-r--r--   0 camel      (501) staff       (20)      591 2024-05-30 19:04:28.000000 unfuncaptcha_bda-0.0.4/pyproject.toml
+-rw-r--r--   0 camel      (501) staff       (20)       38 2024-05-30 19:05:36.258252 unfuncaptcha_bda-0.0.4/setup.cfg
+drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-30 19:05:36.256194 unfuncaptcha_bda-0.0.4/src/
+drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-30 19:05:36.256981 unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda/
+-rw-r--r--   0 camel      (501) staff       (20)       49 2024-05-30 19:01:20.000000 unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda/__init__.py
+-rw-r--r--   0 camel      (501) staff       (20)     1580 2024-05-30 19:01:20.000000 unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda/crypto.py
+-rw-r--r--   0 camel      (501) staff       (20)     3384 2024-05-30 19:04:28.000000 unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda/fingerprint.py
+drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-30 19:05:36.257827 unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda.egg-info/
+-rw-r--r--   0 camel      (501) staff       (20)     1357 2024-05-30 19:05:36.000000 unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda.egg-info/PKG-INFO
+-rw-r--r--   0 camel      (501) staff       (20)      308 2024-05-30 19:05:36.000000 unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda.egg-info/SOURCES.txt
+-rw-r--r--   0 camel      (501) staff       (20)        1 2024-05-30 19:05:36.000000 unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda.egg-info/dependency_links.txt
+-rw-r--r--   0 camel      (501) staff       (20)       17 2024-05-30 19:05:36.000000 unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda.egg-info/top_level.txt
```

### Comparing `unfuncaptcha_bda-0.0.3/LICENSE` & `unfuncaptcha_bda-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unfuncaptcha_bda-0.0.3/PKG-INFO` & `unfuncaptcha_bda-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfuncaptcha_bda
-Version: 0.0.3
+Version: 0.0.4
 Summary: View, edit, and repackage Arkose Labs Funcaptcha fingerprints
 Author-email: bc <no@dont.email.me>
 Project-URL: Homepage, https://github.com/unfuncaptcha/bda
 Project-URL: Issues, https://github.com/unfuncaptcha/bda/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `unfuncaptcha_bda-0.0.3/README.md` & `unfuncaptcha_bda-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `unfuncaptcha_bda-0.0.3/pyproject.toml` & `unfuncaptcha_bda-0.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unfuncaptcha_bda"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "bc", email = "no@dont.email.me" }]
 description = "View, edit, and repackage Arkose Labs Funcaptcha fingerprints"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/crypto.py` & `unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda/crypto.py`

 * *Files identical despite different names*

### Comparing `unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/fingerprint.py` & `unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda/fingerprint.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,31 @@
 from .crypto import BDACrypto
 import base64
 import json
 import time
 
 class ArkoseBrowserFingerprint(object):
     def __init__(self, encoded_fingerprint: str, user_agent: str, timestamp: int = int(time.time())):
-        self._timestamp = str(int(timestamp - (timestamp % 21600)))
-        self._key = user_agent + str(self._timestamp)
+        self._user_agent = user_agent # store user_agent
+        self._timestamp = int(timestamp - (timestamp % 21600))
+        self._key = self._user_agent + str(self._timestamp)
 
         self.crypto = BDACrypto(self._key)
         self._raw_fingeprint = json.loads(base64.b64decode(encoded_fingerprint)) # {"ct": ..., "s": ..., "iv": ... }
         self.fingerprint: list[dict[str, Any]] = json.loads(self.crypto.decrypt(self._raw_fingeprint).decode())
 
 
+    def update_timestamp(self, timestamp: int = int(time.time())) -> int:
+        self._timestamp = int(timestamp - (timestamp % 21600))
+        self._key = self._user_agent + str(self._timestamp)
+        self.crypto = BDACrypto(self._key)
+        
+        return self._timestamp
+
+    
     def repackage(self, encode_base64: bool = True) -> str:
         repacked_bda = json.dumps(
             self.crypto.re_encrypt(json.dumps(self.fingerprint, separators=(',', ':')), self._raw_fingeprint),
             separators=(',', ':'),
             sort_keys=True
         )
```

### Comparing `unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/PKG-INFO` & `unfuncaptcha_bda-0.0.4/src/unfuncaptcha_bda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfuncaptcha_bda
-Version: 0.0.3
+Version: 0.0.4
 Summary: View, edit, and repackage Arkose Labs Funcaptcha fingerprints
 Author-email: bc <no@dont.email.me>
 Project-URL: Homepage, https://github.com/unfuncaptcha/bda
 Project-URL: Issues, https://github.com/unfuncaptcha/bda/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

