# Comparing `tmp/aau_ais_utilities-0.1.12.tar.gz` & `tmp/aau_ais_utilities-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aau_ais_utilities-0.1.12.tar", last modified: Thu May 16 07:02:46 2024, max compression
+gzip compressed data, was "aau_ais_utilities-0.1.13.tar", last modified: Thu May 30 14:54:23 2024, max compression
```

## Comparing `aau_ais_utilities-0.1.12.tar` & `aau_ais_utilities-0.1.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      135 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/README.md
--rw-r--r--   0        0        0      629 2024-05-16 07:02:46.845719 aau_ais_utilities-0.1.12/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/src/aau_ais_utilities/__init__.py
--rw-r--r--   0        0        0      154 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/src/aau_ais_utilities/connections/__init__.py
--rw-r--r--   0        0        0      482 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/src/aau_ais_utilities/connections/engine_settings.py
--rw-r--r--   0        0        0     1812 2024-05-03 12:25:02.811676 aau_ais_utilities-0.1.12/src/aau_ais_utilities/connections/postgresql_connection.py
--rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/src/aau_ais_utilities/lookup/__init__.py
--rw-r--r--   0        0        0    18165 2024-05-16 06:49:17.752795 aau_ais_utilities-0.1.12/src/aau_ais_utilities/lookup/mmsi.py
--rw-r--r--   0        0        0      107 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/src/aau_ais_utilities/validate/__init__.py
--rw-r--r--   0        0        0     2695 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/src/aau_ais_utilities/validate/imo.py
--rw-r--r--   0        0        0     1091 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/src/aau_ais_utilities/validate/mmsi.py
--rw-r--r--   0        0        0     1208 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/src/aau_ais_utilities/validate/validator.py
--rw-r--r--   0        0        0     1478 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/tests/validate/test_imo.py
--rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/tests/validate/test_mmsi.py
--rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.12/tests/validate/test_validator.py
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 aau_ais_utilities-0.1.12/PKG-INFO
+-rw-r--r--   0        0        0      135 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/README.md
+-rw-r--r--   0        0        0      629 2024-05-30 14:54:23.263933 aau_ais_utilities-0.1.13/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/src/aau_ais_utilities/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/src/aau_ais_utilities/connections/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/src/aau_ais_utilities/connections/engine_settings.py
+-rw-r--r--   0        0        0     3206 2024-05-30 07:00:40.274688 aau_ais_utilities-0.1.13/src/aau_ais_utilities/connections/postgresql_connection.py
+-rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/src/aau_ais_utilities/lookup/__init__.py
+-rw-r--r--   0        0        0    18242 2024-05-22 07:31:20.105239 aau_ais_utilities-0.1.13/src/aau_ais_utilities/lookup/mmsi.py
+-rw-r--r--   0        0        0      107 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/src/aau_ais_utilities/validate/__init__.py
+-rw-r--r--   0        0        0     2695 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/src/aau_ais_utilities/validate/imo.py
+-rw-r--r--   0        0        0     1091 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/src/aau_ais_utilities/validate/mmsi.py
+-rw-r--r--   0        0        0     1208 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/src/aau_ais_utilities/validate/validator.py
+-rw-r--r--   0        0        0     1478 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/tests/validate/test_imo.py
+-rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/tests/validate/test_mmsi.py
+-rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_utilities-0.1.13/tests/validate/test_validator.py
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 aau_ais_utilities-0.1.13/PKG-INFO
```

### Comparing `aau_ais_utilities-0.1.12/pyproject.toml` & `aau_ais_utilities-0.1.13/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aau-ais-utilities"
-version = "0.1.12"
+version = "0.1.13"
 description = "Utilities for working with the AAU AIS database."
 authors = [
     { name = "Mikael Vind Mikkelsen", email = "mvmi@cs.aau.dk" },
 ]
 dependencies = [
     "sqlalchemy==2.0.*",
     "pydantic-settings==2.2.*",
```

### Comparing `aau_ais_utilities-0.1.12/src/aau_ais_utilities/lookup/mmsi.py` & `aau_ais_utilities-0.1.13/src/aau_ais_utilities/lookup/mmsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,20 +612,22 @@
             mmsi (str): MMSI number to convert.
 
         Returns:
             str: Country code.
         """
         if len(mmsi) != 3:
             mid = mmsi_to_mid(mmsi)
+            mmsi_or_mid = "MMSI"
         else:
             mid = mmsi
+            mmsi_or_mid = "MID"
 
         return mid_to_alpha_3.get(
             mid,
-            "MMSI not assigned to any country, maybe it's not a ship? (Handheld device, AIS Base Station, etc.)"
+            f"{mmsi_or_mid} not assigned to any country, maybe it's not a ship? (Handheld device, AIS Base Station, etc.)"
         )
 
     @staticmethod
     def to_country_name(mmsi: str) -> str:
         """Looks up the MMSI number to retriever the country name of the vessel per the MMSI MID codes.
 
         Args:
```

### Comparing `aau_ais_utilities-0.1.12/src/aau_ais_utilities/validate/imo.py` & `aau_ais_utilities-0.1.13/src/aau_ais_utilities/validate/imo.py`

 * *Files identical despite different names*

### Comparing `aau_ais_utilities-0.1.12/src/aau_ais_utilities/validate/mmsi.py` & `aau_ais_utilities-0.1.13/src/aau_ais_utilities/validate/mmsi.py`

 * *Files identical despite different names*

### Comparing `aau_ais_utilities-0.1.12/src/aau_ais_utilities/validate/validator.py` & `aau_ais_utilities-0.1.13/src/aau_ais_utilities/validate/validator.py`

 * *Files identical despite different names*

### Comparing `aau_ais_utilities-0.1.12/tests/validate/test_imo.py` & `aau_ais_utilities-0.1.13/tests/validate/test_imo.py`

 * *Files identical despite different names*

