# Comparing `tmp/fortiedr-3.6.8.tar.gz` & `tmp/fortiedr-3.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortiedr-3.6.8.tar", last modified: Wed May 29 00:16:10 2024, max compression
+gzip compressed data, was "fortiedr-3.6.9.tar", last modified: Thu May 30 00:29:54 2024, max compression
```

## Comparing `fortiedr-3.6.8.tar` & `fortiedr-3.6.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:16:10.306486 fortiedr-3.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 00:16:06.000000 fortiedr-3.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 00:16:06.000000 fortiedr-3.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-29 00:16:10.306486 fortiedr-3.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-29 00:16:06.000000 fortiedr-3.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:16:10.306486 fortiedr-3.6.8/fortiedr/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 00:16:06.000000 fortiedr-3.6.8/fortiedr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21615 2024-05-29 00:16:06.000000 fortiedr-3.6.8/fortiedr/api_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-29 00:16:06.000000 fortiedr-3.6.8/fortiedr/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-29 00:16:06.000000 fortiedr-3.6.8/fortiedr/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)   252923 2024-05-29 00:16:06.000000 fortiedr-3.6.8/fortiedr/fortiedr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:16:10.306486 fortiedr-3.6.8/fortiedr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-29 00:16:10.000000 fortiedr-3.6.8/fortiedr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 00:16:10.000000 fortiedr-3.6.8/fortiedr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 00:16:10.000000 fortiedr-3.6.8/fortiedr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 00:16:10.000000 fortiedr-3.6.8/fortiedr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-29 00:16:06.000000 fortiedr-3.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 00:16:06.000000 fortiedr-3.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 00:16:10.306486 fortiedr-3.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-29 00:16:06.000000 fortiedr-3.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:29:54.918597 fortiedr-3.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 00:29:36.000000 fortiedr-3.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-30 00:29:36.000000 fortiedr-3.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-30 00:29:54.918597 fortiedr-3.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 00:29:36.000000 fortiedr-3.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:29:54.914597 fortiedr-3.6.9/fortiedr/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 00:29:36.000000 fortiedr-3.6.9/fortiedr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21615 2024-05-30 00:29:36.000000 fortiedr-3.6.9/fortiedr/api_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-30 00:29:36.000000 fortiedr-3.6.9/fortiedr/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-30 00:29:36.000000 fortiedr-3.6.9/fortiedr/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   261160 2024-05-30 00:29:36.000000 fortiedr-3.6.9/fortiedr/fortiedr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:29:54.918597 fortiedr-3.6.9/fortiedr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-30 00:29:54.000000 fortiedr-3.6.9/fortiedr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 00:29:54.000000 fortiedr-3.6.9/fortiedr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 00:29:54.000000 fortiedr-3.6.9/fortiedr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 00:29:54.000000 fortiedr-3.6.9/fortiedr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-30 00:29:36.000000 fortiedr-3.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 00:29:36.000000 fortiedr-3.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 00:29:54.918597 fortiedr-3.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-30 00:29:36.000000 fortiedr-3.6.9/setup.py
```

### Comparing `fortiedr-3.6.8/LICENSE` & `fortiedr-3.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.8/PKG-INFO` & `fortiedr-3.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.6.8
+Version: 3.6.9
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.6.8/README.md` & `fortiedr-3.6.9/README.md`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.8/fortiedr/api_parameters.json` & `fortiedr-3.6.9/fortiedr/api_parameters.json`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.8/fortiedr/auth.py` & `fortiedr-3.6.9/fortiedr/auth.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.8/fortiedr/connector.py` & `fortiedr-3.6.9/fortiedr/connector.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.8/fortiedr/fortiedr.py` & `fortiedr-3.6.9/fortiedr/fortiedr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import os
 import json
 from typing import BinaryIO
 from fortiedr.auth import Auth as fedrAuth
 from fortiedr.connector import FortiEDR_API_GW
 
-version = '3.6.8'
+version = '3.6.9'
 
 fortiedr_connection = None
 
 class Admin:
 	'''Admin Rest Api Controller'''
 
 	def set_tray_notification_settings(self, enabledPopup: bool = None, enabledTrayNotification: bool = None, message: str = None, organization: str = None) -> tuple[bool, None]:
@@ -24,20 +24,20 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("set_tray_notification_settings", locals())
 
 		url = '/api/admin/set-tray-notification-settings'
 
-		adminSetTrayNotificationSettingsRequest = {
-			"enabledPopup": enabledPopup,
-			"enabledTrayNotification": enabledTrayNotification,
-			"message": message,
-			"organization": organization,
-		}
+		adminSetTrayNotificationSettingsRequest = {}
+		if enabledPopup: adminSetTrayNotificationSettingsRequest["enabledPopup"] = enabledPopup
+		if enabledTrayNotification: adminSetTrayNotificationSettingsRequest["enabledTrayNotification"] = enabledTrayNotification
+		if message: adminSetTrayNotificationSettingsRequest["message"] = message
+		if organization: adminSetTrayNotificationSettingsRequest["organization"] = organization
+
 		return fortiedr_connection.send(url, adminSetTrayNotificationSettingsRequest)
 
 class ApplicationControl:
 	'''Application Control Rest Api Controller'''
 
 	def get_applications(self, currentPage: int, organization: str, fileName: str = None, path: str = None, signer: str = None, enabled: bool = None, hash: str = None, operatingSystem: str = None, policyIds: list = None, tag: str = None) -> tuple[bool, None]:
 		'''
@@ -103,18 +103,18 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("send_applications", locals())
 
 		url = '/api/application-control/applications'
 
-		applicationControlSaveRequest = {
-			"applicationControls": applicationControls,
-			"organization": organization,
-		}
+		applicationControlSaveRequest = {}
+		if applicationControls: applicationControlSaveRequest["applicationControls"] = applicationControls
+		if organization: applicationControlSaveRequest["organization"] = organization
+
 		return fortiedr_connection.send(url, applicationControlSaveRequest)
 
 	def insert_applications(self, appIds: list, organization: str, enabled: bool = None, groupIds: list = None, isOverridePolicies: bool = None, policyIds: list = None, tagId: int = None) -> tuple[bool, list]:
 		'''
 		Class ApplicationControl
 		Description: Edits existing application control and returns the affected ones.
         
@@ -134,21 +134,21 @@
 		url_params = []
 		if appIds:
 			url_params.append('appIds=' + ",".join(map(str, appIds)))
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 
-		modifiedFields = {
-			"enabled": enabled,
-			"groupIds": groupIds,
-			"isOverridePolicies": isOverridePolicies,
-			"policyIds": policyIds,
-			"tagId": str(tagId),
-		}
+		modifiedFields = {}
+		if enabled: modifiedFields["enabled"] = enabled
+		if groupIds: modifiedFields["groupIds"] = groupIds
+		if isOverridePolicies: modifiedFields["isOverridePolicies"] = isOverridePolicies
+		if policyIds: modifiedFields["policyIds"] = policyIds
+		if tagId: modifiedFields["tagId"] = str(tagId)
+
 		return fortiedr_connection.insert(url, modifiedFields)
 
 	def delete_applications(self, organization: str, applicationIds: list = None) -> tuple[bool, None]:
 		'''
 		Class ApplicationControl
 		Description: Deletes application controls.
         
@@ -200,18 +200,18 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("tags", locals())
 
 		url = '/api/application-control/tags'
 
-		applicationControlTagCreateRequest = {
-			"name": name,
-			"organization": organization,
-		}
+		applicationControlTagCreateRequest = {}
+		if name: applicationControlTagCreateRequest["name"] = name
+		if organization: applicationControlTagCreateRequest["organization"] = organization
+
 		return fortiedr_connection.send(url, applicationControlTagCreateRequest)
 
 class dashboardrestapicontroller:
 	'''Dashboard Rest Api Controller'''
 
 	def most_targeted_items(self, organization: str, itemType: str = None, numOfColumns: int = None, numOfDays: int = None) -> tuple[bool, None]:
 		'''
@@ -331,17 +331,17 @@
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("previous_registration_passwords", locals())
 
 		url = '/management-rest/admin/previous-registration-passwords'
 
-		organizationRequest = {
-			"organization": organization,
-		}
+		organizationRequest = {}
+		if organization: organizationRequest["organization"] = organization
+
 		return fortiedr_connection.get(url, organizationRequest)
 
 	def previous_registration_passwords(self, passwordId: int, organization: str = None) -> tuple[bool, str]:
 		'''
 		Class Administrator
 		Description: This API deletes previous registration password for given id.
         
@@ -353,17 +353,17 @@
 			bool: Status of the request (True or False). 
 			str
 		'''
 		validate_params("previous_registration_passwords", locals())
 
 		url = f'/management-rest/admin/previous-registration-passwords/{passwordId}'
 
-		organizationRequest = {
-			"organization": organization,
-		}
+		organizationRequest = {}
+		if organization: organizationRequest["organization"] = organization
+
 		return fortiedr_connection.delete(url, organizationRequest)
 
 	def ready(self) -> tuple[bool, None]:
 		'''
 		Class Administrator
 		Description: Get System Readiness.
         
@@ -390,18 +390,18 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("registration_password", locals())
 
 		url = '/management-rest/admin/registration-password'
 
-		request = {
-			"organization": organization,
-			"password": password,
-		}
+		request = {}
+		if organization: request["organization"] = organization
+		if password: request["password"] = password
+
 		return fortiedr_connection.send(url, request)
 
 	def set_system_mode(self, mode: str, forceAll: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Administrator
 		Description: Set system modeThis API call enables you to switch the system to Simulation mode.
         
@@ -456,17 +456,17 @@
 			url_params.append('collectorGroupIds=' + ",".join(map(str, collectorGroupIds)))
 		if collectorGroups:
 			url_params.append('collectorGroups=' + ",".join(str(collectorGroups)))
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 
-		requestUpdateData = {
-			"updateVersions": updateVersions,
-		}
+		requestUpdateData = {}
+		if updateVersions: requestUpdateData["updateVersions"] = updateVersions
+
 		return fortiedr_connection.send(url, requestUpdateData)
 
 	def upload_content(self, file: BinaryIO, ) -> tuple[bool, str]:
 		'''
 		Class Administrator
 		Description: Upload content to the system.
         
@@ -478,14 +478,16 @@
 			str
 		'''
 		validate_params("upload_content", locals())
 
 		url = '/management-rest/admin/upload-content'
 		if file:
 			file = {'file': file}
+
+
 		return fortiedr_connection.upload(url, file)
 
 	def upload_license(self, licenseBlob: str = None) -> tuple[bool, None]:
 		'''
 		Class Administrator
 		Description: Upload license to the system.
         
@@ -496,17 +498,17 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("upload_license", locals())
 
 		url = '/management-rest/admin/upload-license'
 
-		license = {
-			"licenseBlob": licenseBlob,
-		}
+		license = {}
+		if licenseBlob: license["licenseBlob"] = licenseBlob
+
 		return fortiedr_connection.insert(url, license)
 
 class Audit:
 	'''The Audit module enables you to retrieve system audit based on given dates'''
 
 	def get_audit(self, fromTime: str = None, organization: str = None, toTime: str = None) -> tuple[bool, list]:
 		'''
@@ -1060,27 +1062,27 @@
 			url_params.append('signed=' + signed)
 		if sorting:
 			url_params.append('sorting=' + sorting)
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 
-		updateEventsRequest = {
-			"archive": archive,
-			"classification": classification,
-			"comment": comment,
-			"familyName": familyName,
-			"forceUnmute": forceUnmute,
-			"handle": handle,
-			"malwareType": malwareType,
-			"mute": mute,
-			"muteDuration": muteDuration,
-			"read": read,
-			"threatName": threatName,
-		}
+		updateEventsRequest = {}
+		if archive: updateEventsRequest["archive"] = archive
+		if classification: updateEventsRequest["classification"] = classification
+		if comment: updateEventsRequest["comment"] = comment
+		if familyName: updateEventsRequest["familyName"] = familyName
+		if forceUnmute: updateEventsRequest["forceUnmute"] = forceUnmute
+		if handle: updateEventsRequest["handle"] = handle
+		if malwareType: updateEventsRequest["malwareType"] = malwareType
+		if mute: updateEventsRequest["mute"] = mute
+		if muteDuration: updateEventsRequest["muteDuration"] = muteDuration
+		if read: updateEventsRequest["read"] = read
+		if threatName: updateEventsRequest["threatName"] = threatName
+
 		return fortiedr_connection.insert(url, updateEventsRequest)
 
 	def delete_events(self, actions: list = None, applicationControl: bool = None, archived: bool = None, classifications: list = None, collectorGroups: list = None, deleteAll: bool = None, destinations: list = None, device: str = None, deviceControl: bool = None, deviceIps: list = None, eventIds: list = None, eventType: list = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: list = None, muted: bool = None, operatingSystems: list = None, organization: str = None, pageNumber: int = None, paths: list = None, process: str = None, rule: str = None, seen: bool = None, severities: list = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, None]:
 		'''
 		Class Events
 		Description: This API call delete events.
         
@@ -1407,20 +1409,20 @@
 			url_params.append('forceCreate=' + forceCreate)
 		if organization:
 			url_params.append('organization=' + organization)
 		if users:
 			url_params.append('users=' + ",".join(str(users)))
 		url += '?' + '&'.join(url_params)
 
-		exceptionRequest = {
-			"useAnyPath": useAnyPath,
-			"useInException": useInException,
-			"wildcardFiles": wildcardFiles,
-			"wildcardPaths": wildcardPaths,
-		}
+		exceptionRequest = {}
+		if useAnyPath: exceptionRequest["useAnyPath"] = useAnyPath
+		if useInException: exceptionRequest["useInException"] = useInException
+		if wildcardFiles: exceptionRequest["wildcardFiles"] = wildcardFiles
+		if wildcardPaths: exceptionRequest["wildcardPaths"] = wildcardPaths
+
 		return fortiedr_connection.send(url, exceptionRequest)
 
 	def export_raw_data_items_json(self, organization: str = None, rawItemIds: str = None) -> tuple[bool, None]:
 		'''
 		Class Events
 		Description: Get event as Json format.
         
@@ -1680,14 +1682,16 @@
 		url = '/management-rest/exceptions/create-or-edit-exception'
 		url_params = []
 		if confirmEdit:
 			url_params.append('confirmEdit=' + confirmEdit)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
+
+
 		return fortiedr_connection.send(url, exceptionJSON)
 
 	def delete(self, collectorGroups: list = None, comment: str = None, createdAfter: str = None, createdBefore: str = None, deleteAll: bool = None, destination: str = None, exceptionId: int = None, exceptionIds: list = None, organization: str = None, path: str = None, process: str = None, rules: list = None, updatedAfter: str = None, updatedBefore: str = None, user: str = None) -> tuple[bool, None]:
 		'''
 		Class Exceptions
 		Description: Delete exceptions.
         
@@ -2040,28 +2044,28 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("create_connector", locals())
 
 		url = '/management-rest/integrations/create-connector'
 
-		createConnectorRequest = {
-			"apiKey": apiKey,
-			"connectorActions": connectorActions,
-			"coreId": str(coreId),
-			"enabled": enabled,
-			"host": host,
-			"name": name,
-			"organization": organization,
-			"password": password,
-			"port": port,
-			"type": type,
-			"username": username,
-			"vendor": vendor,
-		}
+		createConnectorRequest = {}
+		if apiKey: createConnectorRequest["apiKey"] = apiKey
+		if connectorActions: createConnectorRequest["connectorActions"] = connectorActions
+		if coreId: createConnectorRequest["coreId"] = str(coreId)
+		if enabled: createConnectorRequest["enabled"] = enabled
+		if host: createConnectorRequest["host"] = host
+		if name: createConnectorRequest["name"] = name
+		if organization: createConnectorRequest["organization"] = organization
+		if password: createConnectorRequest["password"] = password
+		if port: createConnectorRequest["port"] = port
+		if type: createConnectorRequest["type"] = type
+		if username: createConnectorRequest["username"] = username
+		if vendor: createConnectorRequest["vendor"] = vendor
+
 		return fortiedr_connection.send(url, createConnectorRequest)
 
 	def delete_connector(self, connectorName: str, connectorType: str, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Integrations
 		Description: Deletes a connector.
         
@@ -2150,28 +2154,28 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("update_connector", locals())
 
 		url = '/management-rest/integrations/update-connector'
 
-		updateConnectorRequest = {
-			"apiKey": apiKey,
-			"connectorActions": connectorActions,
-			"coreId": str(coreId),
-			"enabled": enabled,
-			"host": host,
-			"name": name,
-			"organization": organization,
-			"password": password,
-			"port": port,
-			"type": type,
-			"username": username,
-			"vendor": vendor,
-		}
+		updateConnectorRequest = {}
+		if apiKey: updateConnectorRequest["apiKey"] = apiKey
+		if connectorActions: updateConnectorRequest["connectorActions"] = connectorActions
+		if coreId: updateConnectorRequest["coreId"] = str(coreId)
+		if enabled: updateConnectorRequest["enabled"] = enabled
+		if host: updateConnectorRequest["host"] = host
+		if name: updateConnectorRequest["name"] = name
+		if organization: updateConnectorRequest["organization"] = organization
+		if password: updateConnectorRequest["password"] = password
+		if port: updateConnectorRequest["port"] = port
+		if type: updateConnectorRequest["type"] = type
+		if username: updateConnectorRequest["username"] = username
+		if vendor: updateConnectorRequest["vendor"] = vendor
+
 		return fortiedr_connection.insert(url, updateConnectorRequest)
 
 class SystemInventory:
 	'''The System Inventory module enables you to monitor the health of Fortinet Endpoint Protection and Response Platform components and to create Collector Groups.'''
 
 	def aggregator_logs(self, device: str = None, deviceId: int = None, organization: str = None) -> tuple[bool, None]:
 		'''
@@ -3350,21 +3354,21 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("create_ip_set", locals())
 
 		url = '/management-rest/ip-sets/create-ip-set'
 
-		ipGroupsRequest = {
-			"description": description,
-			"exclude": exclude,
-			"include": include,
-			"name": name,
-			"organization": organization,
-		}
+		ipGroupsRequest = {}
+		if description: ipGroupsRequest["description"] = description
+		if exclude: ipGroupsRequest["exclude"] = exclude
+		if include: ipGroupsRequest["include"] = include
+		if name: ipGroupsRequest["name"] = name
+		if organization: ipGroupsRequest["organization"] = organization
+
 		return fortiedr_connection.send(url, ipGroupsRequest)
 
 	def delete_ip_set(self, ipSets: list, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class IPsets
 		Description: This API delete IP sets from the system. Use the input parameters to filter organization.
         
@@ -3436,20 +3440,20 @@
 
 		url = '/management-rest/ip-sets/update-ip-set'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 
-		ipGroupsRequest = {
-			"description": description,
-			"exclude": exclude,
-			"include": include,
-			"name": name,
-		}
+		ipGroupsRequest = {}
+		if description: ipGroupsRequest["description"] = description
+		if exclude: ipGroupsRequest["exclude"] = exclude
+		if include: ipGroupsRequest["include"] = include
+		if name: ipGroupsRequest["name"] = name
+
 		return fortiedr_connection.insert(url, ipGroupsRequest)
 
 class Organizations:
 	'''Organizations API'''
 
 	def create_organization(self, eXtendedDetection: bool = None, edr: bool = None, edrAddOnsAllocated: int = None, edrBackupEnabled: bool = None, edrEnabled: bool = None, edrNumberOfShards: int = None, edrStorageAllocatedInMb: int = None, expirationDate: str = None, forensics: bool = None, iotAllocated: int = None, name: str = None, password: str = None, passwordConfirmation: str = None, requestPolicyEngineLibUpdates: bool = None, serialNumber: str = None, serversAllocated: int = None, vulnerabilityAndIoT: bool = None, workstationsAllocated: int = None) -> tuple[bool, None]:
 		'''
@@ -3463,34 +3467,34 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("create_organization", locals())
 
 		url = '/management-rest/organizations/create-organization'
 
-		createAccountRequest = {
-			"eXtendedDetection": eXtendedDetection,
-			"edr": edr,
-			"edrAddOnsAllocated": str(edrAddOnsAllocated),
-			"edrBackupEnabled": edrBackupEnabled,
-			"edrEnabled": edrEnabled,
-			"edrNumberOfShards": str(edrNumberOfShards),
-			"edrStorageAllocatedInMb": str(edrStorageAllocatedInMb),
-			"expirationDate": expirationDate,
-			"forensics": forensics,
-			"iotAllocated": str(iotAllocated),
-			"name": name,
-			"password": password,
-			"passwordConfirmation": passwordConfirmation,
-			"requestPolicyEngineLibUpdates": requestPolicyEngineLibUpdates,
-			"serialNumber": serialNumber,
-			"serversAllocated": str(serversAllocated),
-			"vulnerabilityAndIoT": vulnerabilityAndIoT,
-			"workstationsAllocated": str(workstationsAllocated),
-		}
+		createAccountRequest = {}
+		if eXtendedDetection: createAccountRequest["eXtendedDetection"] = eXtendedDetection
+		if edr: createAccountRequest["edr"] = edr
+		if edrAddOnsAllocated: createAccountRequest["edrAddOnsAllocated"] = str(edrAddOnsAllocated)
+		if edrBackupEnabled: createAccountRequest["edrBackupEnabled"] = edrBackupEnabled
+		if edrEnabled: createAccountRequest["edrEnabled"] = edrEnabled
+		if edrNumberOfShards: createAccountRequest["edrNumberOfShards"] = str(edrNumberOfShards)
+		if edrStorageAllocatedInMb: createAccountRequest["edrStorageAllocatedInMb"] = str(edrStorageAllocatedInMb)
+		if expirationDate: createAccountRequest["expirationDate"] = expirationDate
+		if forensics: createAccountRequest["forensics"] = forensics
+		if iotAllocated: createAccountRequest["iotAllocated"] = str(iotAllocated)
+		if name: createAccountRequest["name"] = name
+		if password: createAccountRequest["password"] = password
+		if passwordConfirmation: createAccountRequest["passwordConfirmation"] = passwordConfirmation
+		if requestPolicyEngineLibUpdates: createAccountRequest["requestPolicyEngineLibUpdates"] = requestPolicyEngineLibUpdates
+		if serialNumber: createAccountRequest["serialNumber"] = serialNumber
+		if serversAllocated: createAccountRequest["serversAllocated"] = str(serversAllocated)
+		if vulnerabilityAndIoT: createAccountRequest["vulnerabilityAndIoT"] = vulnerabilityAndIoT
+		if workstationsAllocated: createAccountRequest["workstationsAllocated"] = str(workstationsAllocated)
+
 		return fortiedr_connection.send(url, createAccountRequest)
 
 	def delete_organization(self, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Organizations
 		Description: This API delete organization in the system (only for Admin role).
         
@@ -3547,14 +3551,16 @@
 			None: This function does not return any data.
 		'''
 		validate_params("import_organization", locals())
 
 		url = '/management-rest/organizations/import-organization'
 		if file:
 			file = {'file': file}
+
+
 		return fortiedr_connection.upload(url, file)
 
 	def list_organizations(self) -> tuple[bool, list]:
 		'''
 		Class Organizations
 		Description: This API call outputs a list of the accounts in the system..
         
@@ -3581,20 +3587,20 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("transfer_collectors", locals())
 
 		url = '/management-rest/organizations/transfer-collectors'
 
-		transferCollectorRequests = {
-			"aggregatorsMap": aggregatorsMap,
-			"sourceOrganization": sourceOrganization,
-			"targetOrganization": targetOrganization,
-			"verificationCode": verificationCode,
-		}
+		transferCollectorRequests = {}
+		if aggregatorsMap: transferCollectorRequests["aggregatorsMap"] = aggregatorsMap
+		if sourceOrganization: transferCollectorRequests["sourceOrganization"] = sourceOrganization
+		if targetOrganization: transferCollectorRequests["targetOrganization"] = targetOrganization
+		if verificationCode: transferCollectorRequests["verificationCode"] = verificationCode
+
 		return fortiedr_connection.send(url, transferCollectorRequests)
 
 	def transfer_collectors_stop(self, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Organizations
 		Description: Transfer collector stop.
         
@@ -3631,32 +3637,32 @@
 
 		url = '/management-rest/organizations/update-organization'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 
-		accountRequest = {
-			"eXtendedDetection": eXtendedDetection,
-			"edr": edr,
-			"edrAddOnsAllocated": str(edrAddOnsAllocated),
-			"edrBackupEnabled": edrBackupEnabled,
-			"edrEnabled": edrEnabled,
-			"edrNumberOfShards": str(edrNumberOfShards),
-			"edrStorageAllocatedInMb": str(edrStorageAllocatedInMb),
-			"expirationDate": expirationDate,
-			"forensics": forensics,
-			"iotAllocated": str(iotAllocated),
-			"name": name,
-			"requestPolicyEngineLibUpdates": requestPolicyEngineLibUpdates,
-			"serialNumber": serialNumber,
-			"serversAllocated": str(serversAllocated),
-			"vulnerabilityAndIoT": vulnerabilityAndIoT,
-			"workstationsAllocated": str(workstationsAllocated),
-		}
+		accountRequest = {}
+		if eXtendedDetection: accountRequest["eXtendedDetection"] = eXtendedDetection
+		if edr: accountRequest["edr"] = edr
+		if edrAddOnsAllocated: accountRequest["edrAddOnsAllocated"] = str(edrAddOnsAllocated)
+		if edrBackupEnabled: accountRequest["edrBackupEnabled"] = edrBackupEnabled
+		if edrEnabled: accountRequest["edrEnabled"] = edrEnabled
+		if edrNumberOfShards: accountRequest["edrNumberOfShards"] = str(edrNumberOfShards)
+		if edrStorageAllocatedInMb: accountRequest["edrStorageAllocatedInMb"] = str(edrStorageAllocatedInMb)
+		if expirationDate: accountRequest["expirationDate"] = expirationDate
+		if forensics: accountRequest["forensics"] = forensics
+		if iotAllocated: accountRequest["iotAllocated"] = str(iotAllocated)
+		if name: accountRequest["name"] = name
+		if requestPolicyEngineLibUpdates: accountRequest["requestPolicyEngineLibUpdates"] = requestPolicyEngineLibUpdates
+		if serialNumber: accountRequest["serialNumber"] = serialNumber
+		if serversAllocated: accountRequest["serversAllocated"] = str(serversAllocated)
+		if vulnerabilityAndIoT: accountRequest["vulnerabilityAndIoT"] = vulnerabilityAndIoT
+		if workstationsAllocated: accountRequest["workstationsAllocated"] = str(workstationsAllocated)
+
 		return fortiedr_connection.insert(url, accountRequest)
 
 class Playbookspolicies:
 	'''Playbooks-policies API'''
 
 	def assign_collector_group(self, collectorGroupNames: list, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
@@ -3756,19 +3762,19 @@
 
 		url = '/management-rest/playbooks-policies/map-connectors-to-actions'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 
-		assignAIRActionsWithConnectorsRequest = {
-			"customActionsToConnectorsMaps": customActionsToConnectorsMaps,
-			"fortinetActionsToConnectorsMaps": fortinetActionsToConnectorsMaps,
-			"policyName": policyName,
-		}
+		assignAIRActionsWithConnectorsRequest = {}
+		if customActionsToConnectorsMaps: assignAIRActionsWithConnectorsRequest["customActionsToConnectorsMaps"] = customActionsToConnectorsMaps
+		if fortinetActionsToConnectorsMaps: assignAIRActionsWithConnectorsRequest["fortinetActionsToConnectorsMaps"] = fortinetActionsToConnectorsMaps
+		if policyName: assignAIRActionsWithConnectorsRequest["policyName"] = policyName
+
 		return fortiedr_connection.insert(url, assignAIRActionsWithConnectorsRequest)
 
 	def set_action_classification(self, organization: str = None, customActionsToClassificationMaps: list = None, fortinetActionsToClassificationMaps: list = None, policyName: str = None) -> tuple[bool, None]:
 		'''
 		Class Playbookspolicies
 		Description: Set the air policy actions' classifications..
         
@@ -3784,19 +3790,19 @@
 
 		url = '/management-rest/playbooks-policies/set-action-classification'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 
-		setActionsClassificationRequest = {
-			"customActionsToClassificationMaps": customActionsToClassificationMaps,
-			"fortinetActionsToClassificationMaps": fortinetActionsToClassificationMaps,
-			"policyName": policyName,
-		}
+		setActionsClassificationRequest = {}
+		if customActionsToClassificationMaps: setActionsClassificationRequest["customActionsToClassificationMaps"] = customActionsToClassificationMaps
+		if fortinetActionsToClassificationMaps: setActionsClassificationRequest["fortinetActionsToClassificationMaps"] = fortinetActionsToClassificationMaps
+		if policyName: setActionsClassificationRequest["policyName"] = policyName
+
 		return fortiedr_connection.insert(url, setActionsClassificationRequest)
 
 	def set_mode(self, mode: str, policyName: str, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Playbookspolicies
 		Description: Set playbook to simulation/prevention.
         
@@ -4080,26 +4086,26 @@
 
 		url = '/management-rest/sendable-entities/syslog'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 
-		syslogRequest = {
-			"certificateBlob": certificateBlob,
-			"host": host,
-			"name": name,
-			"port": str(port),
-			"privateKeyFile": privateKeyFile,
-			"privateKeyPassword": privateKeyPassword,
-			"protocol": protocol,
-			"syslogFormat": syslogFormat,
-			"useClientCertificate": useClientCertificate,
-			"useSSL": useSSL,
-		}
+		syslogRequest = {}
+		if certificateBlob: syslogRequest["certificateBlob"] = certificateBlob
+		if host: syslogRequest["host"] = host
+		if name: syslogRequest["name"] = name
+		if port: syslogRequest["port"] = str(port)
+		if privateKeyFile: syslogRequest["privateKeyFile"] = privateKeyFile
+		if privateKeyPassword: syslogRequest["privateKeyPassword"] = privateKeyPassword
+		if protocol: syslogRequest["protocol"] = protocol
+		if syslogFormat: syslogRequest["syslogFormat"] = syslogFormat
+		if useClientCertificate: syslogRequest["useClientCertificate"] = useClientCertificate
+		if useSSL: syslogRequest["useSSL"] = useSSL
+
 		return fortiedr_connection.send(url, syslogRequest)
 
 class SystemEvents:
 	'''System Events API'''
 
 	def list_system_events(self, componentNames: list = None, componentTypes: list = None, fromDate: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, sorting: str = None, strictMode: bool = None, toDate: str = None) -> tuple[bool, list]:
 		'''
@@ -4165,19 +4171,19 @@
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("send_exclusion", locals())
 
 		url = '/management-rest/threat-hunting-exclusions/exclusion'
 
-		createExclusionsRequest = {
-			"exclusionListName": exclusionListName,
-			"exclusions": exclusions,
-			"organization": organization,
-		}
+		createExclusionsRequest = {}
+		if exclusionListName: createExclusionsRequest["exclusionListName"] = exclusionListName
+		if exclusions: createExclusionsRequest["exclusions"] = exclusions
+		if organization: createExclusionsRequest["organization"] = organization
+
 		return fortiedr_connection.send(url, createExclusionsRequest)
 
 	def insert_exclusions(self, exclusionListName: str = None, exclusions: list = None, organization: str = None) -> tuple[bool, list]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Update exclusions..
         
@@ -4188,19 +4194,19 @@
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("insert_exclusions", locals())
 
 		url = '/management-rest/threat-hunting-exclusions/exclusion'
 
-		updateExclusionsRequest = {
-			"exclusionListName": exclusionListName,
-			"exclusions": exclusions,
-			"organization": organization,
-		}
+		updateExclusionsRequest = {}
+		if exclusionListName: updateExclusionsRequest["exclusionListName"] = exclusionListName
+		if exclusions: updateExclusionsRequest["exclusions"] = exclusions
+		if organization: updateExclusionsRequest["organization"] = organization
+
 		return fortiedr_connection.insert(url, updateExclusionsRequest)
 
 	def delete_exclusion(self, exclusionIds: list = None, organization: str = None) -> tuple[bool, str]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Deletes one or more exclusions by Id..
         
@@ -4211,18 +4217,18 @@
 			bool: Status of the request (True or False). 
 			str
 		'''
 		validate_params("delete_exclusion", locals())
 
 		url = '/management-rest/threat-hunting-exclusions/exclusion'
 
-		deleteExclusionsRequest = {
-			"exclusionIds": exclusionIds,
-			"organization": organization,
-		}
+		deleteExclusionsRequest = {}
+		if exclusionIds: deleteExclusionsRequest["exclusionIds"] = exclusionIds
+		if organization: deleteExclusionsRequest["organization"] = organization
+
 		return fortiedr_connection.delete(url, deleteExclusionsRequest)
 
 	def get_exclusions_list(self, organization: str, ) -> tuple[bool, list]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Get the list of Exclusions lists..
         
@@ -4254,19 +4260,19 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("send_exclusions_list", locals())
 
 		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
 
-		createExclusionListRequest = {
-			"collectorGroupIds": collectorGroupIds,
-			"name": name,
-			"organization": organization,
-		}
+		createExclusionListRequest = {}
+		if collectorGroupIds: createExclusionListRequest["collectorGroupIds"] = collectorGroupIds
+		if name: createExclusionListRequest["name"] = name
+		if organization: createExclusionListRequest["organization"] = organization
+
 		return fortiedr_connection.send(url, createExclusionListRequest)
 
 	def insert_exclusions_list(self, collectorGroupIds: list = None, listName: str = None, newName: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Updates an exclusions list.
         
@@ -4277,20 +4283,20 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("insert_exclusions_list", locals())
 
 		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
 
-		updateExclusionListRequest = {
-			"collectorGroupIds": collectorGroupIds,
-			"listName": listName,
-			"newName": newName,
-			"organization": organization,
-		}
+		updateExclusionListRequest = {}
+		if collectorGroupIds: updateExclusionListRequest["collectorGroupIds"] = collectorGroupIds
+		if listName: updateExclusionListRequest["listName"] = listName
+		if newName: updateExclusionListRequest["newName"] = newName
+		if organization: updateExclusionListRequest["organization"] = organization
+
 		return fortiedr_connection.insert(url, updateExclusionListRequest)
 
 	def delete_exclusions_list(self, listName: str, organization: str, ) -> tuple[bool, None]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Deletes an exclusions list..
         
@@ -4409,21 +4415,21 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("send_threat_hunting_profile", locals())
 
 		url = '/management-rest/threat-hunting-settings/threat-hunting-profile'
 
-		threatHuntingUpdateRequest = {
-			"associatedCollectorGroupIds": associatedCollectorGroupIds,
-			"name": name,
-			"newName": newName,
-			"organization": organization,
-			"threatHuntingCategoryList": threatHuntingCategoryList,
-		}
+		threatHuntingUpdateRequest = {}
+		if associatedCollectorGroupIds: threatHuntingUpdateRequest["associatedCollectorGroupIds"] = associatedCollectorGroupIds
+		if name: threatHuntingUpdateRequest["name"] = name
+		if newName: threatHuntingUpdateRequest["newName"] = newName
+		if organization: threatHuntingUpdateRequest["organization"] = organization
+		if threatHuntingCategoryList: threatHuntingUpdateRequest["threatHuntingCategoryList"] = threatHuntingCategoryList
+
 		return fortiedr_connection.send(url, threatHuntingUpdateRequest)
 
 	def delete_threat_hunting_profile(self, name: str, organization: str, ) -> tuple[bool, None]:
 		'''
 		Class ThreatHuntingSettings
 		Description: Deletes a Threat Hunting profile..
         
@@ -4485,19 +4491,19 @@
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("threat_hunting_profile_assign_collector_groups", locals())
 
 		url = '/management-rest/threat-hunting-settings/threat-hunting-profile/collector-groups'
 
-		threatHuntingAssignGroupsRequest = {
-			"associatedCollectorGroupIds": associatedCollectorGroupIds,
-			"name": name,
-			"organization": organization,
-		}
+		threatHuntingAssignGroupsRequest = {}
+		if associatedCollectorGroupIds: threatHuntingAssignGroupsRequest["associatedCollectorGroupIds"] = associatedCollectorGroupIds
+		if name: threatHuntingAssignGroupsRequest["name"] = name
+		if organization: threatHuntingAssignGroupsRequest["organization"] = organization
+
 		return fortiedr_connection.send(url, threatHuntingAssignGroupsRequest)
 
 class ThreatHunting:
 	'''API for Activity events'''
 
 	def counts(self, accountId: int = None, category: str = None, devices: list = None, filters: list = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: list = None, time: str = None, toTime: str = None) -> tuple[bool, None]:
 		'''
@@ -4511,28 +4517,28 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("counts", locals())
 
 		url = '/management-rest/threat-hunting/counts'
 
-		edrRequest = {
-			"accountId": str(accountId),
-			"category": category,
-			"devices": devices,
-			"filters": filters,
-			"fromTime": fromTime,
-			"itemsPerPage": str(itemsPerPage),
-			"organization": organization,
-			"pageNumber": str(pageNumber),
-			"query": query,
-			"sorting": sorting,
-			"time": time,
-			"toTime": toTime,
-		}
+		edrRequest = {}
+		if accountId: edrRequest["accountId"] = str(accountId)
+		if category: edrRequest["category"] = category
+		if devices: edrRequest["devices"] = devices
+		if filters: edrRequest["filters"] = filters
+		if fromTime: edrRequest["fromTime"] = fromTime
+		if itemsPerPage: edrRequest["itemsPerPage"] = str(itemsPerPage)
+		if organization: edrRequest["organization"] = organization
+		if pageNumber: edrRequest["pageNumber"] = str(pageNumber)
+		if query: edrRequest["query"] = query
+		if sorting: edrRequest["sorting"] = sorting
+		if time: edrRequest["time"] = time
+		if toTime: edrRequest["toTime"] = toTime
+
 		return fortiedr_connection.send(url, edrRequest)
 
 	def create_or_edit_tag(self, newTagName: str = None, organization: str = None, tagId: int = None, tagName: str = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API creates or edits the saved queries tag.
         
@@ -4543,20 +4549,20 @@
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("create_or_edit_tag", locals())
 
 		url = '/management-rest/threat-hunting/create-or-edit-tag'
 
-		createOrEditTagRequest = {
-			"newTagName": newTagName,
-			"organization": organization,
-			"tagId": str(tagId),
-			"tagName": tagName,
-		}
+		createOrEditTagRequest = {}
+		if newTagName: createOrEditTagRequest["newTagName"] = newTagName
+		if organization: createOrEditTagRequest["organization"] = organization
+		if tagId: createOrEditTagRequest["tagId"] = str(tagId)
+		if tagName: createOrEditTagRequest["tagName"] = tagName
+
 		return fortiedr_connection.send(url, createOrEditTagRequest)
 
 	def customize_fortinet_query(self, id: int = None, dayOfMonth: int = None, dayOfWeek: int = None, forceSaving: bool = None, frequency: int = None, frequencyUnit: str = None, fromTime: str = None, hour: int = None, organization: str = None, scheduled: bool = None, state: bool = None, time: str = None, toTime: str = None, queryToEdit: str = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API customizes the scheduling properties of a Fortinet query.
         
@@ -4575,28 +4581,28 @@
 		url_params = []
 		if id:
 			url_params.append('id=' + id)
 		if queryToEdit:
 			url_params.append('queryToEdit=' + queryToEdit)
 		url += '?' + '&'.join(url_params)
 
-		ootbQueryCustomizeRequest = {
-			"dayOfMonth": str(dayOfMonth),
-			"dayOfWeek": str(dayOfWeek),
-			"forceSaving": forceSaving,
-			"frequency": str(frequency),
-			"frequencyUnit": frequencyUnit,
-			"fromTime": fromTime,
-			"hour": str(hour),
-			"organization": organization,
-			"scheduled": scheduled,
-			"state": state,
-			"time": time,
-			"toTime": toTime,
-		}
+		ootbQueryCustomizeRequest = {}
+		if dayOfMonth: ootbQueryCustomizeRequest["dayOfMonth"] = str(dayOfMonth)
+		if dayOfWeek: ootbQueryCustomizeRequest["dayOfWeek"] = str(dayOfWeek)
+		if forceSaving: ootbQueryCustomizeRequest["forceSaving"] = forceSaving
+		if frequency: ootbQueryCustomizeRequest["frequency"] = str(frequency)
+		if frequencyUnit: ootbQueryCustomizeRequest["frequencyUnit"] = frequencyUnit
+		if fromTime: ootbQueryCustomizeRequest["fromTime"] = fromTime
+		if hour: ootbQueryCustomizeRequest["hour"] = str(hour)
+		if organization: ootbQueryCustomizeRequest["organization"] = organization
+		if scheduled: ootbQueryCustomizeRequest["scheduled"] = scheduled
+		if state: ootbQueryCustomizeRequest["state"] = state
+		if time: ootbQueryCustomizeRequest["time"] = time
+		if toTime: ootbQueryCustomizeRequest["toTime"] = toTime
+
 		return fortiedr_connection.send(url, ootbQueryCustomizeRequest)
 
 	def delete_saved_queries(self, deleteAll: bool = None, deleteFromCommunity: bool = None, organization: str = None, queryIds: list = None, queryNames: list = None, scheduled: bool = None, source: list = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API deletes the saved queries.
         
@@ -4682,29 +4688,29 @@
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("facets", locals())
 
 		url = '/management-rest/threat-hunting/facets'
 
-		facetsRequest = {
-			"accountId": str(accountId),
-			"category": category,
-			"devices": devices,
-			"facets": facets,
-			"filters": filters,
-			"fromTime": fromTime,
-			"itemsPerPage": str(itemsPerPage),
-			"organization": organization,
-			"pageNumber": str(pageNumber),
-			"query": query,
-			"sorting": sorting,
-			"time": time,
-			"toTime": toTime,
-		}
+		facetsRequest = {}
+		if accountId: facetsRequest["accountId"] = str(accountId)
+		if category: facetsRequest["category"] = category
+		if devices: facetsRequest["devices"] = devices
+		if facets: facetsRequest["facets"] = facets
+		if filters: facetsRequest["filters"] = filters
+		if fromTime: facetsRequest["fromTime"] = fromTime
+		if itemsPerPage: facetsRequest["itemsPerPage"] = str(itemsPerPage)
+		if organization: facetsRequest["organization"] = organization
+		if pageNumber: facetsRequest["pageNumber"] = str(pageNumber)
+		if query: facetsRequest["query"] = query
+		if sorting: facetsRequest["sorting"] = sorting
+		if time: facetsRequest["time"] = time
+		if toTime: facetsRequest["toTime"] = toTime
+
 		return fortiedr_connection.send(url, facetsRequest)
 
 	def list_saved_queries(self, organization: str = None, scheduled: bool = None, source: list = None) -> tuple[bool, list]:
 		'''
 		Class ThreatHunting
 		Description: This API retrieves the existing saved queries list.
         
@@ -4776,37 +4782,37 @@
 		url_params = []
 		if id:
 			url_params.append('id=' + id)
 		if queryToEdit:
 			url_params.append('queryToEdit=' + queryToEdit)
 		url += '?' + '&'.join(url_params)
 
-		saveQueryRequest = {
-			"category": category,
-			"classification": classification,
-			"collectorNames": collectorNames,
-			"community": community,
-			"dayOfMonth": str(dayOfMonth),
-			"dayOfWeek": str(dayOfWeek),
-			"description": description,
-			"forceSaving": forceSaving,
-			"frequency": str(frequency),
-			"frequencyUnit": frequencyUnit,
-			"fromTime": fromTime,
-			"hour": str(hour),
-			"name": name,
-			"organization": organization,
-			"query": query,
-			"scheduled": scheduled,
-			"state": state,
-			"tagIds": tagIds,
-			"tagNames": tagNames,
-			"time": time,
-			"toTime": toTime,
-		}
+		saveQueryRequest = {}
+		if category: saveQueryRequest["category"] = category
+		if classification: saveQueryRequest["classification"] = classification
+		if collectorNames: saveQueryRequest["collectorNames"] = collectorNames
+		if community: saveQueryRequest["community"] = community
+		if dayOfMonth: saveQueryRequest["dayOfMonth"] = str(dayOfMonth)
+		if dayOfWeek: saveQueryRequest["dayOfWeek"] = str(dayOfWeek)
+		if description: saveQueryRequest["description"] = description
+		if forceSaving: saveQueryRequest["forceSaving"] = forceSaving
+		if frequency: saveQueryRequest["frequency"] = str(frequency)
+		if frequencyUnit: saveQueryRequest["frequencyUnit"] = frequencyUnit
+		if fromTime: saveQueryRequest["fromTime"] = fromTime
+		if hour: saveQueryRequest["hour"] = str(hour)
+		if name: saveQueryRequest["name"] = name
+		if organization: saveQueryRequest["organization"] = organization
+		if query: saveQueryRequest["query"] = query
+		if scheduled: saveQueryRequest["scheduled"] = scheduled
+		if state: saveQueryRequest["state"] = state
+		if tagIds: saveQueryRequest["tagIds"] = tagIds
+		if tagNames: saveQueryRequest["tagNames"] = tagNames
+		if time: saveQueryRequest["time"] = time
+		if toTime: saveQueryRequest["toTime"] = toTime
+
 		return fortiedr_connection.send(url, saveQueryRequest)
 
 	def search(self, accountId: int = None, category: str = None, devices: list = None, filters: list = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: list = None, time: str = None, toTime: str = None) -> tuple[bool, list]:
 		'''
 		Class ThreatHunting
 		Description: This API call outputs a list of Activity events from middleware..
         
@@ -4817,28 +4823,28 @@
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("search", locals())
 
 		url = '/management-rest/threat-hunting/search'
 
-		edrRequest = {
-			"accountId": str(accountId),
-			"category": category,
-			"devices": devices,
-			"filters": filters,
-			"fromTime": fromTime,
-			"itemsPerPage": str(itemsPerPage),
-			"organization": organization,
-			"pageNumber": str(pageNumber),
-			"query": query,
-			"sorting": sorting,
-			"time": time,
-			"toTime": toTime,
-		}
+		edrRequest = {}
+		if accountId: edrRequest["accountId"] = str(accountId)
+		if category: edrRequest["category"] = category
+		if devices: edrRequest["devices"] = devices
+		if filters: edrRequest["filters"] = filters
+		if fromTime: edrRequest["fromTime"] = fromTime
+		if itemsPerPage: edrRequest["itemsPerPage"] = str(itemsPerPage)
+		if organization: edrRequest["organization"] = organization
+		if pageNumber: edrRequest["pageNumber"] = str(pageNumber)
+		if query: edrRequest["query"] = query
+		if sorting: edrRequest["sorting"] = sorting
+		if time: edrRequest["time"] = time
+		if toTime: edrRequest["toTime"] = toTime
+
 		return fortiedr_connection.send(url, edrRequest)
 
 	def set_query_state(self, state: bool, markAll: bool = None, organization: str = None, queryIds: list = None, queryNames: list = None, source: list = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API updates the scheduled saved query state.
         
@@ -4900,27 +4906,27 @@
 
 		url = '/management-rest/users/create-user'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 
-		userRequest = {
-			"confirmPassword": confirmPassword,
-			"customScript": customScript,
-			"email": email,
-			"firstName": firstName,
-			"lastName": lastName,
-			"password": password,
-			"remoteShell": remoteShell,
-			"restApi": restApi,
-			"role": role,
-			"title": title,
-			"username": username,
-		}
+		userRequest = {}
+		if confirmPassword: userRequest["confirmPassword"] = confirmPassword
+		if customScript: userRequest["customScript"] = customScript
+		if email: userRequest["email"] = email
+		if firstName: userRequest["firstName"] = firstName
+		if lastName: userRequest["lastName"] = lastName
+		if password: userRequest["password"] = password
+		if remoteShell: userRequest["remoteShell"] = remoteShell
+		if restApi: userRequest["restApi"] = restApi
+		if role: userRequest["role"] = role
+		if title: userRequest["title"] = title
+		if username: userRequest["username"] = username
+
 		return fortiedr_connection.send(url, userRequest)
 
 	def delete_saml_settings(self, organizationNameRequest: str, ) -> tuple[bool, None]:
 		'''
 		Class Users
 		Description: Delete SAML authentication settings per organization.
         
@@ -5028,18 +5034,18 @@
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		if username:
 			url_params.append('username=' + username)
 		url += '?' + '&'.join(url_params)
 
-		userRequest = {
-			"confirmPassword": confirmPassword,
-			"password": password,
-		}
+		userRequest = {}
+		if confirmPassword: userRequest["confirmPassword"] = confirmPassword
+		if password: userRequest["password"] = password
+
 		return fortiedr_connection.insert(url, userRequest)
 
 	def update_saml_settings(self, idpMetadataFile: BinaryIO, ) -> tuple[bool, None]:
 		'''
 		Class Users
 		Description: Create / Update SAML authentication settings per organization.
         
@@ -5051,14 +5057,16 @@
 			None: This function does not return any data.
 		'''
 		validate_params("update_saml_settings", locals())
 
 		url = '/management-rest/users/update-saml-settings'
 		if idpMetadataFile:
 			idpMetadataFile = {'idpMetadataFile': idpMetadataFile}
+
+
 		return fortiedr_connection.upload(url, idpMetadataFile)
 
 	def update_user(self, username: str, organization: str = None, customScript: bool = None, email: str = None, firstName: str = None, lastName: str = None, remoteShell: bool = None, restApi: bool = None, role: str = None, title: str = None) -> tuple[bool, None]:
 		'''
 		Class Users
 		Description: This API update user in the system. Use the input parameters to filter organization.
         
@@ -5079,27 +5087,26 @@
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		if username:
 			url_params.append('username=' + username)
 		url += '?' + '&'.join(url_params)
 
-		userRequest = {
-			"customScript": customScript,
-			"email": email,
-			"firstName": firstName,
-			"lastName": lastName,
-			"remoteShell": remoteShell,
-			"restApi": restApi,
-			"role": role,
-			"title": title,
-			"username": username,
-		}
-		return fortiedr_connection.insert(url, userRequest)
+		userRequest = {}
+		if customScript: userRequest["customScript"] = customScript
+		if email: userRequest["email"] = email
+		if firstName: userRequest["firstName"] = firstName
+		if lastName: userRequest["lastName"] = lastName
+		if remoteShell: userRequest["remoteShell"] = remoteShell
+		if restApi: userRequest["restApi"] = restApi
+		if role: userRequest["role"] = role
+		if title: userRequest["title"] = title
+		if username: userRequest["username"] = username
 
+		return fortiedr_connection.insert(url, userRequest)
 
 
 debug = None
 ssl_enabled = True
 organization = None
 api_json_params = None
```

### Comparing `fortiedr-3.6.8/fortiedr.egg-info/PKG-INFO` & `fortiedr-3.6.9/fortiedr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.6.8
+Version: 3.6.9
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.6.8/pyproject.toml` & `fortiedr-3.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fortiedr"
-version = "3.6.8"
+version = "3.6.9"
 authors = [
   { name="Rafael Foster", email="rafaelgfoster@gmail.com" }
 ]
 description = "This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fortiedr-3.6.8/setup.py` & `fortiedr-3.6.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 cur_dir = os.path.dirname(__file__)
 
 with open(f"{cur_dir}/requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="fortiedr",
-    version="3.6.8",
+    version="3.6.9",
     description="This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.",
     author="Rafael Foster",
     author_email="rafaelgfoster@gmail.com",
     project_urls={
         "GitHub": "https://github.com/rafaelfoster/fortiedr",
     },
     python_requires=">=3.8",
```

