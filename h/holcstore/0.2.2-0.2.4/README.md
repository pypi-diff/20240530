# Comparing `tmp/holcstore-0.2.2.tar.gz` & `tmp/holcstore-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holcstore-0.2.2.tar", last modified: Tue May 28 17:14:55 2024, max compression
+gzip compressed data, was "holcstore-0.2.4.tar", last modified: Wed May 29 13:48:05 2024, max compression
```

## Comparing `holcstore-0.2.2.tar` & `holcstore-0.2.4.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.654345 holcstore-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-28 17:14:51.000000 holcstore-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 17:14:51.000000 holcstore-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-28 17:14:55.654345 holcstore-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-28 17:14:51.000000 holcstore-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.650345 holcstore-0.2.2/holcstore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:51.000000 holcstore-0.2.2/holcstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-28 17:14:51.000000 holcstore-0.2.2/holcstore/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-28 17:14:51.000000 holcstore-0.2.2/holcstore/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-28 17:14:51.000000 holcstore-0.2.2/holcstore/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-28 17:14:51.000000 holcstore-0.2.2/holcstore/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.654345 holcstore-0.2.2/holcstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-28 17:14:55.000000 holcstore-0.2.2/holcstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-28 17:14:55.000000 holcstore-0.2.2/holcstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:14:55.000000 holcstore-0.2.2/holcstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 17:14:55.000000 holcstore-0.2.2/holcstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 17:14:55.000000 holcstore-0.2.2/holcstore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.654345 holcstore-0.2.2/hostore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.654345 holcstore-0.2.2/hostore/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/0004_testdatastore_created_at.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/0005_alter_testdatastore_prm.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12247 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12663 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.654345 holcstore-0.2.2/hostore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/utils/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 17:14:51.000000 holcstore-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-28 17:14:55.654345 holcstore-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 17:14:51.000000 holcstore-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:48:05.153484 holcstore-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-29 13:47:55.000000 holcstore-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 13:47:55.000000 holcstore-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-29 13:48:05.153484 holcstore-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-29 13:47:55.000000 holcstore-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:48:05.149484 holcstore-0.2.4/holcstore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:55.000000 holcstore-0.2.4/holcstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-29 13:47:55.000000 holcstore-0.2.4/holcstore/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-29 13:47:55.000000 holcstore-0.2.4/holcstore/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-29 13:47:55.000000 holcstore-0.2.4/holcstore/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-29 13:47:55.000000 holcstore-0.2.4/holcstore/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:48:05.153484 holcstore-0.2.4/holcstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-29 13:48:05.000000 holcstore-0.2.4/holcstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-29 13:48:05.000000 holcstore-0.2.4/holcstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:48:05.000000 holcstore-0.2.4/holcstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 13:48:05.000000 holcstore-0.2.4/holcstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 13:48:05.000000 holcstore-0.2.4/holcstore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:48:05.149484 holcstore-0.2.4/hostore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:48:05.149484 holcstore-0.2.4/hostore/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/migrations/0004_testdatastore_created_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/migrations/0005_alter_testdatastore_prm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/migrations/0006_testdatastorewithattribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14127 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:48:05.149484 holcstore-0.2.4/hostore/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/tests/tests_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/tests/tests_slice_with_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/tests/tests_with_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:48:05.153484 holcstore-0.2.4/hostore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/utils/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 13:47:55.000000 holcstore-0.2.4/hostore/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-29 13:47:55.000000 holcstore-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-29 13:48:05.153484 holcstore-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 13:47:55.000000 holcstore-0.2.4/setup.py
```

### Comparing `holcstore-0.2.2/LICENSE` & `holcstore-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.2/PKG-INFO` & `holcstore-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.2.2
+Version: 0.2.4
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.2.2/README.rst` & `holcstore-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.2/holcstore/settings.py` & `holcstore-0.2.4/holcstore/settings.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.2/holcstore/urls.py` & `holcstore-0.2.4/holcstore/urls.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.2/holcstore.egg-info/PKG-INFO` & `holcstore-0.2.4/holcstore.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.2.2
+Version: 0.2.4
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.2.2/holcstore.egg-info/SOURCES.txt` & `holcstore-0.2.4/holcstore.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,18 +15,22 @@
 holcstore.egg-info/requires.txt
 holcstore.egg-info/top_level.txt
 hostore/__init__.py
 hostore/admin.py
 hostore/apps.py
 hostore/manager.py
 hostore/models.py
-hostore/tests.py
 hostore/views.py
 hostore/migrations/0001_initial.py
 hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
 hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
 hostore/migrations/0004_testdatastore_created_at.py
 hostore/migrations/0005_alter_testdatastore_prm.py
+hostore/migrations/0006_testdatastorewithattribute.py
 hostore/migrations/__init__.py
+hostore/tests/__init__.py
+hostore/tests/tests_basics.py
+hostore/tests/tests_slice_with_delay.py
+hostore/tests/tests_with_attributes.py
 hostore/utils/__init__.py
 hostore/utils/timeseries.py
 hostore/utils/utils.py
```

### Comparing `holcstore-0.2.2/hostore/migrations/0001_initial.py` & `holcstore-0.2.4/hostore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.2/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py` & `holcstore-0.2.4/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.2/hostore/models.py` & `holcstore-0.2.4/hostore/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+import datetime as dt
 import io
 import logging
 from collections import defaultdict
 from typing import List, Dict
-import datetime as dt
+
 import pandas as pd
 from django.db import models
 from django.db.models import Max
 from pyarrow import BufferReader
 
 from .manager import StoreQuerySet
 from .utils.timeseries import ts_combine_first, check_ts_completeness
-from .utils.utils import chunks
-
+from .utils.utils import chunks, slice_with_delay
 
 logger = logging.getLogger(__name__)
 
 
 class Store(models.Model):
     client_id = models.IntegerField()
     prm = models.CharField(max_length=70)
@@ -34,16 +34,19 @@
     @classmethod
     def count(cls, client_id: int, custom_filters=None):
         if custom_filters is None:
             custom_filters = {}
         return cls.objects.filter(client_id=client_id, **custom_filters).count()
 
     @classmethod
-    def find_holes(cls, client_id: int, sd: dt.datetime, ed: dt.datetime, freq='30min', prms: List[str] = None, chunk_size=50,
-                   freq_margin=pd.Timedelta(minutes=0), custom_filters=None) -> Dict[str, List]:
+    def find_holes(cls, client_id: int, sd: dt.datetime, ed: dt.datetime, freq='30min', prms: List[str] = None,
+                   chunk_size=50,
+                   freq_margin=pd.Timedelta(minutes=0),
+                   custom_filters=None,
+                   combined_by=('prm',), order_by=('-version',)) -> Dict[str, List]:
         """
         Find holes (missing data periods) for multiple prms within a specified datetime range.
 
         This method retrieves data from a database for each parameter associated with a client_id,
         checks each dataset for missing data within the specified datetime range, and identifies the start
         and end of each missing data period.
 
@@ -52,26 +55,31 @@
         :param ed: End datetime of the range to check for holes.
         :param freq: Frequency at which the data is expected, defaulting to '30min'.
         :param prms: Optional list of prms to check; if None, all parameters for the client are checked.
         :param chunk_size: The size of chunks to break the parameter list into for batch processing.
                            This helps in managing memory and processing large datasets efficiently, defaulting to 50.
         :param freq_margin: Freq margin for null sequences
         :param custom_filters: (optionnal) None or dict
+        :param combined_by: set of attributes for ordering load_curves before combine_first
         :return: A dictionary with prm as keys and a list of tuples (start, end) indicating
                  the missing data periods for each parameter. Start and end are included
         """
         if custom_filters is None:
             custom_filters = {}
         # If no prm are specified, retrieve all prm for the given client from the database
         if prms is None:
             prms = list(cls.objects.filter(client_id=client_id, **custom_filters).values_list('prm', flat=True))
 
         # Iterate over prms in chunks to manage memory usage and efficiency
         for prm_chunk in chunks(prms, chunk_size):
-            data_by_prm = cls.get_many_lc(prm_chunk, client_id, combined_versions=True, **custom_filters)
+            data_by_prm = cls.get_many_lc(prm_chunk, client_id,
+                                          combined_versions=True,
+                                          combined_by=combined_by,
+                                          order_by=order_by,
+                                          **custom_filters)
 
             # Check each parameter's data for completeness
             for prm in prm_chunk:
                 nulls_seqs = []
                 data = data_by_prm[prm]
                 if len(data) == 0:
                     # If there's no data for a prm, the entire range is considered as a hole
@@ -82,31 +90,36 @@
                     nulls_seqs = check_ts_completeness(data[0]['data'], sd, ed, freq=freq, freq_margin=freq_margin)
 
                 # Yield the output for this prm
                 # This allows processing part by part without waiting for the entire operation to complete
                 yield prm, nulls_seqs
 
     @classmethod
-    def get_lc(cls, prm: str, client_id: int, combined_versions=True, version: int = None, custom_filters=None) -> List[Dict]:
+    def get_lc(cls, prm: str, client_id: int, combined_versions=True, version: int = None, custom_filters=None,
+               combined_by=('prm',),
+               order_by=('-version',),
+               combined_delay=pd.Timedelta(days=1)) -> List[Dict]:
         """
         Get the prm load curve
         Args:
             prm: str
             client_id: int, client's id
             combined_versions: bool, if multiple versions exists we combine them (default True)
             version: return only the selected version
             custom_filters: (optionnal) None or dict
+            combined_by: set of attributes to bombined by
+            order_by: set of attributes for ordering load_curves before combine_first
         Returns:
             List[Dict]
         """
         logger.info(f'Getting load curve with prm {prm} for client {client_id}')
         if custom_filters is None:
             custom_filters = {}
 
-        qs = cls.objects.filter(prm=prm, client_id=client_id, **custom_filters).order_by('-version')
+        qs = cls.objects.filter(prm=prm, client_id=client_id, **custom_filters).order_by(*order_by)
         if version is not None:
             qs = qs.filter(version=version)
 
         entries = []
         for entry in qs:
             entry_dict = vars(entry)
             reader = BufferReader(entry_dict['data'])
@@ -115,62 +128,48 @@
                 ds.set_index('index', inplace=True)
             else:
                 logger.info(f'data is malformed, remove key {prm}')
                 entry.delete()
             entry_dict['data'] = ds.iloc[:, 0]
             entries.append(entry_dict)
 
+        cleared_combined_by = set([attr for attr in combined_by])
+        ds_combined_dict = defaultdict(lambda: None)
         if len(entries) > 0 and combined_versions:
-            ds_combined = ts_combine_first([e['data'] for e in entries])
-            entries[0]['data'] = ds_combined
-            return entries[0:1]
-        return entries
-
-    @classmethod
-    def get_lc_by_ids(cls, ids: List[int], client_id: int) -> List[Dict]:
-        """
-        Get the prm load curve
-        Args:
-            ids: List of ids
-            client_id: int, client's id
-        Returns:
-            List[Dict]
-        """
-        logger.info(f'Getting load curve with ids {ids} for client {client_id}')
-
-        qs = cls.objects.filter(id__in=ids, client_id=client_id)
-
-        entries = []
-        for entry in qs:
-            entry_dict = vars(entry)
-            reader = BufferReader(entry_dict['data'])
-            ds = pd.read_feather(reader)
-            if 'index' in ds.columns:
-                ds.set_index('index', inplace=True)
-            else:
-                logger.info(f'data is malformed, remove id {id}')
-                entry.delete()
-            entry_dict['data'] = ds.iloc[:, 0]
-            entries.append(entry_dict)
+            for e in entries:
+                key = str([e[attr] for attr in cleared_combined_by])
+                e['data'] = slice_with_delay(e['data'], combined_delay)
+                if ds_combined_dict[key] is None:
+                    ds_combined_dict[key] = e
+                else:
+                    ds_combined_dict[key]['data'] = ts_combine_first([ds_combined_dict[key]['data'], e['data']])
+            entries = list(ds_combined_dict.values())
         return entries
 
     @classmethod
-    def get_many_lc(cls, prms: [str], client_id: int, combined_versions=True, custom_filters=None) -> Dict[str, List[Dict]]:
+    def get_many_lc(cls, prms: [str], client_id: int, combined_versions=True,
+                    custom_filters=None,
+                    combined_by=('prm',),
+                    order_by=('-version',),
+                    combined_delay=pd.Timedelta(days=1)) -> Dict[str, List[Dict]]:
         """
         Get many prms from cache
         Args:
             prms: list of prms
             client_id: int, client's id
             combined_versions: bool, if multiple versions exists we combine them (default True)
+            custom_filters: dict used in filter
+            combined_by: set of attributes to bombined by
+            order_by: set of attributes for ordering load_curves before combine_first
         Returns:
             Dict[str, List[Dict]]
         """
         if custom_filters is None:
             custom_filters = {}
-        qs = cls.objects.filter(prm__in=prms, client_id=client_id, **custom_filters).order_by('-version')
+        qs = cls.objects.filter(prm__in=prms, client_id=client_id, **custom_filters).order_by(*order_by)
         results = defaultdict(lambda: [])
         invalid_ids = []
         for entry in qs:
             reader = BufferReader(entry.data)
             ds = pd.read_feather(reader)
             try:
                 ds.set_index('index', inplace=True)
@@ -181,31 +180,45 @@
             entry_dict['data'] = ds.iloc[:, 0]
             results[entry.prm].append(entry_dict)
 
         if len(invalid_ids) > 0:
             logger.info(f'data is malformed, for ids {invalid_ids}')
             cls.objects.filter(id__in=invalid_ids).delete()
 
+        cleared_combined_by = set([attr for attr in combined_by])
+        ds_combined_dict = defaultdict(lambda: defaultdict(lambda: None))
         if len(results) > 0 and combined_versions:
             for prm, entries in results.items():
-                ds_combined = ts_combine_first([e['data'] for e in entries])
-                entries[0]['data'] = ds_combined
-                results[prm] = entries[0:1]
+                for e in entries:
+                    key = str([e[attr] for attr in cleared_combined_by])
+                    e['data'] = slice_with_delay(e['data'], combined_delay)
+                    if ds_combined_dict[prm][key] is None:
+                        ds_combined_dict[prm][key] = e
+                    else:
+                        ds_combined_dict[prm][key]['data'] = ts_combine_first([ds_combined_dict[prm][key]['data'], e['data']])
+            for prm in results:
+                results[prm] = list(ds_combined_dict[prm].values())
 
         return results
 
     @classmethod
-    def set_lc(cls, prm: str, value: pd.Series, client_id: int, versionning=False, attributes_to_set=None) -> None:
+    def set_lc(cls, prm: str,
+               value: pd.Series,
+               client_id: int,
+               versionning=False,
+               versionning_by=('prm',),
+               attributes_to_set=None) -> None:
         """
         Set one prm to cache
         Args:
             prm: str
             value: pd.Series
             client_id: int, client's id
             versionning: bool, if True, a new version will be saved else the load curve is replaced (default False)
+            versionning_by: set of attributes used for versionning (prm is mandatory)
             attributes_to_set: (optionnal) None or dict
         Returns:
             None
         """
         if attributes_to_set is None:
             attributes_to_set = {}
         logger.info(f'SET key {prm} in cache')
@@ -217,45 +230,52 @@
             df.reset_index(inplace=True, names=['index'])
             buf = io.BytesIO()
             df.to_feather(buf, compression='lz4')
             v = buf.getvalue()
             if not versionning:
                 cls.objects.update_or_create(client_id=client_id, prm=prm, defaults=dict(data=v), **attributes_to_set)
             else:
-                latest_version = cls.objects.filter(client_id=client_id, prm=prm, **attributes_to_set).aggregate(Max('version'))[
-                    'version__max']
+                assert 'prm' in versionning_by
+                _filters = {'prm': prm, **{k: v for k, v in attributes_to_set.items() if k in versionning_by}}
+                latest_version = cls.objects.filter(client_id=client_id, **_filters).aggregate(Max('version'))['version__max']
                 if latest_version is not None:
                     # If there's at least one object with the same prm, increment the version
                     version = latest_version + 1
                 else:
                     # If there are no objects with the same prm, start with version 0
                     version = 0
                 logger.info(f"version to insert {version}")
                 cls.objects.create(client_id=client_id, prm=prm, data=v, version=version, **attributes_to_set)
             logger.info(f'SET prm {prm} in cache DONE')
         else:
             raise ValueError(f'Cannot cache value of type {type(value)}, only dataframe are accepted')
 
     @classmethod
-    def set_many_lc(cls, dataseries: Dict[str, pd.Series], client_id: int, versionning=False, attributes_to_set=None) -> None:
+    def set_many_lc(cls, dataseries: Dict[str, pd.Series], client_id: int, versionning=False,
+                    versionning_by=('prm',),
+                    attributes_to_set=None) -> None:
         """
         Update prms contained in dataseries dict
         Args:
             dataseries: dict(key: pd.Series)
             client_id: int, client's id
             versionning: bool, if True, a new version will be saved for each prm else the load curve is replaced
+            versionning_by: set of attributes used for versionning (prm is mandatory)
             attributes_to_set: (optionnal) None or dict
         Returns:
             None
         """
         if len(dataseries) > 0:
             logger.info(f'Updating cache for {list(dataseries.keys())}')
         for prm, data in dataseries.items():
             if data is not None and not data.empty:
-                cls.set_lc(prm, data, client_id, versionning=versionning, attributes_to_set=attributes_to_set)
+                cls.set_lc(prm, data, client_id,
+                           versionning=versionning,
+                           versionning_by=versionning_by,
+                           attributes_to_set=attributes_to_set)
 
     @classmethod
     def clear(cls, prms: [str], client_id: int, version=None, custom_filters=None) -> None:
         """
         Method to clear multiple prm from cache
         Args:
             prms: list of prms
@@ -293,7 +313,15 @@
             qs.delete()
 
 
 class TestDataStore(Store):
     class Meta(Store.Meta):
         abstract = False
         app_label = 'hostore'
+
+
+class TestDataStoreWithAttribute(Store):
+    year = models.IntegerField()
+    class Meta(Store.Meta):
+        abstract = False
+        app_label = 'hostore'
+        unique_together = ('prm', 'client_id', 'year', 'created_at')
```

### Comparing `holcstore-0.2.2/hostore/tests.py` & `holcstore-0.2.4/hostore/tests/tests_basics.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import random
 import datetime as dt
 import numpy as np
 import pandas as pd
 import pytz
 from django.test import TestCase
 
-from .models import TestDataStore
+from hostore.models import TestDataStore
 
 
 class HoCacheTestCase(TestCase):
     databases = ('default',)
     def setUp(self):
         # Set up data for the tests
         # For example, create a HoCache instance
@@ -152,26 +152,14 @@
         self.assertEquals(len(data), 1)
         self.assertEquals(data[0]['version'], 0)
         # Vérifier que la combinaison donne la deuxième version
         pd.testing.assert_series_equal(data[0]['data'], self.test_data, check_names=False)
 
     # *******************************************************
 
-    def test_get_by_ids(self):
-        TestDataStore.clear_all(self.test_client_id)
-        # Test get_by_ids method
-        new_prm = 'new_test_prm'
-        TestDataStore.set_lc(prm=new_prm, value=self.test_data, client_id=self.test_client_id)
-
-        ids = TestDataStore.objects.all().values_list('id', flat=True)
-        data = TestDataStore.get_lc_by_ids(ids, self.test_client_id)
-
-        self.assertEquals(len(data), 1)
-        pd.testing.assert_series_equal(data[0]['data'], self.test_data, check_names=False)
-
     def test_clearing(self):
         TestDataStore.clear([self.test_prm], self.test_client_id)
         data_after_clear = TestDataStore.get_lc(self.test_prm, self.test_client_id)
         self.assertEqual(len(data_after_clear), 0)
 
     def test_clearing_version(self):
         TestDataStore.clear([self.test_prm_2], self.test_client_id, version=0)
```

### Comparing `holcstore-0.2.2/hostore/utils/timeseries.py` & `holcstore-0.2.4/hostore/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.2/setup.cfg` & `holcstore-0.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = holcstore
-version = 0.2.2
+version = 0.2.4
 description = A Django App to use a simple load curve store
 long_description = file: README.rst
 url = 
 author = Jean-Pierre Lartigue
 author_email = 
 license = BSD-3-Clause
 classifiers =
```

