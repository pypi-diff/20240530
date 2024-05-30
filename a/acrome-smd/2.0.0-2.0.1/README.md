# Comparing `tmp/acrome_smd-2.0.0.tar.gz` & `tmp/acrome_smd-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrome_smd-2.0.0.tar", last modified: Fri May 24 07:29:37 2024, max compression
+gzip compressed data, was "acrome_smd-2.0.1.tar", last modified: Thu May 30 13:32:01 2024, max compression
```

## Comparing `acrome_smd-2.0.0.tar` & `acrome_smd-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:29:37.418239 acrome_smd-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    34174 2024-05-24 07:29:37.418239 acrome_smd-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34326 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:29:37.418239 acrome_smd-2.0.0/acrome_smd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34174 2024-05-24 07:29:37.000000 acrome_smd-2.0.0/acrome_smd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-24 07:29:37.000000 acrome_smd-2.0.0/acrome_smd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:29:37.000000 acrome_smd-2.0.0/acrome_smd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 07:29:37.000000 acrome_smd-2.0.0/acrome_smd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-24 07:29:37.000000 acrome_smd-2.0.0/acrome_smd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:29:37.418239 acrome_smd-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:29:37.414240 acrome_smd-2.0.0/smd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/smd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/smd/_internals.py
--rw-r--r--   0 runner    (1001) docker     (127)    64185 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/smd/red.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:29:37.418239 acrome_smd-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/tests/test_red.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:01.914839 acrome_smd-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 13:31:58.000000 acrome_smd-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    34174 2024-05-30 13:32:01.914839 acrome_smd-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34326 2024-05-30 13:31:58.000000 acrome_smd-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:01.914839 acrome_smd-2.0.1/acrome_smd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34174 2024-05-30 13:32:01.000000 acrome_smd-2.0.1/acrome_smd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-30 13:32:01.000000 acrome_smd-2.0.1/acrome_smd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:32:01.000000 acrome_smd-2.0.1/acrome_smd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 13:32:01.000000 acrome_smd-2.0.1/acrome_smd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 13:32:01.000000 acrome_smd-2.0.1/acrome_smd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:32:01.914839 acrome_smd-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-30 13:31:58.000000 acrome_smd-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:01.914839 acrome_smd-2.0.1/smd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:31:58.000000 acrome_smd-2.0.1/smd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-30 13:31:58.000000 acrome_smd-2.0.1/smd/_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64526 2024-05-30 13:31:58.000000 acrome_smd-2.0.1/smd/red.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:01.914839 acrome_smd-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-30 13:31:58.000000 acrome_smd-2.0.1/tests/test_red.py
```

### Comparing `acrome_smd-2.0.0/LICENSE` & `acrome_smd-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acrome_smd-2.0.0/PKG-INFO` & `acrome_smd-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrome-smd
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python library for interfacing with Acrome Smart Motor Drivers (SMD) products.
 Home-page: https://github.com/Acrome-Smart-Motor-Driver/python-library
 Author: Furkan Kırlangıç
 Author-email: furkankirlangic@acrome.net
 Project-URL: Bug Tracker, https://github.com/Acrome-Smart-Motor-Driver/python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `acrome_smd-2.0.0/README.md` & `acrome_smd-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `acrome_smd-2.0.0/acrome_smd.egg-info/PKG-INFO` & `acrome_smd-2.0.1/acrome_smd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrome-smd
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python library for interfacing with Acrome Smart Motor Drivers (SMD) products.
 Home-page: https://github.com/Acrome-Smart-Motor-Driver/python-library
 Author: Furkan Kırlangıç
 Author-email: furkankirlangic@acrome.net
 Project-URL: Bug Tracker, https://github.com/Acrome-Smart-Motor-Driver/python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `acrome_smd-2.0.0/setup.py` & `acrome_smd-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="acrome-smd",
-    version="2.0.0",
+    version="2.0.1",
     author="Furkan Kırlangıç",
     author_email="furkankirlangic@acrome.net",
     description="Python library for interfacing with Acrome Smart Motor Drivers (SMD) products.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Acrome-Smart-Motor-Driver/python-library",
     project_urls={
```

### Comparing `acrome_smd-2.0.0/smd/_internals.py` & `acrome_smd-2.0.1/smd/_internals.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,15 @@
     'Pot_4',
     'Pot_5',
     'IMU_1',                        
     'IMU_2',
     'IMU_3',
     'IMU_4',
     'IMU_5',
+    'connected_bitfield',
     'CRCValue',
     ], start=0)
 
 
 class _Data():
     def __init__(self, index, var_type, rw=True, value=0):
         self.__index = index
```

### Comparing `acrome_smd-2.0.0/smd/red.py` & `acrome_smd-2.0.1/smd/red.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
             _Data(Index.Pot_4, 'B'),
             _Data(Index.Pot_5, 'B'),
             _Data(Index.IMU_1, 'ff'),
             _Data(Index.IMU_2, 'ff'),
             _Data(Index.IMU_3, 'ff'),
             _Data(Index.IMU_4, 'ff'),
             _Data(Index.IMU_5, 'ff'),
+            _Data(Index.connected_bitfield, 'II'),
             _Data(Index.CRCValue, 'I')
         ]
 
         if ID > 255 or ID < 0:
             raise ValueError("Device ID can not be higher than 254 or lower than 0!")
         else:
             self.vars[Index.DeviceID].value(ID)
@@ -725,28 +726,39 @@
 
         Returns:
             list: List of the protocol IDs of the connected sensors otherwise None.
         """
 
         _ID_OFFSETS = [[1, Index.Button_1], [6, Index.Light_1], [11, Index.Buzzer_1], [16, Index.Joystick_1], [21, Index.Distance_1], [26, Index.QTR_1], [31, Index.Servo_1], [36, Index.Pot_1], [41, Index.RGB_1], [46, Index.IMU_1]]
         self.__write_bus(self.__driver_list[id].scan_modules())
-        time.sleep(2)
-        self.__write_bus(self.__driver_list[id].scan_modules())
-        ret = self.__read_bus(18)
-        if len(ret) == 18:
-            if CRC32.calc(ret[:-4]) == struct.unpack('<I', ret[-4:])[0]:
-                data = struct.unpack('<Q', ret[6:-4])[0]
-                addrs = [i for i in range(64) if (data & (1 << i)) == (1 << i)]
-                result = []
-                for addr in addrs:
-                    result.append((Index(addr - _ID_OFFSETS[int((addr - 1) / 5)][0] + _ID_OFFSETS[int((addr - 1) / 5)][1])).name)
-                return result
-        else:
+        time.sleep(5.5)
+        connected = None
+        for i in range(0,10):
+            try:
+                connected = self.get_variables(id, [Index.connected_bitfield])[0]
+                if connected == None:
+                    pass
+                else:
+                    break
+            except:
+                pass
+        if connected == None:
             return None
-        
+        else:
+            value1 = 0x12345678  # Örnek değer 1
+            value2 = 0x9ABCDEF0  # Örnek değer 2
+
+            # 64-bitlik tek bir değere dönüştürme
+            connected = (connected[1] << 32) | connected[0]
+            result = []
+            addrs = [i for i in range(64) if (connected & (1 << i)) == (1 << i)]
+            for addr in addrs:
+                result.append((Index(addr - _ID_OFFSETS[int((addr - 1) / 5)][0] + _ID_OFFSETS[int((addr - 1) / 5)][1])).name)
+            return result
+
     def set_connected_modules(self, id: int, modules: list):
         """ Set the list of sensor IDs which are connected to the driver.
 
         Args:
             id (int): The device ID of the driver.
             modules (list): List of the protocol IDs of the connected sensors.
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `acrome_smd-2.0.0/tests/test_red.py` & `acrome_smd-2.0.1/tests/test_red.py`

 * *Files identical despite different names*

