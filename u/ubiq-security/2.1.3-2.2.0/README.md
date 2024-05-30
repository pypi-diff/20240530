# Comparing `tmp/ubiq-security-2.1.3.tar.gz` & `tmp/ubiq_security-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubiq-security-2.1.3.tar", last modified: Mon Oct 23 20:38:22 2023, max compression
+gzip compressed data, was "ubiq_security-2.2.0.tar", last modified: Thu May 30 01:23:11 2024, max compression
```

## Comparing `ubiq-security-2.1.3.tar` & `ubiq_security-2.2.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 ifreshwater   (501) staff       (20)        0 2023-10-23 20:38:22.403556 ubiq-security-2.1.3/
--rw-r--r--   0 ifreshwater   (501) staff       (20)     1104 2022-11-21 21:22:47.000000 ubiq-security-2.1.3/LICENSE
--rw-r--r--   0 ifreshwater   (501) staff       (20)     9750 2023-10-23 20:38:22.403281 ubiq-security-2.1.3/PKG-INFO
--rw-r--r--   0 ifreshwater   (501) staff       (20)     8710 2023-10-23 17:37:24.000000 ubiq-security-2.1.3/README.md
--rw-r--r--   0 ifreshwater   (501) staff       (20)       38 2023-10-23 20:38:22.403596 ubiq-security-2.1.3/setup.cfg
--rw-r--r--   0 ifreshwater   (501) staff       (20)     1742 2022-11-21 21:22:47.000000 ubiq-security-2.1.3/setup.py
-drwxr-xr-x   0 ifreshwater   (501) staff       (20)        0 2023-10-23 20:38:22.401029 ubiq-security-2.1.3/ubiq_security/
--rw-r--r--   0 ifreshwater   (501) staff       (20)      226 2022-11-21 21:22:47.000000 ubiq-security-2.1.3/ubiq_security/__init__.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)     3843 2022-11-21 21:22:47.000000 ubiq-security-2.1.3/ubiq_security/algorithm.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)     5455 2023-08-14 17:08:49.000000 ubiq-security-2.1.3/ubiq_security/auth.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)     2699 2023-10-23 17:37:24.000000 ubiq-security-2.1.3/ubiq_security/common.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)     4691 2023-10-23 17:37:24.000000 ubiq-security-2.1.3/ubiq_security/configuration.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)     5974 2023-06-15 19:59:00.000000 ubiq-security-2.1.3/ubiq_security/credentials.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)    10826 2023-10-23 17:37:24.000000 ubiq-security-2.1.3/ubiq_security/decrypt.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)     8347 2023-10-23 17:37:24.000000 ubiq-security-2.1.3/ubiq_security/encrypt.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)     6687 2023-10-23 20:12:33.000000 ubiq-security-2.1.3/ubiq_security/events.py
-drwxr-xr-x   0 ifreshwater   (501) staff       (20)        0 2023-10-23 20:38:22.402835 ubiq-security-2.1.3/ubiq_security/fpe/
--rw-r--r--   0 ifreshwater   (501) staff       (20)      124 2023-06-15 19:59:00.000000 ubiq-security-2.1.3/ubiq_security/fpe/__init__.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)     6452 2023-06-21 16:35:33.000000 ubiq-security-2.1.3/ubiq_security/fpe/common.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)     2344 2023-06-15 19:59:00.000000 ubiq-security-2.1.3/ubiq_security/fpe/decrypt.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)     3623 2023-07-18 16:04:08.000000 ubiq-security-2.1.3/ubiq_security/fpe/encrypt.py
--rw-r--r--   0 ifreshwater   (501) staff       (20)       18 2023-10-23 17:37:24.000000 ubiq-security-2.1.3/ubiq_security/version.py
-drwxr-xr-x   0 ifreshwater   (501) staff       (20)        0 2023-10-23 20:38:22.401737 ubiq-security-2.1.3/ubiq_security.egg-info/
--rw-r--r--   0 ifreshwater   (501) staff       (20)     9750 2023-10-23 20:38:22.000000 ubiq-security-2.1.3/ubiq_security.egg-info/PKG-INFO
--rw-r--r--   0 ifreshwater   (501) staff       (20)      584 2023-10-23 20:38:22.000000 ubiq-security-2.1.3/ubiq_security.egg-info/SOURCES.txt
--rw-r--r--   0 ifreshwater   (501) staff       (20)        1 2023-10-23 20:38:22.000000 ubiq-security-2.1.3/ubiq_security.egg-info/dependency_links.txt
--rw-r--r--   0 ifreshwater   (501) staff       (20)       44 2023-10-23 20:38:22.000000 ubiq-security-2.1.3/ubiq_security.egg-info/requires.txt
--rw-r--r--   0 ifreshwater   (501) staff       (20)       14 2023-10-23 20:38:22.000000 ubiq-security-2.1.3/ubiq_security.egg-info/top_level.txt
+drwxr-xr-x   0 ifreshwater   (501) staff       (20)        0 2024-05-30 01:23:11.898793 ubiq_security-2.2.0/
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     1104 2022-11-21 21:22:47.000000 ubiq_security-2.2.0/LICENSE
+-rw-r--r--   0 ifreshwater   (501) staff       (20)    13259 2024-05-30 01:23:11.898439 ubiq_security-2.2.0/PKG-INFO
+-rw-r--r--   0 ifreshwater   (501) staff       (20)    12208 2024-05-29 16:54:34.000000 ubiq_security-2.2.0/README.md
+-rw-r--r--   0 ifreshwater   (501) staff       (20)       38 2024-05-30 01:23:11.898860 ubiq_security-2.2.0/setup.cfg
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     1742 2022-11-21 21:22:47.000000 ubiq_security-2.2.0/setup.py
+drwxr-xr-x   0 ifreshwater   (501) staff       (20)        0 2024-05-30 01:23:11.894699 ubiq_security-2.2.0/ubiq_security/
+-rw-r--r--   0 ifreshwater   (501) staff       (20)      226 2024-04-17 16:02:16.000000 ubiq_security-2.2.0/ubiq_security/__init__.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     3843 2022-11-21 21:22:47.000000 ubiq_security-2.2.0/ubiq_security/algorithm.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     5455 2023-08-14 17:08:49.000000 ubiq_security-2.2.0/ubiq_security/auth.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     3410 2024-05-01 17:46:25.000000 ubiq_security-2.2.0/ubiq_security/common.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     6671 2024-05-01 17:46:25.000000 ubiq_security-2.2.0/ubiq_security/configuration.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     6152 2024-05-29 18:14:47.000000 ubiq_security-2.2.0/ubiq_security/credentials.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)    10826 2024-04-17 15:13:30.000000 ubiq_security-2.2.0/ubiq_security/decrypt.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     8347 2024-04-16 21:28:40.000000 ubiq_security-2.2.0/ubiq_security/encrypt.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     8295 2024-05-29 18:50:02.000000 ubiq_security-2.2.0/ubiq_security/events.py
+drwxr-xr-x   0 ifreshwater   (501) staff       (20)        0 2024-05-30 01:23:11.896503 ubiq_security-2.2.0/ubiq_security/structured/
+-rw-r--r--   0 ifreshwater   (501) staff       (20)      124 2024-05-01 17:46:25.000000 ubiq_security-2.2.0/ubiq_security/structured/__init__.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     8404 2024-05-29 16:54:34.000000 ubiq_security-2.2.0/ubiq_security/structured/common.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     2815 2024-05-29 16:54:34.000000 ubiq_security-2.2.0/ubiq_security/structured/decrypt.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     4237 2024-05-29 16:54:34.000000 ubiq_security-2.2.0/ubiq_security/structured/encrypt.py
+drwxr-xr-x   0 ifreshwater   (501) staff       (20)        0 2024-05-30 01:23:11.897631 ubiq_security-2.2.0/ubiq_security/structured/lib/
+-rw-r--r--   0 ifreshwater   (501) staff       (20)        0 2024-05-01 17:46:25.000000 ubiq_security-2.2.0/ubiq_security/structured/lib/__init__.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     3081 2024-05-01 17:46:25.000000 ubiq_security-2.2.0/ubiq_security/structured/lib/ff1.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     4459 2024-05-01 17:46:25.000000 ubiq_security-2.2.0/ubiq_security/structured/lib/ff1_test.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)     2423 2024-05-01 17:46:25.000000 ubiq_security-2.2.0/ubiq_security/structured/lib/ffx.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)      382 2024-05-01 17:46:25.000000 ubiq_security-2.2.0/ubiq_security/structured/lib/ffx_test.py
+-rw-r--r--   0 ifreshwater   (501) staff       (20)       18 2024-05-29 16:54:34.000000 ubiq_security-2.2.0/ubiq_security/version.py
+drwxr-xr-x   0 ifreshwater   (501) staff       (20)        0 2024-05-30 01:23:11.898026 ubiq_security-2.2.0/ubiq_security.egg-info/
+-rw-r--r--   0 ifreshwater   (501) staff       (20)    13259 2024-05-30 01:23:11.000000 ubiq_security-2.2.0/ubiq_security.egg-info/PKG-INFO
+-rw-r--r--   0 ifreshwater   (501) staff       (20)      807 2024-05-30 01:23:11.000000 ubiq_security-2.2.0/ubiq_security.egg-info/SOURCES.txt
+-rw-r--r--   0 ifreshwater   (501) staff       (20)        1 2024-05-30 01:23:11.000000 ubiq_security-2.2.0/ubiq_security.egg-info/dependency_links.txt
+-rw-r--r--   0 ifreshwater   (501) staff       (20)       40 2024-05-30 01:23:11.000000 ubiq_security-2.2.0/ubiq_security.egg-info/requires.txt
+-rw-r--r--   0 ifreshwater   (501) staff       (20)       14 2024-05-30 01:23:11.000000 ubiq_security-2.2.0/ubiq_security.egg-info/top_level.txt
```

### Comparing `ubiq-security-2.1.3/LICENSE` & `ubiq_security-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.3/PKG-INFO` & `ubiq_security-2.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiq-security
-Version: 2.1.3
+Version: 2.2.0
 Summary: Python client library for accessing Ubiq Platform
 Home-page: https://gitlab.com/ubiqsecurity/ubiq-python
 Author: Ubiq Security, Inc.
 Author-email: support@ubiqsecurity.com
 License: Free To Use But Restricted
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,26 +20,25 @@
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography
 Requires-Dist: requests
 Requires-Dist: six
-Requires-Dist: ubiq_security_fpe
+Requires-Dist: swig
+Requires-Dist: M2Crypto
 
 # Ubiq Security Python Library
 
 
 The Ubiq Security Python library provides convenient interaction with the
 Ubiq Security Platform API from applications written in the Python language.
 It includes a pre-defined set of classes that will provide simple interfaces
 to encrypt and decrypt data
 
-This library also incorporates Ubiq Format Preserving Encryption (eFPE).  eFPE allows encrypting so that the output cipher text is in the same format as the original plaintext. This includes preserving special characters and control over what characters are permitted in the cipher text. For example, consider encrypting a social security number '123-45-6789'. The cipher text will maintain the dashes and look something like: 'W$+-qF-oMMV'.
-
 ## Documentation
 
 See the [Python API docs](https://dev.ubiqsecurity.com/docs/api).
 
 ## Installation
 
 #### Using the package manager:
@@ -214,87 +213,178 @@
             break
 
     # Make sure an additional plaintext data is retrieved and
     # release any allocated resources
     plaintext_data += decryption.end()
 
 ```
-## Ubiq Format Preserving Encryption
+## Ubiq Structured Encryption
 
-This library incorporates Ubiq Format Preserving Encryption (eFPE).
+This library incorporates Ubiq Structured Encryption.
 
 ## Requirements
 
--   Please follow the same requirements as described above for the non-eFPE functionality.
--   This library has dependencies on ubiqsecurity-fpe library available for download in the Ubiq GitHub/GitLab repository.
+-   Please follow the same requirements as described above for the non-structured functionality.
 
 ## Usage
 
 You will need to obtain account credentials in the same way as described above for conventional encryption/decryption. When
-you do this in your [Ubiq Dashboard][dashboard] [credentials][credentials], you'll need to enable the eFPE option.
+you do this in your [Ubiq Dashboard][dashboard] [credentials][credentials], you'll need to enable access to structured datasets.
 The credentials can be set using environment variables, loaded from an explicitly
 specified file, or read from the default location (~/.ubiq/credentials).
 
 
 Require the Security Client module in your Python class.
 
 ```python
 import ubiq_security as ubiq
-import ubiq_security.fpe as ubiqfpe
+import ubiq_security.structured as ubiq_structured
 ```
 
 
 ### Encrypt a social security text field - simple interface
-Pass credentials, the name of a Field Format Specification, FFS, and data into the encryption function.
+Pass credentials, the name of a structured dataset, and data into the encryption function.
 The encrypted data will be returned.
 
 ```python
-ffs_name = "SSN";
+dataset_name = "SSN";
 plain_text = "123-45-6789";
 
 credentials = ubiq.ConfigCredentials('./credentials', 'default');
 
-encrypted_data = ubiqfpe.Encrypt(
+encrypted_data = ubiq_structured.Encrypt(
         credentials,
-        ffs_name,
+        dataset_name,
         plain_text);
         
 print('ENCRYPTED ciphertext= ' + encrypted_data + '\n');
 ```
 
 ### Decrypt a social security text field - simple interface
-Pass credentials, the name of a Field Format Specification, FFS, and data into the decryption function.
+Pass credentials, the name of a structured dataset, and data into the decryption function.
 The decrypted data will be returned.
 
 ```python
-ffs_name = "SSN";
+dataset_name = "SSN";
 cipher_text = "300-0E-274t";
 
 credentials = ubiq.ConfigCredentials('./credentials', 'default');
 
-decrypted_text = ubiqfpe.Decrypt(
+decrypted_text = ubiq_structured.Decrypt(
         credentials,
-        ffs_name,
+        dataset_name,
         cipher_text);
         
 print('DECRYPTED decrypted_text= ' + decrypted_text + '\n');
 ```
 
-Additional information on how to use these FFS models in your own applications is available by contacting Ubiq.
+Additional information on how to use these models in your own applications is available by contacting Ubiq.
+
+### Custom Metadata for Usage Reporting
+There are cases where a developer would like to attach metadata to usage information reported by the application.  Both the structured and unstructured interfaces allow user_defined metadata to be sent with the usage information reported by the libraries.
+
+The **add_reporting_user_defined_metadata** function accepts a string in JSON format that will be stored in the database with the usage records.  The string must be less than 1024 characters and be a valid JSON format.  The string must include both the `{` and `}` symbols.  The supplied value will be used until the object goes out of scope.  Due to asynchronous processing, changing the value may be immediately reflected in subsequent usage.  If immediate changes to the values are required, it would be safer to create a new encrypt / decrypt object and call the `add_reporting_user_defined_metadata` function with the new values.
+
+Examples are shown below.
+```python
+  ...
+  credentials = ubiq.ConfigCredentials('./credentials', 'default');
+
+  special_value = "information"
+  credentials.add_reporting_user_defined_metadata("{\"some_key\":\"some_value\"}")
+
+  encrypted_data = ubiq_structured.Encrypt(
+    credentials,
+    dataset_name,
+    plain_text);
+  ...
+  # Structured Encrypt and Decrypt operations
+```
+
+```python
+  ...
+  credentials = ubiq.credentials(access_key_id = "...", secret_signing_key = "...", secret_crypto_access_key = "...")
+  credentials.add_reporting_user_defined_metadata("{\"some_meaningful_flag\" : true }")
+  ct = ubiq.encrypt(creds,
+                  data)
+   ....
+  # Unstructured Encrypt operations
+```
+### Retrieve Current Usage
+Within an encryption session, either Encrypt or Decrypt, the client library can retrieve a copy of the unreported events.  This is for read only purposes and has the potential to be different each time it is called due to encrypt / decrypt activities and the asynchronous event billing process.
+```python
+  ...
+  ct = ubiq.encrypt(creds,data)
+  
+  usage = creds.get_copy_of_usage()
+  
+  ...
+```
 
 ### Encrypt For Search
 
 The same plaintext data will result in different cipher text when encrypted using different data keys. The Encrypt For Search function will encrypt the same plain text for a given dataset using all previously used data keys. This will provide a collection of cipher text values that can be used when searching for existing records where the data was encrypted and the specific version of the data key is not known in advance.
 
 ```python
 
 credentials = ubiq.ConfigCredentials('./credentials', 'default');
-ffs_name = "SSN";
+dataset_name = "SSN";
 plain_text = "123-45-6789";
 
-ct_arr = ubiqfpe.EncryptForSearch(credentials, ffs_name, plain_text)
+ct_arr = ubiq_structured.EncryptForSearch(credentials, dataset_name, plain_text)
+```
+
+
+### Configuration File
+
+A sample configuration file is shown below.  The configuration is in JSON format.  
+
+#### Event Reporting
+The <b>event_reporting</b> section contains values to control how often the usage is reported.  
+
+- <b>wake_interval</b> indicates the number of seconds to sleep before waking to determine if there has been enough activity to report usage
+- <b>minimum_count</b> indicates the minimum number of usage records that must be queued up before sending the usage
+- <b>flush_interval</b> indicates the sleep interval before all usage will be flushed to server.
+- <b>trap_exceptions</b> indicates whether exceptions encountered while reporting usage will be trapped and ignored or if it will become an error that gets reported to the application
+- <b>timestamp_granularity</b> indicates the how granular the timestamp will be when reporting events.  Valid values are
+  - "MICROS"  
+    // DEFAULT: values are reported down to the microsecond resolution when possible
+  - "MILLIS"  
+  // values are reported to the millisecond
+  - "SECONDS"  
+  // values are reported to the second
+  - "MINUTES"  
+  // values are reported to minute
+  - "HOURS"  
+  // values are reported to hour
+  - "HALF_DAYS"  
+  // values are reported to half day
+  - "DAYS"  
+  // values are reported to the day
+
+#### Key Caching
+The <b>key_caching</b> section contains values to control how and when keys are cached.
+
+- <b>unstructured</b> indicates whether keys will be cached when doing unstructured decryption. (default: true)
+- <b>encrypt</b> indicates if keys should be stored encrypted. If keys are encrypted, they will be harder to access via memory, but require them to be decrypted with each use. (default: false)
+
+
+```json
+{
+  "event_reporting": {
+    "wake_interval": 1,
+    "minimum_count": 2,
+    "flush_interval": 2,
+    "trap_exceptions": false,
+    "timestamp_granularity" : "MICROS"
+  },
+  "key_caching":{
+    "unstructured": true,
+    "encrypt": false
+  }
+}
 ```
 
 
 [dashboard]:https://dashboard.ubiqsecurity.com/
 [credentials]:https://dev.ubiqsecurity.com/docs/how-to-create-api-keys
```

### Comparing `ubiq-security-2.1.3/setup.py` & `ubiq_security-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.3/ubiq_security/algorithm.py` & `ubiq_security-2.2.0/ubiq_security/algorithm.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.3/ubiq_security/auth.py` & `ubiq_security-2.2.0/ubiq_security/auth.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.3/ubiq_security/common.py` & `ubiq_security-2.2.0/ubiq_security/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import base64
 import http
 import json
 import requests
 import urllib.error
+from copy import copy
 
 from .auth import http_auth
 from .algorithm import algorithm
 from .configuration import ubiqConfiguration
 
 import cryptography.exceptions as crypto_exceptions
 import cryptography.hazmat.primitives as crypto
 from cryptography.hazmat.backends import default_backend as crypto_backend
 
 
 def fetchDecryptKey(host, papi, sapi, srsa, datakey, client_id, alg):
     config = ubiqConfiguration()
+    key = {}
     # If Missing or Cache is disabled
     if (not papi in fetchDecryptKey.cache or
         not datakey in fetchDecryptKey.cache[papi] or
             not config.get_key_caching_unstructured()):
 
         url = host + '/api/v0/decryption/key'
         response = requests.post(
@@ -33,46 +35,62 @@
             raise urllib.error.HTTPError(
                 url, response.status_code,
                 http.HTTPStatus(response.status_code).phrase,
                 response.headers, response.content)
 
         content = json.loads(response.content.decode('utf-8'))
 
-        key = {}
-
         key['algo'] = algorithm(alg)
         # the client's id for recognizing key reuse
         key['client_id'] = client_id
         # the server's id for sending updates
         key['finger_print'] = content['key_fingerprint']
         key['session'] = content['encryption_session']
 
+        # Need these from the response or we can't decrypt the key later
+        key['encrypted_private_key'] = content['encrypted_private_key']
+        key['wrapped_data_key'] = content['wrapped_data_key']
+
+        # this key hasn't been used (yet)
+        key['uses'] = 0
+
+        if config.get_key_caching_unstructured():
+            # Store in Cache
+            if not papi in fetchDecryptKey.cache:
+                fetchDecryptKey.cache[papi] = {}
+
+            fetchDecryptKey.cache[papi][datakey] = key
+
+    if len(key) == 0:
+        # Get key from cache, key was not fetched.
+        key = fetchDecryptKey.cache[papi][datakey]
+    
+    # Get a copy of the key. If it came from cache, it's a reference.
+    # Decrypting the key would modify the cache, ignoring configuration.
+    key = copy(key)
+
+    if "raw" in key:
+        # Unencrypted, return key
+        return key
+    else:
         # decrypt the client's private key (sent
         # by the server)
         prvkey = crypto.serialization.load_pem_private_key(
-            content['encrypted_private_key'].encode('utf-8'),
+            key['encrypted_private_key'].encode('utf-8'),
             srsa.encode('utf-8'),
             crypto_backend())
         # use the private key to decrypt the data key
         key['raw'] = prvkey.decrypt(
-            base64.b64decode(content['wrapped_data_key']),
+            base64.b64decode(key['wrapped_data_key']),
             crypto.asymmetric.padding.OAEP(
                 mgf=crypto.asymmetric.padding.MGF1(
                     algorithm=crypto.hashes.SHA1()),
                 algorithm=crypto.hashes.SHA1(),
                 label=None))
-
-        # this key hasn't been used (yet)
-        key['uses'] = 0
-
-        if config.get_key_caching_unstructured():
-            # Store in Cache
-            if not papi in fetchDecryptKey.cache:
-                fetchDecryptKey.cache[papi] = {}
+        
+        if config.get_key_caching_unstructured() and not config.get_key_caching_encrypt():
+            # Update store to have unwrapped version of the
             fetchDecryptKey.cache[papi][datakey] = key
-        else:
-            # Return without Caching key
-            return key
-    return fetchDecryptKey.cache[papi][datakey]
-
+        
+        return key
 
 fetchDecryptKey.cache = {}
```

### Comparing `ubiq-security-2.1.3/ubiq_security/credentials.py` & `ubiq_security-2.2.0/ubiq_security/credentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
     def __init__(self, access_key_id, secret_signing_key, secret_crypto_access_key, host):
         self.__access_key_id = access_key_id
         self.__secret_signing_key = secret_signing_key
         self.__secret_crypto_access_key = secret_crypto_access_key
         self.__host = host
 
+        # Event Tracking
+        self.__configuration = ubiqConfiguration()
+        self.__events = events(self, self.__configuration)
+        self.__eventsProcessor = eventsProcessor(self.__configuration, self.__events)
+        self.__eventsProcessor.start()
+
     def get_access_key_id(self):
         return self.__access_key_id
     access_key_id=property(get_access_key_id)
 
     def get_secret_signing_key(self):
         return self.__secret_signing_key
     secret_signing_key=property(get_secret_signing_key)
@@ -30,14 +36,24 @@
     def get_host(self):
         return self.__host
     host = property(get_host)
 
     def set(self):
         return (self.__access_key_id != None and self.__secret_signing_key != None and self.__secret_crypto_access_key != None and 
             self.__access_key_id.strip() != "" and self.__secret_signing_key.strip() != "" and self.__secret_crypto_access_key.strip() != "")
+    
+    def add_reporting_user_defined_metadata(self, data):
+        self.__events.add_user_defined_metadata(data)
+    
+    def get_copy_of_usage(self):
+        return self.__events.list_events()
+
+    # Forward events to event queue
+    def add_event(self, dataset_name, dataset_group_name, billing_action, dataset_type, key_number, count):
+        return self.__events.add_event(self.__access_key_id, dataset_name, dataset_group_name, billing_action, dataset_type, key_number, count)
 
 class configCredentials(credentialsInfo):
 
     def load_config_file(self, config_file, profile):
         config = configparser.ConfigParser()
         config.read(config_file)
 
@@ -75,46 +91,37 @@
         if os.path.exists(config_file):
             self.load_config_file(config_file, profile)
 
         credentialsInfo.__init__(self, self.__access_key_id , self.__secret_signing_key, self.__secret_crypto_access_key, self.__host)
 
         if (not self.set()):
             if (self.__access_key_id == None or self.__access_key_id.strip() == ""):
-               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'access_key_id' value in profile '{1}' or through environment variable for 'UBIQ_ACCESS_KEY_ID'.".format(config_file, profile))
+               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'access_key_id' value in profile '{1}'.".format(config_file, profile))
             elif (self.__secret_signing_key == None or self.__secret_signing_key.strip() == ""):
-               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'secret_signing_key' value in profile '{1}' or through environment variable for 'UBIQ_SECRET_SIGNING_KEY'.".format(config_file, profile))
+               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'secret_signing_key' value in profile '{1}'.".format(config_file, profile))
             elif(self.__secret_crypto_access_key == None or self.__secret_crypto_access_key.strip() == ""):
-               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'secret_crypto_access_key' value in profile '{1}' or through environment variable for 'UBIQ_SECRET_CRYPTO_ACCESS_KEY'.".format(config_file, profile))
-        
-        # Event Tracking
-        self.__configuration = ubiqConfiguration()
-        self.__events = events(self, self.__configuration)
-        self.__eventsProcessor = eventsProcessor(self.__configuration, self.__events)
-        self.__eventsProcessor.start()
+               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'secret_crypto_access_key' value in profile '{1}'.".format(config_file, profile))
 
-    # Forward events to event queue
-    def add_event(self, dataset_name, dataset_group_name, billing_action, dataset_type, key_number, count):
-        return self.__events.add_event(self.__access_key_id, dataset_name, dataset_group_name, billing_action, dataset_type, key_number, count)
 
 
 class credentials(credentialsInfo):
 
     def __init__(self, access_key_id = None, secret_signing_key = None, secret_crypto_access_key = None, host = UBIQ_HOST):
         # If supplied value is None, use ENV variable, otherwise use supplied value.
         # If env value isn't set, use the supplied value anyways (None) but prevent an exception
         self.__access_key_id = (access_key_id, os.getenv('UBIQ_ACCESS_KEY_ID', access_key_id)) [access_key_id == None]
         self.__secret_signing_key = (secret_signing_key, os.getenv('UBIQ_SECRET_SIGNING_KEY', secret_signing_key)) [secret_signing_key == None]
         self.__secret_crypto_access_key = (secret_crypto_access_key, os.getenv('UBIQ_SECRET_CRYPTO_ACCESS_KEY', secret_crypto_access_key)) [secret_crypto_access_key == None]
+        self.__host = (host, os.getenv('UBIQ_SERVER', host)) [host == None]
 
         credentialsInfo.__init__(self, self.__access_key_id,
                                  self.__secret_signing_key,
-                                 self.__secret_crypto_access_key, host)
+                                 self.__secret_crypto_access_key, 
+                                 self.__host)
         
-        # Event Tracking
-        self.__configuration = ubiqConfiguration()
-        self.__events = events(self, self.__configuration)
-        self.__eventsProcessor = eventsProcessor(self.__configuration, self.__events)
-        self.__eventsProcessor.start()
-    
-    # Forward events to event queue
-    def add_event(self, dataset_name, dataset_group_name, billing_action, dataset_type, key_number, count):
-        return self.__events.add_event(self.__access_key_id, dataset_name, dataset_group_name, billing_action, dataset_type, key_number, count)
+        if (not self.set()):
+            if (self.__access_key_id == None or self.__access_key_id.strip() == ""):
+               raise RuntimeError("Environment variable for 'UBIQ_ACCESS_KEY_ID' not set.")
+            elif (self.__secret_signing_key == None or self.__secret_signing_key.strip() == ""):
+               raise RuntimeError("Environment variable for 'UBIQ_SECRET_SIGNING_KEY' not set.")
+            elif(self.__secret_crypto_access_key == None or self.__secret_crypto_access_key.strip() == ""):
+               raise RuntimeError("Environment variable for 'UBIQ_SECRET_CRYPTO_ACCESS_KEY' not set.")
```

### Comparing `ubiq-security-2.1.3/ubiq_security/decrypt.py` & `ubiq_security-2.2.0/ubiq_security/decrypt.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.3/ubiq_security/encrypt.py` & `ubiq_security-2.2.0/ubiq_security/encrypt.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.3/ubiq_security/fpe/decrypt.py` & `ubiq_security-2.2.0/ubiq_security/structured/decrypt.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import base64
 
 from ..credentials import credentials
 
 
 from .common import fmtInput, strConvertRadix, decKeyNumber, fmtOutput
-from .common import fetchFFS, fetchKey
-from ubiq_security_fpe import ff1
+from .common import fetchDataset, fetchKey
+from .lib import ff1
 
 class Decryption:
     def __del__(self):
         # todo: overwrite 'unwrapped_data_key'
         return
 
-    def __init__(self, creds, ffs):
+    def __init__(self, creds, dataset_name):
         if not creds.set():
             raise RuntimeError("credentials not set")
         
         self._creds = creds
 
         # If the host does not begin with either http or https
         # insert https://
@@ -27,39 +27,48 @@
             self._host = "https://" + self._host
         self._host += '/api/v0/'
 
         self._papi = creds.access_key_id
         self._sapi = creds.secret_signing_key
         self._srsa = creds.secret_crypto_access_key
 
-        self._ffs = fetchFFS(self._host, self._papi, self._sapi, ffs)
+        self._dataset = fetchDataset(self._host, self._papi, self._sapi, dataset_name)
 
     def Cipher(self, ct, twk = None):
-        pth = self._ffs['passthrough']
-        ics = self._ffs['input_character_set']
-        ocs = self._ffs['output_character_set']
+        pth = self._dataset['passthrough']
+        ics = self._dataset['input_character_set']
+        ocs = self._dataset['output_character_set']
+        rules = self._dataset.get('passthrough_rules', [])
 
-        fmt, ct = fmtInput(ct, pth, ocs, ics)
-        ct, n = decKeyNumber(ct, ocs, self._ffs['msb_encoding_bits'])
+        input_min = self._dataset['min_input_length']
+        input_max = self._dataset['max_input_length']
+        
+        fmt, ct, rules = fmtInput(ct, pth, ocs, ics, rules)
+
+        input_len = len(ct)
+        if input_len < input_min or input_len > input_max:
+            raise RuntimeError('Invalid input len (%s) min: %s max %s'%(input_len, input_min, input_max))
+
+        ct, n = decKeyNumber(ct, ocs, self._dataset['msb_encoding_bits'])
         if not hasattr(self, '_key') or self._key['key_number'] != n:
             self._key = fetchKey(self._host,
                                  self._papi, self._sapi, self._srsa,
-                                 self._ffs['name'], n)
-            if self._ffs['encryption_algorithm'] == 'FF1':
+                                 self._dataset['name'], n)
+            if self._dataset['encryption_algorithm'] == 'FF1':
                 self._ctx = ff1.Context(
                     self._key['unwrapped_data_key'],
-                    base64.b64decode(self._ffs['tweak']),
-                    self._ffs['tweak_min_len'], self._ffs['tweak_max_len'],
+                    base64.b64decode(self._dataset['tweak']),
+                    self._dataset['tweak_min_len'], self._dataset['tweak_max_len'],
                     len(ics), ics)
             else:
                 raise RuntimeError('unsupported algorithm: ' +
-                                   self._ffs['encryption_algorithm'])
+                                   self._dataset['encryption_algorithm'])
         ct = strConvertRadix(ct, ocs, ics)
 
         pt = self._ctx.Decrypt(ct, twk)
 
-        self._creds.add_event(dataset_name=self._ffs['name'], dataset_group_name="", billing_action="decrypt",
+        self._creds.add_event(dataset_name=self._dataset['name'], dataset_group_name="", billing_action="decrypt",
             dataset_type="structured", key_number=n, count=1)
-        return fmtOutput(fmt, pt, pth)
+        return fmtOutput(fmt, pt, pth, rules)
 
-def Decrypt(creds, ffs, ct, twk = None):
-    return Decryption(creds, ffs).Cipher(ct, twk)
+def Decrypt(creds, dataset_name, ct, twk = None):
+    return Decryption(creds, dataset_name).Cipher(ct, twk)
```

### Comparing `ubiq-security-2.1.3/ubiq_security.egg-info/PKG-INFO` & `ubiq_security-2.2.0/ubiq_security.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiq-security
-Version: 2.1.3
+Version: 2.2.0
 Summary: Python client library for accessing Ubiq Platform
 Home-page: https://gitlab.com/ubiqsecurity/ubiq-python
 Author: Ubiq Security, Inc.
 Author-email: support@ubiqsecurity.com
 License: Free To Use But Restricted
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,26 +20,25 @@
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography
 Requires-Dist: requests
 Requires-Dist: six
-Requires-Dist: ubiq_security_fpe
+Requires-Dist: swig
+Requires-Dist: M2Crypto
 
 # Ubiq Security Python Library
 
 
 The Ubiq Security Python library provides convenient interaction with the
 Ubiq Security Platform API from applications written in the Python language.
 It includes a pre-defined set of classes that will provide simple interfaces
 to encrypt and decrypt data
 
-This library also incorporates Ubiq Format Preserving Encryption (eFPE).  eFPE allows encrypting so that the output cipher text is in the same format as the original plaintext. This includes preserving special characters and control over what characters are permitted in the cipher text. For example, consider encrypting a social security number '123-45-6789'. The cipher text will maintain the dashes and look something like: 'W$+-qF-oMMV'.
-
 ## Documentation
 
 See the [Python API docs](https://dev.ubiqsecurity.com/docs/api).
 
 ## Installation
 
 #### Using the package manager:
@@ -214,87 +213,178 @@
             break
 
     # Make sure an additional plaintext data is retrieved and
     # release any allocated resources
     plaintext_data += decryption.end()
 
 ```
-## Ubiq Format Preserving Encryption
+## Ubiq Structured Encryption
 
-This library incorporates Ubiq Format Preserving Encryption (eFPE).
+This library incorporates Ubiq Structured Encryption.
 
 ## Requirements
 
--   Please follow the same requirements as described above for the non-eFPE functionality.
--   This library has dependencies on ubiqsecurity-fpe library available for download in the Ubiq GitHub/GitLab repository.
+-   Please follow the same requirements as described above for the non-structured functionality.
 
 ## Usage
 
 You will need to obtain account credentials in the same way as described above for conventional encryption/decryption. When
-you do this in your [Ubiq Dashboard][dashboard] [credentials][credentials], you'll need to enable the eFPE option.
+you do this in your [Ubiq Dashboard][dashboard] [credentials][credentials], you'll need to enable access to structured datasets.
 The credentials can be set using environment variables, loaded from an explicitly
 specified file, or read from the default location (~/.ubiq/credentials).
 
 
 Require the Security Client module in your Python class.
 
 ```python
 import ubiq_security as ubiq
-import ubiq_security.fpe as ubiqfpe
+import ubiq_security.structured as ubiq_structured
 ```
 
 
 ### Encrypt a social security text field - simple interface
-Pass credentials, the name of a Field Format Specification, FFS, and data into the encryption function.
+Pass credentials, the name of a structured dataset, and data into the encryption function.
 The encrypted data will be returned.
 
 ```python
-ffs_name = "SSN";
+dataset_name = "SSN";
 plain_text = "123-45-6789";
 
 credentials = ubiq.ConfigCredentials('./credentials', 'default');
 
-encrypted_data = ubiqfpe.Encrypt(
+encrypted_data = ubiq_structured.Encrypt(
         credentials,
-        ffs_name,
+        dataset_name,
         plain_text);
         
 print('ENCRYPTED ciphertext= ' + encrypted_data + '\n');
 ```
 
 ### Decrypt a social security text field - simple interface
-Pass credentials, the name of a Field Format Specification, FFS, and data into the decryption function.
+Pass credentials, the name of a structured dataset, and data into the decryption function.
 The decrypted data will be returned.
 
 ```python
-ffs_name = "SSN";
+dataset_name = "SSN";
 cipher_text = "300-0E-274t";
 
 credentials = ubiq.ConfigCredentials('./credentials', 'default');
 
-decrypted_text = ubiqfpe.Decrypt(
+decrypted_text = ubiq_structured.Decrypt(
         credentials,
-        ffs_name,
+        dataset_name,
         cipher_text);
         
 print('DECRYPTED decrypted_text= ' + decrypted_text + '\n');
 ```
 
-Additional information on how to use these FFS models in your own applications is available by contacting Ubiq.
+Additional information on how to use these models in your own applications is available by contacting Ubiq.
+
+### Custom Metadata for Usage Reporting
+There are cases where a developer would like to attach metadata to usage information reported by the application.  Both the structured and unstructured interfaces allow user_defined metadata to be sent with the usage information reported by the libraries.
+
+The **add_reporting_user_defined_metadata** function accepts a string in JSON format that will be stored in the database with the usage records.  The string must be less than 1024 characters and be a valid JSON format.  The string must include both the `{` and `}` symbols.  The supplied value will be used until the object goes out of scope.  Due to asynchronous processing, changing the value may be immediately reflected in subsequent usage.  If immediate changes to the values are required, it would be safer to create a new encrypt / decrypt object and call the `add_reporting_user_defined_metadata` function with the new values.
+
+Examples are shown below.
+```python
+  ...
+  credentials = ubiq.ConfigCredentials('./credentials', 'default');
+
+  special_value = "information"
+  credentials.add_reporting_user_defined_metadata("{\"some_key\":\"some_value\"}")
+
+  encrypted_data = ubiq_structured.Encrypt(
+    credentials,
+    dataset_name,
+    plain_text);
+  ...
+  # Structured Encrypt and Decrypt operations
+```
+
+```python
+  ...
+  credentials = ubiq.credentials(access_key_id = "...", secret_signing_key = "...", secret_crypto_access_key = "...")
+  credentials.add_reporting_user_defined_metadata("{\"some_meaningful_flag\" : true }")
+  ct = ubiq.encrypt(creds,
+                  data)
+   ....
+  # Unstructured Encrypt operations
+```
+### Retrieve Current Usage
+Within an encryption session, either Encrypt or Decrypt, the client library can retrieve a copy of the unreported events.  This is for read only purposes and has the potential to be different each time it is called due to encrypt / decrypt activities and the asynchronous event billing process.
+```python
+  ...
+  ct = ubiq.encrypt(creds,data)
+  
+  usage = creds.get_copy_of_usage()
+  
+  ...
+```
 
 ### Encrypt For Search
 
 The same plaintext data will result in different cipher text when encrypted using different data keys. The Encrypt For Search function will encrypt the same plain text for a given dataset using all previously used data keys. This will provide a collection of cipher text values that can be used when searching for existing records where the data was encrypted and the specific version of the data key is not known in advance.
 
 ```python
 
 credentials = ubiq.ConfigCredentials('./credentials', 'default');
-ffs_name = "SSN";
+dataset_name = "SSN";
 plain_text = "123-45-6789";
 
-ct_arr = ubiqfpe.EncryptForSearch(credentials, ffs_name, plain_text)
+ct_arr = ubiq_structured.EncryptForSearch(credentials, dataset_name, plain_text)
+```
+
+
+### Configuration File
+
+A sample configuration file is shown below.  The configuration is in JSON format.  
+
+#### Event Reporting
+The <b>event_reporting</b> section contains values to control how often the usage is reported.  
+
+- <b>wake_interval</b> indicates the number of seconds to sleep before waking to determine if there has been enough activity to report usage
+- <b>minimum_count</b> indicates the minimum number of usage records that must be queued up before sending the usage
+- <b>flush_interval</b> indicates the sleep interval before all usage will be flushed to server.
+- <b>trap_exceptions</b> indicates whether exceptions encountered while reporting usage will be trapped and ignored or if it will become an error that gets reported to the application
+- <b>timestamp_granularity</b> indicates the how granular the timestamp will be when reporting events.  Valid values are
+  - "MICROS"  
+    // DEFAULT: values are reported down to the microsecond resolution when possible
+  - "MILLIS"  
+  // values are reported to the millisecond
+  - "SECONDS"  
+  // values are reported to the second
+  - "MINUTES"  
+  // values are reported to minute
+  - "HOURS"  
+  // values are reported to hour
+  - "HALF_DAYS"  
+  // values are reported to half day
+  - "DAYS"  
+  // values are reported to the day
+
+#### Key Caching
+The <b>key_caching</b> section contains values to control how and when keys are cached.
+
+- <b>unstructured</b> indicates whether keys will be cached when doing unstructured decryption. (default: true)
+- <b>encrypt</b> indicates if keys should be stored encrypted. If keys are encrypted, they will be harder to access via memory, but require them to be decrypted with each use. (default: false)
+
+
+```json
+{
+  "event_reporting": {
+    "wake_interval": 1,
+    "minimum_count": 2,
+    "flush_interval": 2,
+    "trap_exceptions": false,
+    "timestamp_granularity" : "MICROS"
+  },
+  "key_caching":{
+    "unstructured": true,
+    "encrypt": false
+  }
+}
 ```
 
 
 [dashboard]:https://dashboard.ubiqsecurity.com/
 [credentials]:https://dev.ubiqsecurity.com/docs/how-to-create-api-keys
```

### Comparing `ubiq-security-2.1.3/ubiq_security.egg-info/SOURCES.txt` & `ubiq_security-2.2.0/ubiq_security.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,11 +12,16 @@
 ubiq_security/events.py
 ubiq_security/version.py
 ubiq_security.egg-info/PKG-INFO
 ubiq_security.egg-info/SOURCES.txt
 ubiq_security.egg-info/dependency_links.txt
 ubiq_security.egg-info/requires.txt
 ubiq_security.egg-info/top_level.txt
-ubiq_security/fpe/__init__.py
-ubiq_security/fpe/common.py
-ubiq_security/fpe/decrypt.py
-ubiq_security/fpe/encrypt.py
+ubiq_security/structured/__init__.py
+ubiq_security/structured/common.py
+ubiq_security/structured/decrypt.py
+ubiq_security/structured/encrypt.py
+ubiq_security/structured/lib/__init__.py
+ubiq_security/structured/lib/ff1.py
+ubiq_security/structured/lib/ff1_test.py
+ubiq_security/structured/lib/ffx.py
+ubiq_security/structured/lib/ffx_test.py
```

