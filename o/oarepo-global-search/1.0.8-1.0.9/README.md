# Comparing `tmp/oarepo_global_search-1.0.8.tar.gz` & `tmp/oarepo_global_search-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo_global_search-1.0.8.tar", last modified: Wed May 22 14:15:29 2024, max compression
+gzip compressed data, was "oarepo_global_search-1.0.9.tar", last modified: Tue May 28 12:58:25 2024, max compression
```

## Comparing `oarepo_global_search-1.0.8.tar` & `oarepo_global_search-1.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/format.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.212615 oarepo_global_search-1.0.8/oarepo_global_search/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.212615 oarepo_global_search-1.0.8/oarepo_global_search/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.212615 oarepo_global_search-1.0.8/oarepo_global_search/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/resources/records/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.212615 oarepo_global_search-1.0.8/oarepo_global_search/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/oarepo_global_search/services/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/params.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/user_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/oarepo_global_search/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.208615 oarepo_global_search-1.0.8/oarepo_global_search/ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.208615 oarepo_global_search-1.0.8/oarepo_global_search/ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/oarepo_global_search/ui/templates/semantic-ui/global_search/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/ui/templates/semantic-ui/global_search/Search.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/oarepo_global_search/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/views/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/views/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:12:25.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      866 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.850683 oarepo_global_search-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-28 12:58:25.850683 oarepo_global_search-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/format.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.846682 oarepo_global_search-1.0.9/oarepo_global_search/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.846682 oarepo_global_search-1.0.9/oarepo_global_search/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.846682 oarepo_global_search-1.0.9/oarepo_global_search/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/resources/records/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.846682 oarepo_global_search-1.0.9/oarepo_global_search/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.850683 oarepo_global_search-1.0.9/oarepo_global_search/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/services/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/services/records/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/services/records/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/services/records/user_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.850683 oarepo_global_search-1.0.9/oarepo_global_search/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.842682 oarepo_global_search-1.0.9/oarepo_global_search/ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.842682 oarepo_global_search-1.0.9/oarepo_global_search/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.850683 oarepo_global_search-1.0.9/oarepo_global_search/ui/templates/semantic-ui/global_search/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/ui/templates/semantic-ui/global_search/Search.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.850683 oarepo_global_search-1.0.9/oarepo_global_search/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/oarepo_global_search/views/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:58:25.850683 oarepo_global_search-1.0.9/oarepo_global_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-28 12:58:25.000000 oarepo_global_search-1.0.9/oarepo_global_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-28 12:58:25.000000 oarepo_global_search-1.0.9/oarepo_global_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:58:25.000000 oarepo_global_search-1.0.9/oarepo_global_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-28 12:58:25.000000 oarepo_global_search-1.0.9/oarepo_global_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:55:31.000000 oarepo_global_search-1.0.9/oarepo_global_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 12:58:25.000000 oarepo_global_search-1.0.9/oarepo_global_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 12:58:25.000000 oarepo_global_search-1.0.9/oarepo_global_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      866 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-28 12:58:25.850683 oarepo_global_search-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 12:54:42.000000 oarepo_global_search-1.0.9/setup.py
```

### Comparing `oarepo_global_search-1.0.8/MANIFEST.in` & `oarepo_global_search-1.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/PKG-INFO` & `oarepo_global_search-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-global-search
-Version: 1.0.8
+Version: 1.0.9
 Summary: "A model builder plugin for global search"
 Home-page: https://github.com/oarepo/oarepo-global-search
 Author: Alzbeta Pokorna
 Author-email: Alzbeta.Pokorna@cesnet.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
```

### Comparing `oarepo_global_search-1.0.8/README.md` & `oarepo_global_search-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/ext.py` & `oarepo_global_search-1.0.9/oarepo_global_search/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/resources/records/config.py` & `oarepo_global_search-1.0.9/oarepo_global_search/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/resources/records/resource.py` & `oarepo_global_search-1.0.9/oarepo_global_search/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/resources/records/response.py` & `oarepo_global_search-1.0.9/oarepo_global_search/resources/records/response.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/services/records/params.py` & `oarepo_global_search-1.0.9/oarepo_global_search/services/records/params.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/services/records/results.py` & `oarepo_global_search-1.0.9/oarepo_global_search/services/records/results.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/services/records/service.py` & `oarepo_global_search-1.0.9/oarepo_global_search/services/records/service.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/services/records/user_service.py` & `oarepo_global_search-1.0.9/oarepo_global_search/services/records/user_service.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/ui/config.py` & `oarepo_global_search-1.0.9/oarepo_global_search/ui/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,17 @@
         resource_defs = current_app.config.get("GLOBAL_SEARCH_MODELS")
         default_components = {}
         for definition in resource_defs:
             ui_resource = obj_or_import_string(definition["ui_resource_config"])
             service_def = obj_or_import_string(definition["model_service"])
             service_cfg = obj_or_import_string(definition["service_config"])
             service = service_def(service_cfg())
-            default_components[service.record_cls.schema.value] = ui_resource.search_component
+            default_components[service.record_cls.schema.value] = getattr(ui_resource ,"search_component", None )
         return default_components
 
 class GlobalSearchUIResource(RecordsUIResource):
     pass
 
 
 def create_blueprint(app):
     """Register blueprint for this resource."""
-    return GlobalSearchUIResource(GlobalSearchUIResourceConfig()).as_blueprint()
+    return GlobalSearchUIResource(GlobalSearchUIResourceConfig()).as_blueprint()
```

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/views/api.py` & `oarepo_global_search-1.0.9/oarepo_global_search/views/api.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search/views/app.py` & `oarepo_global_search-1.0.9/oarepo_global_search/views/app.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search.egg-info/PKG-INFO` & `oarepo_global_search-1.0.9/oarepo_global_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-global-search
-Version: 1.0.8
+Version: 1.0.9
 Summary: "A model builder plugin for global search"
 Home-page: https://github.com/oarepo/oarepo-global-search
 Author: Alzbeta Pokorna
 Author-email: Alzbeta.Pokorna@cesnet.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
```

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search.egg-info/SOURCES.txt` & `oarepo_global_search-1.0.9/oarepo_global_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/oarepo_global_search.egg-info/entry_points.txt` & `oarepo_global_search-1.0.9/oarepo_global_search.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/run-tests.sh` & `oarepo_global_search-1.0.9/run-tests.sh`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.8/setup.cfg` & `oarepo_global_search-1.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-global-search
-version = 1.0.8
+version = 1.0.9
 description = "A model builder plugin for global search"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio relations model builder
 license = MIT
 author = Alzbeta Pokorna
 author_email = Alzbeta.Pokorna@cesnet.cz
```

