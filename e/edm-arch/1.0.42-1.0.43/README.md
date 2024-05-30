# Comparing `tmp/edm_arch-1.0.42.tar.gz` & `tmp/edm_arch-1.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\mcpherro\Local\Source\Python3\edmpy\dist\.tmp-olnn701_\edm_arch-1.0.42.tar", last modified: Wed May 22 13:47:14 2024, max compression
+gzip compressed data, was "C:\Users\mcpherro\Local\Source\Python3\edmpy\dist\.tmp-06l4xtw9\edm_arch-1.0.43.tar", last modified: Thu May 30 13:49:17 2024, max compression
```

## Comparing `edm_arch-1.0.42.tar` & `edm_arch-1.0.43.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:14.537700 edm_arch-1.0.42/
--rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm_arch-1.0.42/LICENSE
--rw-rw-rw-   0        0        0    23114 2024-05-22 13:47:14.536700 edm_arch-1.0.42/PKG-INFO
--rw-rw-rw-   0        0        0    21741 2024-05-22 13:45:45.000000 edm_arch-1.0.42/README.md
--rw-rw-rw-   0        0        0      523 2023-05-11 08:29:35.000000 edm_arch-1.0.42/pyproject.toml
--rw-rw-rw-   0        0        0     1277 2024-05-22 13:47:14.538700 edm_arch-1.0.42/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm_arch-1.0.42/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:14.498896 edm_arch-1.0.42/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:14.535672 edm_arch-1.0.42/src/edm_arch.egg-info/
--rw-rw-rw-   0        0        0    23114 2024-05-22 13:47:14.000000 edm_arch-1.0.42/src/edm_arch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-05-22 13:47:14.000000 edm_arch-1.0.42/src/edm_arch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:47:14.000000 edm_arch-1.0.42/src/edm_arch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm_arch-1.0.42/src/edm_arch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      182 2024-05-22 13:47:14.000000 edm_arch-1.0.42/src/edm_arch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-22 13:47:14.000000 edm_arch-1.0.42/src/edm_arch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:14.528516 edm_arch-1.0.42/src/edmpy/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm_arch-1.0.42/src/edmpy/__init__.py
--rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm_arch-1.0.42/src/edmpy/__main__.py
--rw-rw-rw-   0        0        0    28555 2023-12-06 09:35:46.000000 edm_arch-1.0.42/src/edmpy/cfg.py
--rw-rw-rw-   0        0        0     2125 2023-12-04 13:37:08.000000 edm_arch-1.0.42/src/edmpy/constants.py
--rw-rw-rw-   0        0        0     5450 2023-12-06 09:37:10.000000 edm_arch-1.0.42/src/edmpy/db.py
--rw-rw-rw-   0        0        0    13431 2023-12-05 09:27:43.000000 edm_arch-1.0.42/src/edmpy/edm.kv
--rw-rw-rw-   0        0        0   126256 2024-05-22 13:13:38.000000 edm_arch-1.0.42/src/edmpy/edm.py
--rw-rw-rw-   0        0        0     5653 2024-04-18 08:18:35.000000 edm_arch-1.0.42/src/edmpy/geo.py
--rw-rw-rw-   0        0        0     2495 2023-12-06 09:36:13.000000 edm_arch-1.0.42/src/edmpy/ini.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:14.534671 edm_arch-1.0.42/src/edmpy/lib/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm_arch-1.0.42/src/edmpy/lib/__init__.py
--rw-rw-rw-   0        0        0     4204 2023-12-04 14:38:01.000000 edm_arch-1.0.42/src/edmpy/lib/blockdata.py
--rw-rw-rw-   0        0        0     4333 2023-12-06 09:31:45.000000 edm_arch-1.0.42/src/edmpy/lib/colorscheme.py
--rw-rw-rw-   0        0        0     3994 2023-12-04 14:40:09.000000 edm_arch-1.0.42/src/edmpy/lib/dbs.py
--rw-rw-rw-   0        0        0   195835 2024-05-22 13:06:32.000000 edm_arch-1.0.42/src/edmpy/lib/e5_widgets.py
--rw-rw-rw-   0        0        0     1812 2023-12-04 14:41:01.000000 edm_arch-1.0.42/src/edmpy/lib/misc.py
--rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm_arch-1.0.42/src/edmpy/py.typed
--rw-rw-rw-   0        0        0      531 2024-04-16 00:42:15.000000 edm_arch-1.0.42/src/edmpy/test_edm.py
--rw-rw-rw-   0        0        0    46620 2024-04-18 08:16:59.000000 edm_arch-1.0.42/src/edmpy/totalstation.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:17.620255 edm_arch-1.0.43/
+-rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm_arch-1.0.43/LICENSE
+-rw-rw-rw-   0        0        0    23234 2024-05-30 13:49:17.620255 edm_arch-1.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0    21861 2024-05-30 13:46:27.000000 edm_arch-1.0.43/README.md
+-rw-rw-rw-   0        0        0      523 2023-05-11 08:29:35.000000 edm_arch-1.0.43/pyproject.toml
+-rw-rw-rw-   0        0        0     1277 2024-05-30 13:49:17.623245 edm_arch-1.0.43/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm_arch-1.0.43/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:17.558634 edm_arch-1.0.43/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:17.617248 edm_arch-1.0.43/src/edm_arch.egg-info/
+-rw-rw-rw-   0        0        0    23234 2024-05-30 13:49:17.000000 edm_arch-1.0.43/src/edm_arch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-05-30 13:49:17.000000 edm_arch-1.0.43/src/edm_arch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 13:49:17.000000 edm_arch-1.0.43/src/edm_arch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm_arch-1.0.43/src/edm_arch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      182 2024-05-30 13:49:17.000000 edm_arch-1.0.43/src/edm_arch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 13:49:17.000000 edm_arch-1.0.43/src/edm_arch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:17.605242 edm_arch-1.0.43/src/edmpy/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm_arch-1.0.43/src/edmpy/__init__.py
+-rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm_arch-1.0.43/src/edmpy/__main__.py
+-rw-rw-rw-   0        0        0    28555 2023-12-06 09:35:46.000000 edm_arch-1.0.43/src/edmpy/cfg.py
+-rw-rw-rw-   0        0        0     2125 2023-12-04 13:37:08.000000 edm_arch-1.0.43/src/edmpy/constants.py
+-rw-rw-rw-   0        0        0     5450 2023-12-06 09:37:10.000000 edm_arch-1.0.43/src/edmpy/db.py
+-rw-rw-rw-   0        0        0    13431 2023-12-05 09:27:43.000000 edm_arch-1.0.43/src/edmpy/edm.kv
+-rw-rw-rw-   0        0        0   126353 2024-05-30 13:46:38.000000 edm_arch-1.0.43/src/edmpy/edm.py
+-rw-rw-rw-   0        0        0     5653 2024-04-18 08:18:35.000000 edm_arch-1.0.43/src/edmpy/geo.py
+-rw-rw-rw-   0        0        0     2495 2023-12-06 09:36:13.000000 edm_arch-1.0.43/src/edmpy/ini.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:17.615246 edm_arch-1.0.43/src/edmpy/lib/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm_arch-1.0.43/src/edmpy/lib/__init__.py
+-rw-rw-rw-   0        0        0     4204 2023-12-04 14:38:01.000000 edm_arch-1.0.43/src/edmpy/lib/blockdata.py
+-rw-rw-rw-   0        0        0     4333 2023-12-06 09:31:45.000000 edm_arch-1.0.43/src/edmpy/lib/colorscheme.py
+-rw-rw-rw-   0        0        0     3994 2023-12-04 14:40:09.000000 edm_arch-1.0.43/src/edmpy/lib/dbs.py
+-rw-rw-rw-   0        0        0   195835 2024-05-22 13:06:32.000000 edm_arch-1.0.43/src/edmpy/lib/e5_widgets.py
+-rw-rw-rw-   0        0        0     1812 2023-12-04 14:41:01.000000 edm_arch-1.0.43/src/edmpy/lib/misc.py
+-rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm_arch-1.0.43/src/edmpy/py.typed
+-rw-rw-rw-   0        0        0      531 2024-04-16 00:42:15.000000 edm_arch-1.0.43/src/edmpy/test_edm.py
+-rw-rw-rw-   0        0        0    46794 2024-05-30 13:39:54.000000 edm_arch-1.0.43/src/edmpy/totalstation.py
```

### Comparing `edm_arch-1.0.42/LICENSE` & `edm_arch-1.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/PKG-INFO` & `edm_arch-1.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edm-arch
-Version: 1.0.42
+Version: 1.0.43
 Summary: Total stations for archaeologists
 Home-page: https://github.com/surf3s/EDM
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/EDM/issues
 Platform: unix
@@ -139,14 +139,17 @@
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
 ##### Virus Warning
 
 Recently (May, 2024) I was helping someone put the program on a Windows 10 tablet.  However, the virus protection software (Microsoft) said the Windows exe version was a virus and immediately removed it.  It took a lot of time to find a work around.  Eventually we made exe programs a virus exception.  This is not a great solution.  I can assure you that edm.exe does not contain a virus.  I also personally downloaded the same version and scanned it with my virus detection software.  Nothing.  I will try to find a computer where I can replicate this and see what part of my program is giving this problem.  If you experience this as well, let me know.
 
+##### Changes for Version 1.0.43 (May 20, 2024)
+1.  Fixed bug that broke communication with older Leica instruments
+
 ##### Changes for Version 1.0.42 (May, 2024)
 1.  Fixed bug where default values on speed buttons did not trigger linked fields
 2.  Fixed bug where changing value of a field in edit screen did not trigger linked fields
 
 ##### Changes for Version 1.0.41 (May, 2024)
 1.  Fixed crash when spamming Add button in menu in datagrid
```

### Comparing `edm_arch-1.0.42/README.md` & `edm_arch-1.0.43/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,17 @@
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
 ##### Virus Warning
 
 Recently (May, 2024) I was helping someone put the program on a Windows 10 tablet.  However, the virus protection software (Microsoft) said the Windows exe version was a virus and immediately removed it.  It took a lot of time to find a work around.  Eventually we made exe programs a virus exception.  This is not a great solution.  I can assure you that edm.exe does not contain a virus.  I also personally downloaded the same version and scanned it with my virus detection software.  Nothing.  I will try to find a computer where I can replicate this and see what part of my program is giving this problem.  If you experience this as well, let me know.
 
+##### Changes for Version 1.0.43 (May 20, 2024)
+1.  Fixed bug that broke communication with older Leica instruments
+
 ##### Changes for Version 1.0.42 (May, 2024)
 1.  Fixed bug where default values on speed buttons did not trigger linked fields
 2.  Fixed bug where changing value of a field in edit screen did not trigger linked fields
 
 ##### Changes for Version 1.0.41 (May, 2024)
 1.  Fixed crash when spamming Add button in menu in datagrid
```

### Comparing `edm_arch-1.0.42/pyproject.toml` & `edm_arch-1.0.43/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/setup.cfg` & `edm_arch-1.0.43/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 646d 2d61 7263 680d 0a64 6573   = edm-arch..des
 00000020: 6372 6970 7469 6f6e 203d 2054 6f74 616c  cription = Total
 00000030: 2073 7461 7469 6f6e 7320 666f 7220 6172   stations for ar
 00000040: 6368 6165 6f6c 6f67 6973 7473 0d0a 7665  chaeologists..ve
-00000050: 7273 696f 6e20 3d20 312e 302e 3432 0d0a  rsion = 1.0.42..
+00000050: 7273 696f 6e20 3d20 312e 302e 3433 0d0a  rsion = 1.0.43..
 00000060: 6175 7468 6f72 203d 2053 6861 6e6e 6f6e  author = Shannon
 00000070: 2050 2e20 4d63 5068 6572 726f 6e0d 0a61   P. McPherron..a
 00000080: 7574 686f 725f 656d 6169 6c20 3d20 6d63  uthor_email = mc
 00000090: 7068 6572 726f 6e40 6576 612e 6d70 672e  pherron@eva.mpg.
 000000a0: 6465 0d0a 6c6f 6e67 5f64 6573 6372 6970  de..long_descrip
 000000b0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 000000c0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
```

### Comparing `edm_arch-1.0.42/src/edm_arch.egg-info/PKG-INFO` & `edm_arch-1.0.43/src/edm_arch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edm-arch
-Version: 1.0.42
+Version: 1.0.43
 Summary: Total stations for archaeologists
 Home-page: https://github.com/surf3s/EDM
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/EDM/issues
 Platform: unix
@@ -139,14 +139,17 @@
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
 ##### Virus Warning
 
 Recently (May, 2024) I was helping someone put the program on a Windows 10 tablet.  However, the virus protection software (Microsoft) said the Windows exe version was a virus and immediately removed it.  It took a lot of time to find a work around.  Eventually we made exe programs a virus exception.  This is not a great solution.  I can assure you that edm.exe does not contain a virus.  I also personally downloaded the same version and scanned it with my virus detection software.  Nothing.  I will try to find a computer where I can replicate this and see what part of my program is giving this problem.  If you experience this as well, let me know.
 
+##### Changes for Version 1.0.43 (May 20, 2024)
+1.  Fixed bug that broke communication with older Leica instruments
+
 ##### Changes for Version 1.0.42 (May, 2024)
 1.  Fixed bug where default values on speed buttons did not trigger linked fields
 2.  Fixed bug where changing value of a field in edit screen did not trigger linked fields
 
 ##### Changes for Version 1.0.41 (May, 2024)
 1.  Fixed crash when spamming Add button in menu in datagrid
```

### Comparing `edm_arch-1.0.42/src/edm_arch.egg-info/SOURCES.txt` & `edm_arch-1.0.43/src/edm_arch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/cfg.py` & `edm_arch-1.0.43/src/edmpy/cfg.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/constants.py` & `edm_arch-1.0.43/src/edmpy/constants.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/db.py` & `edm_arch-1.0.43/src/edmpy/db.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/edm.kv` & `edm_arch-1.0.43/src/edmpy/edm.kv`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/edm.py` & `edm_arch-1.0.43/src/edmpy/edm.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,17 @@
 Changes for Version 1.0.41
   fixed crash when Add button is pressed multiple times
 
 Changes for Version 1.0.42
   Fixed bug where default values on speed buttons did not trigger linked fields
   Fixed bug where changing value of a field in edit screen did not trigger linked fields
 
+Changes for Version 1.0.43
+  Fixed bug that broke communication with older Leica instruments
+
 Bugs/To Do
   have to click twice on unit to get it to switch units
   add units to menu as you go along
   need to move load_dialog out of kv and into code and error trap bad paths
   could make menus work better with keyboard (at least with tab)
   Do unitchecking after doing an offset shot on suffix 0 points
   Good way to get random hash IDs
@@ -187,15 +190,15 @@
 """
 try:
     import win32timezone
     win32timezone.TimeZoneInfo.local()
 except ModuleNotFoundError:
     pass
 
-VERSION = '1.0.42'
+VERSION = '1.0.43'
 PRODUCTION_DATE = 'May, 2024'
 __DEFAULT_FIELDS__ = ['X', 'Y', 'Z', 'SLOPED', 'VANGLE', 'HANGLE', 'STATIONX', 'STATIONY', 'STATIONZ', 'DATUMX', 'DATUMY', 'DATUMZ', 'LOCALX', 'LOCALY', 'LOCALZ', 'DATE', 'PRISM', 'ID']
 __BUTTONS__ = 13
 __LASTCOMPORT__ = 16
 MAX_SCREEN_WIDTH = 400
 __program__ = 'EDM'
```

### Comparing `edm_arch-1.0.42/src/edmpy/geo.py` & `edm_arch-1.0.43/src/edmpy/geo.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/ini.py` & `edm_arch-1.0.43/src/edmpy/ini.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/lib/blockdata.py` & `edm_arch-1.0.43/src/edmpy/lib/blockdata.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/lib/colorscheme.py` & `edm_arch-1.0.43/src/edmpy/lib/colorscheme.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/lib/dbs.py` & `edm_arch-1.0.43/src/edmpy/lib/dbs.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/lib/e5_widgets.py` & `edm_arch-1.0.43/src/edmpy/lib/e5_widgets.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/lib/misc.py` & `edm_arch-1.0.43/src/edmpy/lib/misc.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/test_edm.py` & `edm_arch-1.0.43/src/edmpy/test_edm.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.42/src/edmpy/totalstation.py` & `edm_arch-1.0.43/src/edmpy/totalstation.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,14 +491,15 @@
     def receive(self):
         data = ''
         if self.serialcom.is_open:
             data = self.serialcom.read_until().decode() if self.serialcom.is_open else ''
             if data:
                 self.add_to_io('Received <- ' + data)
         self.received = data
+        return data
 
     def close(self):
         if self.serialcom.is_open:
             self.serialcom.close()
             self.clear_io()
         if self.serial_bt_input.is_open:
             self.serial_bt_input.close()
@@ -991,18 +992,22 @@
         return self.receive()
 
     def launch_point_leica(self):
         self.send(b"GET/M/WI21/WI22/WI31/WI51\r\n")
 
     def fetch_point_leica(self):
         self.pnt = self.receive()
+        self.set_response_leica()
         if self.pnt:
             self.parce_leica()
             self.vhd_to_xyz()
 
+    def set_response_leica(self):
+        self.response = self.leica_trim_crlf(self.received) if self.received else ""
+
     def parce_leica(self):
         if self.pnt:
             if self.pnt.startswith('*'):
                 self.pnt = self.pnt[1:]
             for component in self.pnt.split(' '):
                 if component.startswith('21.'):
                     data = component[6:]
```

