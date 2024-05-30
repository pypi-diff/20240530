# Comparing `tmp/brapi_proxy-0.0.8.tar.gz` & `tmp/brapi_proxy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brapi_proxy-0.0.8.tar", last modified: Mon May 27 08:54:00 2024, max compression
+gzip compressed data, was "brapi_proxy-0.0.9.tar", last modified: Wed May 29 12:35:06 2024, max compression
```

## Comparing `brapi_proxy-0.0.8.tar` & `brapi_proxy-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 08:54:00.160663 brapi_proxy-0.0.8/
--rw-r--r--   0 matthijs   (501) staff       (20)     1079 2024-05-23 06:09:10.000000 brapi_proxy-0.0.8/LICENSE
--rw-r--r--   0 matthijs   (501) staff       (20)     5260 2024-05-27 08:54:00.160291 brapi_proxy-0.0.8/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     3282 2024-05-27 08:52:31.000000 brapi_proxy-0.0.8/README.md
--rw-r--r--   0 matthijs   (501) staff       (20)     1038 2024-05-23 09:26:28.000000 brapi_proxy-0.0.8/pyproject.toml
--rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-22 18:03:35.000000 brapi_proxy-0.0.8/requirements.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       38 2024-05-27 08:54:00.160744 brapi_proxy-0.0.8/setup.cfg
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 08:54:00.149055 brapi_proxy-0.0.8/src/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 08:54:00.151960 brapi_proxy-0.0.8/src/brapi_proxy/
--rw-r--r--   0 matthijs   (501) staff       (20)       85 2024-05-21 08:26:30.000000 brapi_proxy-0.0.8/src/brapi_proxy/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)       22 2024-05-27 08:53:27.000000 brapi_proxy-0.0.8/src/brapi_proxy/_version.py
--rw-r--r--   0 matthijs   (501) staff       (20)    10059 2024-05-27 07:25:57.000000 brapi_proxy-0.0.8/src/brapi_proxy/brapi.py
--rw-r--r--   0 matthijs   (501) staff       (20)      827 2024-05-27 05:52:30.000000 brapi_proxy-0.0.8/src/brapi_proxy/config_demo.ini
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 08:54:00.156736 brapi_proxy-0.0.8/src/brapi_proxy/core/
--rw-r--r--   0 matthijs   (501) staff       (20)     2497 2024-05-26 09:58:48.000000 brapi_proxy-0.0.8/src/brapi_proxy/core/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1921 2024-05-26 09:59:04.000000 brapi_proxy-0.0.8/src/brapi_proxy/core/core_commoncropnames.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5214 2024-05-27 07:06:36.000000 brapi_proxy-0.0.8/src/brapi_proxy/core/core_lists.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5880 2024-05-27 05:51:43.000000 brapi_proxy-0.0.8/src/brapi_proxy/core/core_locations.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5091 2024-05-24 16:08:00.000000 brapi_proxy-0.0.8/src/brapi_proxy/core/core_people.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5351 2024-05-24 15:51:59.000000 brapi_proxy-0.0.8/src/brapi_proxy/core/core_programs.py
--rw-r--r--   0 matthijs   (501) staff       (20)     3703 2024-05-24 16:55:30.000000 brapi_proxy-0.0.8/src/brapi_proxy/core/core_seasons.py
--rw-r--r--   0 matthijs   (501) staff       (20)     2432 2024-05-22 17:35:22.000000 brapi_proxy-0.0.8/src/brapi_proxy/core/core_serverinfo.py
--rw-r--r--   0 matthijs   (501) staff       (20)     7012 2024-05-24 15:51:38.000000 brapi_proxy-0.0.8/src/brapi_proxy/core/core_studies.py
--rw-r--r--   0 matthijs   (501) staff       (20)     7669 2024-05-24 15:51:29.000000 brapi_proxy-0.0.8/src/brapi_proxy/core/core_trials.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 08:54:00.159538 brapi_proxy-0.0.8/src/brapi_proxy/genotyping/
--rw-r--r--   0 matthijs   (501) staff       (20)     2598 2024-05-26 08:52:21.000000 brapi_proxy-0.0.8/src/brapi_proxy/genotyping/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)    25296 2024-05-27 07:39:36.000000 brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_allelematrix.py
--rw-r--r--   0 matthijs   (501) staff       (20)     4030 2024-05-22 17:38:37.000000 brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_callsets.py
--rw-r--r--   0 matthijs   (501) staff       (20)     6179 2024-05-22 17:39:08.000000 brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_plates.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5926 2024-05-22 17:39:34.000000 brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_references.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5573 2024-05-22 17:40:06.000000 brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_referencesets.py
--rw-r--r--   0 matthijs   (501) staff       (20)     6186 2024-05-27 08:43:13.000000 brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_samples.py
--rw-r--r--   0 matthijs   (501) staff       (20)     3936 2024-05-22 17:41:59.000000 brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_variants.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5410 2024-05-22 17:42:26.000000 brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_variantsets.py
--rw-r--r--   0 matthijs   (501) staff       (20)    15517 2024-05-27 08:43:05.000000 brapi_proxy-0.0.8/src/brapi_proxy/handler.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1394 2024-05-23 07:16:51.000000 brapi_proxy-0.0.8/src/brapi_proxy/service.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 08:54:00.159878 brapi_proxy-0.0.8/src/brapi_proxy.egg-info/
--rw-r--r--   0 matthijs   (501) staff       (20)     5260 2024-05-27 08:54:00.000000 brapi_proxy-0.0.8/src/brapi_proxy.egg-info/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     1278 2024-05-27 08:54:00.000000 brapi_proxy-0.0.8/src/brapi_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 matthijs   (501) staff       (20)        1 2024-05-27 08:54:00.000000 brapi_proxy-0.0.8/src/brapi_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       60 2024-05-27 08:54:00.000000 brapi_proxy-0.0.8/src/brapi_proxy.egg-info/entry_points.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-27 08:54:00.000000 brapi_proxy-0.0.8/src/brapi_proxy.egg-info/requires.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       12 2024-05-27 08:54:00.000000 brapi_proxy-0.0.8/src/brapi_proxy.egg-info/top_level.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-29 12:35:06.269291 brapi_proxy-0.0.9/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1079 2024-05-23 06:09:10.000000 brapi_proxy-0.0.9/LICENSE
+-rw-r--r--   0 matthijs   (501) staff       (20)     5718 2024-05-29 12:35:06.268938 brapi_proxy-0.0.9/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)     3740 2024-05-28 07:46:22.000000 brapi_proxy-0.0.9/README.md
+-rw-r--r--   0 matthijs   (501) staff       (20)     1038 2024-05-23 09:26:28.000000 brapi_proxy-0.0.9/pyproject.toml
+-rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-22 18:03:35.000000 brapi_proxy-0.0.9/requirements.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       38 2024-05-29 12:35:06.269361 brapi_proxy-0.0.9/setup.cfg
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-29 12:35:06.250115 brapi_proxy-0.0.9/src/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-29 12:35:06.253916 brapi_proxy-0.0.9/src/brapi_proxy/
+-rw-r--r--   0 matthijs   (501) staff       (20)       85 2024-05-21 08:26:30.000000 brapi_proxy-0.0.9/src/brapi_proxy/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)       22 2024-05-29 12:34:19.000000 brapi_proxy-0.0.9/src/brapi_proxy/_version.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    11899 2024-05-29 12:21:35.000000 brapi_proxy-0.0.9/src/brapi_proxy/brapi.py
+-rw-r--r--   0 matthijs   (501) staff       (20)      776 2024-05-29 12:11:36.000000 brapi_proxy-0.0.9/src/brapi_proxy/config_demo.ini
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-29 12:35:06.260930 brapi_proxy-0.0.9/src/brapi_proxy/core/
+-rw-r--r--   0 matthijs   (501) staff       (20)     4123 2024-05-29 09:14:18.000000 brapi_proxy-0.0.9/src/brapi_proxy/core/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1921 2024-05-26 09:59:04.000000 brapi_proxy-0.0.9/src/brapi_proxy/core/core_commoncropnames.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     4549 2024-05-27 14:51:44.000000 brapi_proxy-0.0.9/src/brapi_proxy/core/core_lists.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5880 2024-05-27 05:51:43.000000 brapi_proxy-0.0.9/src/brapi_proxy/core/core_locations.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5091 2024-05-24 16:08:00.000000 brapi_proxy-0.0.9/src/brapi_proxy/core/core_people.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5351 2024-05-24 15:51:59.000000 brapi_proxy-0.0.9/src/brapi_proxy/core/core_programs.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     3703 2024-05-24 16:55:30.000000 brapi_proxy-0.0.9/src/brapi_proxy/core/core_seasons.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     2748 2024-05-29 12:05:35.000000 brapi_proxy-0.0.9/src/brapi_proxy/core/core_serverinfo.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     7012 2024-05-24 15:51:38.000000 brapi_proxy-0.0.9/src/brapi_proxy/core/core_studies.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     7669 2024-05-24 15:51:29.000000 brapi_proxy-0.0.9/src/brapi_proxy/core/core_trials.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-29 12:35:06.266671 brapi_proxy-0.0.9/src/brapi_proxy/genotyping/
+-rw-r--r--   0 matthijs   (501) staff       (20)     4166 2024-05-29 08:55:06.000000 brapi_proxy-0.0.9/src/brapi_proxy/genotyping/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    25296 2024-05-27 07:39:36.000000 brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_allelematrix.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     4030 2024-05-22 17:38:37.000000 brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_callsets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     6179 2024-05-22 17:39:08.000000 brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_plates.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5926 2024-05-22 17:39:34.000000 brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_references.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5573 2024-05-22 17:40:06.000000 brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_referencesets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     6186 2024-05-27 08:43:13.000000 brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_samples.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     3936 2024-05-22 17:41:59.000000 brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_variants.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5410 2024-05-22 17:42:26.000000 brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_variantsets.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-29 12:35:06.267607 brapi_proxy-0.0.9/src/brapi_proxy/germplasm/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1114 2024-05-29 08:54:39.000000 brapi_proxy-0.0.9/src/brapi_proxy/germplasm/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     3095 2024-05-27 16:32:22.000000 brapi_proxy-0.0.9/src/brapi_proxy/germplasm/germplasm_breedingmethods.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    14946 2024-05-29 12:30:57.000000 brapi_proxy-0.0.9/src/brapi_proxy/handler.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-29 12:35:06.268146 brapi_proxy-0.0.9/src/brapi_proxy/phenotyping/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1033 2024-05-29 08:54:29.000000 brapi_proxy-0.0.9/src/brapi_proxy/phenotyping/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     3063 2024-05-27 16:53:03.000000 brapi_proxy-0.0.9/src/brapi_proxy/phenotyping/phenotyping_ontologies.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1394 2024-05-23 07:16:51.000000 brapi_proxy-0.0.9/src/brapi_proxy/service.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-29 12:35:06.268504 brapi_proxy-0.0.9/src/brapi_proxy.egg-info/
+-rw-r--r--   0 matthijs   (501) staff       (20)     5718 2024-05-29 12:35:06.000000 brapi_proxy-0.0.9/src/brapi_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)     1465 2024-05-29 12:35:06.000000 brapi_proxy-0.0.9/src/brapi_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)        1 2024-05-29 12:35:06.000000 brapi_proxy-0.0.9/src/brapi_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       60 2024-05-29 12:35:06.000000 brapi_proxy-0.0.9/src/brapi_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-29 12:35:06.000000 brapi_proxy-0.0.9/src/brapi_proxy.egg-info/requires.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       12 2024-05-29 12:35:06.000000 brapi_proxy-0.0.9/src/brapi_proxy.egg-info/top_level.txt
```

### Comparing `brapi_proxy-0.0.8/LICENSE` & `brapi_proxy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/PKG-INFO` & `brapi_proxy-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brapi-proxy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A BRAPI server instance that functions as a proxy to merge and combine endpoints from existing BRAPI services
 Author-email: Matthijs Brouwer <matthijs.brouwer@wur.nl>
 License: MIT License
         
         Copyright (c) 2024 EU H2020 AGENT project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -94,14 +94,17 @@
   - /programs/{programDbId}
   - /seasons
   - /seasons/{seasonDbId}
   - /studies
   - /studies/{studyDbId}
   - /trials
   - /trials/{trialDbId}
+- BrAPI-Phenotyping
+  - /ontologies
+  - /ontologies/{ontologyDbId}
 - BrAPI-Genotyping
   - /allelematrix
   - /callsets
   - /callsets/{callSetDbId}
   - /plates
   - /plates/{plateDbId}
   - /references
@@ -110,20 +113,21 @@
   - /referencesets/{referenceSetDbId}
   - /samples
   - /samples/{sampleDbId}
   - /variants
   - /variants/{variantDbId}
   - /variantsets
   - /variantsets/{variantSetDbId}
-  
+- BrAPI-Germplasm
+  - /breedingmethods
+  - /breedingmethods/{breedingMethodDbId}
+
 ### ToDo
 
 - Implement additional endpoints
-- Possibly support other methods (now only get)
-- Enable authentication for underlying servers
   
 ---
 
 ### Structure Configuration File
 
 Create a `config.ini` file with the necessary configuration settings.
 
@@ -137,14 +141,28 @@
 host=0.0.0.0
 location=/
 threads=4
 debug=False
 version=2.1
 ```
 
+**Optional: Serverinfo**
+
+Optionally, provide `serverinfo` entries:
+
+```
+contactEmail=noreply@wur.nl
+documentationURL=https://github.com/matthijsbrouwer/brapi-proxy/
+location=Wageningen
+organizationName=Wageningen University and Research
+organizationURL=https://www.plantbreeding.wur.nl/
+serverDescription=Demo-version proxy to combine multiple BrAPI services
+serverName=BrAPI-Proxy
+```
+
 **Optional: Authorization**
 
 Optionally, provide authentication tokens to restrict access in the `authorization` section:
 
 ```
 [authorization]
 john=tokenjohn123abc
@@ -155,14 +173,15 @@
 
 Within sections prefixed with `server.`, define the underlying servers:
 
 ```
 [server.test1]
 url=https://test-server.brapi.org/brapi/v2
 calls=commoncropnames,variants,allelematrix
+authorization=XXXX
 prefix.variants=barley:
 prefix.variantsets=barley:
 prefix.references=barley:
 prefix.referencesets=barley:
 prefix.callsets=barley:
 
 [server.test2]
```

### Comparing `brapi_proxy-0.0.8/README.md` & `brapi_proxy-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,17 @@
   - /programs/{programDbId}
   - /seasons
   - /seasons/{seasonDbId}
   - /studies
   - /studies/{studyDbId}
   - /trials
   - /trials/{trialDbId}
+- BrAPI-Phenotyping
+  - /ontologies
+  - /ontologies/{ontologyDbId}
 - BrAPI-Genotyping
   - /allelematrix
   - /callsets
   - /callsets/{callSetDbId}
   - /plates
   - /plates/{plateDbId}
   - /references
@@ -70,20 +73,21 @@
   - /referencesets/{referenceSetDbId}
   - /samples
   - /samples/{sampleDbId}
   - /variants
   - /variants/{variantDbId}
   - /variantsets
   - /variantsets/{variantSetDbId}
-  
+- BrAPI-Germplasm
+  - /breedingmethods
+  - /breedingmethods/{breedingMethodDbId}
+
 ### ToDo
 
 - Implement additional endpoints
-- Possibly support other methods (now only get)
-- Enable authentication for underlying servers
   
 ---
 
 ### Structure Configuration File
 
 Create a `config.ini` file with the necessary configuration settings.
 
@@ -97,14 +101,28 @@
 host=0.0.0.0
 location=/
 threads=4
 debug=False
 version=2.1
 ```
 
+**Optional: Serverinfo**
+
+Optionally, provide `serverinfo` entries:
+
+```
+contactEmail=noreply@wur.nl
+documentationURL=https://github.com/matthijsbrouwer/brapi-proxy/
+location=Wageningen
+organizationName=Wageningen University and Research
+organizationURL=https://www.plantbreeding.wur.nl/
+serverDescription=Demo-version proxy to combine multiple BrAPI services
+serverName=BrAPI-Proxy
+```
+
 **Optional: Authorization**
 
 Optionally, provide authentication tokens to restrict access in the `authorization` section:
 
 ```
 [authorization]
 john=tokenjohn123abc
@@ -115,14 +133,15 @@
 
 Within sections prefixed with `server.`, define the underlying servers:
 
 ```
 [server.test1]
 url=https://test-server.brapi.org/brapi/v2
 calls=commoncropnames,variants,allelematrix
+authorization=XXXX
 prefix.variants=barley:
 prefix.variantsets=barley:
 prefix.references=barley:
 prefix.referencesets=barley:
 prefix.callsets=barley:
 
 [server.test2]
```

### Comparing `brapi_proxy-0.0.8/pyproject.toml` & `brapi_proxy-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/brapi.py` & `brapi_proxy-0.0.9/src/brapi_proxy/brapi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=line-too-long
+
 """Main BrAPI module"""
 
 import os
 import sys
 import configparser
 import logging
 import time
@@ -9,20 +11,29 @@
 from flask import Flask, Blueprint
 from flask_restx import Api
 from flask_restx.apidoc import apidoc
 
 from waitress import serve
 
 from . import handler
+from ._version import __version__
 from .core import calls_api_core, ns_api_core
+from .phenotyping import calls_api_phenotyping, ns_api_phenotyping
 from .genotyping import calls_api_genotyping, ns_api_genotyping
+from .germplasm import calls_api_germplasm, ns_api_germplasm
+
+api_list = [(calls_api_core, ns_api_core),
+            (calls_api_phenotyping, ns_api_phenotyping),
+            (calls_api_genotyping, ns_api_genotyping),
+            (calls_api_germplasm, ns_api_germplasm)]
 
 supportedCalls = {}
-for key,value in calls_api_core.items(): supportedCalls[key] = (value[0],value[1],value[2])
-for key,value in calls_api_genotyping.items(): supportedCalls[key] = (value[0],value[1],value[2])
+for api_entry in api_list:
+    for supportedCall,value in api_entry[0].items():
+        supportedCalls[supportedCall] = value
 
 class BrAPI:
     """Main BrAPI class"""
 
     def __init__(self,location,config_file="config.ini"):
         #solve reload problem when using spawn method (osx/windows)
         if get_start_method()=="spawn":
@@ -39,16 +50,15 @@
         self.config.read(os.path.join(self.location,config_file))
         self.logger.info("read configuration file")
         if self.config.getboolean("brapi","debug",fallback=False):
             self.logger.setLevel(logging.DEBUG)
             self.logger.debug("run in debug mode")
         else:
             self.logger.setLevel(logging.INFO)
-        self.version = self.config.get("brapi","version",fallback="2.1")
-        assert self.version in ["2.1"], "version {} not supported".format(self.version)
+        self.version = self.config.get("brapi","version",fallback=__version__)
         #restart on errors
         while True:
             try:
                 process_api = Process(target=self.process_api_messages, args=[])
                 self.logger.debug("try to start server")
                 process_api.start()
                 #wait until ends
@@ -72,121 +82,148 @@
         authorizations = {
             "apikey": {
                 "type": "apiKey",
                 "in": "header",
                 "name": "Authorization"
             }
         }
-        api_title = self.config.get("brapi","serverName",fallback="BrAPI")
-        api_description = self.config.get("brapi","serverDescription",fallback="The Breeding API")
+        api_title = self.config.get("serverinfo","serverName",fallback="BrAPI")
+        api_description = self.config.get("serverinfo","serverDescription",fallback="The Breeding API")
         api = Api(blueprint, title=api_title,
                   authorizations=authorizations, security="apikey",
                   description=api_description, version=self.version)
         #config
         apidoc.static_url_path = os.path.join(server_location,"swaggerui")
         api.config = self.config
         api.brapi = {
             "servers": {},
-            "calls": {"serverinfo":{}},
+            "calls": {"serverinfo": {
+                "resources": supportedCalls["serverinfo"].get("resources",[]),
+                "acceptedVersions": supportedCalls["serverinfo"].get("acceptedVersions",[]),
+                "additionalVersions": supportedCalls["serverinfo"].get("acceptedVersions",[]),
+                "servers":{}
+            }},
             "authorization": {},
-            "identifiers": {call : value[0] for call,value in supportedCalls.items()},
-            "version": self.version
+            "identifiers": {call : value.get("identifier",None) for call,value in supportedCalls.items()}
         }
+        #check serverinfo
+        assert "serverinfo" in supportedCalls, "serverinfo should be supported"
         #get configuration
         if self.config.has_section("authorization"):
             for option in self.config.options("authorization"):
                 api.brapi["authorization"][option] = str(self.config.get("authorization",option))
         servers = [entry[7:] for entry in self.config.sections()
                    if entry.startswith("server.") and len(entry)>7]
         for server_name in servers:
             server_section="server.{}".format(server_name)
             if self.config.has_option(server_section,"url"):
                 api.brapi["servers"][server_name] = {}
                 api.brapi["servers"][server_name]["url"] = self.config.get(server_section,"url")
+                api.brapi["servers"][server_name]["authorization"] = None
                 api.brapi["servers"][server_name]["name"] = server_name
                 api.brapi["servers"][server_name]["calls"] = []
                 api.brapi["servers"][server_name]["prefixes"] = {}
                 for key in self.config.options(server_section):
-                    if key.startswith("prefix."):
+                    if key=="authorization":
+                        api.brapi["servers"][server_name][key] = self.config.get(server_section,key)
+                    elif key.startswith("prefix."):
                         api.brapi["servers"][server_name]["prefixes"][key[7:]] = str(
                             self.config.get(server_section,key))
                 serverinfo,_,_ = handler.brapiGetRequest(
                     api.brapi["servers"][server_name],"serverinfo")
                 if not serverinfo:
                     self.logger.error("server %s unreachable",server_name)
                     time.sleep(60)
                     raise ConnectionError("retry because server {} unreachable".format(server_name))
+                #get serverinfo versions
+                server_calls = serverinfo.get("result",{}).get("calls",[])
+                serverinfo_versions = []
+                for server_call in server_calls:
+                    if server_call.get("service")=="serverinfo":
+                        serverinfo_versions.extend(server_call.get("versions"))
                 if self.config.has_option(server_section,"calls"):
-                    calls = self.config.get(server_section,"calls").split(",")
-                    server_calls = serverinfo.get("result",{}).get("calls",[])
                     #get available method/services with the right version and contentType
                     availableServerCalls = set()
+                    availableServerCallVersions = {}
                     for server_call in server_calls:
                         if (
-                            "application/json" in server_call.get("contentTypes",[])
-                            and
-                            "application/json" in server_call.get("dataTypes",[])
-                            and
-                            self.version in server_call.get("versions",[])
+                            ("application/json" in server_call.get("contentTypes",[])
+                            or
+                            "application/json" in server_call.get("dataTypes",[]))
                         ) :
                             for method in server_call.get("methods",[]):
-                                availableServerCalls.add((str(method).lower(),server_call.get("service")))
+                                method_service = (str(method).lower(),server_call.get("service"))
+                                availableServerCalls.add(method_service)
+                                availableServerCallVersions[method_service] = server_call.get("versions",[])
+                    #get configured calls
+                    calls = set()
+                    for callEntry in self.config.get(server_section,"calls").split(","):
+                        if callEntry=="*":
+                            for call,call_value in supportedCalls.items():
+                                if availableServerCalls.issuperset(call_value.get("requiredServices",[])):
+                                    calls.add(call)
+                        elif callEntry.endswith(".*"):
+                            namespace = callEntry[:-2]
+                            for call,call_value in supportedCalls.items():
+                                if not value.get("namespace",None)==namespace:
+                                    continue
+                                if availableServerCalls.issuperset(call_value.get("requiredServices",[])):
+                                    calls.add(call)
+                        else:
+                            calls.add(callEntry)
+                    #try to add configured calls
                     for call in calls:
                         if not call in supportedCalls:
                             self.logger.warning(
                                 "call %s for %s not supported by proxy",call,server_name)
-                        elif not availableServerCalls.issuperset(supportedCalls[call][1]):
-                            self.logger.warning(
-                                "call %s not supported by %s",call,server_name)
                         else:
+                            requiredServices = supportedCalls[call].get("requiredServices",[])
+                            if not availableServerCalls.issuperset(requiredServices):
+                                self.logger.warning(
+                                    "call %s not supported by %s",call,server_name)
+                                continue
+                            if len(requiredServices)>0:
+                                versions = set.intersection(*[set(availableServerCallVersions[method_service])
+                                                              for method_service in requiredServices])
+                                if len(set(supportedCalls[call].get("acceptedVersions",[])).intersection(versions))==0:
+                                    self.logger.warning(
+                                        "call %s not supported by %s with right version",call,server_name)
+                                    continue
+                            #register call
                             if not call in api.brapi["calls"]:
-                                api.brapi["calls"][call] = {}
+                                api.brapi["calls"][call] = {
+                                    "resources": supportedCalls[call].get("resources",[]),
+                                    "acceptedVersions": supportedCalls[call].get("acceptedVersions",[]),
+                                    "additionalVersions": supportedCalls[call].get("acceptedVersions",[]),
+                                    "servers":{}
+                                }
                             if not server_name in api.brapi["calls"][call]:
-                                api.brapi["calls"][call][server_name] = []
-                            for server_call in server_calls:
-                                for method in server_call["methods"]:
-                                    callKey = (method.lower(),server_call["service"])
-                                    if callKey in supportedCalls[call][1] or callKey in supportedCalls[call][2]:
-                                        for method in server_call.get("methods"):
-                                            entry = (method.lower(),server_call.get("service"))
-                                            if entry in supportedCalls[call][1] or entry in supportedCalls[call][2]:
-                                                api.brapi["calls"][call][server_name].append(entry)
-                self.logger.debug("checked configuration server %s",server_name)
-        
-        #always provide core namespace
-        api.add_namespace(ns_api_core)
-        core_calls = set(calls_api_core.keys()).intersection(api.brapi["calls"])
-        core_calls.add("serverinfo")
-        for call in core_calls:
-            for resource in calls_api_core[call][3]:
-                servers = list(api.brapi["calls"][call].keys())
-                if len(servers)>0:
-                    shared = set.intersection(*[set([tuple(entry) for entry in item]) for item in api.brapi["calls"][call].values()])
-                else:
-                    shared = set()
-                methods = resource[0]._methods(shared,servers) if callable(getattr(resource[0], "_methods", None)) else ["get"]
-                ns_api_core.add_resource(resource[0], resource[1], methods=methods)
-        #genotyping namespace
-        genotyping_calls = set(calls_api_genotyping.keys()).intersection(api.brapi["calls"])
-        if len(genotyping_calls)>0:
-            api.add_namespace(ns_api_genotyping)
-            for call in genotyping_calls:
-                servers = list(api.brapi["calls"][call].keys())
-                shared = set.intersection(*[set([tuple(entry) for entry in item]) for item in api.brapi["calls"][call].values()])
-                if len(servers)>0:
-                    shared = set.intersection(*[set([tuple(entry) for entry in item]) for item in api.brapi["calls"][call].values()])
-                else:
-                    shared = set()
-                for resource in calls_api_genotyping[call][3]:
-                    methods = resource[0]._methods(shared,servers) if callable(getattr(resource[0], "_methods", None)) else ["get"]
-                    ns_api_genotyping.add_resource(resource[0], resource[1], methods=methods)
+                                api.brapi["calls"][call]["servers"][server_name] = []
+                            for entry in availableServerCalls:
+                                if (entry in supportedCalls[call].get("requiredServices",[]) or
+                                    entry in supportedCalls[call].get("optionalServices",[])):
+                                    api.brapi["calls"][call]["servers"][server_name].append(entry)
+                                    api.brapi["servers"][server_name]["calls"].append(entry)
+
+                self.logger.debug("checked serverinfo %s, supported versions: %s",server_name,",".join(serverinfo_versions))
+
+
+        #add namespaces
+        for api_entry in api_list:
+            api_calls = set(api_entry[0].keys()).intersection(api.brapi["calls"])
+            if len(api_calls)>0:
+                api.add_namespace(api_entry[1])
+                for call in api_calls:
+                    for resource in api_entry[0][call].get("resources",[]):
+                        api_entry[1].add_resource(resource[0], resource[1])
+
         #register blueprint
         app.register_blueprint(blueprint)
         app.config.SWAGGER_UI_DOC_EXPANSION = "list"
-        
+
         #--- start webserver ---
         server_host = self.config.get("brapi","host", fallback="0.0.0.0")
         server_port = self.config.get("brapi","port", fallback="8080")
         server_threads = self.config.get("brapi","threads", fallback="4")
         self.logger.info("start server on host %s and port %s with %s threads",
             server_host,server_port,server_threads)
         serve(app, host=server_host, port=server_port, threads=server_threads)
```

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/core/core_commoncropnames.py` & `brapi_proxy-0.0.9/src/brapi_proxy/core/core_commoncropnames.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/core/core_lists.py` & `brapi_proxy-0.0.9/src/brapi_proxy/core/core_lists.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,21 +25,14 @@
         help="Used to request a specific page of data to be returned<br>The page indexing starts at 0 (the first page is 'page'= 0). Default is `0`")
 parser.add_argument("pageSize", type=int, required=False,
         help="The size of the pages to be returned. Default is `1000`")
 parser.add_argument("Authorization", type=str, required=False,
         help="HTTP HEADER - Token used for Authorization<br>**Bearer {token_string}**", 
         location="headers")
 
-newRequestItem = namespace.model("List", {})
-
-parserPost = namespace.parser()
-parserPost.add_argument("Authorization", type=str, required=False,
-        help="HTTP HEADER - Token used for Authorization<br>**Bearer {token_string}**", 
-        location="headers")
-
 class CoreLists(Resource):
 
     @namespace.expect(parser, validate=True)
     @handler.authorization
     def get(self):
         args = parser.parse_args(strict=True)
         try:            
@@ -58,29 +51,15 @@
             else:
                 response = Response(json.dumps(str(brapiError)), mimetype="application/json")
                 response.status_code = brapiStatus
                 return response
         except Exception as e:
             response = Response(json.dumps(str(e)), mimetype="application/json")
             response.status_code = 500
-            return response
-
-    @namespace.expect(parserPost,[newRequestItem])
-    @handler.authorization
-    def post(self):
-        response = Response("to be implemented", mimetype="content/text")
-        response.status_code = 500
-        return response
-
-    def _methods(shared,servers):
-        if len(servers)==1 and ("post","lists") in shared:
-            return ["get","post"]
-        else:
-            return ["get"]
-            
+            return response            
 
 parserId = namespace.parser()
 parserId.add_argument("Authorization", type=str, required=False,
         help="HTTP HEADER - Token used for Authorization<br>**Bearer {token_string}**", 
         location="headers")
             
 class CoreListsId(Resource):
```

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/core/core_locations.py` & `brapi_proxy-0.0.9/src/brapi_proxy/core/core_locations.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/core/core_people.py` & `brapi_proxy-0.0.9/src/brapi_proxy/core/core_people.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/core/core_programs.py` & `brapi_proxy-0.0.9/src/brapi_proxy/core/core_programs.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/core/core_seasons.py` & `brapi_proxy-0.0.9/src/brapi_proxy/core/core_seasons.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/core/core_serverinfo.py` & `brapi_proxy-0.0.9/src/brapi_proxy/core/core_serverinfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,29 @@
 
     @namespace.expect(parser, validate=True)
     @handler.authorization
     def get(self):
         args = parser.parse_args(strict=True)
         try:
             result = {"calls": []}
-            for call,definition in self.api.__schema__["paths"].items():
-                entry = {
-                    "contentTypes":["application/json"],
-                    "dataTypes":["application/json"],
-                    "methods": [method.upper() for method in definition.keys() 
-                                if method.upper() in ["GET","PUT","POST","DELETE"]],
-                    "service": str(call).removeprefix("/"),
-                    "versions":[self.api.version]
-                }
+            for call,value in self.api.brapi["calls"].items():
+                versions = value.get("acceptedVersions",[])
+                for resource in value.get("resources",[]):
+                    methods = []
+                    # print(resource[0].methods)
+                    for method in ["get","post","put","delete"]:
+                        if hasattr(resource[0], method) and callable(getattr(resource[0],method)): 
+                            methods.append(method.upper())
+                    entry = {
+                        "contentTypes":["application/json"],
+                        "dataTypes":["application/json"],
+                        "methods": methods,
+                        "service": str(resource[1]).removeprefix("/"),
+                        "versions": versions
+                    }
                 result["calls"].append(entry)
             if not args["contentType"] is None:
                 result["calls"] = [entry for entry in result["calls"] if args["contentType"] in entry["contentTypes"]]
             elif not args["dataType"] is None:
                 result["calls"] = [entry for entry in result["calls"] if args["dataType"] in entry["dataTypes"]]
             for item in ["contactEmail","documentationURL","location","organizationName",
                          "organizationURL","serverDescription","serverName"]:
```

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/core/core_studies.py` & `brapi_proxy-0.0.9/src/brapi_proxy/core/core_studies.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/core/core_trials.py` & `brapi_proxy-0.0.9/src/brapi_proxy/core/core_trials.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_allelematrix.py` & `brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_allelematrix.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_callsets.py` & `brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_callsets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_plates.py` & `brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_plates.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_references.py` & `brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_references.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_referencesets.py` & `brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_referencesets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_samples.py` & `brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_samples.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_variants.py` & `brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_variants.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/genotyping/genotyping_variantsets.py` & `brapi_proxy-0.0.9/src/brapi_proxy/genotyping/genotyping_variantsets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/handler.py` & `brapi_proxy-0.0.9/src/brapi_proxy/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=line-too-long
+
 """Handler BrAPI requests"""
 
 import math
 import logging
 from functools import wraps
 import requests
 from flask import Response, request
@@ -65,60 +67,44 @@
     response["result"] = result
     return response
 
 def brapiGetRequest(server,call,**args):
     try:
         params = args.get("params",{})
         headers = {"Accept": "application/json"}
+        if not server["authorization"] is None:
+            headers["Authorization"] = "Bearer {}".format(server["authorization"])
         url = "{}/{}".format(server["url"],call)
         response = requests.get(url, params=params, headers=headers)
         try:
             if response.ok:
                 return response.json(), response.status_code, None
-            else:
-                return None, response.status_code, response.text
+            return None, response.status_code, response.text
         except:
             return None, 500, response.text
     except Exception as e:
         return None, 500, "error: {}".format(str(e))
 
 def brapiPostRequest(server,call,payload):
     try:
         headers = {"Accept": "application/json"}
+        if not server["authorization"] is None:
+            headers["Authorization"] = "Bearer {}".format(server["authorization"])
         url = "{}/{}".format(server["url"],call)
         response = requests.post(url, data=payload, headers=headers)
         try:
             if response.ok:
                 return response.json(), response.status_code, None
-            else:
-                return None, response.status_code, response.text
+            return None, response.status_code, response.text
         except:
             return None, 500, response.text
     except Exception as e:
         return None, 500, "error: {}".format(str(e))
 
-def brapiPostRequestResponse(brapi, call, payload):
-    #get servers
-    servers = []
-    for server in brapi["calls"][call]:
-        servers.append(brapi["servers"].get(server,{}))
-    #construct response
-    response = {}
-    response["@context"] = ["https://brapi.org/jsonld/context/metadata.jsonld"]
-    response["metadata"] = {}
-    for server in servers:
-        try:
-            if ("post", call) in brapi["calls"][call][server["name"]]:
-                itemResponse,itemStatus,itemError = brapiPostRequest(server,serverCall,payload)
-        except Exception as e:
-                return None, 500, "problem processing response from {}: {}".format(
-                    server["name"],str(e))
-    return None, 501, "unsupported post to {}".format(call)
-
-def brapiIdRequestResponse(brapi, call, name, id, method="get", **args):
+def brapiIdRequestResponse(brapi, call, name, id, method="get"):
     #get servers
     servers = []
     for server in brapi["calls"][call]:
         servers.append(brapi["servers"].get(server,{}))
     #handle request
     callById="{}/{{{}}}".format(call,name)
     if method=="get":
@@ -153,17 +139,16 @@
                                     entry,server["prefixes"],
                                     brapi["identifiers"]) for entry in data]
                                 if len(data)==1:
                                     if name in data[0]:
                                         if data[0][name]==id:
                                             response["result"] = data[0]
                                             return response, 200, None
-                                        else:
-                                            logger.warning("unexpected response with "+
-                                                           "{}: {} from {}".format(
+                                        logger.warning("unexpected response with "+
+                                                        "{}: {} from {}".format(
                                                 name,data[0][name],server["name"]))
                                     else:
                                         logger.warning("unexpected response without "+
                                                        "{} from {}".format(
                                                 name,server["name"]))
                                 elif len(data)>1:
                                     logger.warning("unexpected multiple ({}) ".format(len(data))+
@@ -175,15 +160,14 @@
             except Exception as e:
                 return None, 500, "problem processing response from {}: {}".format(
                     server["name"],str(e))
         return None, 404, "{} {} not found in {}".format(name,id,call)
     else:
         return None, 501, "unsupported method {}".format(method)
 
-
 def brapiRepaginateRequestResponse(brapi, call, **args):
     #get servers
     servers = []
     for server in brapi["calls"][call]:
         servers.append(brapi["servers"].get(server,{}))
     #handle request
     params = args.get("params",{})
```

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy/service.py` & `brapi_proxy-0.0.9/src/brapi_proxy/service.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy.egg-info/PKG-INFO` & `brapi_proxy-0.0.9/src/brapi_proxy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brapi-proxy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A BRAPI server instance that functions as a proxy to merge and combine endpoints from existing BRAPI services
 Author-email: Matthijs Brouwer <matthijs.brouwer@wur.nl>
 License: MIT License
         
         Copyright (c) 2024 EU H2020 AGENT project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -94,14 +94,17 @@
   - /programs/{programDbId}
   - /seasons
   - /seasons/{seasonDbId}
   - /studies
   - /studies/{studyDbId}
   - /trials
   - /trials/{trialDbId}
+- BrAPI-Phenotyping
+  - /ontologies
+  - /ontologies/{ontologyDbId}
 - BrAPI-Genotyping
   - /allelematrix
   - /callsets
   - /callsets/{callSetDbId}
   - /plates
   - /plates/{plateDbId}
   - /references
@@ -110,20 +113,21 @@
   - /referencesets/{referenceSetDbId}
   - /samples
   - /samples/{sampleDbId}
   - /variants
   - /variants/{variantDbId}
   - /variantsets
   - /variantsets/{variantSetDbId}
-  
+- BrAPI-Germplasm
+  - /breedingmethods
+  - /breedingmethods/{breedingMethodDbId}
+
 ### ToDo
 
 - Implement additional endpoints
-- Possibly support other methods (now only get)
-- Enable authentication for underlying servers
   
 ---
 
 ### Structure Configuration File
 
 Create a `config.ini` file with the necessary configuration settings.
 
@@ -137,14 +141,28 @@
 host=0.0.0.0
 location=/
 threads=4
 debug=False
 version=2.1
 ```
 
+**Optional: Serverinfo**
+
+Optionally, provide `serverinfo` entries:
+
+```
+contactEmail=noreply@wur.nl
+documentationURL=https://github.com/matthijsbrouwer/brapi-proxy/
+location=Wageningen
+organizationName=Wageningen University and Research
+organizationURL=https://www.plantbreeding.wur.nl/
+serverDescription=Demo-version proxy to combine multiple BrAPI services
+serverName=BrAPI-Proxy
+```
+
 **Optional: Authorization**
 
 Optionally, provide authentication tokens to restrict access in the `authorization` section:
 
 ```
 [authorization]
 john=tokenjohn123abc
@@ -155,14 +173,15 @@
 
 Within sections prefixed with `server.`, define the underlying servers:
 
 ```
 [server.test1]
 url=https://test-server.brapi.org/brapi/v2
 calls=commoncropnames,variants,allelematrix
+authorization=XXXX
 prefix.variants=barley:
 prefix.variantsets=barley:
 prefix.references=barley:
 prefix.referencesets=barley:
 prefix.callsets=barley:
 
 [server.test2]
```

### Comparing `brapi_proxy-0.0.8/src/brapi_proxy.egg-info/SOURCES.txt` & `brapi_proxy-0.0.9/src/brapi_proxy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,8 +28,12 @@
 src/brapi_proxy/genotyping/genotyping_allelematrix.py
 src/brapi_proxy/genotyping/genotyping_callsets.py
 src/brapi_proxy/genotyping/genotyping_plates.py
 src/brapi_proxy/genotyping/genotyping_references.py
 src/brapi_proxy/genotyping/genotyping_referencesets.py
 src/brapi_proxy/genotyping/genotyping_samples.py
 src/brapi_proxy/genotyping/genotyping_variants.py
-src/brapi_proxy/genotyping/genotyping_variantsets.py
+src/brapi_proxy/genotyping/genotyping_variantsets.py
+src/brapi_proxy/germplasm/__init__.py
+src/brapi_proxy/germplasm/germplasm_breedingmethods.py
+src/brapi_proxy/phenotyping/__init__.py
+src/brapi_proxy/phenotyping/phenotyping_ontologies.py
```

