# Comparing `tmp/lightphe-0.0.6.tar.gz` & `tmp/lightphe-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightphe-0.0.6.tar", last modified: Fri Jan 26 17:37:16 2024, max compression
+gzip compressed data, was "dist/lightphe-0.0.7.tar", last modified: Thu May 30 18:35:46 2024, max compression
```

## Comparing `lightphe-0.0.6.tar` & `lightphe-0.0.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-01-26 17:37:16.460300 lightphe-0.0.6/
--rw-r--r--   0 sefik      (501) staff       (20)     1076 2023-11-19 11:42:45.000000 lightphe-0.0.6/LICENSE
--rw-r--r--   0 sefik      (501) staff       (20)    11486 2024-01-26 17:37:16.459982 lightphe-0.0.6/PKG-INFO
--rw-r--r--   0 sefik      (501) staff       (20)    10978 2024-01-26 17:36:03.000000 lightphe-0.0.6/README.md
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-01-26 17:37:16.448265 lightphe-0.0.6/lightphe/
--rw-r--r--   0 sefik      (501) staff       (20)    13538 2024-01-26 17:36:03.000000 lightphe-0.0.6/lightphe/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-01-26 17:37:16.450165 lightphe-0.0.6/lightphe/commons/
--rw-r--r--   0 sefik      (501) staff       (20)        0 2023-11-23 19:13:11.000000 lightphe-0.0.6/lightphe/commons/__init__.py
--rw-r--r--   0 sefik      (501) staff       (20)     1236 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/commons/logger.py
--rw-r--r--   0 sefik      (501) staff       (20)     1967 2023-12-20 19:16:18.000000 lightphe-0.0.6/lightphe/commons/phe_utils.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-01-26 17:37:16.452621 lightphe-0.0.6/lightphe/cryptosystems/
--rw-r--r--   0 sefik      (501) staff       (20)     7204 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/cryptosystems/Benaloh.py
--rw-r--r--   0 sefik      (501) staff       (20)     6601 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/cryptosystems/DamgardJurik.py
--rw-r--r--   0 sefik      (501) staff       (20)     7357 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/cryptosystems/ElGamal.py
--rw-r--r--   0 sefik      (501) staff       (20)     6154 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/cryptosystems/EllipticCurveElGamal.py
--rw-r--r--   0 sefik      (501) staff       (20)     5567 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/cryptosystems/GoldwasserMicali.py
--rw-r--r--   0 sefik      (501) staff       (20)    11531 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/cryptosystems/NaccacheStern.py
--rw-r--r--   0 sefik      (501) staff       (20)     6716 2024-01-26 17:36:03.000000 lightphe-0.0.6/lightphe/cryptosystems/OkamotoUchiyama.py
--rw-r--r--   0 sefik      (501) staff       (20)     5866 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/cryptosystems/Paillier.py
--rw-r--r--   0 sefik      (501) staff       (20)     5277 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/cryptosystems/RSA.py
--rw-r--r--   0 sefik      (501) staff       (20)        0 2023-11-23 19:13:14.000000 lightphe-0.0.6/lightphe/cryptosystems/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-01-26 17:37:16.453027 lightphe-0.0.6/lightphe/elliptic/
--rw-r--r--   0 sefik      (501) staff       (20)     3147 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/elliptic/Weierstrass.py
--rw-r--r--   0 sefik      (501) staff       (20)        0 2023-11-23 19:13:16.000000 lightphe-0.0.6/lightphe/elliptic/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-01-26 17:37:16.454267 lightphe-0.0.6/lightphe/models/
--rw-r--r--   0 sefik      (501) staff       (20)      402 2023-11-19 11:42:45.000000 lightphe-0.0.6/lightphe/models/Algorithm.py
--rw-r--r--   0 sefik      (501) staff       (20)     5137 2023-12-20 19:16:18.000000 lightphe-0.0.6/lightphe/models/Ciphertext.py
--rw-r--r--   0 sefik      (501) staff       (20)      468 2023-11-19 11:42:45.000000 lightphe-0.0.6/lightphe/models/EllipticCurve.py
--rw-r--r--   0 sefik      (501) staff       (20)     1354 2023-12-12 17:42:37.000000 lightphe-0.0.6/lightphe/models/Homomorphic.py
--rw-r--r--   0 sefik      (501) staff       (20)     6438 2023-12-20 19:16:18.000000 lightphe-0.0.6/lightphe/models/Tensor.py
--rw-r--r--   0 sefik      (501) staff       (20)        0 2023-11-23 19:13:20.000000 lightphe-0.0.6/lightphe/models/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-01-26 17:37:16.449414 lightphe-0.0.6/lightphe.egg-info/
--rw-r--r--   0 sefik      (501) staff       (20)    11486 2024-01-26 17:37:15.000000 lightphe-0.0.6/lightphe.egg-info/PKG-INFO
--rw-r--r--   0 sefik      (501) staff       (20)     1250 2024-01-26 17:37:16.000000 lightphe-0.0.6/lightphe.egg-info/SOURCES.txt
--rw-r--r--   0 sefik      (501) staff       (20)        1 2024-01-26 17:37:15.000000 lightphe-0.0.6/lightphe.egg-info/dependency_links.txt
--rw-r--r--   0 sefik      (501) staff       (20)       26 2024-01-26 17:37:16.000000 lightphe-0.0.6/lightphe.egg-info/requires.txt
--rw-r--r--   0 sefik      (501) staff       (20)       15 2024-01-26 17:37:16.000000 lightphe-0.0.6/lightphe.egg-info/top_level.txt
--rw-r--r--   0 sefik      (501) staff       (20)       25 2023-11-19 11:42:45.000000 lightphe-0.0.6/requirements.txt
--rw-r--r--   0 sefik      (501) staff       (20)       38 2024-01-26 17:37:16.460386 lightphe-0.0.6/setup.cfg
--rw-r--r--   0 sefik      (501) staff       (20)      898 2024-01-26 17:36:03.000000 lightphe-0.0.6/setup.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-01-26 17:37:16.459285 lightphe-0.0.6/tests/
--rw-r--r--   0 sefik      (501) staff       (20)     8478 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/__init__.py
--rw-r--r--   0 sefik      (501) staff       (20)     1546 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/test_benaloh.py
--rw-r--r--   0 sefik      (501) staff       (20)     1541 2024-01-26 17:36:03.000000 lightphe-0.0.6/tests/test_cloud.py
--rw-r--r--   0 sefik      (501) staff       (20)     1574 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/test_damgard.py
--rw-r--r--   0 sefik      (501) staff       (20)     3549 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/test_elgamal.py
--rw-r--r--   0 sefik      (501) staff       (20)     1535 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/test_ellipticcurveelgamal.py
--rw-r--r--   0 sefik      (501) staff       (20)      888 2024-01-26 17:36:03.000000 lightphe-0.0.6/tests/test_exporting_keys.py
--rw-r--r--   0 sefik      (501) staff       (20)     1371 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/test_goldwasser.py
--rw-r--r--   0 sefik      (501) staff       (20)     2427 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/test_naccache.py
--rw-r--r--   0 sefik      (501) staff       (20)     1575 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/test_okamoto.py
--rw-r--r--   0 sefik      (501) staff       (20)     2336 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/test_paillier.py
--rw-r--r--   0 sefik      (501) staff       (20)     1644 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/test_rsa.py
--rw-r--r--   0 sefik      (501) staff       (20)     1570 2023-12-12 17:42:37.000000 lightphe-0.0.6/tests/test_salary.py
--rw-r--r--   0 sefik      (501) staff       (20)     4773 2023-12-20 19:16:18.000000 lightphe-0.0.6/tests/test_tensors.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-30 18:35:46.955000 lightphe-0.0.7/
+-rw-r--r--   0 sefik      (501) staff       (20)     1076 2023-11-19 11:42:45.000000 lightphe-0.0.7/LICENSE
+-rw-r--r--   0 sefik      (501) staff       (20)    11486 2024-05-30 18:35:46.954700 lightphe-0.0.7/PKG-INFO
+-rw-r--r--   0 sefik      (501) staff       (20)    10978 2024-01-26 17:36:03.000000 lightphe-0.0.7/README.md
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-30 18:35:46.933474 lightphe-0.0.7/lightphe/
+-rw-r--r--   0 sefik      (501) staff       (20)    13538 2024-01-26 17:36:03.000000 lightphe-0.0.7/lightphe/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-30 18:35:46.936115 lightphe-0.0.7/lightphe/commons/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2023-11-23 19:13:11.000000 lightphe-0.0.7/lightphe/commons/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1236 2023-12-12 17:42:37.000000 lightphe-0.0.7/lightphe/commons/logger.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1967 2023-12-20 19:16:18.000000 lightphe-0.0.7/lightphe/commons/phe_utils.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-30 18:35:46.940386 lightphe-0.0.7/lightphe/cryptosystems/
+-rw-r--r--   0 sefik      (501) staff       (20)     7204 2023-12-12 17:42:37.000000 lightphe-0.0.7/lightphe/cryptosystems/Benaloh.py
+-rw-r--r--   0 sefik      (501) staff       (20)     6601 2023-12-12 17:42:37.000000 lightphe-0.0.7/lightphe/cryptosystems/DamgardJurik.py
+-rw-r--r--   0 sefik      (501) staff       (20)     7606 2024-05-30 18:33:47.000000 lightphe-0.0.7/lightphe/cryptosystems/ElGamal.py
+-rw-r--r--   0 sefik      (501) staff       (20)     6154 2023-12-12 17:42:37.000000 lightphe-0.0.7/lightphe/cryptosystems/EllipticCurveElGamal.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5756 2024-05-29 18:28:26.000000 lightphe-0.0.7/lightphe/cryptosystems/GoldwasserMicali.py
+-rw-r--r--   0 sefik      (501) staff       (20)    11531 2023-12-12 17:42:37.000000 lightphe-0.0.7/lightphe/cryptosystems/NaccacheStern.py
+-rw-r--r--   0 sefik      (501) staff       (20)     6716 2024-01-26 17:36:03.000000 lightphe-0.0.7/lightphe/cryptosystems/OkamotoUchiyama.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5866 2023-12-12 17:42:37.000000 lightphe-0.0.7/lightphe/cryptosystems/Paillier.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5277 2023-12-12 17:42:37.000000 lightphe-0.0.7/lightphe/cryptosystems/RSA.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2023-11-23 19:13:14.000000 lightphe-0.0.7/lightphe/cryptosystems/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-30 18:35:46.941229 lightphe-0.0.7/lightphe/elliptic/
+-rw-r--r--   0 sefik      (501) staff       (20)     3147 2023-12-12 17:42:37.000000 lightphe-0.0.7/lightphe/elliptic/Weierstrass.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2023-11-23 19:13:16.000000 lightphe-0.0.7/lightphe/elliptic/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-30 18:35:46.944458 lightphe-0.0.7/lightphe/models/
+-rw-r--r--   0 sefik      (501) staff       (20)      402 2023-11-19 11:42:45.000000 lightphe-0.0.7/lightphe/models/Algorithm.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5137 2023-12-20 19:16:18.000000 lightphe-0.0.7/lightphe/models/Ciphertext.py
+-rw-r--r--   0 sefik      (501) staff       (20)      468 2023-11-19 11:42:45.000000 lightphe-0.0.7/lightphe/models/EllipticCurve.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1354 2023-12-12 17:42:37.000000 lightphe-0.0.7/lightphe/models/Homomorphic.py
+-rw-r--r--   0 sefik      (501) staff       (20)     6438 2023-12-20 19:16:18.000000 lightphe-0.0.7/lightphe/models/Tensor.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2023-11-23 19:13:20.000000 lightphe-0.0.7/lightphe/models/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-30 18:35:46.935268 lightphe-0.0.7/lightphe.egg-info/
+-rw-r--r--   0 sefik      (501) staff       (20)    11486 2024-05-30 18:35:46.000000 lightphe-0.0.7/lightphe.egg-info/PKG-INFO
+-rw-r--r--   0 sefik      (501) staff       (20)     1250 2024-05-30 18:35:46.000000 lightphe-0.0.7/lightphe.egg-info/SOURCES.txt
+-rw-r--r--   0 sefik      (501) staff       (20)        1 2024-05-30 18:35:46.000000 lightphe-0.0.7/lightphe.egg-info/dependency_links.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       26 2024-05-30 18:35:46.000000 lightphe-0.0.7/lightphe.egg-info/requires.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       15 2024-05-30 18:35:46.000000 lightphe-0.0.7/lightphe.egg-info/top_level.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       25 2023-11-19 11:42:45.000000 lightphe-0.0.7/requirements.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       38 2024-05-30 18:35:46.955122 lightphe-0.0.7/setup.cfg
+-rw-r--r--   0 sefik      (501) staff       (20)      898 2024-05-30 18:34:49.000000 lightphe-0.0.7/setup.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-30 18:35:46.953431 lightphe-0.0.7/tests/
+-rw-r--r--   0 sefik      (501) staff       (20)     8478 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1546 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/test_benaloh.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1541 2024-01-26 17:36:03.000000 lightphe-0.0.7/tests/test_cloud.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1574 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/test_damgard.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3549 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/test_elgamal.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1535 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/test_ellipticcurveelgamal.py
+-rw-r--r--   0 sefik      (501) staff       (20)      888 2024-01-26 17:36:03.000000 lightphe-0.0.7/tests/test_exporting_keys.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1371 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/test_goldwasser.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2427 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/test_naccache.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1575 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/test_okamoto.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2336 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/test_paillier.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1644 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/test_rsa.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1570 2023-12-12 17:42:37.000000 lightphe-0.0.7/tests/test_salary.py
+-rw-r--r--   0 sefik      (501) staff       (20)     4773 2023-12-20 19:16:18.000000 lightphe-0.0.7/tests/test_tensors.py
```

### Comparing `lightphe-0.0.6/LICENSE` & `lightphe-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/PKG-INFO` & `lightphe-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightphe
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Lightweight Partially Homomorphic Encryption Library for Python
 Home-page: https://github.com/serengil/LightPHE
 Author: Sefik Ilkin Serengil
 Author-email: serengil@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lightphe-0.0.6/README.md` & `lightphe-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/__init__.py` & `lightphe-0.0.7/lightphe/__init__.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/commons/logger.py` & `lightphe-0.0.7/lightphe/commons/logger.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/commons/phe_utils.py` & `lightphe-0.0.7/lightphe/commons/phe_utils.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/cryptosystems/Benaloh.py` & `lightphe-0.0.7/lightphe/cryptosystems/Benaloh.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/cryptosystems/DamgardJurik.py` & `lightphe-0.0.7/lightphe/cryptosystems/DamgardJurik.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/cryptosystems/ElGamal.py` & `lightphe-0.0.7/lightphe/cryptosystems/ElGamal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+# built-in dependencies
 import random
-import math
+import decimal
 from typing import Optional
+
+# 3rd party dependencies
 import sympy
+
+# project dependencies
 from lightphe.models.Homomorphic import Homomorphic
 from lightphe.commons.logger import Logger
 
 logger = Logger(module="lightphe/cryptosystems/ElGamal.py")
 
 
 class ElGamal(Homomorphic):
@@ -41,15 +46,17 @@
         keys["private_key"] = {}
         keys["public_key"] = {}
 
         # picking a prime modulus p
         p = sympy.randprime(100, 2 ** int(key_size / 2) - 1)
 
         # picking a generator g
-        g = random.randint(2, int(math.sqrt(p)))
+        # g = random.randint(2, int(math.sqrt(p))) # reaches int limit for 3072-bit key
+        # g = int(random.uniform(2, float(decimal.Decimal(p).sqrt())))
+        g = random.randint(2, int(decimal.Decimal(p).sqrt()))
 
         # picking a private key x
         x = random.randint(1, p - 2)
 
         # public key
         y = pow(g, x, p)
```

### Comparing `lightphe-0.0.6/lightphe/cryptosystems/EllipticCurveElGamal.py` & `lightphe-0.0.7/lightphe/cryptosystems/EllipticCurveElGamal.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/cryptosystems/GoldwasserMicali.py` & `lightphe-0.0.7/lightphe/cryptosystems/GoldwasserMicali.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,20 @@
         p = self.keys["private_key"]["p"]
         q = self.keys["private_key"]["q"]
 
         for i in ciphertext:
             xp = i % p
             xq = i % q
 
-            if pow(xp, int((p - 1) / 2), p) == 1 and pow(xq, int((q - 1) / 2), q) == 1:
+            # reaches int limit for 3072-bit key
+            # if pow(xp, int((p - 1) / 2), p) == 1 and pow(xq, int((q - 1) / 2), q) == 1:
+            if (
+                pow(xp, int((p - 1) // 2), p) == 1
+                and pow(xq, int((q - 1) // 2), q) == 1
+            ):
                 m_binaries.append("0")
             else:
                 m_binaries.append("1")
 
         m_binary = "".join(m_binaries)
         return int(m_binary, 2)
```

### Comparing `lightphe-0.0.6/lightphe/cryptosystems/NaccacheStern.py` & `lightphe-0.0.7/lightphe/cryptosystems/NaccacheStern.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/cryptosystems/OkamotoUchiyama.py` & `lightphe-0.0.7/lightphe/cryptosystems/OkamotoUchiyama.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/cryptosystems/Paillier.py` & `lightphe-0.0.7/lightphe/cryptosystems/Paillier.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/cryptosystems/RSA.py` & `lightphe-0.0.7/lightphe/cryptosystems/RSA.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/elliptic/Weierstrass.py` & `lightphe-0.0.7/lightphe/elliptic/Weierstrass.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/models/Ciphertext.py` & `lightphe-0.0.7/lightphe/models/Ciphertext.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/models/Homomorphic.py` & `lightphe-0.0.7/lightphe/models/Homomorphic.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe/models/Tensor.py` & `lightphe-0.0.7/lightphe/models/Tensor.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/lightphe.egg-info/PKG-INFO` & `lightphe-0.0.7/lightphe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightphe
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Lightweight Partially Homomorphic Encryption Library for Python
 Home-page: https://github.com/serengil/LightPHE
 Author: Sefik Ilkin Serengil
 Author-email: serengil@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lightphe-0.0.6/lightphe.egg-info/SOURCES.txt` & `lightphe-0.0.7/lightphe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/setup.py` & `lightphe-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.read().split("\n")
 
 setuptools.setup(
     name="lightphe",
-    version="0.0.6",
+    version="0.0.7",
     author="Sefik Ilkin Serengil",
     author_email="serengil@gmail.com",
     description="A Lightweight Partially Homomorphic Encryption Library for Python",
     data_files=[("", ["README.md", "requirements.txt"])],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/serengil/LightPHE",
```

### Comparing `lightphe-0.0.6/tests/__init__.py` & `lightphe-0.0.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_benaloh.py` & `lightphe-0.0.7/tests/test_benaloh.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_cloud.py` & `lightphe-0.0.7/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_damgard.py` & `lightphe-0.0.7/tests/test_damgard.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_elgamal.py` & `lightphe-0.0.7/tests/test_elgamal.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_ellipticcurveelgamal.py` & `lightphe-0.0.7/tests/test_ellipticcurveelgamal.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_exporting_keys.py` & `lightphe-0.0.7/tests/test_exporting_keys.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_goldwasser.py` & `lightphe-0.0.7/tests/test_goldwasser.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_naccache.py` & `lightphe-0.0.7/tests/test_naccache.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_okamoto.py` & `lightphe-0.0.7/tests/test_okamoto.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_paillier.py` & `lightphe-0.0.7/tests/test_paillier.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_rsa.py` & `lightphe-0.0.7/tests/test_rsa.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_salary.py` & `lightphe-0.0.7/tests/test_salary.py`

 * *Files identical despite different names*

### Comparing `lightphe-0.0.6/tests/test_tensors.py` & `lightphe-0.0.7/tests/test_tensors.py`

 * *Files identical despite different names*

