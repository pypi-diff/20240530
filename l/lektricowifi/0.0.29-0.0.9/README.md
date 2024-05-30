# Comparing `tmp/lektricowifi-0.0.29.tar.gz` & `tmp/lektricowifi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektricowifi-0.0.29.tar", last modified: Thu May 30 14:21:40 2024, max compression
+gzip compressed data, was "D:\proiecte\liClipse workspace\lektricowifi\dist\tmpvnc96b0h\lektricowifi-0.0.9.tar", last modified: Mon Nov 22 09:21:05 2021, max compression
```

## Comparing `lektricowifi-0.0.29.tar` & `lektricowifi-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:21:40.873765 lektricowifi-0.0.29/
--rw-rw-rw-   0        0        0     1091 2021-10-29 11:44:25.000000 lektricowifi-0.0.29/LICENSE
--rw-rw-rw-   0        0        0      656 2024-05-30 14:21:40.872745 lektricowifi-0.0.29/PKG-INFO
--rw-rw-rw-   0        0        0       80 2021-10-29 11:34:08.000000 lektricowifi-0.0.29/README.md
--rw-rw-rw-   0        0        0      108 2024-05-30 12:27:40.000000 lektricowifi-0.0.29/pyproject.toml
--rw-rw-rw-   0        0        0      755 2024-05-30 14:21:40.885757 lektricowifi-0.0.29/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-30 14:21:40.811564 lektricowifi-0.0.29/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:21:40.843147 lektricowifi-0.0.29/src/lektricowifi/
--rw-rw-rw-   0        0        0      365 2023-03-01 12:52:53.000000 lektricowifi-0.0.29/src/lektricowifi/__init__.py
--rw-rw-rw-   0        0        0      214 2023-02-20 14:44:44.000000 lektricowifi-0.0.29/src/lektricowifi/exceptions.py
--rw-rw-rw-   0        0        0    13507 2024-05-24 12:02:56.000000 lektricowifi-0.0.29/src/lektricowifi/lektricowifi.py
--rw-rw-rw-   0        0        0     5205 2024-05-13 19:33:11.000000 lektricowifi-0.0.29/src/lektricowifi/models.py
--rw-rw-rw-   0        0        0        0 2024-05-30 11:05:06.000000 lektricowifi-0.0.29/src/lektricowifi/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-30 14:21:40.869373 lektricowifi-0.0.29/src/lektricowifi.egg-info/
--rw-rw-rw-   0        0        0      656 2024-05-30 14:21:40.000000 lektricowifi-0.0.29/src/lektricowifi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-05-30 14:21:40.000000 lektricowifi-0.0.29/src/lektricowifi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:21:40.000000 lektricowifi-0.0.29/src/lektricowifi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-30 14:21:40.000000 lektricowifi-0.0.29/src/lektricowifi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 14:21:40.000000 lektricowifi-0.0.29/src/lektricowifi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-11-22 09:21:05.379634 lektricowifi-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2021-10-29 11:44:25.000000 lektricowifi-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      598 2021-11-22 09:21:05.379634 lektricowifi-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2021-10-29 11:34:08.000000 lektricowifi-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-10-29 11:04:25.000000 lektricowifi-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      616 2021-11-22 09:21:05.379634 lektricowifi-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2021-11-22 09:21:05.321827 lektricowifi-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2021-11-22 09:21:05.363998 lektricowifi-0.0.9/src/lektricowifi/
+-rw-rw-rw-   0        0        0      279 2021-11-04 07:18:12.000000 lektricowifi-0.0.9/src/lektricowifi/__init__.py
+-rw-rw-rw-   0        0        0      220 2021-11-04 10:41:51.000000 lektricowifi-0.0.9/src/lektricowifi/exceptions.py
+-rw-rw-rw-   0        0        0     4975 2021-11-22 08:45:07.000000 lektricowifi-0.0.9/src/lektricowifi/lektricowifi.py
+-rw-rw-rw-   0        0        0     2613 2021-11-22 08:43:22.000000 lektricowifi-0.0.9/src/lektricowifi/models.py
+drwxrwxrwx   0        0        0        0 2021-11-22 09:21:05.379634 lektricowifi-0.0.9/src/lektricowifi.egg-info/
+-rw-rw-rw-   0        0        0      598 2021-11-22 09:21:05.000000 lektricowifi-0.0.9/src/lektricowifi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2021-11-22 09:21:05.000000 lektricowifi-0.0.9/src/lektricowifi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-11-22 09:21:05.000000 lektricowifi-0.0.9/src/lektricowifi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2021-11-22 09:21:05.000000 lektricowifi-0.0.9/src/lektricowifi.egg-info/top_level.txt
```

### Comparing `lektricowifi-0.0.29/LICENSE` & `lektricowifi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lektricowifi-0.0.29/PKG-INFO` & `lektricowifi-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lektricowifi
-Version: 0.0.29
+Version: 0.0.9
 Summary: Communication with Lektrico's chargers
 Home-page: https://lektri.co
 Author: Lektrico
 Author-email: mihaela@civitronic.ro
+License: UNKNOWN
 Project-URL: Bug Tracker, https://lektri.co
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp>=3.9.5
-Requires-Dist: async_timeout>=4.0.3
-Requires-Dist: yarl>=1.9.4
 
 # LektricoWifi 
 
 This is a package for communicating with Lektrico's chargers.
+
```

### Comparing `lektricowifi-0.0.29/setup.cfg` & `lektricowifi-0.0.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,39 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 656b 7472 6963 6f77 6966 690d   = lektricowifi.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
-00000030: 390d 0a61 7574 686f 7220 3d20 4c65 6b74  9..author = Lekt
-00000040: 7269 636f 0d0a 6175 7468 6f72 5f65 6d61  rico..author_ema
-00000050: 696c 203d 206d 6968 6165 6c61 4063 6976  il = mihaela@civ
-00000060: 6974 726f 6e69 632e 726f 0d0a 6465 7363  itronic.ro..desc
-00000070: 7269 7074 696f 6e20 3d20 436f 6d6d 756e  ription = Commun
-00000080: 6963 6174 696f 6e20 7769 7468 204c 656b  ication with Lek
-00000090: 7472 6963 6f27 7320 6368 6172 6765 7273  trico's chargers
-000000a0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000b0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-000000c0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
-000000d0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-000000e0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-000000f0: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
-00000100: 3a2f 2f6c 656b 7472 692e 636f 0d0a 7072  ://lektri.co..pr
-00000110: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-00000120: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
-00000130: 7470 733a 2f2f 6c65 6b74 7269 2e63 6f0d  tps://lektri.co.
-00000140: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-00000150: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000160: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000170: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
-00000180: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000190: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-000001a0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-000001b0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000001c0: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
-000001d0: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-000001e0: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
-000001f0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-00000200: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000210: 332e 360d 0a69 6e73 7461 6c6c 5f72 6571  3.6..install_req
-00000220: 7569 7265 7320 3d20 0d0a 0961 696f 6874  uires = ...aioht
-00000230: 7470 203e 3d20 332e 392e 350d 0a09 6173  tp >= 3.9.5...as
-00000240: 796e 635f 7469 6d65 6f75 7420 3e3d 2034  ync_timeout >= 4
-00000250: 2e30 2e33 0d0a 0979 6172 6c20 3e3d 2031  .0.3...yarl >= 1
-00000260: 2e39 2e34 0d0a 0d0a 5b6f 7074 696f 6e73  .9.4....[options
-00000270: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-00000280: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-00000290: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-000002a0: 5f64 6174 615d 0d0a 226c 656b 7472 6963  _data].."lektric
-000002b0: 6f77 6966 6922 203d 205b 2270 792e 7479  owifi" = ["py.ty
-000002c0: 7065 6422 5d0d 0a0d 0a5b 6567 675f 696e  ped"]....[egg_in
-000002d0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000002e0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000002f0: 0a0d 0a                                  ...
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e39  .version = 0.0.9
+00000030: 0d0a 6175 7468 6f72 203d 204c 656b 7472  ..author = Lektr
+00000040: 6963 6f0d 0a61 7574 686f 725f 656d 6169  ico..author_emai
+00000050: 6c20 3d20 6d69 6861 656c 6140 6369 7669  l = mihaela@civi
+00000060: 7472 6f6e 6963 2e72 6f0d 0a64 6573 6372  tronic.ro..descr
+00000070: 6970 7469 6f6e 203d 2043 6f6d 6d75 6e69  iption = Communi
+00000080: 6361 7469 6f6e 2077 6974 6820 4c65 6b74  cation with Lekt
+00000090: 7269 636f 2773 2063 6861 7267 6572 730d  rico's chargers.
+000000a0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000b0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000c0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+000000d0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+000000e0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+000000f0: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
+00000100: 2f2f 6c65 6b74 7269 2e63 6f0d 0a70 726f  //lektri.co..pro
+00000110: 6a65 6374 5f75 726c 7320 3d20 0d0a 0942  ject_urls = ...B
+00000120: 7567 2054 7261 636b 6572 203d 2068 7474  ug Tracker = htt
+00000130: 7073 3a2f 2f6c 656b 7472 692e 636f 0d0a  ps://lektri.co..
+00000140: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+00000150: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000160: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000170: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
+00000180: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000190: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
+000001a0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000001b0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000001c0: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
+000001d0: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+000001e0: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
+000001f0: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
+00000200: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000210: 2e36 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .6....[options.p
+00000220: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+00000230: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
+00000240: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000250: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000260: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `lektricowifi-0.0.29/src/lektricowifi.egg-info/PKG-INFO` & `lektricowifi-0.0.9/src/lektricowifi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lektricowifi
-Version: 0.0.29
+Version: 0.0.9
 Summary: Communication with Lektrico's chargers
 Home-page: https://lektri.co
 Author: Lektrico
 Author-email: mihaela@civitronic.ro
+License: UNKNOWN
 Project-URL: Bug Tracker, https://lektri.co
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp>=3.9.5
-Requires-Dist: async_timeout>=4.0.3
-Requires-Dist: yarl>=1.9.4
 
 # LektricoWifi 
 
 This is a package for communicating with Lektrico's chargers.
+
```

