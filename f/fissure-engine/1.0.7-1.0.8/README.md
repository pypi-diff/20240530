# Comparing `tmp/fissure_engine-1.0.7.tar.gz` & `tmp/fissure_engine-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fissure_engine-1.0.7.tar", last modified: Fri May 17 23:49:22 2024, max compression
+gzip compressed data, was "fissure_engine-1.0.8.tar", last modified: Thu May 30 15:53:11 2024, max compression
```

## Comparing `fissure_engine-1.0.7.tar` & `fissure_engine-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:49:22.989657 fissure_engine-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-17 23:49:22.989657 fissure_engine-1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:49:22.989657 fissure_engine-1.0.7/fissure_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 23:49:19.000000 fissure_engine-1.0.7/fissure_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72700 2024-05-17 23:49:19.000000 fissure_engine-1.0.7/fissure_engine/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    18790 2024-05-17 23:49:19.000000 fissure_engine-1.0.7/fissure_engine/fissure_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:49:22.989657 fissure_engine-1.0.7/fissure_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-17 23:49:22.000000 fissure_engine-1.0.7/fissure_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-17 23:49:22.000000 fissure_engine-1.0.7/fissure_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:49:22.000000 fissure_engine-1.0.7/fissure_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-17 23:49:22.000000 fissure_engine-1.0.7/fissure_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 23:49:22.000000 fissure_engine-1.0.7/fissure_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:49:22.989657 fissure_engine-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-17 23:49:19.000000 fissure_engine-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:11.636273 fissure_engine-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 15:53:11.636273 fissure_engine-1.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:11.636273 fissure_engine-1.0.8/fissure_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:07.000000 fissure_engine-1.0.8/fissure_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72700 2024-05-30 15:53:07.000000 fissure_engine-1.0.8/fissure_engine/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18627 2024-05-30 15:53:07.000000 fissure_engine-1.0.8/fissure_engine/fissure_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:11.636273 fissure_engine-1.0.8/fissure_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 15:53:11.000000 fissure_engine-1.0.8/fissure_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-30 15:53:11.000000 fissure_engine-1.0.8/fissure_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:53:11.000000 fissure_engine-1.0.8/fissure_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:53:11.000000 fissure_engine-1.0.8/fissure_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 15:53:11.000000 fissure_engine-1.0.8/fissure_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:53:11.636273 fissure_engine-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-30 15:53:07.000000 fissure_engine-1.0.8/setup.py
```

### Comparing `fissure_engine-1.0.7/fissure_engine/common.py` & `fissure_engine-1.0.8/fissure_engine/common.py`

 * *Files identical despite different names*

### Comparing `fissure_engine-1.0.7/fissure_engine/fissure_engine.py` & `fissure_engine-1.0.8/fissure_engine/fissure_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,20 +41,14 @@
     era: str
     tier: int
     expiry: datetime
     fissure_type: str
     activation: datetime
     duration: timedelta
 
-    @property
-    def time_left(self):
-        now = datetime.now()
-        time_remaining = self.expiry - now
-        return int(time_remaining.total_seconds())
-
     def __eq__(self, other):
         if isinstance(other, Fissure):
             return (self.node == other.node and
                     self.mission == other.mission and
                     self.planet == other.planet and
                     self.tileset == other.tileset and
                     self.enemy == other.enemy and
```

### Comparing `fissure_engine-1.0.7/setup.py` & `fissure_engine-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 DESCRIPTION = 'Engine for getting fissure information in Warframe.'
 LONG_DESCRIPTION = 'Engine for getting the current fissures for Warframe in a dictionary object.'
 
 
 setup(
     name='fissure-engine',
     version=VERSION,
```

