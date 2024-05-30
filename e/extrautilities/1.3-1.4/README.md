# Comparing `tmp/extrautilities-1.3.tar.gz` & `tmp/extrautilities-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-1.3.tar", last modified: Sun May 26 08:26:45 2024, max compression
+gzip compressed data, was "extrautilities-1.4.tar", last modified: Wed May 29 18:25:05 2024, max compression
```

## Comparing `extrautilities-1.3.tar` & `extrautilities-1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 08:26:45.507007 extrautilities-1.3/
-drwxrwxrwx   0        0        0        0 2024-05-26 08:26:45.492727 extrautilities-1.3/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.3/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.3/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-1.3/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-1.3/ExtraUtils/callbackVoid.py
--rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.3/ExtraUtils/getFileContent.py
--rw-rw-rw-   0        0        0     4453 2024-05-16 16:25:09.000000 extrautilities-1.3/ExtraUtils/timeBasedToken.py
--rw-rw-rw-   0        0        0     2032 2024-05-25 07:02:09.000000 extrautilities-1.3/ExtraUtils/validate_dict.py
--rw-rw-rw-   0        0        0     3349 2024-05-26 08:26:45.506004 extrautilities-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 08:26:45.505505 extrautilities-1.3/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     3349 2024-05-26 08:26:45.000000 extrautilities-1.3/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-05-26 08:26:45.000000 extrautilities-1.3/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 08:26:45.000000 extrautilities-1.3/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 08:26:45.000000 extrautilities-1.3/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-26 08:26:45.000000 extrautilities-1.3/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 08:26:45.507007 extrautilities-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1132 2024-05-26 08:26:40.000000 extrautilities-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:25:05.862550 extrautilities-1.4/
+drwxrwxrwx   0        0        0        0 2024-05-29 18:25:05.846329 extrautilities-1.4/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.4/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.4/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0     2258 2024-05-29 18:24:23.000000 extrautilities-1.4/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-1.4/ExtraUtils/callbackVoid.py
+-rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.4/ExtraUtils/getFileContent.py
+-rw-rw-rw-   0        0        0     3181 2024-05-28 18:10:03.000000 extrautilities-1.4/ExtraUtils/timeBasedToken.py
+-rw-rw-rw-   0        0        0     2032 2024-05-25 07:02:09.000000 extrautilities-1.4/ExtraUtils/validate_dict.py
+-rw-rw-rw-   0        0        0     3349 2024-05-29 18:25:05.862550 extrautilities-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 18:25:05.861042 extrautilities-1.4/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     3349 2024-05-29 18:25:05.000000 extrautilities-1.4/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-29 18:25:05.000000 extrautilities-1.4/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:25:05.000000 extrautilities-1.4/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:25:05.000000 extrautilities-1.4/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 18:25:05.000000 extrautilities-1.4/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:25:05.863569 extrautilities-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2024-05-29 18:24:30.000000 extrautilities-1.4/setup.py
```

### Comparing `extrautilities-1.3/ExtraUtils/RateLimit.py` & `extrautilities-1.4/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.3/ExtraUtils/asyncTokens.py` & `extrautilities-1.4/ExtraUtils/asyncTokens.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,18 +23,33 @@
             algorithm=hashes.SHA256(),
             label=None
         )
     )
     return message
 
 def serial(key):
-    return key.public_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PublicFormat.SubjectPublicKeyInfo
-    ).decode('utf-8')
+    try:
+        return key.public_bytes(
+            encoding=serialization.Encoding.PEM,
+            format=serialization.PublicFormat.SubjectPublicKeyInfo
+        ).decode('utf-8')
+    except AttributeError:
+        return key.private_bytes(
+            encoding=serialization.Encoding.PEM,
+            format=serialization.PrivateFormat.TraditionalOpenSSL,
+            encryption_algorithm=serialization.NoEncryption()
+        ).decode('utf-8')
+
+def load_private(key):
+    priv_key = serialization.load_pem_private_key(
+        key.encode('utf-8'),
+        password=None,
+        backend=default_backend()
+    )
+    return priv_key
 
 def load(key):
     pub_key = load_pem_public_key(
         key.encode('utf-8'),
         backend=default_backend()
     )
     return pub_key
```

### Comparing `extrautilities-1.3/ExtraUtils/getFileContent.py` & `extrautilities-1.4/ExtraUtils/getFileContent.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.3/ExtraUtils/timeBasedToken.py` & `extrautilities-1.4/ExtraUtils/timeBasedToken.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,90 +12,54 @@
         self.__enckey = None
         if not primary_toke or not secondary_token:
             raise ValueError("Token can't be empty")
         if not isinstance(primary_toke, str) or not isinstance(secondary_token, str):
             raise ValueError("Token must be string")
         self.__primary = primary_toke
         self.__special = secondary_token
-        self.__iv = None
         self.regenerate()
-        self.__geniv()
 
 
     def regenerate(self):
-        # Berechne den gerundeten Unix-Zeitstempel
         timestamp = int(time.time() // 10 * 10)
-
-        # Kombiniere Token und Zeitstempel und erstelle einen SHA-256 Hash
         combined = f"{self.__special}{timestamp}".encode()
         hash_result = hashlib.sha256(combined).hexdigest()
-
-        # Erstelle eine Bitmap aus den ersten 8 Zeichen des Hashes
         bitmap = bin(int(hash_result[:8], 16))[2:].zfill(32)
-
-
-        # Erstelle eine "zufällige" Reihenfolge aus den nächsten 8 Zeichen
         order_seed = int(hash_result[8:16], 16)
         order = sorted(range(32), key=lambda x: (order_seed >> (x % 8)) & 1)
-
-
-        # Extrahiere und sortiere Zeichen basierend auf der Bitmap und der Reihenfolge
         extracted_chars = ''.join([self.__special[i] for i, bit in enumerate(bitmap) if bit == '1'])
         sorted_chars = ''.join([extracted_chars[i] for i in order if i < len(extracted_chars)])
-
-        # Kombiniere den self.__primary mit den sortierten Zeichen und erstelle einen finalen Hash
         final_combined = f"{self.__primary}{sorted_chars}".encode()
         final_hash = hashlib.sha256(final_combined).hexdigest()
         self.__enckey = final_hash
         return str(final_hash)
     
-    def __geniv(self):
-        # Kombiniere die Token
-        combined_tokens = self.__primary + self.__special
-
-        # Erstelle einen SHA-256 Hash des kombinierten Strings
-        hash_obj = SHA256.new(combined_tokens.encode())
-
-        # Extrahiere die ersten 16 Bytes des Hashes für den IV
-        iv = hash_obj.digest()[:16]
-
-        self.__iv = iv
-    
     def encrypt(self, plaintext):
-        # Konvertiere den Hex-Schlüssel in Bytes
+        # Generiere einen zufälligen IV für jede Verschlüsselung
+        iv = get_random_bytes(AES.block_size)
         key_bytes = bytes.fromhex(self.__enckey)
-        
-        # Initialisiere den AES Cipher im CBC Modus
-        cipher = AES.new(key_bytes, AES.MODE_CBC, self.__iv)
-        
-        # Verschlüssle den Klartext mit Padding
+
+        cipher = AES.new(key_bytes, AES.MODE_CBC, iv)
         encrypted_bytes = cipher.encrypt(pad(plaintext.encode(), AES.block_size))
-        
-        # Kombiniere IV und verschlüsselten Text, kodiere beides in Base64 für einfache Handhabung
-        encrypted_data = base64.b64encode(self.__iv + encrypted_bytes).decode()
-        
+        encrypted_data = base64.b64encode(iv + encrypted_bytes).decode()
         return encrypted_data
 
     def decrypt(self, encrypted):
         # Konvertiere den Hex-Schlüssel in Bytes
         key_bytes = bytes.fromhex(self.__enckey)
-        if not encrypted:
-            raise ValueError("Encrypted data can't be empty")
         if not isinstance(encrypted, str):
             raise ValueError("Encrypted data must be string")
         # Dekodiere die Daten aus Base64
         encrypted_bytes = base64.b64decode(encrypted)
         
 
+        iv = encrypted_bytes[:AES.block_size]
         encrypted_text = encrypted_bytes[AES.block_size:]
-        
-        # Initialisiere den AES Cipher im CBC Modus
-        cipher = AES.new(key_bytes, AES.MODE_CBC, self.__iv)
-        
-        # Entschlüssle den Text und entferne das Padding
+
+        cipher = AES.new(key_bytes, AES.MODE_CBC, iv)
         decrypted_bytes = unpad(cipher.decrypt(encrypted_text), AES.block_size)
         
         return decrypted_bytes.decode()
     
     def __str__(self):
         return self.__enckey
```

### Comparing `extrautilities-1.3/ExtraUtils/validate_dict.py` & `extrautilities-1.4/ExtraUtils/validate_dict.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.3/PKG-INFO` & `extrautilities-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.3
+Version: 1.4
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid,validate_dict
 Platform: UNKNOWN
```

### Comparing `extrautilities-1.3/README.md` & `extrautilities-1.4/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-1.3/extrautilities.egg-info/PKG-INFO` & `extrautilities-1.4/extrautilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.3
+Version: 1.4
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid,validate_dict
 Platform: UNKNOWN
```

### Comparing `extrautilities-1.3/setup.py` & `extrautilities-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='1.3',
+    version='1.4',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
```

