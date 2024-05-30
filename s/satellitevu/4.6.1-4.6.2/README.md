# Comparing `tmp/satellitevu-4.6.1.tar.gz` & `tmp/satellitevu-4.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellitevu-4.6.1.tar", max compression
+gzip compressed data, was "satellitevu-4.6.2.tar", max compression
```

## Comparing `satellitevu-4.6.1.tar` & `satellitevu-4.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1080 2024-04-26 13:10:23.664295 satellitevu-4.6.1/LICENSE
--rw-r--r--   0        0        0     3934 2024-04-26 13:10:23.664295 satellitevu-4.6.1/README.md
--rw-r--r--   0        0        0     1082 2024-04-26 13:10:33.340248 satellitevu-4.6.1/pyproject.toml
--rw-r--r--   0        0        0       80 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/archive.py
--rw-r--r--   0        0        0     3012 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/archive_test.py
--rw-r--r--   0        0        0     1519 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/base.py
--rw-r--r--   0        0        0     1287 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/base_test.py
--rw-r--r--   0        0        0     3788 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/catalog.py
--rw-r--r--   0        0        0     3123 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/catalog_test.py
--rw-r--r--   0        0        0     1331 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/contracts.py
--rw-r--r--   0        0        0      814 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/exceptions.py
--rw-r--r--   0        0        0     7623 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/orders.py
--rw-r--r--   0        0        0    11483 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/orders_test.py
--rw-r--r--   0        0        0    24308 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/apis/otm.py
--rw-r--r--   0        0        0    13873 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/apis/otm_test.py
--rw-r--r--   0        0        0      149 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/__init__.py
--rw-r--r--   0        0        0     2799 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/auth.py
--rw-r--r--   0        0        0     1664 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/auth_test.py
--rw-r--r--   0        0        0     1956 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/cache.py
--rw-r--r--   0        0        0     2144 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/cache_test.py
--rw-r--r--   0        0        0      122 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/exc.py
--rw-r--r--   0        0        0     3004 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/client.py
--rw-r--r--   0        0        0     1363 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/config.py
--rw-r--r--   0        0        0     5073 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/conftest.py
--rw-r--r--   0        0        0      148 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/__init__.py
--rw-r--r--   0        0        0     2038 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/base.py
--rw-r--r--   0        0        0     3327 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/http_test.py
--rw-r--r--   0        0        0     1305 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/httpx.py
--rw-r--r--   0        0        0     1334 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/requests.py
--rw-r--r--   0        0        0     1744 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/urllib.py
--rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 satellitevu-4.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-30 14:20:41.891547 satellitevu-4.6.2/LICENSE
+-rw-r--r--   0        0        0     3934 2024-05-30 14:20:41.891547 satellitevu-4.6.2/README.md
+-rw-r--r--   0        0        0     1082 2024-05-30 14:20:51.451688 satellitevu-4.6.2/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/__init__.py
+-rw-r--r--   0        0        0     3050 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/archive.py
+-rw-r--r--   0        0        0     3012 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/archive_test.py
+-rw-r--r--   0        0        0     1519 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/base.py
+-rw-r--r--   0        0        0     1287 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/base_test.py
+-rw-r--r--   0        0        0     3788 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/catalog.py
+-rw-r--r--   0        0        0     3123 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/catalog_test.py
+-rw-r--r--   0        0        0     1331 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/contracts.py
+-rw-r--r--   0        0        0      814 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/exceptions.py
+-rw-r--r--   0        0        0     7623 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/orders.py
+-rw-r--r--   0        0        0    11483 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/orders_test.py
+-rw-r--r--   0        0        0    24687 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/otm.py
+-rw-r--r--   0        0        0    13941 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/apis/otm_test.py
+-rw-r--r--   0        0        0      149 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/auth/__init__.py
+-rw-r--r--   0        0        0     2799 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/auth/auth.py
+-rw-r--r--   0        0        0     1664 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/auth/auth_test.py
+-rw-r--r--   0        0        0     1956 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/auth/cache.py
+-rw-r--r--   0        0        0     2144 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/auth/cache_test.py
+-rw-r--r--   0        0        0      122 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/auth/exc.py
+-rw-r--r--   0        0        0     3004 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/client.py
+-rw-r--r--   0        0        0     1363 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/config.py
+-rw-r--r--   0        0        0     5073 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/conftest.py
+-rw-r--r--   0        0        0      148 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/http/__init__.py
+-rw-r--r--   0        0        0     2038 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/http/base.py
+-rw-r--r--   0        0        0     3327 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/http/http_test.py
+-rw-r--r--   0        0        0     1305 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/http/httpx.py
+-rw-r--r--   0        0        0     1334 2024-05-30 14:20:41.891547 satellitevu-4.6.2/satellitevu/http/requests.py
+-rw-r--r--   0        0        0     1744 2024-05-30 14:20:41.895547 satellitevu-4.6.2/satellitevu/http/urllib.py
+-rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 satellitevu-4.6.2/PKG-INFO
```

### Comparing `satellitevu-4.6.1/LICENSE` & `satellitevu-4.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/README.md` & `satellitevu-4.6.2/README.md`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/pyproject.toml` & `satellitevu-4.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "satellitevu"
-version = "4.6.1"
+version = "4.6.2"
 description = "Client SDK for SatelliteVu's platform APIs"
 authors = ["Christian Wygoda <christian.wygoda@satellitevu.com>", "Zhelini Sivanesan <zhelini.sivanesan@satellitevu.com>", "James Harrison <james.harrison@satellitevu.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `satellitevu-4.6.1/satellitevu/apis/archive.py` & `satellitevu-4.6.2/satellitevu/apis/archive.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/apis/archive_test.py` & `satellitevu-4.6.2/satellitevu/apis/archive_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/apis/base.py` & `satellitevu-4.6.2/satellitevu/apis/base.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/apis/base_test.py` & `satellitevu-4.6.2/satellitevu/apis/base_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/apis/catalog.py` & `satellitevu-4.6.2/satellitevu/apis/catalog.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/apis/catalog_test.py` & `satellitevu-4.6.2/satellitevu/apis/catalog_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/apis/contracts.py` & `satellitevu-4.6.2/satellitevu/apis/contracts.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/apis/exceptions.py` & `satellitevu-4.6.2/satellitevu/apis/exceptions.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/apis/orders.py` & `satellitevu-4.6.2/satellitevu/apis/orders.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/apis/orders_test.py` & `satellitevu-4.6.2/satellitevu/apis/orders_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/apis/otm.py` & `satellitevu-4.6.2/satellitevu/apis/otm.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,17 @@
         )
         return response.json()
 
     def create_order(
         self,
         *,
         contract_id: Union[UUID, str],
-        coordinates: Union[Tuple[float, float], Tuple[float, float, float]],
+        coordinates: Optional[
+            Union[Tuple[float, float], Tuple[float, float, float]]
+        ] = None,
         date_from: Optional[datetime] = None,
         date_to: Optional[datetime] = None,
         day_night_mode: Literal["day", "night", "day-night"] = "day-night",
         product: Literal["standard", "assured"] = "standard",
         max_cloud_cover: Optional[int] = MAX_CLOUD_COVER_DEFAULT,
         min_off_nadir: Optional[int] = None,
         max_off_nadir: Optional[int] = None,
@@ -244,15 +246,16 @@
         Creates a tasking order request.
 
         Args:
             contract_id: Associated ID of the Contract under which the tasking
             order will be submitted.
 
             coordinates: An array of coordinates - (longitude, latitude) or
-            (longitude, latitude, altitude).
+            (longitude, latitude, altitude). Only required for orders with
+            standard priority. Defaults to None.
 
             date_from: Datetime representing the start date of the order. Required
             for orders with standard priority. Defaults to None.
 
             date_to: Datetime representing the end date of the order. Required for
             orders with standard priority. Defaults to None
 
@@ -297,55 +300,60 @@
             added to this SDK yet.
 
         Returns:
             A dictionary containing properties of the order created.
         """
         url = self.url(f"{str(contract_id)}/tasking/orders/")
 
+        payload = {"properties": {"product": product}}
+
         if product == "standard":
+            if not "coordinates":
+                raise OTMParametersError(
+                    "`coordinates` must be specified for a standard priority order"
+                )
             if not date_from or not date_to:
                 raise OTMParametersError(
                     "`date_to` and `date_from` must be specified for a standard "
                     "priority order"
                 )
 
             if not any([min_gsd, max_gsd, min_off_nadir, max_off_nadir]):
                 raise OTMParametersError(
                     "One pair of Off Nadir or GSD values must be specified for a "
                     "standard priority order."
                 )
 
-        payload = {
-            "type": "Feature",
-            "geometry": {
-                "type": "Point",
-                "coordinates": coordinates,
-            },
-            "properties": {
-                "product": product,
-                **kwargs,
-            },
-        }
-
         if product == "assured":
             if not signature:
                 raise Exception(
-                    "Orders with assured priority must also have a signature token."
+                    "Orders with assured priority must have a signature token."
                 )
             payload["properties"].update({"signature": signature})
 
         else:
             payload["properties"].update(
                 {
                     "datetime": f"{date_from.isoformat()}/{date_to.isoformat()}",
                     "satvu:day_night_mode": day_night_mode,
                     "max_cloud_cover": max_cloud_cover,
                 }
             )
 
+            payload.update(
+                {
+                    "type": "Feature",
+                    "geometry": {
+                        "type": "Point",
+                        "coordinates": coordinates,
+                    },
+                }
+            )
+            payload["properties"].update(kwargs)
+
             for k, v in {
                 "min_off_nadir": min_off_nadir,
                 "max_off_nadir": max_off_nadir,
                 "min_gsd": min_gsd,
                 "max_gsd": max_gsd,
             }.items():
                 if v is None:
```

### Comparing `satellitevu-4.6.1/satellitevu/apis/otm_test.py` & `satellitevu-4.6.2/satellitevu/apis/otm_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,26 +243,27 @@
     api_request = requests[-1]
     assert api_request.headers["Host"] == urlparse(client._gateway_url).hostname
     assert api_request.path == "/" + api_path
     assert api_request.headers["Content-Type"] == "application/json"
     assert api_request.headers["Authorization"] == "Bearer mock-token"
 
     api_request_body = loads(api_request.body)
-    assert api_request_body["geometry"] == {
-        "type": "Point",
-        "coordinates": otm_request_parameters["coordinates"],
-    }
 
     properties_keys = ["max_cloud_cover", "min_off_nadir", "max_off_nadir"]
 
     if product == "assured":
+        assert "geometry" not in api_request_body.keys()
         assert "signature" in api_request_body["properties"].keys()
         for key in properties_keys:
             assert not api_request_body["properties"].get(key)
     else:
+        assert api_request_body["geometry"] == {
+            "type": "Point",
+            "coordinates": otm_request_parameters["coordinates"],
+        }
         assert "signature" not in api_request_body["properties"].keys()
         for key in properties_keys:
             assert api_request_body["properties"][key] == otm_request_parameters[key]
         assert (
             api_request_body["properties"]["datetime"]
             == f"{otm_request_parameters['date_from'].isoformat()}/{otm_request_parameters['date_to'].isoformat()}"  # noqa: E501
         )
@@ -307,15 +308,15 @@
     otm_request_parameters,
     otm_response,
 ):
     otm_request_parameters["product"] = "assured"
 
     with raises(
         Exception,
-        match="Orders with assured priority must also have a signature token.",
+        match="Orders with assured priority must have a signature token.",
     ):
         client.otm_v2.create_order(**otm_request_parameters)
 
 
 @mocketize(strict_mode=True)
 @mark.parametrize(
     "per_page",
```

### Comparing `satellitevu-4.6.1/satellitevu/auth/auth.py` & `satellitevu-4.6.2/satellitevu/auth/auth.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/auth/auth_test.py` & `satellitevu-4.6.2/satellitevu/auth/auth_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/auth/cache.py` & `satellitevu-4.6.2/satellitevu/auth/cache.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/auth/cache_test.py` & `satellitevu-4.6.2/satellitevu/auth/cache_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/client.py` & `satellitevu-4.6.2/satellitevu/client.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/config.py` & `satellitevu-4.6.2/satellitevu/config.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/conftest.py` & `satellitevu-4.6.2/satellitevu/conftest.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/http/base.py` & `satellitevu-4.6.2/satellitevu/http/base.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/http/http_test.py` & `satellitevu-4.6.2/satellitevu/http/http_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/http/httpx.py` & `satellitevu-4.6.2/satellitevu/http/httpx.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/http/requests.py` & `satellitevu-4.6.2/satellitevu/http/requests.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/satellitevu/http/urllib.py` & `satellitevu-4.6.2/satellitevu/http/urllib.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.1/PKG-INFO` & `satellitevu-4.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satellitevu
-Version: 4.6.1
+Version: 4.6.2
 Summary: Client SDK for SatelliteVu's platform APIs
 License: MIT
 Author: Christian Wygoda
 Author-email: christian.wygoda@satellitevu.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

