# Comparing `tmp/oianalytics-0.5.2b6.tar.gz` & `tmp/oianalytics-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oianalytics-0.5.2b6.tar", max compression
+gzip compressed data, was "oianalytics-0.5.3.tar", max compression
```

## Comparing `oianalytics-0.5.2b6.tar` & `oianalytics-0.5.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    13799 2023-03-15 14:01:49.113528 oianalytics-0.5.2b6/LICENSE
--rw-r--r--   0        0        0       94 2024-03-14 14:29:49.510717 oianalytics-0.5.2b6/oianalytics/__init__.py
--rw-r--r--   0        0        0      124 2024-02-12 10:28:03.022129 oianalytics-0.5.2b6/oianalytics/api/__init__.py
--rw-r--r--   0        0        0     2373 2023-03-15 14:01:49.113932 oianalytics-0.5.2b6/oianalytics/api/_credentials.py
--rw-r--r--   0        0        0     2442 2024-02-12 10:28:03.022426 oianalytics-0.5.2b6/oianalytics/api/_dataframes/__init__.py
--rw-r--r--   0        0        0    16024 2023-11-06 09:30:13.500439 oianalytics-0.5.2b6/oianalytics/api/_dataframes/assets.py
--rw-r--r--   0        0        0     3847 2023-11-06 09:30:13.500761 oianalytics-0.5.2b6/oianalytics/api/_dataframes/azure_blob_sources.py
--rw-r--r--   0        0        0    48788 2024-02-12 10:28:03.022749 oianalytics-0.5.2b6/oianalytics/api/_dataframes/batches.py
--rw-r--r--   0        0        0    41856 2023-10-30 14:56:38.145683 oianalytics-0.5.2b6/oianalytics/api/_dataframes/data.py
--rw-r--r--   0        0        0     9979 2023-03-15 14:01:49.114785 oianalytics-0.5.2b6/oianalytics/api/_dataframes/events.py
--rw-r--r--   0        0        0     4631 2023-03-15 14:01:49.114887 oianalytics-0.5.2b6/oianalytics/api/_dataframes/files.py
--rw-r--r--   0        0        0     7991 2023-11-06 09:30:13.501670 oianalytics-0.5.2b6/oianalytics/api/_dataframes/model_instances.py
--rw-r--r--   0        0        0     3933 2023-11-06 09:30:13.502064 oianalytics-0.5.2b6/oianalytics/api/_dataframes/profiles.py
--rw-r--r--   0        0        0     2416 2023-10-30 14:56:38.146077 oianalytics-0.5.2b6/oianalytics/api/_dataframes/quantities.py
--rw-r--r--   0        0        0     5581 2024-02-12 10:28:10.083841 oianalytics-0.5.2b6/oianalytics/api/_dataframes/tags.py
--rw-r--r--   0        0        0     5463 2023-11-06 09:30:13.502604 oianalytics-0.5.2b6/oianalytics/api/_dataframes/units.py
--rw-r--r--   0        0        0     4251 2023-11-06 09:30:13.502818 oianalytics-0.5.2b6/oianalytics/api/_dataframes/users.py
--rw-r--r--   0        0        0      705 2024-03-14 10:52:51.096568 oianalytics-0.5.2b6/oianalytics/api/endpoints/__init__.py
--rw-r--r--   0        0        0     5806 2024-02-12 10:28:03.023906 oianalytics-0.5.2b6/oianalytics/api/endpoints/assets.py
--rw-r--r--   0        0        0     1437 2023-11-06 09:30:13.503405 oianalytics-0.5.2b6/oianalytics/api/endpoints/azure_blob_sources.py
--rw-r--r--   0        0        0    11949 2024-02-12 10:28:03.024141 oianalytics-0.5.2b6/oianalytics/api/endpoints/batches.py
--rw-r--r--   0        0        0     2646 2024-03-14 15:40:38.164002 oianalytics-0.5.2b6/oianalytics/api/endpoints/computation_jobs.py
--rw-r--r--   0        0        0    13255 2023-11-06 09:30:13.503842 oianalytics-0.5.2b6/oianalytics/api/endpoints/data.py
--rw-r--r--   0        0        0     2635 2023-11-06 09:30:13.504076 oianalytics-0.5.2b6/oianalytics/api/endpoints/events.py
--rw-r--r--   0        0        0     3204 2023-11-06 09:30:13.504386 oianalytics-0.5.2b6/oianalytics/api/endpoints/files.py
--rw-r--r--   0        0        0     1387 2023-11-06 09:30:13.504678 oianalytics-0.5.2b6/oianalytics/api/endpoints/model_instances.py
--rw-r--r--   0        0        0     2779 2024-02-12 10:28:03.024389 oianalytics-0.5.2b6/oianalytics/api/endpoints/profiles.py
--rw-r--r--   0        0        0      772 2023-10-30 14:56:38.147329 oianalytics-0.5.2b6/oianalytics/api/endpoints/quantities.py
--rw-r--r--   0        0        0     4519 2024-02-12 10:28:10.090400 oianalytics-0.5.2b6/oianalytics/api/endpoints/tags.py
--rw-r--r--   0        0        0     1787 2023-11-06 09:30:13.505426 oianalytics-0.5.2b6/oianalytics/api/endpoints/units.py
--rw-r--r--   0        0        0     2170 2024-02-12 10:28:03.024745 oianalytics-0.5.2b6/oianalytics/api/endpoints/users.py
--rw-r--r--   0        0        0     5881 2023-04-18 12:32:43.955607 oianalytics-0.5.2b6/oianalytics/api/utils.py
--rw-r--r--   0        0        0      133 2023-03-15 14:01:49.115833 oianalytics-0.5.2b6/oianalytics/models/__init__.py
--rw-r--r--   0        0        0    40900 2024-03-14 16:32:03.066552 oianalytics-0.5.2b6/oianalytics/models/_dtos.py
--rw-r--r--   0        0        0      346 2023-04-18 12:32:43.955722 oianalytics-0.5.2b6/oianalytics/models/_queries/__init__.py
--rw-r--r--   0        0        0     1965 2023-11-06 09:30:13.505992 oianalytics-0.5.2b6/oianalytics/models/_queries/files.py
--rw-r--r--   0        0        0      727 2023-11-06 09:30:13.506204 oianalytics-0.5.2b6/oianalytics/models/_queries/instances.py
--rw-r--r--   0        0        0    13883 2023-10-30 14:56:38.148516 oianalytics-0.5.2b6/oianalytics/models/_queries/single_observation.py
--rw-r--r--   0        0        0        0 2023-03-15 14:01:49.116471 oianalytics-0.5.2b6/oianalytics/models/_template_resources/__init__.py
--rw-r--r--   0        0        0     2796 2023-04-18 12:32:43.955950 oianalytics-0.5.2b6/oianalytics/models/_template_resources/file_processing_template.py
--rw-r--r--   0        0        0     3841 2023-03-15 14:01:49.116690 oianalytics-0.5.2b6/oianalytics/models/_template_resources/free_from_api_template.py
--rw-r--r--   0        0        0     2078 2023-03-15 14:01:49.116764 oianalytics-0.5.2b6/oianalytics/models/_template_resources/single_observation_template.py
--rw-r--r--   0        0        0    68166 2024-03-18 10:42:07.989496 oianalytics-0.5.2b6/oianalytics/models/outputs.py
--rw-r--r--   0        0        0      993 2023-11-06 09:30:13.506909 oianalytics-0.5.2b6/oianalytics/models/templates.py
--rw-r--r--   0        0        0      117 2023-03-15 14:01:49.117158 oianalytics-0.5.2b6/oianalytics/models/testing/__init__.py
--rw-r--r--   0        0        0    32133 2023-11-06 09:30:13.507306 oianalytics-0.5.2b6/oianalytics/models/testing/_mocking.py
--rw-r--r--   0        0        0     1067 2023-03-15 14:01:49.117460 oianalytics-0.5.2b6/oianalytics/models/testing/_tests_setup.py
--rw-r--r--   0        0        0     2811 2023-11-06 09:30:13.507566 oianalytics-0.5.2b6/oianalytics/models/testing/file_processing.py
--rw-r--r--   0        0        0     2669 2023-11-06 09:30:13.507835 oianalytics-0.5.2b6/oianalytics/models/testing/free_from_api.py
--rw-r--r--   0        0        0     7242 2023-11-06 09:30:13.508110 oianalytics-0.5.2b6/oianalytics/models/testing/single_observation.py
--rw-r--r--   0        0        0      256 2023-03-15 14:01:49.117791 oianalytics-0.5.2b6/oianalytics/models/utils.py
--rw-r--r--   0        0        0      471 2024-03-14 14:29:42.202229 oianalytics-0.5.2b6/pyproject.toml
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 oianalytics-0.5.2b6/PKG-INFO
+-rw-r--r--   0        0        0    13799 2023-03-15 14:01:49.113528 oianalytics-0.5.3/LICENSE
+-rw-r--r--   0        0        0       92 2024-04-11 08:26:37.003147 oianalytics-0.5.3/oianalytics/__init__.py
+-rw-r--r--   0        0        0      124 2024-02-12 10:28:03.022129 oianalytics-0.5.3/oianalytics/api/__init__.py
+-rw-r--r--   0        0        0     2373 2023-03-15 14:01:49.113932 oianalytics-0.5.3/oianalytics/api/_credentials.py
+-rw-r--r--   0        0        0     2442 2024-02-12 10:28:03.022426 oianalytics-0.5.3/oianalytics/api/_dataframes/__init__.py
+-rw-r--r--   0        0        0    16024 2023-11-06 09:30:13.500439 oianalytics-0.5.3/oianalytics/api/_dataframes/assets.py
+-rw-r--r--   0        0        0     3847 2023-11-06 09:30:13.500761 oianalytics-0.5.3/oianalytics/api/_dataframes/azure_blob_sources.py
+-rw-r--r--   0        0        0    48788 2024-02-12 10:28:03.022749 oianalytics-0.5.3/oianalytics/api/_dataframes/batches.py
+-rw-r--r--   0        0        0    41856 2023-10-30 14:56:38.145683 oianalytics-0.5.3/oianalytics/api/_dataframes/data.py
+-rw-r--r--   0        0        0     9979 2023-03-15 14:01:49.114785 oianalytics-0.5.3/oianalytics/api/_dataframes/events.py
+-rw-r--r--   0        0        0     4631 2023-03-15 14:01:49.114887 oianalytics-0.5.3/oianalytics/api/_dataframes/files.py
+-rw-r--r--   0        0        0     7991 2023-11-06 09:30:13.501670 oianalytics-0.5.3/oianalytics/api/_dataframes/model_instances.py
+-rw-r--r--   0        0        0     3933 2023-11-06 09:30:13.502064 oianalytics-0.5.3/oianalytics/api/_dataframes/profiles.py
+-rw-r--r--   0        0        0     2416 2023-10-30 14:56:38.146077 oianalytics-0.5.3/oianalytics/api/_dataframes/quantities.py
+-rw-r--r--   0        0        0     5581 2024-02-12 10:28:10.083841 oianalytics-0.5.3/oianalytics/api/_dataframes/tags.py
+-rw-r--r--   0        0        0     5463 2023-11-06 09:30:13.502604 oianalytics-0.5.3/oianalytics/api/_dataframes/units.py
+-rw-r--r--   0        0        0     4251 2023-11-06 09:30:13.502818 oianalytics-0.5.3/oianalytics/api/_dataframes/users.py
+-rw-r--r--   0        0        0      705 2024-04-11 08:26:37.003541 oianalytics-0.5.3/oianalytics/api/endpoints/__init__.py
+-rw-r--r--   0        0        0     5806 2024-02-12 10:28:03.023906 oianalytics-0.5.3/oianalytics/api/endpoints/assets.py
+-rw-r--r--   0        0        0     1437 2023-11-06 09:30:13.503405 oianalytics-0.5.3/oianalytics/api/endpoints/azure_blob_sources.py
+-rw-r--r--   0        0        0    11949 2024-02-12 10:28:03.024141 oianalytics-0.5.3/oianalytics/api/endpoints/batches.py
+-rw-r--r--   0        0        0     2646 2024-04-11 08:26:37.003805 oianalytics-0.5.3/oianalytics/api/endpoints/computation_jobs.py
+-rw-r--r--   0        0        0    13255 2023-11-06 09:30:13.503842 oianalytics-0.5.3/oianalytics/api/endpoints/data.py
+-rw-r--r--   0        0        0     2635 2023-11-06 09:30:13.504076 oianalytics-0.5.3/oianalytics/api/endpoints/events.py
+-rw-r--r--   0        0        0     3204 2023-11-06 09:30:13.504386 oianalytics-0.5.3/oianalytics/api/endpoints/files.py
+-rw-r--r--   0        0        0     1387 2023-11-06 09:30:13.504678 oianalytics-0.5.3/oianalytics/api/endpoints/model_instances.py
+-rw-r--r--   0        0        0     2779 2024-02-12 10:28:03.024389 oianalytics-0.5.3/oianalytics/api/endpoints/profiles.py
+-rw-r--r--   0        0        0      772 2023-10-30 14:56:38.147329 oianalytics-0.5.3/oianalytics/api/endpoints/quantities.py
+-rw-r--r--   0        0        0     4519 2024-02-12 10:28:10.090400 oianalytics-0.5.3/oianalytics/api/endpoints/tags.py
+-rw-r--r--   0        0        0     1787 2023-11-06 09:30:13.505426 oianalytics-0.5.3/oianalytics/api/endpoints/units.py
+-rw-r--r--   0        0        0     2170 2024-02-12 10:28:03.024745 oianalytics-0.5.3/oianalytics/api/endpoints/users.py
+-rw-r--r--   0        0        0     5881 2023-04-18 12:32:43.955607 oianalytics-0.5.3/oianalytics/api/utils.py
+-rw-r--r--   0        0        0      133 2023-03-15 14:01:49.115833 oianalytics-0.5.3/oianalytics/models/__init__.py
+-rw-r--r--   0        0        0    40900 2024-04-11 08:26:37.004294 oianalytics-0.5.3/oianalytics/models/_dtos.py
+-rw-r--r--   0        0        0      346 2023-04-18 12:32:43.955722 oianalytics-0.5.3/oianalytics/models/_queries/__init__.py
+-rw-r--r--   0        0        0     1965 2023-11-06 09:30:13.505992 oianalytics-0.5.3/oianalytics/models/_queries/files.py
+-rw-r--r--   0        0        0      727 2023-11-06 09:30:13.506204 oianalytics-0.5.3/oianalytics/models/_queries/instances.py
+-rw-r--r--   0        0        0    13883 2023-10-30 14:56:38.148516 oianalytics-0.5.3/oianalytics/models/_queries/single_observation.py
+-rw-r--r--   0        0        0        0 2023-03-15 14:01:49.116471 oianalytics-0.5.3/oianalytics/models/_template_resources/__init__.py
+-rw-r--r--   0        0        0     2796 2023-04-18 12:32:43.955950 oianalytics-0.5.3/oianalytics/models/_template_resources/file_processing_template.py
+-rw-r--r--   0        0        0     3841 2023-03-15 14:01:49.116690 oianalytics-0.5.3/oianalytics/models/_template_resources/free_from_api_template.py
+-rw-r--r--   0        0        0     2078 2023-03-15 14:01:49.116764 oianalytics-0.5.3/oianalytics/models/_template_resources/single_observation_template.py
+-rw-r--r--   0        0        0    68166 2024-04-11 08:26:37.004822 oianalytics-0.5.3/oianalytics/models/outputs.py
+-rw-r--r--   0        0        0      993 2023-11-06 09:30:13.506909 oianalytics-0.5.3/oianalytics/models/templates.py
+-rw-r--r--   0        0        0      117 2023-03-15 14:01:49.117158 oianalytics-0.5.3/oianalytics/models/testing/__init__.py
+-rw-r--r--   0        0        0    32133 2023-11-06 09:30:13.507306 oianalytics-0.5.3/oianalytics/models/testing/_mocking.py
+-rw-r--r--   0        0        0     1067 2023-03-15 14:01:49.117460 oianalytics-0.5.3/oianalytics/models/testing/_tests_setup.py
+-rw-r--r--   0        0        0     2811 2023-11-06 09:30:13.507566 oianalytics-0.5.3/oianalytics/models/testing/file_processing.py
+-rw-r--r--   0        0        0     2710 2024-04-11 08:26:37.005487 oianalytics-0.5.3/oianalytics/models/testing/free_from_api.py
+-rw-r--r--   0        0        0     7242 2023-11-06 09:30:13.508110 oianalytics-0.5.3/oianalytics/models/testing/single_observation.py
+-rw-r--r--   0        0        0      256 2023-03-15 14:01:49.117791 oianalytics-0.5.3/oianalytics/models/utils.py
+-rw-r--r--   0        0        0      475 2024-04-11 08:31:53.204621 oianalytics-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 oianalytics-0.5.3/PKG-INFO
```

### Comparing `oianalytics-0.5.2b6/LICENSE` & `oianalytics-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_credentials.py` & `oianalytics-0.5.3/oianalytics/api/_credentials.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/__init__.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/assets.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/assets.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/azure_blob_sources.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/azure_blob_sources.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/batches.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/batches.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/data.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/data.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/events.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/events.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/files.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/files.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/model_instances.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/model_instances.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/profiles.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/profiles.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/quantities.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/quantities.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/tags.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/tags.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/units.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/units.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/_dataframes/users.py` & `oianalytics-0.5.3/oianalytics/api/_dataframes/users.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/__init__.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/assets.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/azure_blob_sources.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/azure_blob_sources.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/batches.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/batches.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/computation_jobs.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/computation_jobs.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/data.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/events.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/files.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/model_instances.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/model_instances.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/profiles.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/profiles.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/quantities.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/quantities.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/tags.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/tags.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/units.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/units.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/endpoints/users.py` & `oianalytics-0.5.3/oianalytics/api/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/api/utils.py` & `oianalytics-0.5.3/oianalytics/api/utils.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/_dtos.py` & `oianalytics-0.5.3/oianalytics/models/_dtos.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/_queries/files.py` & `oianalytics-0.5.3/oianalytics/models/_queries/files.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/_queries/instances.py` & `oianalytics-0.5.3/oianalytics/models/_queries/instances.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/_queries/single_observation.py` & `oianalytics-0.5.3/oianalytics/models/_queries/single_observation.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/_template_resources/file_processing_template.py` & `oianalytics-0.5.3/oianalytics/models/_template_resources/file_processing_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/_template_resources/free_from_api_template.py` & `oianalytics-0.5.3/oianalytics/models/_template_resources/free_from_api_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/_template_resources/single_observation_template.py` & `oianalytics-0.5.3/oianalytics/models/_template_resources/single_observation_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/outputs.py` & `oianalytics-0.5.3/oianalytics/models/outputs.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/templates.py` & `oianalytics-0.5.3/oianalytics/models/templates.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/testing/_mocking.py` & `oianalytics-0.5.3/oianalytics/models/testing/_mocking.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/testing/_tests_setup.py` & `oianalytics-0.5.3/oianalytics/models/testing/_tests_setup.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/testing/file_processing.py` & `oianalytics-0.5.3/oianalytics/models/testing/file_processing.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/oianalytics/models/testing/free_from_api.py` & `oianalytics-0.5.3/oianalytics/models/testing/free_from_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             outputs.OIModelOutputs,
             outputs.FileOutput,
             outputs.TimeValuesOutput,
             outputs.VectorTimeValuesOutput,
             outputs.BatchValuesOutput,
             outputs.VectorBatchValuesOutput,
             outputs.BatchFeaturesOutput,
+            outputs.BatchComputationJob,
             outputs.CustomJsonOutput,
             outputs.CustomTextOutput,
             outputs.Delay,
         ),
     ):
         print(
             "Warning: the model output should be an instance of an output class from oianalytics.models.outputs"
```

### Comparing `oianalytics-0.5.2b6/oianalytics/models/testing/single_observation.py` & `oianalytics-0.5.3/oianalytics/models/testing/single_observation.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b6/PKG-INFO` & `oianalytics-0.5.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: oianalytics
-Version: 0.5.2b6
+Version: 0.5.3
 Summary: Python tools for working with OIAnalytics
 License: EUPL-1.2
 Author: Optimistik SAS
 Author-email: arthur.martel@optimistik.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=1.3.4,<2.0.0)
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
-Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: pandas (>=1.3.4)
+Requires-Dist: pydantic (>=1.9.0)
+Requires-Dist: requests (>=2.26.0)
```

