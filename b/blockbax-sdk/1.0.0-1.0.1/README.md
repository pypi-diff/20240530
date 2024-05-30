# Comparing `tmp/blockbax_sdk-1.0.0.tar.gz` & `tmp/blockbax_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockbax_sdk-1.0.0.tar", max compression
+gzip compressed data, was "blockbax_sdk-1.0.1.tar", max compression
```

## Comparing `blockbax_sdk-1.0.0.tar` & `blockbax_sdk-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1065 2024-01-26 09:33:16.016140 blockbax_sdk-1.0.0/LICENSE
--rw-r--r--   0        0        0      250 2024-01-26 09:33:16.016140 blockbax_sdk-1.0.0/README.md
--rw-r--r--   0        0        0     1856 2024-01-26 09:33:27.140300 blockbax_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      583 2024-01-26 09:33:16.016140 blockbax_sdk-1.0.0/src/blockbax_sdk/__init__.py
--rw-r--r--   0        0        0      101 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/client/__init__.py
--rw-r--r--   0        0        0       47 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/client/api/__init__.py
--rw-r--r--   0        0        0    16281 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/client/api/api.py
--rw-r--r--   0        0        0     5019 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/client/api/api_utils.py
--rw-r--r--   0        0        0     3465 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/client/api/readme.md
--rw-r--r--   0        0        0    29968 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/client/http_client.py
--rw-r--r--   0        0        0     1092 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/errors.py
--rw-r--r--   0        0        0     1888 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/__init__.py
--rw-r--r--   0        0        0     1775 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/base.py
--rw-r--r--   0        0        0     7016 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/data_types.py
--rw-r--r--   0        0        0     2418 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/ingestion.py
--rw-r--r--   0        0        0     1676 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/ingestion_collection.py
--rw-r--r--   0        0        0     4583 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/ingestions_utils.py
--rw-r--r--   0        0        0     1291 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/measurement.py
--rw-r--r--   0        0        0      981 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/metric.py
--rw-r--r--   0        0        0      612 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/project.py
--rw-r--r--   0        0        0     3635 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/property_type.py
--rw-r--r--   0        0        0     1909 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/property_type_value.py
--rw-r--r--   0        0        0      775 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/series.py
--rw-r--r--   0        0        0     8634 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/subject.py
--rw-r--r--   0        0        0     1860 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/subject_property.py
--rw-r--r--   0        0        0     2496 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/subject_type.py
--rw-r--r--   0        0        0     1557 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/type_hints.py
--rw-r--r--   0        0        0      561 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/models/utils.py
--rw-r--r--   0        0        0        0 2024-01-26 09:33:16.052140 blockbax_sdk-1.0.0/src/blockbax_sdk/py.typed
--rw-r--r--   0        0        0      103 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/util/__init__.py
--rw-r--r--   0        0        0     3485 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/util/conversions.py
--rw-r--r--   0        0        0      546 2024-01-26 09:33:16.020140 blockbax_sdk-1.0.0/src/blockbax_sdk/util/deprecated.py
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 blockbax_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-30 15:07:04.647558 blockbax_sdk-1.0.1/LICENSE
+-rw-r--r--   0        0        0      250 2024-05-30 15:07:04.647558 blockbax_sdk-1.0.1/README.md
+-rw-r--r--   0        0        0     1856 2024-05-30 15:07:16.063535 blockbax_sdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      583 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/client/__init__.py
+-rw-r--r--   0        0        0       47 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/client/api/__init__.py
+-rw-r--r--   0        0        0    16281 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/client/api/api.py
+-rw-r--r--   0        0        0     5019 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/client/api/api_utils.py
+-rw-r--r--   0        0        0     3465 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/client/api/readme.md
+-rw-r--r--   0        0        0    29968 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/client/http_client.py
+-rw-r--r--   0        0        0     1092 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/errors.py
+-rw-r--r--   0        0        0     1888 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/base.py
+-rw-r--r--   0        0        0     7016 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/data_types.py
+-rw-r--r--   0        0        0     2418 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/ingestion.py
+-rw-r--r--   0        0        0     1676 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/ingestion_collection.py
+-rw-r--r--   0        0        0     4583 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/ingestions_utils.py
+-rw-r--r--   0        0        0     1291 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/measurement.py
+-rw-r--r--   0        0        0      981 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/metric.py
+-rw-r--r--   0        0        0      612 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/project.py
+-rw-r--r--   0        0        0     3703 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/property_type.py
+-rw-r--r--   0        0        0     1909 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/property_type_value.py
+-rw-r--r--   0        0        0      775 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/series.py
+-rw-r--r--   0        0        0     8634 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/subject.py
+-rw-r--r--   0        0        0     1860 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/subject_property.py
+-rw-r--r--   0        0        0     2496 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/subject_type.py
+-rw-r--r--   0        0        0     1557 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/type_hints.py
+-rw-r--r--   0        0        0      561 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/models/utils.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:07:04.683558 blockbax_sdk-1.0.1/src/blockbax_sdk/py.typed
+-rw-r--r--   0        0        0      103 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/util/__init__.py
+-rw-r--r--   0        0        0     3556 2024-05-30 15:07:04.651558 blockbax_sdk-1.0.1/src/blockbax_sdk/util/conversions.py
+-rw-r--r--   0        0        0      546 2024-05-30 15:07:04.655558 blockbax_sdk-1.0.1/src/blockbax_sdk/util/deprecated.py
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 blockbax_sdk-1.0.1/PKG-INFO
```

### Comparing `blockbax_sdk-1.0.0/LICENSE` & `blockbax_sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/pyproject.toml` & `blockbax_sdk-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blockbax-sdk"
-version = "1.0.0"
+version = "1.0.1"
 description = "Blockbax Python SDK"
 authors = ["Blockbax <development@blockbax.com>"]
 maintainers = ["Blockbax <development@blockbax.com>"]
 readme = "README.md"
 homepage = "https://blockbax.com/docs/integrations/python-sdk/"
 documentation = "https://blockbax.com/docs/python-sdk/"
 keywords = [
```

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/__init__.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/client/api/api.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/client/api/api.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/client/api/api_utils.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/client/api/api_utils.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/client/api/readme.md` & `blockbax_sdk-1.0.1/src/blockbax_sdk/client/api/readme.md`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/client/http_client.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/client/http_client.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/errors.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/__init__.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/base.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/data_types.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/data_types.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/ingestion.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/ingestion.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/ingestion_collection.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/ingestion_collection.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/ingestions_utils.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/ingestions_utils.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/measurement.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/measurement.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/metric.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/metric.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/project.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/project.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/property_type.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/property_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     predefined_values: bool = False
     values: Optional[List[PropertyTypeValue]] = None
     updated_date: Optional[BlockbaxDatetime] = None
 
     def contains_value(self, value: Any) -> bool:
         """ "Returns `True` if Property type has a Property value with given value"""
         return (
-            any(property_value == value for property_value in self.values)
+            any(
+                property_type_value.get_value() == value
+                for property_type_value in self.values
+            )
             if self.values
             else False
         )
 
     def ensure_values_initialized(self):
         """In case PropertyType object is created by the user without values; The values field default is not set to
         match the default arg of the create_property_type method of the Api interface
```

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/property_type_value.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/property_type_value.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/series.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/series.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/subject.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/subject.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/subject_property.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/subject_property.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/subject_type.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/subject_type.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/type_hints.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/type_hints.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/models/utils.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/models/utils.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/util/conversions.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/util/conversions.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def convert_any_date_to_unix_millis(date: Union[datetime, int, float, str]) -> int:
     if isinstance(date, int) or isinstance(date, float):
         try:
             datetime.fromtimestamp(date)
             return int(date * 1000)
-        except ValueError:
+        except (ValueError, OSError):
             try:
                 # Try to parse the numeric date as epoch milliseconds
                 datetime.fromtimestamp(date / 1000)
                 return int(date)
             except ValueError as exc:
                 raise ValueError(
                     "Cannot parse numeric date as a valid datetime"
@@ -66,19 +66,21 @@
         ]
     ]
 ) -> Optional[str]:
     if isinstance(property_value_ids, (tuple, list)):
         seperator = "," if isinstance(property_value_ids, tuple) else ";"
         return seperator.join(
             [
-                str(id_)
-                if isinstance(id_, (str, UUID))
-                else cast(
-                    Union[str, PropertyValueId],
-                    convert_property_value_ids_to_query_filter(id_),
+                (
+                    str(id_)
+                    if isinstance(id_, (str, UUID))
+                    else cast(
+                        Union[str, PropertyValueId],
+                        convert_property_value_ids_to_query_filter(id_),
+                    )
                 )
                 for id_ in property_value_ids
             ]
         )
     elif isinstance(property_value_ids, str):
         return property_value_ids
     elif isinstance(property_value_ids, UUID):
```

### Comparing `blockbax_sdk-1.0.0/src/blockbax_sdk/util/deprecated.py` & `blockbax_sdk-1.0.1/src/blockbax_sdk/util/deprecated.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-1.0.0/PKG-INFO` & `blockbax_sdk-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockbax-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Blockbax Python SDK
 Home-page: https://blockbax.com/docs/integrations/python-sdk/
 License: MIT
 Keywords: Blockbax,Data,Sensor,IoT
 Author: Blockbax
 Author-email: development@blockbax.com
 Maintainer: Blockbax
```

