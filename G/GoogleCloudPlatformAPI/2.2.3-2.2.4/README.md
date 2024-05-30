# Comparing `tmp/GoogleCloudPlatformAPI-2.2.3.tar.gz` & `tmp/googlecloudplatformapi-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleCloudPlatformAPI-2.2.3.tar", last modified: Thu Feb 15 12:00:20 2024, max compression
+gzip compressed data, was "googlecloudplatformapi-2.2.4.tar", last modified: Thu May 30 15:05:01 2024, max compression
```

## Comparing `GoogleCloudPlatformAPI-2.2.3.tar` & `googlecloudplatformapi-2.2.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:00:20.035908 GoogleCloudPlatformAPI-2.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:00:20.035908 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/
--rw-r--r--   0 runner    (1001) docker     (127)    35826 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/AdManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/Analytics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22712 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/BigQuery.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7227 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/CloudStorage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2641 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/ServiceAccount.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2276 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:00:20.035908 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-15 12:00:20.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-15 12:00:20.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 12:00:20.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-15 12:00:20.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-15 12:00:20.000000 GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-15 12:00:20.035908 GoogleCloudPlatformAPI-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 12:00:20.035908 GoogleCloudPlatformAPI-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-15 12:00:09.000000 GoogleCloudPlatformAPI-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:05:01.191957 googlecloudplatformapi-2.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:05:01.187957 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)    35674 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/AdManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/Analytics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22712 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/BigQuery.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7227 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/CloudStorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2641 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/ServiceAccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2276 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:05:01.187957 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 15:05:01.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-30 15:05:01.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:05:01.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 15:05:01.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:05:01.000000 googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 15:05:01.187957 googlecloudplatformapi-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-30 15:04:56.000000 googlecloudplatformapi-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:05:01.191957 googlecloudplatformapi-2.2.4/setup.cfg
```

### Comparing `GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/AdManager.py` & `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/AdManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
            'TOTAL_LINE_ITEM_LEVEL_IMPRESSIONS',
            'TOTAL_LINE_ITEM_LEVEL_CPM_AND_CPC_REVENUE']
 
 DIMENSIONS = ['DATE', 'AD_UNIT_NAME', 'CUSTOM_TARGETING_VALUE_ID']
 
 GAM_VERSION = "v202305"
 NETWORK_CODE = '5574'
-APP_NAME = 'AdManager'
+APP_NAME = 'AdManagerAPIClient'
 
 # region objects
 gam_adUnit = Dict[int, bool]
 
 gam_adUnits = List[gam_adUnit]
 gam_targetingValues = List[int]
 logical_operator = Literal["AND", "OR"]
@@ -393,16 +393,14 @@
 
     def __init__(self,
                  app_name: str = APP_NAME,
                  network_code:  str = NETWORK_CODE,
                  gam_version: str = GAM_VERSION):
         gam_client = GamClient(app_name=app_name,
                                network_code=network_code)
-        self.__gam_service = gam_client.get_service(service_name=self.service_name,
-                                                    gam_version=gam_version)
         self.data_downloader = gam_client.get_data_downloader(
             gam_version=gam_version)
 
     def __get_report_by_report_job(self, report_job):
 
         logging.debug('Report::___get_report_by_report_job')
         # Initialize a DataDownloader.
@@ -469,15 +467,15 @@
                            .Offset(None))
 
         return built_statement
 
     @ staticmethod
     def gen_report_query(report_statement,
                          report_end: datetime.date = datetime.date.today(),
-                         report_days: int = 7,
+                         report_days: int = 1,
                          dimensions: List[str] = DIMENSIONS,
                          metrics: List[str] = METRICS,
                          ad_unit_view: str = AD_UNIT_VIEW):
         logging.debug('api_build_report_query')
 
         start_date = report_end - datetime.timedelta(days=report_days)
 
@@ -520,15 +518,15 @@
             data_frame['ad_unit_id_5'] = '-'
         return data_frame.reindex(sorted(data_frame.columns), axis=1)
 
     def get_report_dataframe(self,
                              ad_units: Optional[Union[int, List[int]]] = None,
                              targeting_value_ids: Optional[gam_targetingValues] = None,
                              report_date: datetime.date = datetime.date.today(),
-                             days: int = 7,
+                             days: int = 1,
                              dimensions: List[str] = DIMENSIONS,
                              metrics: List[str] = METRICS,
                              ad_unit_view: str = AD_UNIT_VIEW) -> pd.DataFrame:
         if type(ad_units) == int:
             ad_units = [ad_units]
         statement = self.gen_report_statement(
             ad_units=ad_units, targeting_value_ids=targeting_value_ids)
@@ -539,15 +537,15 @@
                                                     metrics=metrics,
                                                     ad_unit_view=ad_unit_view)
         return df
 
     def get_report_dataframe_by_statement(self,
                                           statement,
                                           report_date: datetime.date = datetime.date.today(),
-                                          days: int = 7,
+                                          days: int = 1,
                                           dimensions: List[str] = DIMENSIONS,
                                           metrics: List[str] = METRICS,
                                           ad_unit_view: str = AD_UNIT_VIEW) -> pd.DataFrame:
         report_job = self.gen_report_query(statement,
                                            report_date,
                                            days,
                                            dimensions,
```

### Comparing `GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/Analytics.py` & `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/Analytics.py`

 * *Files identical despite different names*

### Comparing `GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/BigQuery.py` & `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/BigQuery.py`

 * *Files identical despite different names*

### Comparing `GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/CloudStorage.py` & `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/ServiceAccount.py` & `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/ServiceAccount.py`

 * *Files identical despite different names*

### Comparing `GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI/Utils.py` & `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI/Utils.py`

 * *Files identical despite different names*

### Comparing `GoogleCloudPlatformAPI-2.2.3/GoogleCloudPlatformAPI.egg-info/SOURCES.txt` & `googlecloudplatformapi-2.2.4/GoogleCloudPlatformAPI.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 GoogleCloudPlatformAPI/AdManager.py
 GoogleCloudPlatformAPI/Analytics.py
 GoogleCloudPlatformAPI/BigQuery.py
 GoogleCloudPlatformAPI/CloudStorage.py
 GoogleCloudPlatformAPI/ServiceAccount.py
 GoogleCloudPlatformAPI/Utils.py
 GoogleCloudPlatformAPI/__init__.py
```

### Comparing `GoogleCloudPlatformAPI-2.2.3/LICENSE` & `googlecloudplatformapi-2.2.4/LICENSE`

 * *Files identical despite different names*

