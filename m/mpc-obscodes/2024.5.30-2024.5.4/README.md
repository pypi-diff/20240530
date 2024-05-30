# Comparing `tmp/mpc_obscodes-2024.5.30.tar.gz` & `tmp/mpc_obscodes-2024.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2024.5.30.tar", last modified: Thu May 30 02:25:06 2024, max compression
+gzip compressed data, was "mpc_obscodes-2024.5.4.tar", last modified: Sat May  4 02:22:39 2024, max compression
```

## Comparing `mpc_obscodes-2024.5.30.tar` & `mpc_obscodes-2024.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:25:06.230387 mpc_obscodes-2024.5.30/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-30 02:24:56.000000 mpc_obscodes-2024.5.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-30 02:25:06.226387 mpc_obscodes-2024.5.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-30 02:24:56.000000 mpc_obscodes-2024.5.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:25:06.226387 mpc_obscodes-2024.5.30/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 02:24:56.000000 mpc_obscodes-2024.5.30/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-30 02:24:56.000000 mpc_obscodes-2024.5.30/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-30 02:24:56.000000 mpc_obscodes-2024.5.30/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)   254689 2024-05-30 02:24:58.000000 mpc_obscodes-2024.5.30/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 02:24:58.000000 mpc_obscodes-2024.5.30/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:25:06.226387 mpc_obscodes-2024.5.30/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:56.000000 mpc_obscodes-2024.5.30/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 02:24:56.000000 mpc_obscodes-2024.5.30/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-30 02:24:56.000000 mpc_obscodes-2024.5.30/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-30 02:24:56.000000 mpc_obscodes-2024.5.30/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:25:06.226387 mpc_obscodes-2024.5.30/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-30 02:25:06.000000 mpc_obscodes-2024.5.30/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-30 02:25:06.000000 mpc_obscodes-2024.5.30/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 02:25:06.000000 mpc_obscodes-2024.5.30/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 02:25:06.000000 mpc_obscodes-2024.5.30/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 02:25:06.000000 mpc_obscodes-2024.5.30/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-30 02:24:58.000000 mpc_obscodes-2024.5.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 02:25:06.230387 mpc_obscodes-2024.5.30/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:22:39.569850 mpc_obscodes-2024.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-04 02:22:39.569850 mpc_obscodes-2024.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:22:39.565850 mpc_obscodes-2024.5.4/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)   254259 2024-05-04 02:22:33.000000 mpc_obscodes-2024.5.4/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-04 02:22:33.000000 mpc_obscodes-2024.5.4/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:22:39.569850 mpc_obscodes-2024.5.4/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:22:39.569850 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-04 02:22:39.000000 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-04 02:22:39.000000 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 02:22:39.000000 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 02:22:39.000000 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 02:22:39.000000 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-04 02:22:33.000000 mpc_obscodes-2024.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 02:22:39.569850 mpc_obscodes-2024.5.4/setup.cfg
```

### Comparing `mpc_obscodes-2024.5.30/PKG-INFO` & `mpc_obscodes-2024.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2024.5.30
+Version: 2024.5.4
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `mpc_obscodes-2024.5.30/README.md` & `mpc_obscodes-2024.5.4/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.30/mpc_obscodes/compare.py` & `mpc_obscodes-2024.5.4/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.30/mpc_obscodes/fetch.py` & `mpc_obscodes-2024.5.4/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.30/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2024.5.4/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982625099285147%*

 * *Differences: {"'267'": "{'Longitude': 204.5311, 'cos': 0.941718, 'sin': 0.337237}",*

 * * "'T14'": "{'Longitude': 204.5311, 'cos': 0.941718, 'sin': 0.337237}",*

 * * 'delete': "['D48', 'P68', 'R78', 'Y75']"}*

```diff
@@ -1565,18 +1565,18 @@
     "266": {
         "Longitude": 204.52396,
         "Name": "New Horizons KBO Search-Subaru",
         "cos": 0.941711,
         "sin": 0.337239
     },
     "267": {
-        "Longitude": 204.53109,
+        "Longitude": 204.5311,
         "Name": "New Horizons KBO Search-CFHT",
-        "cos": 0.941717,
-        "sin": 0.33724
+        "cos": 0.941718,
+        "sin": 0.337237
     },
     "268": {
         "Longitude": 289.30803,
         "Name": "New Horizons KBO Search-Magellan/Clay",
         "cos": 0.875516,
         "sin": -0.482342
     },
@@ -7873,20 +7873,14 @@
     },
     "D47": {
         "Longitude": 11.56366,
         "Name": "BigBang Observatory, Manciano",
         "cos": 0.738665,
         "sin": 0.671859
     },
-    "D48": {
-        "Longitude": 7.26381,
-        "Name": "Niederbexbach Observatory",
-        "cos": 0.652979,
-        "sin": 0.754898
-    },
     "D53": {
         "Longitude": 127.482,
         "Name": "ISON-Blagoveschensk Observatory",
         "cos": 0.63981,
         "sin": 0.766
     },
     "D54": {
@@ -12679,20 +12673,14 @@
     },
     "P67": {
         "Longitude": 127.7415,
         "Name": "Kangwon National University Observatory",
         "cos": 0.7904,
         "sin": 0.61057
     },
-    "P68": {
-        "Longitude": 127.4744,
-        "Name": "DDSHS Biryong Observatory",
-        "cos": 0.806556,
-        "sin": 0.589222
-    },
     "P71": {
         "Longitude": 128.76108,
         "Name": "Miryang Arirang Astronomical Observatory",
         "cos": 0.815026,
         "sin": 0.57752
     },
     "P72": {
@@ -12943,20 +12931,14 @@
     },
     "R66": {
         "Longitude": 172.58761,
         "Name": "Mooray Observatory, Christchurch",
         "cos": 0.726587,
         "sin": -0.684777
     },
-    "R78": {
-        "Longitude": 175.09104,
-        "Name": "Crystal Lake Observatory, Ngutunui",
-        "cos": 0.788021,
-        "sin": -0.613626
-    },
     "T03": {
         "Longitude": 203.74247,
         "Name": "Haleakala-LCO Clamshell #3",
         "cos": 0.93624,
         "sin": 0.351538
     },
     "T04": {
@@ -13010,18 +12992,18 @@
     "T13": {
         "Longitude": 204.52797,
         "Name": "NASA Infrared Telescope Facility, Maunakea",
         "cos": 0.941707,
         "sin": 0.337251
     },
     "T14": {
-        "Longitude": 204.53109,
+        "Longitude": 204.5311,
         "Name": "Canada-France-Hawaii Telescope, Maunakea",
-        "cos": 0.941717,
-        "sin": 0.33724
+        "cos": 0.941718,
+        "sin": 0.337237
     },
     "T15": {
         "Longitude": 204.53093,
         "Name": "Gemini North Observatory, Maunakea",
         "cos": 0.941728,
         "sin": 0.337214
     },
@@ -14329,20 +14311,14 @@
     },
     "Y66": {
         "Longitude": 343.49053,
         "Name": "Two-Meter Twin Telescope, TTT2, Teide",
         "cos": 0.881484,
         "sin": 0.471429
     },
-    "Y75": {
-        "Longitude": 354.58128,
-        "Name": "Abraham Zacut, Salamanca",
-        "cos": 0.786275,
-        "sin": 0.615972
-    },
     "Y82": {
         "Longitude": 358.06548,
         "Name": "LPMR Observatory, Broad Chalke",
         "cos": 0.630258,
         "sin": 0.77381
     },
     "Y83": {
```

### Comparing `mpc_obscodes-2024.5.30/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.30/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.30/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.30/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2024.5.30
+Version: 2024.5.4
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `mpc_obscodes-2024.5.30/pyproject.toml` & `mpc_obscodes-2024.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2024.05.30"
+version = "2024.05.04"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

