# Comparing `tmp/slurpit_netbox-0.8.46.tar.gz` & `tmp/slurpit_netbox-0.8.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpit_netbox-0.8.46.tar", max compression
+gzip compressed data, was "slurpit_netbox-0.8.63.tar", max compression
```

## Comparing `slurpit_netbox-0.8.46.tar` & `slurpit_netbox-0.8.63.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0     1064 2024-02-05 14:18:19.675269 slurpit_netbox-0.8.46/LICENSE
--rw-r--r--   0        0        0      956 2024-02-05 14:18:19.675269 slurpit_netbox-0.8.46/README.md
--rw-r--r--   0        0        0      499 2024-02-05 16:34:52.592416 slurpit_netbox-0.8.46/pyproject.toml
--rw-r--r--   0        0        0     1281 2024-02-05 16:34:52.592416 slurpit_netbox-0.8.46/src/slurpit_netbox/__init__.py
--rw-r--r--   0        0        0       46 2024-01-10 18:02:33.255412 slurpit_netbox-0.8.46/src/slurpit_netbox/api/__init__.py
--rw-r--r--   0        0        0     1805 2024-01-30 07:22:17.014693 slurpit_netbox-0.8.46/src/slurpit_netbox/api/serializers.py
--rw-r--r--   0        0        0      459 2024-02-05 15:45:00.314212 slurpit_netbox-0.8.46/src/slurpit_netbox/api/urls.py
--rw-r--r--   0        0        0     8716 2024-02-05 15:45:00.314212 slurpit_netbox-0.8.46/src/slurpit_netbox/api/views.py
--rw-r--r--   0        0        0     2528 2024-01-28 21:08:09.602468 slurpit_netbox-0.8.46/src/slurpit_netbox/decorators.py
--rw-r--r--   0        0        0     2107 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.46/src/slurpit_netbox/filtersets.py
--rw-r--r--   0        0        0     6543 2024-02-05 15:45:00.314212 slurpit_netbox-0.8.46/src/slurpit_netbox/forms.py
--rw-r--r--   0        0        0    11378 2024-02-06 10:30:03.586076 slurpit_netbox-0.8.46/src/slurpit_netbox/importer.py
--rw-r--r--   0        0        0        0 2024-02-06 16:48:55.848790 slurpit_netbox-0.8.46/src/slurpit_netbox/management/__init__.py
--rw-r--r--   0        0        0     1223 2024-02-05 15:45:00.314212 slurpit_netbox-0.8.46/src/slurpit_netbox/management/choices.py
--rw-r--r--   0        0        0     7223 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.46/src/slurpit_netbox/migrations/0001_initial.py
--rw-r--r--   0        0        0      574 2024-01-27 14:54:44.310903 slurpit_netbox-0.8.46/src/slurpit_netbox/migrations/0002_alter_slurpitplanning_name_and_more.py
--rw-r--r--   0        0        0      609 2024-01-27 22:08:44.267940 slurpit_netbox-0.8.46/src/slurpit_netbox/migrations/0003_alter_slurpitimporteddevice_ipv4_and_more.py
--rw-r--r--   0        0        0     1195 2024-01-30 07:22:17.014693 slurpit_netbox-0.8.46/src/slurpit_netbox/migrations/0004_slurpitmapping.py
--rw-r--r--   0        0        0        0 2024-02-06 16:48:55.848790 slurpit_netbox-0.8.46/src/slurpit_netbox/migrations/__init__.py
--rw-r--r--   0        0        0     4612 2024-02-05 15:45:00.314212 slurpit_netbox-0.8.46/src/slurpit_netbox/models/__init__.py
--rw-r--r--   0        0        0     2496 2024-01-29 22:12:05.111124 slurpit_netbox-0.8.46/src/slurpit_netbox/models/device.py
--rw-r--r--   0        0        0     1530 2024-01-24 10:31:25.575355 slurpit_netbox-0.8.46/src/slurpit_netbox/models/logs.py
--rw-r--r--   0        0        0      281 2024-01-30 07:22:17.014693 slurpit_netbox-0.8.46/src/slurpit_netbox/models/mapping.py
--rw-r--r--   0        0        0      709 2024-01-27 14:54:44.310903 slurpit_netbox-0.8.46/src/slurpit_netbox/models/planning.py
--rw-r--r--   0        0        0     1138 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.46/src/slurpit_netbox/models/setting.py
--rw-r--r--   0        0        0     1693 2024-01-23 14:56:31.506780 slurpit_netbox-0.8.46/src/slurpit_netbox/navigation.py
--rw-r--r--   0        0        0      268 2024-01-23 21:13:22.330062 slurpit_netbox-0.8.46/src/slurpit_netbox/search.py
--rw-r--r--   0        0        0      528 2023-12-11 21:28:49.339333 slurpit_netbox-0.8.46/src/slurpit_netbox/slurpitch.py
--rw-r--r--   0        0        0     4637 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.46/src/slurpit_netbox/tables.py
--rw-r--r--   0        0        0      326 2024-01-23 21:13:22.330062 slurpit_netbox-0.8.46/src/slurpit_netbox/template_content.py
--rw-r--r--   0        0        0     4849 2023-12-28 16:41:37.982711 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/bulk_edit.html
--rw-r--r--   0        0        0     1588 2024-01-23 21:13:22.330062 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/comingsoon.html
--rw-r--r--   0        0        0     2759 2024-02-05 15:45:00.318212 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/data_mapping.html
--rw-r--r--   0        0        0    21670 2023-12-27 09:11:50.918673 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/logo.html
--rw-r--r--   0        0        0    14338 2024-02-06 07:53:46.462658 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/mapping/netbox_to_slurpit.html
--rw-r--r--   0        0        0     3519 2024-01-27 14:47:32.984336 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/onboard/conflict_device_list.html
--rw-r--r--   0        0        0     3518 2024-01-27 14:42:23.690498 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/onboard/migrate_device_list.html
--rw-r--r--   0        0        0     5645 2024-02-05 15:45:00.318212 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/onboard/new_device_list.html
--rw-r--r--   0        0        0     1561 2023-12-12 12:17:55.376088 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/onboard/onboarded_device_list.html
--rw-r--r--   0        0        0     3139 2024-01-24 16:17:49.444492 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/onboard_device.html
--rw-r--r--   0        0        0     3864 2024-02-05 15:45:00.318212 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/planning_table.html
--rw-r--r--   0        0        0     3099 2024-01-23 14:56:31.506780 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/settings/data_tabs.html
--rw-r--r--   0        0        0     8607 2024-01-30 15:53:27.126783 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/settings/general.html
--rw-r--r--   0        0        0     2323 2024-01-27 14:42:23.690498 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/settings.html
--rw-r--r--   0        0        0     1813 2024-02-05 15:45:00.318212 slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/slurpitlog_list.html
--rw-r--r--   0        0        0      950 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.46/src/slurpit_netbox/urls.py
--rw-r--r--   0        0        0      459 2024-01-04 13:14:53.399355 slurpit_netbox-0.8.46/src/slurpit_netbox/utilities.py
--rw-r--r--   0        0        0     1400 2024-01-23 21:13:22.334062 slurpit_netbox-0.8.46/src/slurpit_netbox/validator.py
--rw-r--r--   0        0        0      252 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.46/src/slurpit_netbox/views/__init__.py
--rw-r--r--   0        0        0     9255 2024-02-06 10:30:03.586076 slurpit_netbox-0.8.46/src/slurpit_netbox/views/datamapping.py
--rw-r--r--   0        0        0     1006 2024-02-05 15:45:00.318212 slurpit_netbox-0.8.46/src/slurpit_netbox/views/logging.py
--rw-r--r--   0        0        0    14382 2024-02-05 16:34:52.592416 slurpit_netbox-0.8.46/src/slurpit_netbox/views/onboarding.py
--rw-r--r--   0        0        0      487 2024-01-23 21:13:22.334062 slurpit_netbox-0.8.46/src/slurpit_netbox/views/reconcile.py
--rw-r--r--   0        0        0    17333 2024-02-06 10:30:03.586076 slurpit_netbox-0.8.46/src/slurpit_netbox/views/setting.py
--rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 slurpit_netbox-0.8.46/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-02-05 14:18:19.675269 slurpit_netbox-0.8.63/LICENSE
+-rw-r--r--   0        0        0      956 2024-02-05 14:18:19.675269 slurpit_netbox-0.8.63/README.md
+-rw-r--r--   0        0        0      499 2024-02-09 12:29:33.576704 slurpit_netbox-0.8.63/pyproject.toml
+-rw-r--r--   0        0        0     1281 2024-02-08 16:53:29.564978 slurpit_netbox-0.8.63/src/slurpit_netbox/__init__.py
+-rw-r--r--   0        0        0       46 2024-01-10 18:02:33.255412 slurpit_netbox-0.8.63/src/slurpit_netbox/api/__init__.py
+-rw-r--r--   0        0        0     1805 2024-01-30 07:22:17.014693 slurpit_netbox-0.8.63/src/slurpit_netbox/api/serializers.py
+-rw-r--r--   0        0        0      459 2024-02-05 15:45:00.314212 slurpit_netbox-0.8.63/src/slurpit_netbox/api/urls.py
+-rw-r--r--   0        0        0     8716 2024-02-05 15:45:00.314212 slurpit_netbox-0.8.63/src/slurpit_netbox/api/views.py
+-rw-r--r--   0        0        0     2528 2024-01-28 21:08:09.602468 slurpit_netbox-0.8.63/src/slurpit_netbox/decorators.py
+-rw-r--r--   0        0        0     2107 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.63/src/slurpit_netbox/filtersets.py
+-rw-r--r--   0        0        0     6543 2024-02-05 15:45:00.314212 slurpit_netbox-0.8.63/src/slurpit_netbox/forms.py
+-rw-r--r--   0        0        0    11378 2024-02-06 10:30:03.586076 slurpit_netbox-0.8.63/src/slurpit_netbox/importer.py
+-rw-r--r--   0        0        0        0 2024-02-09 12:29:33.628704 slurpit_netbox-0.8.63/src/slurpit_netbox/management/__init__.py
+-rw-r--r--   0        0        0     1223 2024-02-05 15:45:00.314212 slurpit_netbox-0.8.63/src/slurpit_netbox/management/choices.py
+-rw-r--r--   0        0        0     7223 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.63/src/slurpit_netbox/migrations/0001_initial.py
+-rw-r--r--   0        0        0      574 2024-01-27 14:54:44.310903 slurpit_netbox-0.8.63/src/slurpit_netbox/migrations/0002_alter_slurpitplanning_name_and_more.py
+-rw-r--r--   0        0        0      609 2024-01-27 22:08:44.267940 slurpit_netbox-0.8.63/src/slurpit_netbox/migrations/0003_alter_slurpitimporteddevice_ipv4_and_more.py
+-rw-r--r--   0        0        0     1195 2024-01-30 07:22:17.014693 slurpit_netbox-0.8.63/src/slurpit_netbox/migrations/0004_slurpitmapping.py
+-rw-r--r--   0        0        0        0 2024-02-09 12:29:33.628704 slurpit_netbox-0.8.63/src/slurpit_netbox/migrations/__init__.py
+-rw-r--r--   0        0        0     5017 2024-02-08 17:13:52.564318 slurpit_netbox-0.8.63/src/slurpit_netbox/models/__init__.py
+-rw-r--r--   0        0        0     2496 2024-01-29 22:12:05.111124 slurpit_netbox-0.8.63/src/slurpit_netbox/models/device.py
+-rw-r--r--   0        0        0     1530 2024-01-24 10:31:25.575355 slurpit_netbox-0.8.63/src/slurpit_netbox/models/logs.py
+-rw-r--r--   0        0        0      281 2024-01-30 07:22:17.014693 slurpit_netbox-0.8.63/src/slurpit_netbox/models/mapping.py
+-rw-r--r--   0        0        0      709 2024-01-27 14:54:44.310903 slurpit_netbox-0.8.63/src/slurpit_netbox/models/planning.py
+-rw-r--r--   0        0        0     1138 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.63/src/slurpit_netbox/models/setting.py
+-rw-r--r--   0        0        0     1693 2024-01-23 14:56:31.506780 slurpit_netbox-0.8.63/src/slurpit_netbox/navigation.py
+-rw-r--r--   0        0        0      268 2024-01-23 21:13:22.330062 slurpit_netbox-0.8.63/src/slurpit_netbox/search.py
+-rw-r--r--   0        0        0      528 2023-12-11 21:28:49.339333 slurpit_netbox-0.8.63/src/slurpit_netbox/slurpitch.py
+-rw-r--r--   0        0        0     4637 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.63/src/slurpit_netbox/tables.py
+-rw-r--r--   0        0        0      326 2024-01-23 21:13:22.330062 slurpit_netbox-0.8.63/src/slurpit_netbox/template_content.py
+-rw-r--r--   0        0        0     4849 2023-12-28 16:41:37.982711 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/bulk_edit.html
+-rw-r--r--   0        0        0     1588 2024-01-23 21:13:22.330062 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/comingsoon.html
+-rw-r--r--   0        0        0     2482 2024-02-08 17:13:52.564318 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/data_mapping.html
+-rw-r--r--   0        0        0    21670 2023-12-27 09:11:50.918673 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/logo.html
+-rw-r--r--   0        0        0      342 2024-02-08 17:13:52.568318 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/mapping/commingsoon.html
+-rw-r--r--   0        0        0    15815 2024-02-08 17:13:52.568318 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/mapping/netbox_to_slurpit.html
+-rw-r--r--   0        0        0     3519 2024-01-27 14:47:32.984336 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/onboard/conflict_device_list.html
+-rw-r--r--   0        0        0     3518 2024-01-27 14:42:23.690498 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/onboard/migrate_device_list.html
+-rw-r--r--   0        0        0     5645 2024-02-05 15:45:00.318212 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/onboard/new_device_list.html
+-rw-r--r--   0        0        0     1561 2023-12-12 12:17:55.376088 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/onboard/onboarded_device_list.html
+-rw-r--r--   0        0        0     3139 2024-01-24 16:17:49.444492 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/onboard_device.html
+-rw-r--r--   0        0        0     3863 2024-02-08 17:13:52.568318 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/planning_table.html
+-rw-r--r--   0        0        0     3099 2024-01-23 14:56:31.506780 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/settings/data_tabs.html
+-rw-r--r--   0        0        0     8607 2024-01-30 15:53:27.126783 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/settings/general.html
+-rw-r--r--   0        0        0     2323 2024-01-27 14:42:23.690498 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/settings.html
+-rw-r--r--   0        0        0     1813 2024-02-05 15:45:00.318212 slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/slurpitlog_list.html
+-rw-r--r--   0        0        0      950 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.63/src/slurpit_netbox/urls.py
+-rw-r--r--   0        0        0      459 2024-01-04 13:14:53.399355 slurpit_netbox-0.8.63/src/slurpit_netbox/utilities.py
+-rw-r--r--   0        0        0     1400 2024-01-23 21:13:22.334062 slurpit_netbox-0.8.63/src/slurpit_netbox/validator.py
+-rw-r--r--   0        0        0      252 2024-01-25 15:56:28.843525 slurpit_netbox-0.8.63/src/slurpit_netbox/views/__init__.py
+-rw-r--r--   0        0        0     9633 2024-02-08 17:13:52.568318 slurpit_netbox-0.8.63/src/slurpit_netbox/views/datamapping.py
+-rw-r--r--   0        0        0     1006 2024-02-05 15:45:00.318212 slurpit_netbox-0.8.63/src/slurpit_netbox/views/logging.py
+-rw-r--r--   0        0        0    14382 2024-02-05 16:34:52.592416 slurpit_netbox-0.8.63/src/slurpit_netbox/views/onboarding.py
+-rw-r--r--   0        0        0      487 2024-01-23 21:13:22.334062 slurpit_netbox-0.8.63/src/slurpit_netbox/views/reconcile.py
+-rw-r--r--   0        0        0    17459 2024-02-08 17:13:52.568318 slurpit_netbox-0.8.63/src/slurpit_netbox/views/setting.py
+-rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 slurpit_netbox-0.8.63/PKG-INFO
```

### Comparing `slurpit_netbox-0.8.46/LICENSE` & `slurpit_netbox-0.8.63/LICENSE`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/README.md` & `slurpit_netbox-0.8.63/README.md`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/__init__.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.db.models.signals import post_migrate
 from extras.plugins import PluginConfig, get_plugin_config
 
 class SlurpitConfig(PluginConfig):
     name = "slurpit_netbox"
     verbose_name = "Slurp'it Plugin"
     description = "Sync Slurp'it into NetBox"
-    version = '0.8.46'
+    version = '0.8.63'
     base_url = "slurpit"   
     default_settings = {
         'DeviceType': {'model': "Slurp'it", 'slug': 'slurpit'},
         'DeviceRole': {'name': "Slurp'it", 'slug': 'slurpit'},
         'Site': {'name': "Slurp'it", 'slug': 'slurpit'},
         'Location': {'name': 'Slurp\'it', 'slug': 'slurpit'},
         'Region': {'name': 'Slurp\'it', 'slug': 'slurpit'},
```

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/api/serializers.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/api/serializers.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/api/views.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/api/views.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/decorators.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/decorators.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/filtersets.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/filtersets.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/forms.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/forms.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/importer.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/importer.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/management/choices.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/management/choices.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/migrations/0001_initial.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/migrations/0002_alter_slurpitplanning_name_and_more.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/migrations/0002_alter_slurpitplanning_name_and_more.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/migrations/0003_alter_slurpitimporteddevice_ipv4_and_more.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/migrations/0003_alter_slurpitimporteddevice_ipv4_and_more.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/migrations/0004_slurpitmapping.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/migrations/0004_slurpitmapping.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/models/__init__.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dcim.models import DeviceRole, DeviceType, Manufacturer, Site, Location, Region, SiteGroup, Rack
 from django.contrib.contenttypes.models import ContentType
 from extras.choices import CustomFieldTypeChoices
 from extras.models import CustomField, CustomFieldChoiceSet, ConfigTemplate
 from extras.models.tags import Tag
+from django.db.models import Q
 
 from .. import get_config
 from .device import SlurpitImportedDevice, SlurpitStagedDevice
 from .planning import SlurpitPlanning, SlurpitSnapshot
 from .setting import SlurpitSetting
 from .logs import SlurpitLog
 from .mapping import SlurpitMapping
@@ -15,89 +16,93 @@
     'SlurpitImportedDevice', 'SlurpitStagedDevice',
     'post_migration', 'SlurpitLog', 'SlurpitSetting'
 ]
 
 def ensure_slurpit_tags(*items):
     if (tags := getattr(ensure_slurpit_tags, 'cache', None)) is None:
         name = 'slurpit'
-        tag, _ = Tag.objects.get_or_create(name=name, slug=name, description='Slurp\'it onboarded', color='F09640')
+        tag, _ = Tag.objects.get_or_create(name=name, defaults={'slug':name, 'description':'Slurp\'it onboarded', 'color': 'F09640'})
 
-        applicable_to = 'device', 'devicerole', 'devicetype', 'manufacturer', 'site'
-        tagged_types = ContentType.objects.filter(app_label='dcim',
-                                                  model__in=applicable_to)
+        dcim_applicable_to = 'device', 'devicerole', 'devicetype', 'manufacturer', 'site'
+        ipam_applicable = 'iprange'
+
+        dcim_Q = Q(app_label='dcim', model__in=dcim_applicable_to)
+        ipam_Q = Q(app_label='ipam', model=ipam_applicable)
+        tagged_types = ContentType.objects.filter(ipam_Q | dcim_Q)
         tag.object_types.set(tagged_types.all())
         tags = {tag}
         ensure_slurpit_tags.cache = tags
     for item in items:
         item.tags.set(tags)
     return tags
 
 def create_custom_fields():   
     device = ContentType.objects.get(app_label='dcim', model='device')
-    
-    cf, _ = CustomField.objects.get_or_create(
-                name='slurpit_hostname',               
-                type=CustomFieldTypeChoices.TYPE_TEXT,
-                description="",
-                is_cloneable=True,
-                label='Hostname',
-                group_name="Slurp'it",
-        )
-    cf.content_types.set({device})
-
-    cf, _ = CustomField.objects.get_or_create(
-                name='slurpit_fqdn',           
-                type=CustomFieldTypeChoices.TYPE_TEXT,
-                description="",
-                is_cloneable=True,
-                label='Fqdn',
-                group_name="Slurp'it",
-                )
-    cf.content_types.set({device})
+    try:
+        cf, _ = CustomField.objects.get_or_create(
+                    name='slurpit_hostname',               
+                    type=CustomFieldTypeChoices.TYPE_TEXT,
+                    description="",
+                    is_cloneable=True,
+                    label='Hostname',
+                    group_name="Slurp'it",
+            )
+        cf.content_types.set({device})
+
+        cf, _ = CustomField.objects.get_or_create(
+                    name='slurpit_fqdn',           
+                    type=CustomFieldTypeChoices.TYPE_TEXT,
+                    description="",
+                    is_cloneable=True,
+                    label='Fqdn',
+                    group_name="Slurp'it",
+                    )
+        cf.content_types.set({device})
+            
+        cf, _ = CustomField.objects.get_or_create(
+                    name='slurpit_platform',
+                    type=CustomFieldTypeChoices.TYPE_TEXT,
+                    description="",
+                    is_cloneable=True,
+                    label='Platform',
+                    group_name="Slurp'it",
+                    )
+        cf.content_types.set({device})
+
+        cf, _ = CustomField.objects.get_or_create(
+                    name='slurpit_manufactor', 
+                    type=CustomFieldTypeChoices.TYPE_TEXT,
+                    description="",
+                    is_cloneable=True,
+                    label='Manufactor',
+                    group_name="Slurp'it",
+                    )
+        cf.content_types.set({device})
         
-    cf, _ = CustomField.objects.get_or_create(
-                name='slurpit_platform',
-                type=CustomFieldTypeChoices.TYPE_TEXT,
-                description="",
-                is_cloneable=True,
-                label='Platform',
-                group_name="Slurp'it",
-                )
-    cf.content_types.set({device})
-
-    cf, _ = CustomField.objects.get_or_create(
-                name='slurpit_manufactor', 
-                type=CustomFieldTypeChoices.TYPE_TEXT,
-                description="",
-                is_cloneable=True,
-                label='Manufactor',
-                group_name="Slurp'it",
-                )
-    cf.content_types.set({device})
-    
-    cf, _ = CustomField.objects.get_or_create(
-                name='slurpit_devicetype',
-                type=CustomFieldTypeChoices.TYPE_TEXT,
-                description="",
-                is_cloneable=True,
-                label='Device Type',
-                group_name="Slurp'it",
-                )
-    cf.content_types.set({device})
-    
-    cf, _ = CustomField.objects.get_or_create(
-                name='slurpit_ipv4',
-                type=CustomFieldTypeChoices.TYPE_TEXT,
-                description="",
-                is_cloneable=True,
-                label='Ipv4',
-                group_name="Slurp'it",
-                )
-    cf.content_types.set({device})
-
+        cf, _ = CustomField.objects.get_or_create(
+                    name='slurpit_devicetype',
+                    type=CustomFieldTypeChoices.TYPE_TEXT,
+                    description="",
+                    is_cloneable=True,
+                    label='Device Type',
+                    group_name="Slurp'it",
+                    )
+        cf.content_types.set({device})
+        
+        cf, _ = CustomField.objects.get_or_create(
+                    name='slurpit_ipv4',
+                    type=CustomFieldTypeChoices.TYPE_TEXT,
+                    description="",
+                    is_cloneable=True,
+                    label='Ipv4',
+                    group_name="Slurp'it",
+                    )
+        cf.content_types.set({device})
+    except:
+        pass
 
 
 def add_default_mandatory_objects(tags):
     site, _ = Site.objects.get_or_create(**get_config('Site'))
     site.tags.set(tags)
 
     manu, _ = Manufacturer.objects.get_or_create(**get_config('Manufacturer'))
@@ -115,14 +120,14 @@
         {"source_field": "hostname", "target_field": "device|name"},
         {"source_field": "fqdn", "target_field": "device|primary_ip4"},
         {"source_field": "ipv4", "target_field": "device|primary_ip4"},
         {"source_field": "device_os", "target_field": "device|platform"},
         {"source_field": "device_type", "target_field": "device|device_type"},
     ]
     for mapping in mappings:
-        SlurpitMapping.objects.create(**mapping)
+        SlurpitMapping.objects.get_or_create(**mapping)
 
 
 def post_migration(sender, **kwargs):
     create_custom_fields()
     tags = ensure_slurpit_tags()
     add_default_mandatory_objects(tags)
```

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/models/device.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/models/device.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/models/logs.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/models/logs.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/models/planning.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/models/planning.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/models/setting.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/models/setting.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/navigation.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/navigation.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/slurpitch.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/slurpitch.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/tables.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/tables.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/bulk_edit.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/bulk_edit.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/comingsoon.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/comingsoon.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/data_mapping.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/data_mapping.html`

 * *Files 6% similar despite different names*

```diff
@@ -62,112 +62,95 @@
 000003d0: 2027 736c 7572 7069 745f 746f 5f6e 6574   'slurpit_to_net
 000003e0: 626f 7827 2025 7d61 6374 6976 657b 2520  box' %}active{% 
 000003f0: 656e 6469 6620 257d 2220 6872 6566 3d22  endif %}" href="
 00000400: 3f74 6162 3d73 6c75 7270 6974 5f74 6f5f  ?tab=slurpit_to_
 00000410: 6e65 7462 6f78 223e 0a20 2020 2020 2020  netbox">.       
 00000420: 2053 6c75 7270 e280 9969 7420 746f 204e   Slurp...it to N
 00000430: 6574 426f 780a 2020 2020 2020 3c2f 613e  etBox.      </a>
-00000440: 0a20 2020 203c 2f6c 693e 0a20 2020 200a  .    </li>.    .
-00000450: 2020 3c2f 756c 3e0a 7b25 2065 6e64 626c    </ul>.{% endbl
-00000460: 6f63 6b20 7461 6273 2025 7d0a 0a7b 2520  ock tabs %}..{% 
-00000470: 626c 6f63 6b20 636f 6e74 656e 742d 7772  block content-wr
-00000480: 6170 7065 7220 257d 0a20 203c 6469 7620  apper %}.  <div 
-00000490: 636c 6173 733d 2274 6162 2d63 6f6e 7465  class="tab-conte
-000004a0: 6e74 223e 0a20 2020 207b 2520 6966 2072  nt">.    {% if r
-000004b0: 6571 7565 7374 2e47 4554 2e74 6162 203d  equest.GET.tab =
-000004c0: 3d20 2773 6c75 7270 6974 5f74 6f5f 6e65  = 'slurpit_to_ne
-000004d0: 7462 6f78 2720 2025 7d0a 0a20 2020 2020  tbox'  %}..     
-000004e0: 2020 203c 6831 2063 6c61 7373 3d22 772d     <h1 class="w-
-000004f0: 3130 3020 7465 7874 2d63 656e 7465 7222  100 text-center"
-00000500: 2073 7479 6c65 3d22 7061 6464 696e 672d   style="padding-
-00000510: 746f 703a 2031 3025 3b22 3e43 6f6d 696e  top: 10%;">Comin
-00000520: 6720 536f 6f6e 3c2f 6831 3e0a 2020 2020  g Soon</h1>.    
-00000530: 2020 2020 3c70 2063 6c61 7373 3d22 772d      <p class="w-
-00000540: 3130 3020 7465 7874 2d63 656e 7465 7220  100 text-center 
-00000550: 6673 2d36 223e 5369 676e 2075 7020 666f  fs-6">Sign up fo
-00000560: 7220 6f75 7220 6e65 7773 6c65 7474 6572  r our newsletter
-00000570: 2061 6e64 2077 6520 7769 6c6c 2069 6e66   and we will inf
-00000580: 6f72 6d20 796f 7520 7768 656e 2074 6865  orm you when the
-00000590: 206e 6578 7420 6e65 7720 6675 6e63 7469   next new functi
-000005a0: 6f6e 616c 6974 6965 7320 6172 6520 7265  onalities are re
-000005b0: 6c65 6173 6564 2e3c 6272 3e3c 6272 3e0a  leased.<br><br>.
-000005c0: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-000005d0: 2268 7474 7073 3a2f 2f73 6c75 7270 6974  "https://slurpit
-000005e0: 2e69 6f2f 6765 7474 696e 672d 7374 6172  .io/getting-star
-000005f0: 7465 642f 2373 7562 7363 7269 6265 2220  ted/#subscribe" 
-00000600: 7461 7267 6574 3d22 5f62 6c61 6e6b 2220  target="_blank" 
-00000610: 636c 6173 733d 2262 746e 2062 746e 2d70  class="btn btn-p
-00000620: 7269 6d61 7279 223e 5375 6273 6372 6962  rimary">Subscrib
-00000630: 653c 2f61 3e3c 2f70 3e0a 2020 2020 7b25  e</a></p>.    {%
-00000640: 2065 6c69 6620 7265 7175 6573 742e 4745   elif request.GE
-00000650: 542e 7461 6220 3d3d 2027 6e65 7462 6f78  T.tab == 'netbox
-00000660: 5f74 6f5f 736c 7572 7069 7427 206f 7220  _to_slurpit' or 
-00000670: 7265 7175 6573 742e 4745 542e 7461 6220  request.GET.tab 
-00000680: 6973 204e 6f6e 6520 257d 0a20 2020 2020  is None %}.     
-00000690: 207b 2520 696e 636c 7564 6520 2273 6c75   {% include "slu
-000006a0: 7270 6974 5f6e 6574 626f 782f 6d61 7070  rpit_netbox/mapp
-000006b0: 696e 672f 6e65 7462 6f78 5f74 6f5f 736c  ing/netbox_to_sl
-000006c0: 7572 7069 742e 6874 6d6c 2220 257d 0a20  urpit.html" %}. 
-000006d0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-000006e0: 203c 2f64 6976 3e20 0a0a 7b25 2065 6e64   </div> ..{% end
-000006f0: 626c 6f63 6b20 636f 6e74 656e 742d 7772  block content-wr
-00000700: 6170 7065 7220 257d 0a0a 0a0a 0a0a 3c66  apper %}......<f
-00000710: 6f6f 7465 7220 636c 6173 733d 2266 6f6f  ooter class="foo
-00000720: 7465 7220 636f 6e74 6169 6e65 722d 666c  ter container-fl
-00000730: 7569 6422 3e0a 2020 7b25 2062 6c6f 636b  uid">.  {% block
-00000740: 2066 6f6f 7465 7220 257d 0a20 2020 203c   footer %}.    <
-00000750: 6469 7620 636c 6173 733d 2272 6f77 2061  div class="row a
-00000760: 6c69 676e 2d69 7465 6d73 2d63 656e 7465  lign-items-cente
-00000770: 7220 6a75 7374 6966 792d 636f 6e74 656e  r justify-conten
-00000780: 742d 6265 7477 6565 6e20 6d78 2d30 223e  t-between mx-0">
-00000790: 0a0a 2020 2020 2020 3c64 6976 2063 6c61  ..      <div cla
-000007a0: 7373 3d22 636f 6c2d 736d 2d31 3220 636f  ss="col-sm-12 co
-000007b0: 6c2d 6d64 2d61 7574 6f20 6673 2d34 206e  l-md-auto fs-4 n
-000007c0: 6f70 7269 6e74 223e 0a20 2020 2020 2020  oprint">.       
-000007d0: 203c 6e61 7620 636c 6173 733d 226e 6176   <nav class="nav
-000007e0: 206a 7573 7469 6679 2d63 6f6e 7465 6e74   justify-content
-000007f0: 2d63 656e 7465 7220 6a75 7374 6966 792d  -center justify-
-00000800: 636f 6e74 656e 742d 6c67 2d73 7461 7274  content-lg-start
-00000810: 223e 0a20 2020 2020 2020 2020 207b 2520  ">.          {% 
-00000820: 626c 6f63 6b20 666f 6f74 6572 5f6c 696e  block footer_lin
-00000830: 6b73 2025 7d0a 2020 2020 2020 2020 2020  ks %}.          
-00000840: 2020 3c61 2074 7970 653d 2262 7574 746f    <a type="butto
-00000850: 6e22 2063 6c61 7373 3d22 6e61 762d 6c69  n" class="nav-li
-00000860: 6e6b 2068 3622 2068 7265 663d 2268 7474  nk h6" href="htt
-00000870: 7073 3a2f 2f73 6c75 7270 6974 2e69 6f22  ps://slurpit.io"
-00000880: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00000890: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000008a0: 6874 7470 733a 2f2f 736c 7572 7069 742e  https://slurpit.
-000008b0: 696f 0a20 2020 2020 2020 2020 2020 203c  io.            <
-000008c0: 2f61 3e0a 2020 2020 2020 2020 2020 7b25  /a>.          {%
-000008d0: 2065 6e64 626c 6f63 6b20 666f 6f74 6572   endblock footer
-000008e0: 5f6c 696e 6b73 2025 7d0a 2020 2020 2020  _links %}.      
-000008f0: 2020 3c2f 6e61 763e 0a20 2020 2020 203c    </nav>.      <
-00000900: 2f64 6976 3e0a 0a20 2020 2020 203c 6469  /div>..      <di
-00000910: 7620 636c 6173 733d 2263 6f6c 2d73 6d2d  v class="col-sm-
-00000920: 3132 2063 6f6c 2d6d 642d 6175 746f 2074  12 col-md-auto t
-00000930: 6578 742d 6365 6e74 6572 2074 6578 742d  ext-center text-
-00000940: 6c67 2d65 6e64 2074 6578 742d 6d75 7465  lg-end text-mute
-00000950: 6422 2020 3e0a 2020 2020 2020 2020 3c73  d"  >.        <s
-00000960: 7061 6e20 636c 6173 733d 2264 2d62 6c6f  pan class="d-blo
-00000970: 636b 2064 2d6d 642d 696e 6c69 6e65 223e  ck d-md-inline">
-00000980: 7b25 2061 6e6e 6f74 6174 6564 5f6e 6f77  {% annotated_now
-00000990: 2025 7d20 7b25 206e 6f77 2027 5427 2025   %} {% now 'T' %
-000009a0: 7d3c 2f73 7061 6e3e 0a20 2020 2020 2020  }</span>.       
-000009b0: 203c 7370 616e 2063 6c61 7373 3d22 6d73   <span class="ms
-000009c0: 2d6d 642d 3320 642d 626c 6f63 6b20 642d  -md-3 d-block d-
-000009d0: 6d64 2d69 6e6c 696e 6522 3e7b 7b20 7365  md-inline">{{ se
-000009e0: 7474 696e 6773 2e48 4f53 544e 414d 4520  ttings.HOSTNAME 
-000009f0: 7d7d 2028 767b 7b20 7365 7474 696e 6773  }} (v{{ settings
-00000a00: 2e56 4552 5349 4f4e 207d 7d29 3c2f 7370  .VERSION }})</sp
-00000a10: 616e 3e0a 2020 2020 2020 2020 3c73 7061  an>.        <spa
-00000a20: 6e20 636c 6173 733d 226d 732d 6d64 2d33  n class="ms-md-3
-00000a30: 2064 2d62 6c6f 636b 2064 2d6d 642d 696e   d-block d-md-in
-00000a40: 6c69 6e65 223e 536c 7572 7069 7428 767b  line">Slurpit(v{
-00000a50: 7b20 7365 7474 696e 6773 2e50 4c55 4749  { settings.PLUGI
-00000a60: 4e53 5f43 4f4e 4649 472e 736c 7572 7069  NS_CONFIG.slurpi
-00000a70: 745f 6e65 7462 6f78 2e76 6572 7369 6f6e  t_netbox.version
-00000a80: 207d 7d29 3c2f 7370 616e 3e0a 2020 2020   }})</span>.    
-00000a90: 2020 3c2f 6469 763e 0a0a 2020 2020 3c2f    </div>..    </
-00000aa0: 6469 763e 0a20 207b 2520 656e 6462 6c6f  div>.  {% endblo
-00000ab0: 636b 2066 6f6f 7465 7220 257d 0a3c 2f66  ck footer %}.</f
-00000ac0: 6f6f 7465 723e 0a                        ooter>.
+00000440: 0a20 2020 203c 2f6c 693e 0a0a 2020 3c2f  .    </li>..  </
+00000450: 756c 3e0a 7b25 2065 6e64 626c 6f63 6b20  ul>.{% endblock 
+00000460: 7461 6273 2025 7d0a 0a7b 2520 626c 6f63  tabs %}..{% bloc
+00000470: 6b20 636f 6e74 656e 742d 7772 6170 7065  k content-wrappe
+00000480: 7220 257d 0a20 203c 6469 7620 636c 6173  r %}.  <div clas
+00000490: 733d 2274 6162 2d63 6f6e 7465 6e74 2073  s="tab-content s
+000004a0: 7562 2d74 6162 2d63 6f6e 7465 6e74 223e  ub-tab-content">
+000004b0: 0a20 2020 207b 2520 6966 2072 6571 7565  .    {% if reque
+000004c0: 7374 2e47 4554 2e74 6162 203d 3d20 2773  st.GET.tab == 's
+000004d0: 6c75 7270 6974 5f74 6f5f 6e65 7462 6f78  lurpit_to_netbox
+000004e0: 2720 2025 7d0a 2020 2020 2020 7b25 2069  '  %}.      {% i
+000004f0: 6e63 6c75 6465 2022 736c 7572 7069 745f  nclude "slurpit_
+00000500: 6e65 7462 6f78 2f6d 6170 7069 6e67 2f63  netbox/mapping/c
+00000510: 6f6d 6d69 6e67 736f 6f6e 2e68 746d 6c22  ommingsoon.html"
+00000520: 2025 7d0a 2020 2020 7b25 2065 6c69 6620   %}.    {% elif 
+00000530: 7265 7175 6573 742e 4745 542e 7461 6220  request.GET.tab 
+00000540: 3d3d 2027 6e65 7462 6f78 5f74 6f5f 736c  == 'netbox_to_sl
+00000550: 7572 7069 7427 206f 7220 7265 7175 6573  urpit' or reques
+00000560: 742e 4745 542e 7461 6220 6973 204e 6f6e  t.GET.tab is Non
+00000570: 6520 257d 0a20 2020 2020 207b 2520 696e  e %}.      {% in
+00000580: 636c 7564 6520 2273 6c75 7270 6974 5f6e  clude "slurpit_n
+00000590: 6574 626f 782f 6d61 7070 696e 672f 6e65  etbox/mapping/ne
+000005a0: 7462 6f78 5f74 6f5f 736c 7572 7069 742e  tbox_to_slurpit.
+000005b0: 6874 6d6c 2220 257d 0a20 2020 207b 2520  html" %}.    {% 
+000005c0: 656e 6469 6620 257d 0a20 203c 2f64 6976  endif %}.  </div
+000005d0: 3e20 0a0a 7b25 2065 6e64 626c 6f63 6b20  > ..{% endblock 
+000005e0: 636f 6e74 656e 742d 7772 6170 7065 7220  content-wrapper 
+000005f0: 257d 0a0a 0a0a 0a0a 3c66 6f6f 7465 7220  %}......<footer 
+00000600: 636c 6173 733d 2266 6f6f 7465 7220 636f  class="footer co
+00000610: 6e74 6169 6e65 722d 666c 7569 6422 3e0a  ntainer-fluid">.
+00000620: 2020 7b25 2062 6c6f 636b 2066 6f6f 7465    {% block foote
+00000630: 7220 257d 0a20 2020 203c 6469 7620 636c  r %}.    <div cl
+00000640: 6173 733d 2272 6f77 2061 6c69 676e 2d69  ass="row align-i
+00000650: 7465 6d73 2d63 656e 7465 7220 6a75 7374  tems-center just
+00000660: 6966 792d 636f 6e74 656e 742d 6265 7477  ify-content-betw
+00000670: 6565 6e20 6d78 2d30 223e 0a0a 2020 2020  een mx-0">..    
+00000680: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+00000690: 6c2d 736d 2d31 3220 636f 6c2d 6d64 2d61  l-sm-12 col-md-a
+000006a0: 7574 6f20 6673 2d34 206e 6f70 7269 6e74  uto fs-4 noprint
+000006b0: 223e 0a20 2020 2020 2020 203c 6e61 7620  ">.        <nav 
+000006c0: 636c 6173 733d 226e 6176 206a 7573 7469  class="nav justi
+000006d0: 6679 2d63 6f6e 7465 6e74 2d63 656e 7465  fy-content-cente
+000006e0: 7220 6a75 7374 6966 792d 636f 6e74 656e  r justify-conten
+000006f0: 742d 6c67 2d73 7461 7274 223e 0a20 2020  t-lg-start">.   
+00000700: 2020 2020 2020 207b 2520 626c 6f63 6b20         {% block 
+00000710: 666f 6f74 6572 5f6c 696e 6b73 2025 7d0a  footer_links %}.
+00000720: 2020 2020 2020 2020 2020 2020 3c61 2074              <a t
+00000730: 7970 653d 2262 7574 746f 6e22 2063 6c61  ype="button" cla
+00000740: 7373 3d22 6e61 762d 6c69 6e6b 2068 3622  ss="nav-link h6"
+00000750: 2068 7265 663d 2268 7474 7073 3a2f 2f73   href="https://s
+00000760: 6c75 7270 6974 2e69 6f22 2074 6172 6765  lurpit.io" targe
+00000770: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
+00000780: 2020 2020 2020 2020 2020 6874 7470 733a            https:
+00000790: 2f2f 736c 7572 7069 742e 696f 0a20 2020  //slurpit.io.   
+000007a0: 2020 2020 2020 2020 203c 2f61 3e0a 2020           </a>.  
+000007b0: 2020 2020 2020 2020 7b25 2065 6e64 626c          {% endbl
+000007c0: 6f63 6b20 666f 6f74 6572 5f6c 696e 6b73  ock footer_links
+000007d0: 2025 7d0a 2020 2020 2020 2020 3c2f 6e61   %}.        </na
+000007e0: 763e 0a20 2020 2020 203c 2f64 6976 3e0a  v>.      </div>.
+000007f0: 0a20 2020 2020 203c 6469 7620 636c 6173  .      <div clas
+00000800: 733d 2263 6f6c 2d73 6d2d 3132 2063 6f6c  s="col-sm-12 col
+00000810: 2d6d 642d 6175 746f 2074 6578 742d 6365  -md-auto text-ce
+00000820: 6e74 6572 2074 6578 742d 6c67 2d65 6e64  nter text-lg-end
+00000830: 2074 6578 742d 6d75 7465 6422 2020 3e0a   text-muted"  >.
+00000840: 2020 2020 2020 2020 3c73 7061 6e20 636c          <span cl
+00000850: 6173 733d 2264 2d62 6c6f 636b 2064 2d6d  ass="d-block d-m
+00000860: 642d 696e 6c69 6e65 223e 7b25 2061 6e6e  d-inline">{% ann
+00000870: 6f74 6174 6564 5f6e 6f77 2025 7d20 7b25  otated_now %} {%
+00000880: 206e 6f77 2027 5427 2025 7d3c 2f73 7061   now 'T' %}</spa
+00000890: 6e3e 0a20 2020 2020 2020 203c 7370 616e  n>.        <span
+000008a0: 2063 6c61 7373 3d22 6d73 2d6d 642d 3320   class="ms-md-3 
+000008b0: 642d 626c 6f63 6b20 642d 6d64 2d69 6e6c  d-block d-md-inl
+000008c0: 696e 6522 3e7b 7b20 7365 7474 696e 6773  ine">{{ settings
+000008d0: 2e48 4f53 544e 414d 4520 7d7d 2028 767b  .HOSTNAME }} (v{
+000008e0: 7b20 7365 7474 696e 6773 2e56 4552 5349  { settings.VERSI
+000008f0: 4f4e 207d 7d29 3c2f 7370 616e 3e0a 2020  ON }})</span>.  
+00000900: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
+00000910: 733d 226d 732d 6d64 2d33 2064 2d62 6c6f  s="ms-md-3 d-blo
+00000920: 636b 2064 2d6d 642d 696e 6c69 6e65 223e  ck d-md-inline">
+00000930: 536c 7572 7069 7428 767b 7b20 7365 7474  Slurpit(v{{ sett
+00000940: 696e 6773 2e50 4c55 4749 4e53 5f43 4f4e  ings.PLUGINS_CON
+00000950: 4649 472e 736c 7572 7069 745f 6e65 7462  FIG.slurpit_netb
+00000960: 6f78 2e76 6572 7369 6f6e 207d 7d29 3c2f  ox.version }})</
+00000970: 7370 616e 3e0a 2020 2020 2020 3c2f 6469  span>.      </di
+00000980: 763e 0a0a 2020 2020 3c2f 6469 763e 0a20  v>..    </div>. 
+00000990: 207b 2520 656e 6462 6c6f 636b 2066 6f6f   {% endblock foo
+000009a0: 7465 7220 257d 0a3c 2f66 6f6f 7465 723e  ter %}.</footer>
+000009b0: 0a0a                                     ..
```

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/logo.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/logo.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/mapping/netbox_to_slurpit.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/mapping/netbox_to_slurpit.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,120 @@
 {% load buttons %}
 {% load i18n %}
 {% load helpers %}
 {% load static %}
 {% load form_helpers %}
 
-<div class=" show {% if request.GET.tab == 'netbox_to_slurpit' %}active{% endif %}">
-    {% if appliance_type != 'cloud' %}
-      <!-- <a name="sync"  class="btn btn-sm btn-orange my-2" href="{% url 'plugins:slurpit_netbox:data_mapping_list' %}?sync=true{% if request.GET %}&{{ request.GET.urlencode }}{% endif %}">
+<ul class="nav nav-tabs px-3 sub-nav">    
+
+  <li class="nav-item" role="presentation">
+    <a class="nav-tab nav-link {% if request.GET.subtab == 'devices' or request.GET.subtab is None %}active{% endif %}" href="?tab=netbox_to_slurpit&subtab=devices">
+      Devices
+    </a>
+  </li>
+
+  <li class="nav-item" role="presentation">
+    <a class="nav-tab nav-link {% if request.GET.subtab == 'ipam' %}active{% endif %}" href="?tab=netbox_to_slurpit&subtab=ipam">
+      IPAM
+    </a>
+  </li>
+  
+</ul>
+
+<div class="tab-content">
+  {% if request.GET.subtab == 'devices' or request.GET.subtab is None %}
+    <div class=" show {% if request.GET.tab == 'netbox_to_slurpit' %}active{% endif %}">
+      {% if appliance_type != 'cloud' %}
+        <!-- <a name="sync"  class="btn btn-sm btn-orange my-2" href="{% url 'plugins:slurpit_netbox:data_mapping_list' %}?sync=true{% if request.GET %}&{{ request.GET.urlencode }}{% endif %}">
+            <i class="mdi mdi-sync"></i> {% trans "Sync" %}
+        </a> -->
+        <a name="sync"  id="sync-btn" class="btn btn-sm btn-orange my-2" data-bs-toggle="modal" data-bs-target="#syncStatusModal">
           <i class="mdi mdi-sync"></i> {% trans "Sync" %}
-      </a> -->
-      <a name="sync"  id="sync-btn" class="btn btn-sm btn-orange my-2" data-bs-toggle="modal" data-bs-target="#syncStatusModal">
-        <i class="mdi mdi-sync"></i> {% trans "Sync" %}
-      </a>
-    {% endif %}
-    <div class="row my-2">
-      <div class="col col-md-6">
-        <div class="card">
-          
-          <div class="card-header">
-              <h6>Sync your NetBox devices to Slurp'it</h6>
-              <span>
-                In case you already have a filled NetBox system, and you want to sync those to Slurp'it to start collecting data then this is the page you are looking for.
-                Below on the left you see the required attributes for in Slurp'it and on the right you can map those against your data from NetBox. If you need more information we can advise you to <a href="https://learning.slurpit.io/courses/offers/783fcc2c-f0f8-4a41-bc7c-64f1d03e43e8" target="_BLANK">
-                click here</a> for our online course.
-              </span>
+        </a>
+      {% endif %}
+      <div class="row my-2">
+        <div class="col col-md-6">
+          <div class="card">
+            
+            <div class="card-header">
+                <h6>Sync your NetBox devices to Slurp'it</h6>
+                <span>
+                  In case you already have a filled NetBox system, and you want to sync those to Slurp'it to start collecting data then this is the page you are looking for.
+                  Below on the left you see the required attributes for in Slurp'it and on the right you can map those against your data from NetBox. If you need more information we can advise you to <a href="https://learning.slurpit.io/courses/offers/783fcc2c-f0f8-4a41-bc7c-64f1d03e43e8" target="_BLANK">
+                  click here</a> for our online course.
+                </span>
+            </div>
           </div>
         </div>
       </div>
-    </div>
-    <div class="row mt-1">
-      <div class="col col-md-6">
-        <div class="card management-status-card">
-          
-          <div class="card-header">
-            <h6>Management status</h6>
-            <div class="my-1">
-              Select here the device status you want to sync.
-            </div>
-            {% render_form device_status_form %}
+      <div class="row mt-1">
+        <div class="col col-md-6">
+          <div class="card management-status-card">
             
+            <div class="card-header">
+              <h6>Management status</h6>
+              <div class="my-1">
+                Select here the device status you want to sync.
+              </div>
+              {% render_form device_status_form %}
+              
+            </div>
           </div>
         </div>
       </div>
-    </div>
-    <div class="row mb-3">
-        <div class="col col-md-6">
-            <form action="?tab=netbox_to_slurpit" method="post" id="mapping-form" class="form form-horizontal mb-3">
-                
-                <div class="card mt-2">
-                
-                  <div class="card-header" style="display:flex;justify-content: space-between;">
-                      <h5>Mapping Fields</h5>
-                      <div class="action">
-                        
-                        <a class="btn btn-purple btn-sm px-3" data-bs-toggle="modal" data-bs-target="#testMapModal">
-                          {% trans "Test" %}
-                        </a>
-                        <button class="btn btn-blue btn-sm px-3">
-                            {% trans "Save" %}
-                        </button>
-                      </div>
-                  </div>
-                  <div class="card-body">
-                    {% csrf_token %}
-                    <input type="hidden" name="action" value="save" id="actionInput" />
-                    {% for choice_item in form %}
-                      <div class="d-flex map-item">
-                        <input type="checkbox" name="pk" value="{{ choice_item.choice }}"/>
-                        <input type="hidden" name="source_field" value="{{ choice_item.choice }}"/>
-                        {% render_form choice_item.form %}
-                      </div>
-                    {% endfor %}
-                  </div>
-                  <div class="card-footer">
-                    <button type="button" class="btn btn-sm btn-success" data-bs-toggle="modal" data-bs-target="#addMapModal">
-                        <i class="mdi mdi-plus-thick"></i> Add
-                    </button>
-                    <button id="delete-btn" class="btn btn-danger btn-sm">
-                        <i class="mdi mdi-trash-can-outline" aria-hidden="true"></i> Delete Selected
-                    </button>
+      <div class="row mb-3">
+          <div class="col col-md-6">
+              <form action="?tab=netbox_to_slurpit" method="post" id="mapping-form" class="form form-horizontal mb-3">
+                  
+                  <div class="card mt-2">
+                  
+                    <div class="card-header" style="display:flex;justify-content: space-between;">
+                        <h5>Mapping Fields</h5>
+                        <div class="action">
+                          
+                          <a class="btn btn-purple btn-sm px-3" data-bs-toggle="modal" data-bs-target="#testMapModal">
+                            {% trans "Test" %}
+                          </a>
+                          <button class="btn btn-blue btn-sm px-3">
+                              {% trans "Save" %}
+                          </button>
+                        </div>
+                    </div>
+                    <div class="card-body">
+                      {% csrf_token %}
+                      <input type="hidden" name="action" value="save" id="actionInput" />
+                      {% for choice_item in form %}
+                        <div class="d-flex map-item">
+                          <input type="checkbox" name="pk" value="{{ choice_item.choice }}"/>
+                          <input type="hidden" name="source_field" value="{{ choice_item.choice }}"/>
+                          {% render_form choice_item.form %}
+                        </div>
+                      {% endfor %}
+                    </div>
+                    <div class="card-footer">
+                      <button type="button" class="btn btn-sm btn-success" data-bs-toggle="modal" data-bs-target="#addMapModal">
+                          <i class="mdi mdi-plus-thick"></i> Add
+                      </button>
+                      <button id="delete-btn" class="btn btn-danger btn-sm">
+                          <i class="mdi mdi-trash-can-outline" aria-hidden="true"></i> Delete Selected
+                      </button>
+                    </div>
                   </div>
-                </div>
-              </form>
-        </div>
+                </form>
+          </div>
+      </div>
     </div>
+  {% elif request.GET.subtab == 'ipam'  %}
+    {% include "slurpit_netbox/mapping/commingsoon.html" %}
+  {% endif %}
+  
 </div>
 
+
+
 <div class="modal fade" tabindex="-1" id="addMapModal">
   <div class="modal-dialog modal-lg">
     <div class="modal-content">
 
       <!-- Modal Header -->
       <div class="modal-header">
         <h4 class="modal-title">Create a mapping</h4>
@@ -165,26 +190,27 @@
               <div class="progress-text" id="progressText">
                 Sending devices <br> from Netbox to Slurpit<br><span class="sync-percent" id="percent">0%</span><br>
                 <span> Total Devices: <span id="total-cnt">100</span></span><br>
                 <span> Done Devices: <span id="done-cnt">30</span></span><br>
                 <span> Failed Devices: <span id="failed-cnt">10</span></span>
               </div>
             </div>
-            
+            <textarea  name="logs" cols="40" rows="10" class=" form-control mb-2" placeholder="Logs" id="logs" style="height: 80px;"></textarea>
             <p><b>Don't refresh website or close modal before 100%</b></p>
           </div>
-  
+          
       </form>
       <!-- Modal Body -->
       
     </div>
   </div>
 </div>
 
 
+
 <style>
   .map-item {
     width: 100% !important;
     gap: 100px;
   }
   .map-item .mb-3 {
     margin-bottom: 0px !important;
@@ -232,14 +258,27 @@
     line-height: 33px !important;
     color: #4CAF50
   }
 
   .management-status-card label {
     display: none !important;
   }
+
+  .sub-nav .nav-tab.nav-link.active {
+    border: 0px !important;
+    border-bottom: 2px solid #0d6efd !important;
+    font-weight: bold !important;
+  }
+
+  .sub-tab-content {
+    padding: 1rem 0 !important;
+  }
+  .sub-nav {
+    background: transparent !important;
+  }
 </style>
 
 <script>
   var delElement = document.getElementById('delete-btn');
   var form = document.getElementById('mapping-form');
   var actionInput = document.getElementById('actionInput');
   var payloadResultTextarea = document.getElementById('payload-result');
@@ -321,14 +360,16 @@
     });
   });
 
   var syncButton = document.getElementById("sync-btn");
   var totalElement = document.getElementById("total-cnt");
   var doneElement = document.getElementById("done-cnt");
   var failedElement = document.getElementById("failed-cnt");
+  var logsElement = document.getElementById("logs");
+
   var total_count = 0;
   var failed_count = 0;
   var done_count = 0;
   var percent = 0;
   var devices;
   var current_cnt = 0;
   var url = '/plugins/slurpit/data_mapping/?tab=netbox_to_slurpit';
@@ -348,15 +389,15 @@
   syncButton.addEventListener("click", function(event) {
     total_count = 0;
     failed_count = 0;
     done_count = 0;
     percent = 0;
     devices = [];
     current_cnt = 0;
-
+    logsElement.innerHTML = "";
     update_status()
     deviceStatus = document.querySelector('select[name="device_status"]').value;
 
     var data = new URLSearchParams();
     data.append('action', 'sync')
     data.append('csrfmiddlewaretoken', csrfToken);
     data.append('status', deviceStatus);
@@ -398,15 +439,18 @@
       },
       body: data
     }).then(function(response) {
       return response.json();
     }).then(function(res){
       current_cnt++;
       if(res["status"] == undefined) done_count++;  
-      else failed_count++;
+      else {
+        failed_count++;
+        logsElement.append("Failed to import "+res["device_name"]+"\n")
+      }
       update_status();  
       send_device();
     }).catch(function(error) {
       failed_count++;
       current_cnt++;
       update_status();
       send_device();
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
 {% load buttons %} {% load i18n %} {% load helpers %} {% load static %} {% load
 form_helpers %}
+    * _D_e_v_i_c_e_s
+    * _I_P_A_M
+{% if request.GET.subtab == 'devices' or request.GET.subtab is None %}
 {% if appliance_type != 'cloud' %}
 {% trans "Sync" %}
 {% endif %}
 ** SSyynncc yyoouurr NNeettBBooxx ddeevviicceess ttoo SSlluurrpp''iitt **
 In case you already have a filled NetBox system, and you want to sync those to
 Slurp'it to start collecting data then this is the page you are looking for.
 Below on the left you see the required attributes for in Slurp'it and on the
@@ -14,14 +17,16 @@
 {% render_form device_status_form %}
 **** MMaappppiinngg FFiieellddss ****
 {% trans "Test" %} {% trans "Save" %}
 {% csrf_token %} {% for choice_item in form %}
 ??{% render_form choice_item.form %}
 {% endfor %}
 Add Delete Selected
+{% elif request.GET.subtab == 'ipam' %} {% include "slurpit_netbox/mapping/
+commingsoon.html" %} {% endif %}
 ****** CCrreeaattee aa mmaappppiinngg ******
 {% csrf_token %}
 {% render_form new_form %}
 {% trans "Add" %} Close
 ****** TTeesstt ddeevviiccee mmaappppiinngg ******
 {% csrf_token %}
 {% render_form device_form %}
```

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/onboard/conflict_device_list.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/onboard/conflict_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/onboard/migrate_device_list.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/onboard/migrate_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/onboard/new_device_list.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/onboard/new_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/onboard/onboarded_device_list.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/onboard/onboarded_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/onboard_device.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/onboard_device.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/planning_table.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/planning_table.html`

 * *Files 0% similar despite different names*

```diff
@@ -92,31 +92,31 @@
     var form = document.getElementById('plan-form');
     // Add an event listener for the 'change' event
     selectElement.addEventListener('change', function(event) {
       // The event target is the select element, and its value is the selected option's value
       form.submit();
     });
 
-    
-
-    var syncElement = document.getElementById('sync');
-    var syncInput = document.getElementById('syncInput');
+    var refreshElement = document.getElementById('refresh');
+    var refreshInput = document.getElementById('refreshInput');
 
-    syncElement.addEventListener('click', function(event) {
+    refreshElement.addEventListener('click', function(event) {
       // The event target is the select element, and its value is the selected option's value
-      syncInput.value = "sync";
+      refreshInput.value = "refresh";
       form.submit();
     });
 
-    var refreshElement = document.getElementById('refresh');
-    var refreshInput = document.getElementById('refreshInput');
 
-    refreshElement.addEventListener('click', function(event) {
+    var syncElement = document.getElementById('sync');
+    var syncInput = document.getElementById('syncInput');
+
+    syncElement.addEventListener('click', function(event) {
       // The event target is the select element, and its value is the selected option's value
-      refreshInput.value = "refresh";
+      syncInput.value = "sync";
       form.submit();
     });
 
+   
   </script>
 {% endblock %}
```

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/settings/data_tabs.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/settings/data_tabs.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/settings/general.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/settings/general.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/settings.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/settings.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/templates/slurpit_netbox/slurpitlog_list.html` & `slurpit_netbox-0.8.63/src/slurpit_netbox/templates/slurpit_netbox/slurpitlog_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/urls.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/urls.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/validator.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/validator.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/views/datamapping.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/views/datamapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from django.forms.models import model_to_dict
 import requests
 from django.core.exceptions import ObjectDoesNotExist
 from django.http import HttpResponse, JsonResponse
 from django.utils.safestring import mark_safe
 from django.contrib.contenttypes.models import ContentType
 from extras.models import CustomField
+from extras.models.tags import Tag
+from ipam.models import IPRange
 
 BATCH_SIZE = 128
 
 def get_device_dict(instance):
     device_dict = model_to_dict(instance)
     # Assuming 'device_type' is a ForeignKey, for example.
     device_dict['device_type'] = str(instance.device_type)
@@ -27,15 +29,15 @@
     device_dict['primary_ip6'] = str(instance.primary_ip6)
 
     for custom_field in device_dict['custom_field_data']:
         device_dict[f'cf_{custom_field}'] = device_dict['custom_field_data'][custom_field]
 
     return device_dict
 
-def post_slurpit_device(row):
+def post_slurpit_device(row, device_name):
     try:
         setting = SlurpitSetting.objects.get()
         uri_base = setting.server_url
         headers = {
                         'Authorization': f'Bearer {setting.api_key}',
                         'useragent': 'netbox/requests',
                         'accept': 'application/json',
@@ -44,24 +46,25 @@
 
         uri_devices = f"{uri_base}/api/devices/sync"
         
         try:
             row["ignore_plugin"] = str(1)
             r = requests.post(uri_devices, headers=headers, json=row, verify=False)
             r = r.json()
+            r["device_name"] = device_name
             return r
         except Exception as e:
-            return {"error": str(e)}
+            return {"error": str(e), "device_name": device_name}
 
     except ObjectDoesNotExist:
         setting = None
         log_message = "Need to set the setting parameter"
         SlurpitLog.failure(category=LogCategoryChoices.DATA_MAPPING, message=log_message)
 
-        return {"error": "Need to set the setting parameter"}
+        return {"error": "Need to set the setting parameter", "device_name": device_name}
     
     return None
 
 @method_decorator(slurpit_plugin_registered, name='dispatch')
 class DataMappingView(View):
     template_name = "slurpit_netbox/data_mapping.html"
     app_label = "dcim"
@@ -82,15 +85,15 @@
             for device in devices_array:
                 row = {}
                 for obj in objs:
                     target_field = obj.target_field.split('|')[1]
                     row[obj.source_field] = str(device[target_field])
                 # request_body.append(row)
 
-                res = post_slurpit_device(row)
+                res = post_slurpit_device(row, device["name"])
 
                 if res is None:
                     return redirect(f'{request.path}?tab={tab}')
                 
                 if res['status'] != 200:
                     error_message = ''
                     for error in res["messages"]:
@@ -111,14 +114,18 @@
         appliance_type = ''
         try:
             setting = SlurpitSetting.objects.get()
             appliance_type = setting.appliance_type
         except ObjectDoesNotExist:
             setting = None
 
+        if tab == "devices":
+            slurpit_tag = Tag.objects.get(name="slurpit")
+            ip_ranges = IPRange.objects.filter(tags__in=[slurpit_tag])
+        
         for mapping in mappings:
             form.append({
                 "choice": mapping,
                 "form": SlurpitMappingForm(choice_name=mapping, initial={"target_field": mapping.target_field})
             })
 
         new_form = SlurpitMappingForm(doaction="add")
@@ -154,15 +161,15 @@
                 row = {}
                 objs = SlurpitMapping.objects.all()
                 for obj in objs:
                     target_field = obj.target_field.split('|')[1]
                     row[obj.source_field] = str(device[target_field])
 
                 if test is not None:
-                    res = post_slurpit_device(row)
+                    res = post_slurpit_device(row, device["name"])
 
                     if res is None:
                         return JsonResponse({"error": "Server Internal Error."})
                     
                     return JsonResponse(res)
 
                 return JsonResponse(row)
```

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/views/logging.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/views/logging.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/views/onboarding.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/views/onboarding.py`

 * *Files identical despite different names*

### Comparing `slurpit_netbox-0.8.46/src/slurpit_netbox/views/setting.py` & `slurpit_netbox-0.8.63/src/slurpit_netbox/views/setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,23 @@
     template_name = "slurpit_netbox/planning_table.html"
     tab = ViewTab("Slurpit", permission="slurpit_netbox.view_devicetable")
     form = SlurpitPlanningTableForm()
 
     def get(self, request, pk):
         device = get_object_or_404(Device, pk=pk)
         
+        connection_status = appliance_type = ''
+        setting = None
+        try:
+            setting = SlurpitSetting.objects.get()
+            appliance_type = setting.appliance_type
+            connection_status = setting.connection_status
+        except ObjectDoesNotExist:
+            pass
+        
         data = None
         cached_time = None
         result_status = "No Data"
         columns = []
         refresh = request.GET.get('refresh')
         sync = request.GET.get('sync')
         if 'planning_id' in request.GET and (planning := SlurpitPlanning.objects.filter(planning_id=request.GET.get('planning_id')).first()):
@@ -326,15 +335,16 @@
             cache_key = (
                 f"slurpit_plan_{planning.planning_id}_{device.serial}_{result_type}"
             )
 
             url_no_refresh = get_refresh_url(request, pk)
 
             if sync == "sync":
-                sync_snapshot(cache_key, device.name, planning)
+                if appliance_type != "cloud":
+                    sync_snapshot(cache_key, device.name, planning)
                 
                 return HttpResponseRedirect(url_no_refresh)
             
             if refresh == "refresh":
                 cache.delete(cache_key)
                 return HttpResponseRedirect(url_no_refresh)
 
@@ -347,15 +357,16 @@
                 data = []
                 try: 
                     temp = SlurpitSnapshot.objects.filter(hostname=device.name, planning_id=planning.planning_id)
                     result_key = f"{result_type}_result"
                     
                     # Empty case
                     if temp.count() == 0:
-                        sync_snapshot(cache_key, device.name, planning)
+                        if appliance_type != "cloud":
+                            sync_snapshot(cache_key, device.name, planning)
                         temp = SlurpitSnapshot.objects.filter(hostname=device.name, planning_id=planning.planning_id)
 
                     for r in temp:
                         r = r.content
                         raw = r[result_key]
                         data.append({**raw})
                     result_status = "Live"
@@ -391,22 +402,15 @@
                 request,
                 "htmx/table.html",
                 {
                     "table": table,
                 },
             )
 
-        connection_status = appliance_type = ''
-        setting = None
-        try:
-            setting = SlurpitSetting.objects.get()
-            appliance_type = setting.appliance_type
-            connection_status = setting.connection_status
-        except ObjectDoesNotExist:
-            pass
+        
 
         return render(
             request,
             self.template_name,
             {
                 "object": device,
                 "tab": self.tab,
```

### Comparing `slurpit_netbox-0.8.46/PKG-INFO` & `slurpit_netbox-0.8.63/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurpit_netbox
-Version: 0.8.46
+Version: 0.8.63
 Summary: 
 Author: Pieter
 Author-email: pieter@slurpit.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

