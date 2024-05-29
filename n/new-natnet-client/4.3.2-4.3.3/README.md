# Comparing `tmp/new_natnet_client-4.3.2.tar.gz` & `tmp/new_natnet_client-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_natnet_client-4.3.2.tar", max compression
+gzip compressed data, was "new_natnet_client-4.3.3.tar", max compression
```

## Comparing `new_natnet_client-4.3.2.tar` & `new_natnet_client-4.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.3.2/LICENSE
--rw-r--r--   0        0        0     1758 2024-05-16 01:55:55.789326 new_natnet_client-4.3.2/README.md
--rw-r--r--   0        0        0    16555 2024-05-17 16:08:17.438026 new_natnet_client-4.3.2/new_natnet_client/Client.py
--rw-r--r--   0        0        0     9381 2024-05-16 01:10:23.380136 new_natnet_client-4.3.2/new_natnet_client/NatNetTypes.py
--rw-r--r--   0        0        0    25548 2024-05-16 02:29:37.345534 new_natnet_client-4.3.2/new_natnet_client/Unpackers.py
--rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.3.2/new_natnet_client/__init__.py
--rw-r--r--   0        0        0      464 2024-05-17 16:09:07.777132 new_natnet_client-4.3.2/pyproject.toml
--rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 new_natnet_client-4.3.2/PKG-INFO
+-rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.3.3/LICENSE
+-rw-r--r--   0        0        0     1758 2024-05-16 01:55:55.789326 new_natnet_client-4.3.3/README.md
+-rw-r--r--   0        0        0    16729 2024-05-29 17:18:42.013322 new_natnet_client-4.3.3/new_natnet_client/Client.py
+-rw-r--r--   0        0        0     9381 2024-05-16 01:10:23.380136 new_natnet_client-4.3.3/new_natnet_client/NatNetTypes.py
+-rw-r--r--   0        0        0    25548 2024-05-16 02:29:37.345534 new_natnet_client-4.3.3/new_natnet_client/Unpackers.py
+-rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.3.3/new_natnet_client/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-29 17:19:36.306616 new_natnet_client-4.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 new_natnet_client-4.3.3/PKG-INFO
```

### Comparing `new_natnet_client-4.3.2/LICENSE` & `new_natnet_client-4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.2/README.md` & `new_natnet_client-4.3.3/README.md`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.2/new_natnet_client/Client.py` & `new_natnet_client-4.3.3/new_natnet_client/Client.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,20 +377,23 @@
     logging.info("Data thread stopped")
 
   def __command_thread_function(self) -> None:
     data = bytes()
     logging.info("Command thread start")
     recv_buffer_size=64*1024
     run = True
+    keep_alive = b'\n\x00\x00\x00\x00'
     while run:
       with self.__running_lock:
         run = self.__running
       try:
         with self.__command_socket_lock:
           if self.__command_socket is None: return
+          if not self.use_multicast:
+            self.__command_socket.sendto(keep_alive, (self.server_address, self.command_port))
           data = self.__command_socket.recv(recv_buffer_size)
       except socket.timeout:
         data = bytes()
       except socket.error as msg:
         logging.error(f"Command thread {self.local_ip_address}: {msg}")
         data = bytes()
       if len(data):
```

### Comparing `new_natnet_client-4.3.2/new_natnet_client/NatNetTypes.py` & `new_natnet_client-4.3.3/new_natnet_client/NatNetTypes.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.2/new_natnet_client/Unpackers.py` & `new_natnet_client-4.3.3/new_natnet_client/Unpackers.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.2/PKG-INFO` & `new_natnet_client-4.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: new-natnet-client
-Version: 4.3.2
+Version: 4.3.3
 Summary: natnet client for motive application for python
 Home-page: https://optitrack.com/
 License: GLWTPL
 Author: Ignacio de la Torre Arias
 Author-email: ignaciodlta@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
```

