# Comparing `tmp/cave_utils-2.2.0b5.tar.gz` & `tmp/cave_utils-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-2.2.0b5.tar", last modified: Thu May  2 19:58:48 2024, max compression
+gzip compressed data, was "cave_utils-2.2.1.tar", last modified: Thu May 30 12:44:10 2024, max compression
```

## Comparing `cave_utils-2.2.0b5.tar` & `cave_utils-2.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-2.2.0b5/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-2.2.0b5/NOTICE.md
--rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     2946 2024-03-06 18:01:37.000000 cave_utils-2.2.0b5/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.636477 cave_utils-2.2.0b5/cave_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      447 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/__init__.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/cave_utils/api/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     8447 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4977 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/appBar.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1064 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/extraKwargs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2211 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/globalOutputs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    17148 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/groupedOutputs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    12103 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/mapFeatures.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    30325 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/maps.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    12768 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/pages.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     7086 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/panes.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    14927 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/settings.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/cave_utils/api_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      311 2024-03-04 20:53:07.000000 cave_utils-2.2.0b5/cave_utils/api_utils/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    35210 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api_utils/general.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      991 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api_utils/validator.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    16322 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api_utils/validator_utils.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-10-16 13:43:50.000000 cave_utils-2.2.0b5/cave_utils/arguments.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/cave_utils/builders/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      273 2024-03-06 18:02:20.000000 cave_utils-2.2.0b5/cave_utils/builders/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    15444 2024-03-14 15:24:47.000000 cave_utils-2.2.0b5/cave_utils/builders/groups.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4924 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/geo_utils.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1529 2023-11-30 18:55:27.000000 cave_utils-2.2.0b5/cave_utils/log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      351 2024-05-02 19:54:40.000000 cave_utils-2.2.0b5/cave_utils/socket.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/cave_utils.egg-info/
--rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-05-02 19:58:48.000000 cave_utils-2.2.0b5/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      942 2024-05-02 19:58:48.000000 cave_utils-2.2.0b5/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-05-02 19:58:48.000000 cave_utils-2.2.0b5/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-05-02 19:58:48.000000 cave_utils-2.2.0b5/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2024-05-02 19:58:48.000000 cave_utils-2.2.0b5/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      743 2024-05-02 19:53:36.000000 cave_utils-2.2.0b5/pyproject.toml
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      143 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/setup.cfg
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      306 2023-11-30 18:55:27.000000 cave_utils-2.2.0b5/test/test_arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     5107 2024-03-06 18:02:20.000000 cave_utils-2.2.0b5/test/test_builders_groups.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      570 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/test/test_geo_utils.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       40 2024-03-06 17:54:00.000000 cave_utils-2.2.0b5/test/test_import.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      233 2023-11-30 18:55:27.000000 cave_utils-2.2.0b5/test/test_log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    75749 2024-01-31 16:20:08.000000 cave_utils-2.2.0b5/test/test_validator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-30 12:44:10.643406 cave_utils-2.2.1/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-2.2.1/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-2.2.1/NOTICE.md
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     3502 2024-05-30 12:44:10.643406 cave_utils-2.2.1/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     2946 2024-03-06 18:01:37.000000 cave_utils-2.2.1/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-30 12:44:10.639406 cave_utils-2.2.1/cave_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      447 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/__init__.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-30 12:44:10.643406 cave_utils-2.2.1/cave_utils/api/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     8447 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4977 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api/appBar.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1064 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api/extraKwargs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2211 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api/globalOutputs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    17148 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api/groupedOutputs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    12103 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api/mapFeatures.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    30325 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api/maps.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    12768 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api/pages.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     7086 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api/panes.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    14927 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api/settings.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-30 12:44:10.643406 cave_utils-2.2.1/cave_utils/api_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      311 2024-03-04 20:53:07.000000 cave_utils-2.2.1/cave_utils/api_utils/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    35220 2024-05-30 12:36:31.000000 cave_utils-2.2.1/cave_utils/api_utils/general.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      991 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api_utils/validator.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    16322 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/api_utils/validator_utils.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-10-16 13:43:50.000000 cave_utils-2.2.1/cave_utils/arguments.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-30 12:44:10.643406 cave_utils-2.2.1/cave_utils/builders/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      273 2024-03-06 18:02:20.000000 cave_utils-2.2.1/cave_utils/builders/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    15444 2024-03-14 15:24:47.000000 cave_utils-2.2.1/cave_utils/builders/groups.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4924 2024-05-02 19:54:41.000000 cave_utils-2.2.1/cave_utils/geo_utils.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1529 2023-11-30 18:55:27.000000 cave_utils-2.2.1/cave_utils/log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      351 2024-05-02 19:54:40.000000 cave_utils-2.2.1/cave_utils/socket.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-30 12:44:10.643406 cave_utils-2.2.1/cave_utils.egg-info/
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     3502 2024-05-30 12:44:10.000000 cave_utils-2.2.1/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      942 2024-05-30 12:44:10.000000 cave_utils-2.2.1/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-05-30 12:44:10.000000 cave_utils-2.2.1/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-05-30 12:44:10.000000 cave_utils-2.2.1/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2024-05-30 12:44:10.000000 cave_utils-2.2.1/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      741 2024-05-30 12:40:44.000000 cave_utils-2.2.1/pyproject.toml
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      141 2024-05-30 12:44:10.643406 cave_utils-2.2.1/setup.cfg
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-30 12:44:10.643406 cave_utils-2.2.1/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      306 2023-11-30 18:55:27.000000 cave_utils-2.2.1/test/test_arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     5107 2024-03-06 18:02:20.000000 cave_utils-2.2.1/test/test_builders_groups.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      570 2024-05-02 19:54:41.000000 cave_utils-2.2.1/test/test_geo_utils.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       40 2024-03-06 17:54:00.000000 cave_utils-2.2.1/test/test_import.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      233 2023-11-30 18:55:27.000000 cave_utils-2.2.1/test/test_log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    75749 2024-01-31 16:20:08.000000 cave_utils-2.2.1/test/test_validator.py
```

### Comparing `cave_utils-2.2.0b5/LICENSE` & `cave_utils-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/NOTICE.md` & `cave_utils-2.2.1/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/PKG-INFO` & `cave_utils-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 2.2.0b5
+Version: 2.2.1
 Summary: Python wrapper for api use in the cave_app
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/mit-cave/cave_utils
 Project-URL: Bug Tracker, https://github.com/mit-cave/cave_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `cave_utils-2.2.0b5/README.md` & `cave_utils-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api/__init__.py` & `cave_utils-2.2.1/cave_utils/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api/appBar.py` & `cave_utils-2.2.1/cave_utils/api/appBar.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api/extraKwargs.py` & `cave_utils-2.2.1/cave_utils/api/extraKwargs.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api/globalOutputs.py` & `cave_utils-2.2.1/cave_utils/api/globalOutputs.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api/groupedOutputs.py` & `cave_utils-2.2.1/cave_utils/api/groupedOutputs.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api/mapFeatures.py` & `cave_utils-2.2.1/cave_utils/api/mapFeatures.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api/maps.py` & `cave_utils-2.2.1/cave_utils/api/maps.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api/pages.py` & `cave_utils-2.2.1/cave_utils/api/pages.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api/panes.py` & `cave_utils-2.2.1/cave_utils/api/panes.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api/settings.py` & `cave_utils-2.2.1/cave_utils/api/settings.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api_utils/general.py` & `cave_utils-2.2.1/cave_utils/api_utils/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
                 "unitPlacement": ["after", "afterWithSpace", "before", "beforeWithSpace"],
                 "notation": ["compact", "precision", "scientific", "engineering"],
                 "notationDisplay": notationDisplay_options_dict.get(notation, []),
                 "legendNotation": ["compact", "precision", "scientific", "engineering"],
                 "legendNotationDisplay": notationDisplay_options_dict.get(legendNotation, []),
                 "variant": {
                     "head": ["column", "row", "icon", "iconRow"],
-                    "text": ["textarea"],
+                    "text": ["single", "textarea"],
                     "num": ["field", "slider", "icon", "iconCompact"],
                     "selector": [
                         "dropdown",
                         "checkbox",
                         "radio",
                         "combobox",
                         "hstepper",
```

### Comparing `cave_utils-2.2.0b5/cave_utils/api_utils/validator.py` & `cave_utils-2.2.1/cave_utils/api_utils/validator.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/api_utils/validator_utils.py` & `cave_utils-2.2.1/cave_utils/api_utils/validator_utils.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/arguments.py` & `cave_utils-2.2.1/cave_utils/arguments.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/builders/groups.py` & `cave_utils-2.2.1/cave_utils/builders/groups.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/geo_utils.py` & `cave_utils-2.2.1/cave_utils/geo_utils.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils/log.py` & `cave_utils-2.2.1/cave_utils/log.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/cave_utils.egg-info/PKG-INFO` & `cave_utils-2.2.1/cave_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 2.2.0b5
+Version: 2.2.1
 Summary: Python wrapper for api use in the cave_app
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/mit-cave/cave_utils
 Project-URL: Bug Tracker, https://github.com/mit-cave/cave_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `cave_utils-2.2.0b5/cave_utils.egg-info/SOURCES.txt` & `cave_utils-2.2.1/cave_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/pyproject.toml` & `cave_utils-2.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cave_utils"
-version = "2.2.0b5"
+version = "2.2.1"
 description = "Python wrapper for api use in the cave_app"
 authors = [
     {name="Connor Makowski", email="conmak@mit.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cave_utils-2.2.0b5/test/test_builders_groups.py` & `cave_utils-2.2.1/test/test_builders_groups.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/test/test_geo_utils.py` & `cave_utils-2.2.1/test/test_geo_utils.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b5/test/test_validator.py` & `cave_utils-2.2.1/test/test_validator.py`

 * *Files identical despite different names*

