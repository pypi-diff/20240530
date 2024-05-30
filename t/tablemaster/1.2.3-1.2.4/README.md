# Comparing `tmp/tablemaster-1.2.3.tar.gz` & `tmp/tablemaster-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemaster-1.2.3.tar", last modified: Mon May 27 03:21:55 2024, max compression
+gzip compressed data, was "tablemaster-1.2.4.tar", last modified: Thu May 30 05:26:33 2024, max compression
```

## Comparing `tablemaster-1.2.3.tar` & `tablemaster-1.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 03:21:55.772473 tablemaster-1.2.3/
--rw-rw-rw-   0        0        0    11357 2024-05-20 11:04:14.000000 tablemaster-1.2.3/LICENSE
--rw-rw-rw-   0        0        0      468 2024-05-27 03:21:55.771462 tablemaster-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2560 2024-05-20 11:04:14.000000 tablemaster-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-27 03:21:55.772473 tablemaster-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      517 2024-05-27 03:20:45.000000 tablemaster-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 03:21:55.762939 tablemaster-1.2.3/tablemaster/
--rw-rw-rw-   0        0        0      632 2024-05-20 11:04:14.000000 tablemaster-1.2.3/tablemaster/__init__.py
--rw-rw-rw-   0        0        0     1716 2024-05-20 11:04:14.000000 tablemaster-1.2.3/tablemaster/feishu.py
--rw-rw-rw-   0        0        0     1265 2024-05-27 03:19:37.000000 tablemaster-1.2.3/tablemaster/gspread.py
--rw-rw-rw-   0        0        0     3334 2024-05-20 11:04:14.000000 tablemaster-1.2.3/tablemaster/local.py
--rw-rw-rw-   0        0        0     5829 2024-05-20 11:45:13.000000 tablemaster-1.2.3/tablemaster/mysql.py
--rw-rw-rw-   0        0        0      810 2024-05-20 11:04:14.000000 tablemaster-1.2.3/tablemaster/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 03:21:55.770431 tablemaster-1.2.3/tablemaster.egg-info/
--rw-rw-rw-   0        0        0      468 2024-05-27 03:21:55.000000 tablemaster-1.2.3/tablemaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-27 03:21:55.000000 tablemaster-1.2.3/tablemaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 03:21:55.000000 tablemaster-1.2.3/tablemaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-05-27 03:21:55.000000 tablemaster-1.2.3/tablemaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-27 03:21:55.000000 tablemaster-1.2.3/tablemaster.egg-info/top_level.txt
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-30 05:26:33.837568 tablemaster-1.2.4/
+-rw-r--r--   0 livid      (501) staff       (20)    11357 2024-05-20 11:04:14.000000 tablemaster-1.2.4/LICENSE
+-rw-r--r--   0 livid      (501) staff       (20)      451 2024-05-30 05:26:33.832441 tablemaster-1.2.4/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)     2560 2024-05-20 11:04:14.000000 tablemaster-1.2.4/README.md
+-rw-r--r--   0 livid      (501) staff       (20)       38 2024-05-30 05:26:33.837646 tablemaster-1.2.4/setup.cfg
+-rw-r--r--   0 livid      (501) staff       (20)      517 2024-05-30 05:23:55.000000 tablemaster-1.2.4/setup.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-30 05:26:33.831525 tablemaster-1.2.4/tablemaster/
+-rw-r--r--   0 livid      (501) staff       (20)      685 2024-05-30 05:22:49.000000 tablemaster-1.2.4/tablemaster/__init__.py
+-rw-r--r--   0 livid      (501) staff       (20)     1716 2024-05-20 11:04:14.000000 tablemaster-1.2.4/tablemaster/feishu.py
+-rw-r--r--   0 livid      (501) staff       (20)     1266 2024-05-30 05:21:07.000000 tablemaster-1.2.4/tablemaster/gspread.py
+-rw-r--r--   0 livid      (501) staff       (20)     3334 2024-05-20 11:04:14.000000 tablemaster-1.2.4/tablemaster/local.py
+-rw-r--r--   0 livid      (501) staff       (20)     5829 2024-05-20 11:45:13.000000 tablemaster-1.2.4/tablemaster/mysql.py
+-rw-r--r--   0 livid      (501) staff       (20)      810 2024-05-20 11:04:14.000000 tablemaster-1.2.4/tablemaster/utils.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-30 05:26:33.832194 tablemaster-1.2.4/tablemaster.egg-info/
+-rw-r--r--   0 livid      (501) staff       (20)      451 2024-05-30 05:26:33.000000 tablemaster-1.2.4/tablemaster.egg-info/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)      332 2024-05-30 05:26:33.000000 tablemaster-1.2.4/tablemaster.egg-info/SOURCES.txt
+-rw-r--r--   0 livid      (501) staff       (20)        1 2024-05-30 05:26:33.000000 tablemaster-1.2.4/tablemaster.egg-info/dependency_links.txt
+-rw-r--r--   0 livid      (501) staff       (20)       77 2024-05-30 05:26:33.000000 tablemaster-1.2.4/tablemaster.egg-info/requires.txt
+-rw-r--r--   0 livid      (501) staff       (20)       12 2024-05-30 05:26:33.000000 tablemaster-1.2.4/tablemaster.egg-info/top_level.txt
```

### Comparing `tablemaster-1.2.3/LICENSE` & `tablemaster-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.3/README.md` & `tablemaster-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.3/setup.py` & `tablemaster-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tablemaster',
-    version='1.2.3',
+    version='1.2.4',
     packages=find_packages(),
     install_requires=[
         'PyMySQL',
         'SQLAlchemy',
         'pandas',
         'python-dateutil',
         'gspread',
```

### Comparing `tablemaster-1.2.3/tablemaster/__init__.py` & `tablemaster-1.2.4/tablemaster/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,20 @@
     from yaml import CLoader as Loader, CDumper as Dumper
 except ImportError:
     from yaml import Loader, Dumper
 import json
 from types import SimpleNamespace
 import pandas as pd
 
-
-with open('cfg.yaml') as cfg:
-    cfg = json.loads(json.dumps(load(cfg, Loader=Loader)), object_hook=lambda d: SimpleNamespace(**d))
+try:
+    with open('cfg.yaml') as cfg:
+        cfg = json.loads(json.dumps(load(cfg, Loader=Loader)), object_hook=lambda d: SimpleNamespace(**d))
+except Exception as e:
+    print(e)
+    
 
 from . import utils
 
 from .mysql import (
     query,
     opt,
     ManageTable,
```

### Comparing `tablemaster-1.2.3/tablemaster/feishu.py` & `tablemaster-1.2.4/tablemaster/feishu.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.3/tablemaster/gspread.py` & `tablemaster-1.2.4/tablemaster/gspread.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
         else:
             print(e)
     wks.clear()
     non_float_int_columns = df.select_dtypes(exclude=['float64', 'int64']).columns
     for col in non_float_int_columns:
         df[col] = df[col].astype(str)
     wks.update(loc,([df.columns.values.tolist()] + df.values.tolist()))
-    print('data is written!')
+    print('data is written!')
```

### Comparing `tablemaster-1.2.3/tablemaster/local.py` & `tablemaster-1.2.4/tablemaster/local.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.3/tablemaster/mysql.py` & `tablemaster-1.2.4/tablemaster/mysql.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.3/tablemaster/utils.py` & `tablemaster-1.2.4/tablemaster/utils.py`

 * *Files identical despite different names*

