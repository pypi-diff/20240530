# Comparing `tmp/transmission_rpc-7.0.7a0.tar.gz` & `tmp/transmission_rpc-7.0.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission_rpc-7.0.7a0.tar", max compression
+gzip compressed data, was "transmission_rpc-7.0.7a1.tar", max compression
```

## Comparing `transmission_rpc-7.0.7a0.tar` & `transmission_rpc-7.0.7a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1127 2024-05-30 17:26:51.879074 transmission_rpc-7.0.7a0/LICENSE
--rw-r--r--   0        0        0     2277 2024-05-30 17:26:51.879074 transmission_rpc-7.0.7a0/README.md
--rw-r--r--   0        0        0     3057 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/pyproject.toml
--rw-r--r--   0        0        0     2230 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/__init__.py
--rw-r--r--   0        0        0    45352 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/client.py
--rw-r--r--   0        0        0    10080 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/constants.py
--rw-r--r--   0        0        0     1673 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/error.py
--rw-r--r--   0        0        0        0 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/py.typed
--rw-r--r--   0        0        0    12488 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/session.py
--rw-r--r--   0        0        0    23901 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/torrent.py
--rw-r--r--   0        0        0     1900 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/types.py
--rw-r--r--   0        0        0     2643 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/utils.py
--rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 transmission_rpc-7.0.7a0/PKG-INFO
+-rw-r--r--   0        0        0     1127 2024-05-30 17:46:00.296672 transmission_rpc-7.0.7a1/LICENSE
+-rw-r--r--   0        0        0     2277 2024-05-30 17:46:00.296672 transmission_rpc-7.0.7a1/README.md
+-rw-r--r--   0        0        0     3057 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/pyproject.toml
+-rw-r--r--   0        0        0     2230 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/__init__.py
+-rw-r--r--   0        0        0    45352 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/client.py
+-rw-r--r--   0        0        0    10080 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/constants.py
+-rw-r--r--   0        0        0     1673 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/error.py
+-rw-r--r--   0        0        0        0 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/py.typed
+-rw-r--r--   0        0        0    12488 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/session.py
+-rw-r--r--   0        0        0    23901 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/torrent.py
+-rw-r--r--   0        0        0     1900 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/types.py
+-rw-r--r--   0        0        0     2643 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/utils.py
+-rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 transmission_rpc-7.0.7a1/PKG-INFO
```

### Comparing `transmission_rpc-7.0.7a0/LICENSE` & `transmission_rpc-7.0.7a1/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a0/README.md` & `transmission_rpc-7.0.7a1/README.md`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a0/pyproject.toml` & `transmission_rpc-7.0.7a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "transmission-rpc"
-version = "7.0.7a0"
+version = "7.0.7a1"
 description = "Python module that implements the Transmission bittorent client JSON-RPC protocol"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'README.md'
 repository = 'https://github.com/Trim21/transmission-rpc'
 license = 'MIT'
 packages = [{ include = 'transmission_rpc' }]
 keywords = ['transmission', 'rpc']
```

### Comparing `transmission_rpc-7.0.7a0/transmission_rpc/__init__.py` & `transmission_rpc-7.0.7a1/transmission_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a0/transmission_rpc/client.py` & `transmission_rpc-7.0.7a1/transmission_rpc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -713,15 +713,15 @@
                 "seedIdleMode": seed_idle_mode,
                 "seedRatioLimit": seed_ratio_limit,
                 "seedRatioMode": seed_ratio_mode,
                 "trackerAdd": tracker_add,
                 "trackerRemove": tracker_remove,
                 "trackerReplace": tracker_replace,
                 "labels": list_or_none(_single_str_as_list(labels)),
-                "trackerlist": None if tracker_list is None else "\n".join("\n\n".join(x) for x in tracker_list),
+                "trackerList": None if tracker_list is None else "\n".join("\n\n".join(x) for x in tracker_list),
                 "group": group,
             }
         )
 
         args.update(kwargs)
 
         if args:
```

### Comparing `transmission_rpc-7.0.7a0/transmission_rpc/constants.py` & `transmission_rpc-7.0.7a1/transmission_rpc/constants.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a0/transmission_rpc/error.py` & `transmission_rpc-7.0.7a1/transmission_rpc/error.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a0/transmission_rpc/session.py` & `transmission_rpc-7.0.7a1/transmission_rpc/session.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a0/transmission_rpc/torrent.py` & `transmission_rpc-7.0.7a1/transmission_rpc/torrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,15 +620,15 @@
     def trackers(self) -> list[Tracker]:
         """trackers of torrent"""
         return [Tracker(fields=x) for x in self.fields["trackers"]]
 
     @property
     def tracker_list(self) -> list[str]:
         """list of str of announce URLs"""
-        return [x for x in self.fields["trackerlist"].splitlines() if x]
+        return [x for x in self.fields["trackerList"].splitlines() if x]
 
     @property
     def tracker_stats(self) -> list[TrackerStats]:
         """tracker status, for example, announce success/failure status"""
         return [TrackerStats(fields=x) for x in self.fields["trackerStats"]]
 
     @property
```

### Comparing `transmission_rpc-7.0.7a0/transmission_rpc/types.py` & `transmission_rpc-7.0.7a1/transmission_rpc/types.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a0/transmission_rpc/utils.py` & `transmission_rpc-7.0.7a1/transmission_rpc/utils.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a0/PKG-INFO` & `transmission_rpc-7.0.7a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmission-rpc
-Version: 7.0.7a0
+Version: 7.0.7a1
 Summary: Python module that implements the Transmission bittorent client JSON-RPC protocol
 Home-page: https://github.com/Trim21/transmission-rpc
 License: MIT
 Keywords: transmission,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
```

