# Comparing `tmp/asconnect-3.0.4.tar.gz` & `tmp/asconnect-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asconnect-3.0.4.tar", max compression
+gzip compressed data, was "asconnect-3.0.6.tar", max compression
```

## Comparing `asconnect-3.0.4.tar` & `asconnect-3.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1141 2024-02-21 04:09:12.268248 asconnect-3.0.4/LICENSE
--rw-r--r--   0        0        0     4502 2024-02-21 04:09:12.268248 asconnect-3.0.4/README.md
--rwxr-xr-x   0        0        0      297 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/__init__.py
--rw-r--r--   0        0        0     3165 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/altool.py
--rwxr-xr-x   0        0        0     4060 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/app_client.py
--rwxr-xr-x   0        0        0     5930 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/app_info_client.py
--rwxr-xr-x   0        0        0    10487 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/beta_review_client.py
--rwxr-xr-x   0        0        0     6296 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/build_client.py
--rwxr-xr-x   0        0        0     2301 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/client.py
--rw-r--r--   0        0        0     1301 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/exceptions.py
--rwxr-xr-x   0        0        0    12747 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/httpclient.py
--rw-r--r--   0        0        0      537 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/__init__.py
--rw-r--r--   0        0        0     2166 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/app_info.py
--rw-r--r--   0        0        0     4313 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/app_store.py
--rw-r--r--   0        0        0      933 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/app_store_version_localizations.py
--rw-r--r--   0        0        0     2721 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/apps.py
--rw-r--r--   0        0        0     1178 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/beta_app_review.py
--rw-r--r--   0        0        0     1866 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/beta_detail.py
--rw-r--r--   0        0        0     1277 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/beta_groups.py
--rw-r--r--   0        0        0     1225 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/builds.py
--rw-r--r--   0        0        0     1221 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/common.py
--rw-r--r--   0        0        0      978 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/idfa.py
--rw-r--r--   0        0        0     1373 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/localization.py
--rw-r--r--   0        0        0     4556 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/screenshots.py
--rw-r--r--   0        0        0     1364 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/models/users.py
--rwxr-xr-x   0        0        0     9963 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/screenshot_client.py
--rw-r--r--   0        0        0      352 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/sorting.py
--rwxr-xr-x   0        0        0     1216 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/users_client.py
--rw-r--r--   0        0        0     2219 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/utilities.py
--rwxr-xr-x   0        0        0    16470 2024-02-21 04:09:12.268248 asconnect-3.0.4/asconnect/version_client.py
--rw-r--r--   0        0        0     1343 2024-02-21 04:09:12.272248 asconnect-3.0.4/pyproject.toml
--rw-r--r--   0        0        0     5705 1970-01-01 00:00:00.000000 asconnect-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1141 2024-03-20 17:04:39.304362 asconnect-3.0.6/LICENSE
+-rw-r--r--   0        0        0     4502 2024-03-20 17:04:39.304727 asconnect-3.0.6/README.md
+-rwxr-xr-x   0        0        0      297 2024-03-20 17:04:39.305400 asconnect-3.0.6/asconnect/__init__.py
+-rw-r--r--   0        0        0     3165 2024-03-20 17:04:39.305654 asconnect-3.0.6/asconnect/altool.py
+-rwxr-xr-x   0        0        0     4098 2024-05-30 11:41:50.315538 asconnect-3.0.6/asconnect/app_client.py
+-rwxr-xr-x   0        0        0     5930 2024-03-20 17:04:39.306405 asconnect-3.0.6/asconnect/app_info_client.py
+-rwxr-xr-x   0        0        0    10677 2024-05-30 11:41:50.317673 asconnect-3.0.6/asconnect/beta_review_client.py
+-rwxr-xr-x   0        0        0     6296 2024-03-20 17:04:39.307189 asconnect-3.0.6/asconnect/build_client.py
+-rwxr-xr-x   0        0        0     2301 2024-03-20 17:04:39.307443 asconnect-3.0.6/asconnect/client.py
+-rw-r--r--   0        0        0     1301 2024-03-20 17:04:39.307694 asconnect-3.0.6/asconnect/exceptions.py
+-rwxr-xr-x   0        0        0    12747 2024-03-20 17:04:39.308046 asconnect-3.0.6/asconnect/httpclient.py
+-rw-r--r--   0        0        0      537 2024-03-20 17:04:39.308619 asconnect-3.0.6/asconnect/models/__init__.py
+-rw-r--r--   0        0        0     2176 2024-05-30 11:41:50.320253 asconnect-3.0.6/asconnect/models/app_info.py
+-rw-r--r--   0        0        0     4340 2024-05-30 11:41:50.322414 asconnect-3.0.6/asconnect/models/app_store.py
+-rw-r--r--   0        0        0      933 2024-03-20 17:04:39.309813 asconnect-3.0.6/asconnect/models/app_store_version_localizations.py
+-rw-r--r--   0        0        0     2721 2024-03-20 17:04:39.310080 asconnect-3.0.6/asconnect/models/apps.py
+-rw-r--r--   0        0        0     1178 2024-03-20 17:04:39.310368 asconnect-3.0.6/asconnect/models/beta_app_review.py
+-rw-r--r--   0        0        0     1866 2024-03-20 17:04:39.310669 asconnect-3.0.6/asconnect/models/beta_detail.py
+-rw-r--r--   0        0        0     1277 2024-03-20 17:04:39.312437 asconnect-3.0.6/asconnect/models/beta_groups.py
+-rw-r--r--   0        0        0     1225 2024-03-20 17:04:39.313388 asconnect-3.0.6/asconnect/models/builds.py
+-rw-r--r--   0        0        0     1221 2024-03-20 17:04:39.313649 asconnect-3.0.6/asconnect/models/common.py
+-rw-r--r--   0        0        0      978 2024-03-20 17:04:39.313953 asconnect-3.0.6/asconnect/models/idfa.py
+-rw-r--r--   0        0        0     1373 2024-03-20 17:04:39.314170 asconnect-3.0.6/asconnect/models/localization.py
+-rw-r--r--   0        0        0     4556 2024-03-20 17:04:39.314443 asconnect-3.0.6/asconnect/models/screenshots.py
+-rw-r--r--   0        0        0     1364 2024-03-20 17:04:39.314681 asconnect-3.0.6/asconnect/models/users.py
+-rwxr-xr-x   0        0        0     9963 2024-03-20 17:04:39.314943 asconnect-3.0.6/asconnect/screenshot_client.py
+-rw-r--r--   0        0        0      352 2024-03-20 17:04:39.315183 asconnect-3.0.6/asconnect/sorting.py
+-rwxr-xr-x   0        0        0     1216 2024-03-20 17:04:39.315482 asconnect-3.0.6/asconnect/users_client.py
+-rw-r--r--   0        0        0     2220 2024-05-30 11:41:50.323834 asconnect-3.0.6/asconnect/utilities.py
+-rwxr-xr-x   0        0        0    16936 2024-05-30 11:41:50.326435 asconnect-3.0.6/asconnect/version_client.py
+-rw-r--r--   0        0        0     1339 2024-05-30 11:41:50.331491 asconnect-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5705 1970-01-01 00:00:00.000000 asconnect-3.0.6/PKG-INFO
```

### Comparing `asconnect-3.0.4/LICENSE` & `asconnect-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/README.md` & `asconnect-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/altool.py` & `asconnect-3.0.6/asconnect/altool.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/app_client.py` & `asconnect-3.0.6/asconnect/app_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,17 @@
             "platform": platform.value,
             "versionString": version,
             "releaseType": release_type.value,
         }
 
         if release_type == ReleaseType.SCHEDULED:
             if not earliest_release_date:
-                raise TypeError("earliest_release_date must be supplied when release_type is SCHEDULED")
+                raise TypeError(
+                    "earliest_release_date must be supplied when release_type is SCHEDULED"
+                )
             attributes["earliestReleaseDate"] = earliest_release_date
 
         if copyright_text:
             attributes["copyright"] = copyright_text
 
         if uses_idfa is not None:
             attributes["usesIdfa"] = uses_idfa
```

### Comparing `asconnect-3.0.4/asconnect/app_info_client.py` & `asconnect-3.0.6/asconnect/app_info_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/beta_review_client.py` & `asconnect-3.0.6/asconnect/beta_review_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         :param http_client: The API HTTP client
         :param log: Any base logger to be used (one will be created if not supplied)
         """
 
         self.http_client = http_client
         self.log = log.getChild("beta_review")
 
+    # pylint:disable=too-many-arguments
     def set_beta_app_review_details(
         self,
         *,
         app_id: str,
         contact_email: str,
         contact_first_name: str,
         contact_last_name: str,
@@ -82,22 +83,32 @@
 
         if demo_account_required is not None:
             attributes["demoAccountRequired"] = demo_account_required
 
         if notes is not None:
             attributes["notes"] = notes
 
-        body = {"data": {"attributes": attributes, "id": app_id, "type": "betaAppReviewDetails"}}
+        body = {
+            "data": {
+                "attributes": attributes,
+                "id": app_id,
+                "type": "betaAppReviewDetails",
+            }
+        }
 
         self.log.debug(f"Beta review details: {body}")
 
         return self.http_client.patch(
-            endpoint=f"betaAppReviewDetails/{app_id}", data=body, data_type=BetaAppReviewDetail
+            endpoint=f"betaAppReviewDetails/{app_id}",
+            data=body,
+            data_type=BetaAppReviewDetail,
         )
 
+    # pylint:enable=too-many-arguments
+
     def get_beta_app_localizations(self, app_id: str) -> Iterator[BetaAppLocalization]:
         """Get the beta app localizations.
 
         :param app_id: The apple identifier for the app to get the localizations for
 
         :returns: An iterator to the beta app localizations
         """
```

### Comparing `asconnect-3.0.4/asconnect/build_client.py` & `asconnect-3.0.6/asconnect/build_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/client.py` & `asconnect-3.0.6/asconnect/client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/exceptions.py` & `asconnect-3.0.6/asconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/httpclient.py` & `asconnect-3.0.6/asconnect/httpclient.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/__init__.py` & `asconnect-3.0.6/asconnect/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/app_info.py` & `asconnect-3.0.6/asconnect/models/app_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,14 @@
     @deserialize.key("brazil_age_rating", "brazilAgeRating")
     @deserialize.key("kids_age_band", "kidsAgeBand")
     class Attributes(BaseAttributes):
         """Represents app info localization attributes."""
 
         app_store_age_rating: AppStoreAgeRating
         app_store_state: AppStoreVersionState
-        brazil_age_rating: BrazilAgeRating
+        brazil_age_rating: Optional[BrazilAgeRating]
         kids_age_band: Optional[KidsAgeBand]
 
     identifier: str
     attributes: Attributes
     relationships: Optional[Dict[str, Relationship]]
     links: Links
```

### Comparing `asconnect-3.0.4/asconnect/models/app_store.py` & `asconnect-3.0.6/asconnect/models/app_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 class Platform(enum.Enum):
     """The different platforms an app can be for."""
 
     IOS = "IOS"
     MACOS = "MAC_OS"
     TVOS = "TV_OS"
+    VISIONOS = "VISION_OS"
 
 
 class ReleaseType(enum.Enum):
     """App store release type."""
 
     MANUAL = "MANUAL"
     AFTER_APPROVAL = "AFTER_APPROVAL"
```

### Comparing `asconnect-3.0.4/asconnect/models/app_store_version_localizations.py` & `asconnect-3.0.6/asconnect/models/app_store_version_localizations.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/apps.py` & `asconnect-3.0.6/asconnect/models/apps.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/beta_app_review.py` & `asconnect-3.0.6/asconnect/models/beta_app_review.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/beta_detail.py` & `asconnect-3.0.6/asconnect/models/beta_detail.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/beta_groups.py` & `asconnect-3.0.6/asconnect/models/beta_groups.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/builds.py` & `asconnect-3.0.6/asconnect/models/builds.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/common.py` & `asconnect-3.0.6/asconnect/models/common.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/idfa.py` & `asconnect-3.0.6/asconnect/models/idfa.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/localization.py` & `asconnect-3.0.6/asconnect/models/localization.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/screenshots.py` & `asconnect-3.0.6/asconnect/models/screenshots.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/models/users.py` & `asconnect-3.0.6/asconnect/models/users.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/screenshot_client.py` & `asconnect-3.0.6/asconnect/screenshot_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/users_client.py` & `asconnect-3.0.6/asconnect/users_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.4/asconnect/utilities.py` & `asconnect-3.0.6/asconnect/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import hashlib
 import os
 from typing import Dict, Iterator, Optional, TypeVar
 import urllib.parse
 
 IteratorType = TypeVar("IteratorType")  # pylint: disable=invalid-name
 
+
 def next_or_none(iterator: Iterator[IteratorType]) -> Optional[IteratorType]:
     """Get the next value from an iterator, or return None when it is exhausted.
 
     :param iterator: The iterator to get the next value from
 
     :returns: The next value or None if exhausted
     """
```

### Comparing `asconnect-3.0.4/asconnect/version_client.py` & `asconnect-3.0.6/asconnect/version_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,14 +251,15 @@
         return next_or_none(
             self.http_client.get(
                 endpoint=f"appStoreVersions/{version_id}/appStoreReviewDetail",
                 data_type=AppStoreReviewDetails,
             )
         )
 
+    # pylint:disable=too-many-arguments
     def set_app_review_details(
         self,
         *,
         version_id: str,
         contact_email: str,
         contact_first_name: str,
         contact_last_name: str,
@@ -323,14 +324,16 @@
                         "appStoreVersion": {"data": {"type": "appStoreVersions", "id": version_id}}
                     },
                 }
             },
             data_type=AppStoreReviewDetails,
         )
 
+    # pylint:enable=too-many-arguments
+
     def get_idfa(self, *, version_id: str) -> Optional[IdfaDeclaration]:
         """Get the advertising ID declaration.
 
         :param version_id: The version to get the declaration for
 
         :returns: The declaration if set, None otherwise
         """
@@ -433,37 +436,50 @@
             data_type=AppStoreVersion,
         )
 
     def submit_for_review(
         self,
         *,
         version_id: str,
+        platform: Platform = Platform.IOS,
         attempt: int = 1,
         max_attempts: int = 3,
     ) -> None:
         """Submit the version for review
 
         :param version_id: The ID of the version to submit for review
+        :param platform: The platform the app is for
         :param attempt: The attempt this is
         :param max_attempts: The number of attempts allowed
         """
 
-        self.log.info(f"Submitting version for review {version_id}")
+        self.log.info(f"Submitting version for review {version_id}, platform: {platform}")
 
         try:
             self.http_client.post(
-                endpoint="appStoreVersionSubmissions",
+                endpoint="reviewSubmissions",
                 data={
                     "data": {
-                    "type": "appStoreVersionSubmissions",
-                    "relationships": {
-                        "appStoreVersion": {"data": {"type": "appStoreVersions", "id": version_id}}
-                    },
-                }
-            },
+                        "type": "reviewSubmissions",
+                        "attributes": {
+                            "platform": platform.value
+                        },
+                        "relationships": {
+                            "app": {
+                                "data": {"type": "apps", "id": version_id}
+                            }
+                        },
+                    }
+                },
                 data_type=None,
             )
         except AppStoreConnectError as ex:
-            if attempt < max_attempts and ex.response.status_code >= 500 and ex.response.status_code < 600:
-                self.log.info("Submit failed due to server-side intermittent issue. Will sleep for 1 minute and try again.")
+            if (
+                attempt < max_attempts
+                and ex.response.status_code >= 500
+                and ex.response.status_code < 600
+            ):
+                self.log.info(
+                    "Submit failed due to server-side intermittent issue. Will sleep for 1 minute and try again."
+                )
                 time.sleep(60)
                 self.submit_for_review(version_id=version_id)
```

### Comparing `asconnect-3.0.4/pyproject.toml` & `asconnect-3.0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asconnect"
-version = "3.0.4"
+version = "3.0.6"
 description = "A wrapper around the Apple App Store Connect APIs"
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dalemy@microsoft.com>"
 ]
@@ -35,19 +35,19 @@
 cryptography = ">=40,<43"
 deserialize = "^2.0.1"
 pyjwt = "^2.6.0"
 requests = "^2.28.2"
 tenacity = "^8.2.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
-mypy = "^1.1.1"
-pylint = "^2.17.1"
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
+black = "24.3.0"
+mypy = "1.9.0"
+pylint = "3.1.0"
+pytest = "^8.1.1"
+pytest-cov = "^4.1.0"
 pytest-dependency = "^0.5.1"
 types-requests = "^2.28.11.16"
 
 [[tool.mypy.overrides]]
 module = [
     "deserialize"
 ]
```

### Comparing `asconnect-3.0.4/PKG-INFO` & `asconnect-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asconnect
-Version: 3.0.4
+Version: 3.0.6
 Summary: A wrapper around the Apple App Store Connect APIs
 Home-page: https://github.com/microsoft/asconnect
 License: MIT
 Keywords: apple,app store,itunes,connect
 Author: Dale Myers
 Author-email: dalemy@microsoft.com
 Requires-Python: >=3.8,<4.0
```

