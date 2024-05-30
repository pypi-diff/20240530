# Comparing `tmp/shipyard_api-0.2.0a2.tar.gz` & `tmp/shipyard_api-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_api-0.2.0a2.tar", max compression
+gzip compressed data, was "shipyard_api-0.3.0a0.tar", max compression
```

## Comparing `shipyard_api-0.2.0a2.tar` & `shipyard_api-0.3.0a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-18 20:05:24.210595 shipyard_api-0.2.0a2/README.md
--rw-r--r--   0        0        0      538 2024-05-14 13:34:40.631138 shipyard_api-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0       35 2024-04-18 20:05:24.211332 shipyard_api-0.2.0a2/shipyard_api/__init__.py
--rw-r--r--   0        0        0      695 2024-05-06 20:06:59.600682 shipyard_api-0.2.0a2/shipyard_api/cli/authtest.py
--rw-r--r--   0        0        0     1443 2024-04-18 20:05:24.211506 shipyard_api-0.2.0a2/shipyard_api/cli/get_logs.py
--rw-r--r--   0        0        0     2397 2024-05-13 18:01:57.037107 shipyard_api-0.2.0a2/shipyard_api/cli/trigger_fleet.py
--rw-r--r--   0        0        0    10366 2024-05-14 13:34:40.623911 shipyard_api-0.2.0a2/shipyard_api/client.py
--rw-r--r--   0        0        0     1099 2024-05-14 13:34:40.615839 shipyard_api-0.2.0a2/shipyard_api/errors.py
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 shipyard_api-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 20:05:24.210595 shipyard_api-0.3.0a0/README.md
+-rw-r--r--   0        0        0      538 2024-05-30 14:14:32.433965 shipyard_api-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-04-18 20:05:24.211332 shipyard_api-0.3.0a0/shipyard_api/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-06 20:06:59.600682 shipyard_api-0.3.0a0/shipyard_api/cli/authtest.py
+-rw-r--r--   0        0        0     1490 2024-05-30 14:20:37.889448 shipyard_api-0.3.0a0/shipyard_api/cli/get_logs.py
+-rw-r--r--   0        0        0     2397 2024-05-13 18:01:57.037107 shipyard_api-0.3.0a0/shipyard_api/cli/trigger_fleet.py
+-rw-r--r--   0        0        0    10850 2024-05-30 14:20:37.927142 shipyard_api-0.3.0a0/shipyard_api/client.py
+-rw-r--r--   0        0        0     1149 2024-05-22 14:23:26.310032 shipyard_api-0.3.0a0/shipyard_api/errors.py
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 shipyard_api-0.3.0a0/PKG-INFO
```

### Comparing `shipyard_api-0.2.0a2/pyproject.toml` & `shipyard_api-0.3.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-api"
-version = "0.2.0a2"
+version = "0.3.0a0"
 description = ""
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
```

### Comparing `shipyard_api-0.2.0a2/shipyard_api/cli/authtest.py` & `shipyard_api-0.3.0a0/shipyard_api/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.2.0a2/shipyard_api/cli/get_logs.py` & `shipyard_api-0.3.0a0/shipyard_api/cli/get_logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import argparse
 import sys
+
 import shipyard_bp_utils as utils
-from shipyard_api import ShipyardClient
 from shipyard_templates import ShipyardLogger, ExitCodeException
+
+from shipyard_api import ShipyardClient
 from shipyard_api.errors import EXIT_CODE_UNKNOWN_ERROR
 
 logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--organization-id", dest="org_id", required=True)
     parser.add_argument("--api-key", dest="api_key", required=True)
     parser.add_argument("--file-name", dest="file_name", required=True)
     parser.add_argument("--folder-name", dest="folder_name", required=False, default="")
+    parser.add_argument("--days", dest="days", required=False)
     return parser.parse_args()
 
 
 def main():
     try:
         args = get_args()
-        org_id = args.org_id
-        api_key = args.api_key
-        file_name = args.file_name
         folder_name = args.folder_name
         if folder_name:
             utils.files.create_folder_if_dne(folder_name)
-        target_path = utils.files.combine_folder_and_file_name(folder_name, file_name)
-        shipyard = ShipyardClient(org_id=org_id, api_key=api_key)
-        shipyard.export_voyages(target_path)
-        logger.info("Successfully exported fleet runs to ")
+        target_path = utils.files.combine_folder_and_file_name(
+            folder_name, args.file_name
+        )
+
+        shipyard = ShipyardClient(org_id=args.org_id, api_key=args.api_key)
+        shipyard.export_voyages(target_path, num_of_days=args.days)
+
+        logger.info(f"Successfully exported fleet runs to {target_path}")
+
     except ExitCodeException as ec:
         logger.error(ec.message)
         sys.exit(ec.exit_code)
     except Exception as e:
         logger.error(f"An unexpected error occurred: {e}")
         sys.exit(EXIT_CODE_UNKNOWN_ERROR)
```

### Comparing `shipyard_api-0.2.0a2/shipyard_api/cli/trigger_fleet.py` & `shipyard_api-0.3.0a0/shipyard_api/cli/trigger_fleet.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.2.0a2/shipyard_api/client.py` & `shipyard_api-0.3.0a0/shipyard_api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,33 +8,38 @@
 from shipyard_templates import ShipyardLogger, ExitCodeException
 
 from shipyard_api.errors import (
     EXIT_CODE_LIST_FLEET_RUNS_ERROR,
     EXIT_CODE_VOYAGE_EXPORT_ERROR,
     EXIT_CODE_TRIGGER_FLEET_ERROR,
     EXIT_CODE_UNKNOWN_ERROR,
+    EXIT_CODE_FLEET_RUN_DETAILS_ERROR,
     InvalidFileType,
     MissingProjectID,
     UnauthorizedAccess,
-
 )
 
 logger = ShipyardLogger.get_logger()
 
 
 class ShipyardClient:
     def __init__(self, org_id: str, api_key: str, project_id: Optional[str] = None):
         self.org_id = org_id
         self.api_key = api_key
         self.base_url = f"https://api.app.shipyardapp.com/orgs/{org_id}"
         self.headers = {"X-Shipyard-API-Key": self.api_key}
         self.project_id = project_id
 
-    def _request(self, method: str, url: str, data: Optional[Dict[str, Any]] = None,
-                 headers: Optional[Dict[str, Any]] = None):
+    def _request(
+        self,
+        method: str,
+        url: str,
+        data: Optional[Dict[str, Any]] = None,
+        headers: Optional[Dict[str, Any]] = None,
+    ):
         """
         A helper method to make requests to the Shipyard API.
 
         Args:
             method (str): The HTTP method to use.
             url (str): The URL to make the request to.
             data (Optional[Dict[str, Any]]): The data to send with the request.
@@ -46,19 +51,15 @@
         Raises:
             ExitCodeException: If an error occurs during the request.
             UnauthorizedAccess: If the API returns a 401 status code.
         """
         if headers is None:
             headers = self.headers
 
-        request_args = {
-            "method": method,
-            "url": url,
-            "headers": headers
-        }
+        request_args = {"method": method, "url": url, "headers": headers}
         if data:
             request_args["data"] = data
         response = None
         try:
 
             response = requests.request(**request_args)
             if response.ok:
@@ -100,15 +101,15 @@
                 f"Error fetching fleet runs: {e}",
                 exit_code=EXIT_CODE_LIST_FLEET_RUNS_ERROR,
             ) from e
         else:
             return response.json()
 
     def export_fleet_runs(
-            self, fleet_id: str, target_path: str, file_type: str = "csv"
+        self, fleet_id: str, target_path: str, file_type: str = "csv"
     ):
         """
         Export fleet runs to a file.
 
         Args:
             fleet_id (str): The ID of the fleet.
             target_path (str): The path to the target file.
@@ -135,26 +136,32 @@
                 raise InvalidFileType
         except ExitCodeException:
             raise
 
         except Exception as e:
             logger.error(f"Error exporting fleet runs: {e}")
 
-    def get_voyages(self):
+    def get_voyages(self, num_of_days: int = None):
         """
         Retrieves the voyages from the shipyard API.
 
+        Args:
+            num_of_days (int): The number of days to retrieve the voyages for.
+
         Returns:
             str: The response text from the API.
 
         Raises:
             ExitCodeException: If an exit code exception occurs.
             UnauthorizedAccess: If the API returns a 401 status code.
         """
         url = f"{self.base_url}/voyages"
+        if num_of_days:
+            url += f"?days={num_of_days}"
+
         try:
             response = requests.get(url, headers=self.headers)
             logger.debug(f"Status code for fleet runs {response.status_code}")
 
             response.raise_for_status()
         except Exception as e:
             logger.debug(f"Error fetching logs: {e}")
@@ -163,27 +170,28 @@
             raise ExitCodeException(
                 f"Error fetching fleet runs: {e}",
                 exit_code=EXIT_CODE_LIST_FLEET_RUNS_ERROR,
             ) from e
         else:
             return response.text
 
-    def export_voyages(self, target_path: str):
+    def export_voyages(self, target_path: str, num_of_days: int = None):
         """
         Export voyages data to a file.
 
         Args:
             target_path (str): The path of the file to export the voyages data to.
+            num_of_days (int): The number of days to retrieve the voyages for.
 
         Raises:
             ExitCodeException: If an error occurs during the export process.
 
         """
         try:
-            data = self.get_voyages()
+            data = self.get_voyages(num_of_days)
             with open(target_path, "w") as f:
                 f.write(data)
                 logger.debug("Successfully exported voyages")
         except ExitCodeException:
             raise
 
         except Exception as e:
@@ -209,16 +217,16 @@
         logger.debug(f"Attempting to trigger fleet run for fleet {fleet_id}")
         request_details = {
             "method": "POST",
             "url": f"{self.base_url}/projects/{self.project_id}/fleets/{fleet_id}/fleetruns",
             "headers": {
                 "accept": "application/json",
                 "content-type": "application/json",
-                "X-Shipyard-API-Key": self.api_key
-            }
+                "X-Shipyard-API-Key": self.api_key,
+            },
         }
 
         if fleet_overrides:
             logger.info("Triggering fleet run with overrides")
             request_details["data"] = fleet_overrides
         else:
             logger.info("Triggering fleet run...")
@@ -243,56 +251,66 @@
         Returns:
             requests.Response: The response from the API.
 
         Raises:
             ExitCodeException: If an exit code exception occurs.
         """
         try:
-            response = self._request(method="PUT",
-                                     url=f"{self.base_url}/projects/{self.project_id}/fleets",
-                                     headers={
-                                         "accept": "application/json",
-                                         "content-type": "application/json",
-                                         "X-Shipyard-API-Key": self.api_key
-                                     },
-                                     data=yaml.dump(fleet_yaml)
-                                     )
+            response = self._request(
+                method="PUT",
+                url=f"{self.base_url}/projects/{self.project_id}/fleets",
+                headers={
+                    "accept": "application/json",
+                    "content-type": "application/json",
+                    "X-Shipyard-API-Key": self.api_key,
+                },
+                data=yaml.dump(fleet_yaml),
+            )
             logger.info("Successfully upserted fleet")
             return response
 
         except ExitCodeException:
             raise
         except Exception as e:
             raise ExitCodeException(
                 f"Error upserting fleet: {e}",
                 exit_code=EXIT_CODE_UNKNOWN_ERROR,
             ) from e
 
-
     def get_run_status(self, fleet_id: str, run_id: str):
         """
         Get the status of a fleet run.
 
         Args:
             fleet_id (str): The ID of the fleet.
             run_id (str): The ID of the run.
 
         Returns:
             str: The status of the fleet run.
 
         Raises:
             ExitCodeException: If an exit code exception occurs.
         """
-
-        response = self._request("GET", f"{self.base_url}/projects/{self.project_id}/fleets/{fleet_id}/fleetruns",
-                                 headers={
-                                     "accept": "application/json",
-                                     "content-type": "application/json",
-                                     "X-Shipyard-API-Key": self.api_key
-                                 }
-                                 )
-
-        log_data = response.content.decode('utf-8')
-
-        df = pandas.read_csv(io.StringIO(log_data))
-        fleet_run = df[df['Fleet Log ID'] == run_id]
-        return fleet_run["Status"].values[0]
+        try:
+            response = self._request(
+                "GET",
+                f"{self.base_url}/projects/{self.project_id}/fleets/{fleet_id}/fleetruns",
+                headers={
+                    "accept": "application/json",
+                    "content-type": "application/json",
+                    "X-Shipyard-API-Key": self.api_key,
+                },
+            )
+
+            log_data = response.content.decode("utf-8")
+
+            df = pandas.read_csv(io.StringIO(log_data))
+            fleet_run = df[df["Fleet Log ID"] == run_id]
+            return fleet_run["Status"].values[0]
+        except ExitCodeException:
+            raise
+        except Exception as e:
+            raise ExitCodeException(
+                f"Error getting fleet run status. Confirm the fleet_id and run_id are valid and try again. "
+                f"Message from server: {e}",
+                exit_code=EXIT_CODE_FLEET_RUN_DETAILS_ERROR,
+            ) from e
```

### Comparing `shipyard_api-0.2.0a2/shipyard_api/errors.py` & `shipyard_api-0.3.0a0/shipyard_api/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 EXIT_CODE_LIST_FLEET_RUNS_ERROR = 104
 EXIT_CODE_LIST_VOYAGES_ERROR = 105
 EXIT_CODE_VOYAGE_EXPORT_ERROR = 106
 EXIT_CODE_TRIGGER_FLEET_ERROR = 107
 EXIT_CODE_ARTIFACTS_ERROR = 108
 EXIT_CODE_FLEET_FINAL_STATE_ERROR = 109
 EXIT_CODE_FLEET_UPSERT_ERROR = 110
+EXIT_CODE_FLEET_RUN_DETAILS_ERROR = 111
 EXIT_CODE_UNKNOWN_ERROR = 249
 
 
 class MissingProjectID(ExitCodeException):
     def __init__(self):
         self.message = "Project ID is required in order to perform this operation"
         self.exit_code = EXIT_CODE_MISSING_PROJECT_ID
@@ -23,10 +24,12 @@
     def __init__(self):
         self.message = "Invalid file type, valid choices are csv and json"
         self.exit_code = 102
 
 
 class UnauthorizedAccess(ExitCodeException):
     def __init__(self):
-        self.message = ("Unauthorized access, ensure that your API key has the correct access for the fleet and "
-                        "project provided")
+        self.message = (
+            "Unauthorized access, ensure that your API key has the correct access for the fleet and "
+            "project provided"
+        )
         self.exit_code = EXIT_CODE_UNAUTHORIZED_ACCESS
```

### Comparing `shipyard_api-0.2.0a2/PKG-INFO` & `shipyard_api-0.3.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-api
-Version: 0.2.0a2
+Version: 0.3.0a0
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

