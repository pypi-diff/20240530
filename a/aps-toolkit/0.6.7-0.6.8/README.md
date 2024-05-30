# Comparing `tmp/aps-toolkit-0.6.7.tar.gz` & `tmp/aps-toolkit-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps-toolkit-0.6.7.tar", last modified: Fri May 17 07:00:06 2024, max compression
+gzip compressed data, was "aps-toolkit-0.6.8.tar", last modified: Thu May 30 06:00:05 2024, max compression
```

## Comparing `aps-toolkit-0.6.7.tar` & `aps-toolkit-0.6.8.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 07:00:06.596045 aps-toolkit-0.6.7/
--rw-rw-rw-   0        0        0     1990 2024-05-17 07:00:06.595045 aps-toolkit-0.6.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-17 07:00:06.596045 aps-toolkit-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1013 2024-05-17 06:58:36.000000 aps-toolkit-0.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:00:06.551046 aps-toolkit-0.6.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 07:00:06.577045 aps-toolkit-0.6.7/src/aps_toolkit/
--rw-rw-rw-   0        0        0    12957 2024-05-15 08:02:24.000000 aps-toolkit-0.6.7/src/aps_toolkit/Auth.py
--rw-rw-rw-   0        0        0     5643 2024-05-15 08:02:24.000000 aps-toolkit-0.6.7/src/aps_toolkit/AuthGoogleColab.py
--rw-rw-rw-   0        0        0    32484 2024-05-17 06:53:43.000000 aps-toolkit-0.6.7/src/aps_toolkit/BIM360.py
--rw-rw-rw-   0        0        0     9080 2024-05-15 08:02:24.000000 aps-toolkit-0.6.7/src/aps_toolkit/Bucket.py
--rw-rw-rw-   0        0        0     2557 2024-05-15 08:02:24.000000 aps-toolkit-0.6.7/src/aps_toolkit/DbReader.py
--rw-rw-rw-   0        0        0    13050 2024-05-08 09:57:59.000000 aps-toolkit-0.6.7/src/aps_toolkit/Derivative.py
--rw-rw-rw-   0        0        0     3998 2024-05-08 10:00:23.000000 aps-toolkit-0.6.7/src/aps_toolkit/Fragments.py
--rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/InputStream.py
--rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.6.7/src/aps_toolkit/ManifestItem.py
--rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/MaterialProperties.py
--rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/Materials.py
--rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/PackFileReader.py
--rw-rw-rw-   0        0        0      978 2024-05-08 09:58:31.000000 aps-toolkit-0.6.7/src/aps_toolkit/PathInfo.py
--rw-rw-rw-   0        0        0     4636 2024-05-08 09:59:04.000000 aps-toolkit-0.6.7/src/aps_toolkit/ProDbReaderCad.py
--rw-rw-rw-   0        0        0     3635 2024-05-08 09:53:38.000000 aps-toolkit-0.6.7/src/aps_toolkit/ProDbReaderNavis.py
--rw-rw-rw-   0        0        0    21677 2024-05-08 09:41:50.000000 aps-toolkit-0.6.7/src/aps_toolkit/ProDbReaderRevit.py
--rw-rw-rw-   0        0        0    16159 2024-05-08 09:59:09.000000 aps-toolkit-0.6.7/src/aps_toolkit/PropReader.py
--rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.6.7/src/aps_toolkit/Resource.py
--rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFContent.py
--rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFGeometries.py
--rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFImage.py
--rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFLines.py
--rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFManifestType.py
--rw-rw-rw-   0        0        0      910 2024-05-08 02:57:09.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFMaterialGroup.py
--rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFMaterialMap.py
--rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFMaterialMapScale.py
--rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFMaterials.py
--rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFMesh.py
--rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFMetadata.py
--rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFPoints.py
--rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFReader.py
--rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFTransform.py
--rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/SVFUVMap.py
--rw-rw-rw-   0        0        0     9163 2024-05-17 05:36:10.000000 aps-toolkit-0.6.7/src/aps_toolkit/Token.py
--rw-rw-rw-   0        0        0     5076 2024-05-08 09:51:14.000000 aps-toolkit-0.6.7/src/aps_toolkit/Webhooks.py
--rw-rw-rw-   0        0        0      888 2024-05-17 05:24:22.000000 aps-toolkit-0.6.7/src/aps_toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:00:06.581045 aps-toolkit-0.6.7/src/aps_toolkit/units/
--rw-rw-rw-   0        0        0     1481 2024-05-08 09:45:28.000000 aps-toolkit-0.6.7/src/aps_toolkit/units/DisplayUnits.py
--rw-rw-rw-   0        0        0        0 2024-05-08 09:41:50.000000 aps-toolkit-0.6.7/src/aps_toolkit/units/__init__.py
--rw-rw-rw-   0        0        0    38555 2024-05-08 09:41:50.000000 aps-toolkit-0.6.7/src/aps_toolkit/units/units.json
-drwxrwxrwx   0        0        0        0 2024-05-17 07:00:06.580045 aps-toolkit-0.6.7/src/aps_toolkit.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-05-17 07:00:06.000000 aps-toolkit-0.6.7/src/aps_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1967 2024-05-17 07:00:06.000000 aps-toolkit-0.6.7/src/aps_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 07:00:06.000000 aps-toolkit-0.6.7/src/aps_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-17 07:00:06.000000 aps-toolkit-0.6.7/src/aps_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-17 07:00:06.000000 aps-toolkit-0.6.7/src/aps_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 07:00:06.595045 aps-toolkit-0.6.7/src/test/
--rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.6.7/src/test/__init__.py
--rw-rw-rw-   0        0        0     1141 2024-05-17 05:25:10.000000 aps-toolkit-0.6.7/src/test/context.py
--rw-rw-rw-   0        0        0     1381 2024-05-08 09:51:14.000000 aps-toolkit-0.6.7/src/test/test_Webhooks.py
--rw-rw-rw-   0        0        0     2006 2024-05-08 07:26:15.000000 aps-toolkit-0.6.7/src/test/test_auth.py
--rw-rw-rw-   0        0        0     1429 2024-05-06 09:51:01.000000 aps-toolkit-0.6.7/src/test/test_auth_colab.py
--rw-rw-rw-   0        0        0     5850 2024-05-17 05:50:12.000000 aps-toolkit-0.6.7/src/test/test_bim360.py
--rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.6.7/src/test/test_bucket.py
--rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.6.7/src/test/test_db_reader.py
--rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.6.7/src/test/test_derivative.py
--rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.6.7/src/test/test_fragment.py
--rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.6.7/src/test/test_geometries.py
--rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.6.7/src/test/test_image.py
--rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.6.7/src/test/test_material.py
--rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.6.7/src/test/test_mesh.py
--rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.6.7/src/test/test_metadata.py
--rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.6.7/src/test/test_prop_reader.py
--rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.6.7/src/test/test_prop_reader_cad.py
--rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.6.7/src/test/test_prop_reader_navis.py
--rw-rw-rw-   0        0        0     3516 2024-05-08 09:41:50.000000 aps-toolkit-0.6.7/src/test/test_prop_reader_revit.py
--rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.6.7/src/test/test_svf_reader.py
--rw-rw-rw-   0        0        0      808 2024-05-17 05:35:41.000000 aps-toolkit-0.6.7/src/test/test_token.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:00:05.102429 aps-toolkit-0.6.8/
+-rw-rw-rw-   0        0        0     1990 2024-05-30 06:00:05.102429 aps-toolkit-0.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:00:05.103428 aps-toolkit-0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2024-05-30 05:59:41.000000 aps-toolkit-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:00:05.047429 aps-toolkit-0.6.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 06:00:05.078428 aps-toolkit-0.6.8/src/aps_toolkit/
+-rw-rw-rw-   0        0        0    12957 2024-05-15 08:02:24.000000 aps-toolkit-0.6.8/src/aps_toolkit/Auth.py
+-rw-rw-rw-   0        0        0     5643 2024-05-15 08:02:24.000000 aps-toolkit-0.6.8/src/aps_toolkit/AuthGoogleColab.py
+-rw-rw-rw-   0        0        0    33736 2024-05-30 05:59:03.000000 aps-toolkit-0.6.8/src/aps_toolkit/BIM360.py
+-rw-rw-rw-   0        0        0     9080 2024-05-15 08:02:24.000000 aps-toolkit-0.6.8/src/aps_toolkit/Bucket.py
+-rw-rw-rw-   0        0        0     2557 2024-05-15 08:02:24.000000 aps-toolkit-0.6.8/src/aps_toolkit/DbReader.py
+-rw-rw-rw-   0        0        0    13168 2024-05-17 07:46:20.000000 aps-toolkit-0.6.8/src/aps_toolkit/Derivative.py
+-rw-rw-rw-   0        0        0     3998 2024-05-08 10:00:23.000000 aps-toolkit-0.6.8/src/aps_toolkit/Fragments.py
+-rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/InputStream.py
+-rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.6.8/src/aps_toolkit/ManifestItem.py
+-rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/MaterialProperties.py
+-rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/Materials.py
+-rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/PackFileReader.py
+-rw-rw-rw-   0        0        0      978 2024-05-08 09:58:31.000000 aps-toolkit-0.6.8/src/aps_toolkit/PathInfo.py
+-rw-rw-rw-   0        0        0     4636 2024-05-08 09:59:04.000000 aps-toolkit-0.6.8/src/aps_toolkit/ProDbReaderCad.py
+-rw-rw-rw-   0        0        0     3635 2024-05-08 09:53:38.000000 aps-toolkit-0.6.8/src/aps_toolkit/ProDbReaderNavis.py
+-rw-rw-rw-   0        0        0    21677 2024-05-08 09:41:50.000000 aps-toolkit-0.6.8/src/aps_toolkit/ProDbReaderRevit.py
+-rw-rw-rw-   0        0        0    16159 2024-05-08 09:59:09.000000 aps-toolkit-0.6.8/src/aps_toolkit/PropReader.py
+-rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.6.8/src/aps_toolkit/Resource.py
+-rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFContent.py
+-rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFGeometries.py
+-rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFImage.py
+-rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFLines.py
+-rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFManifestType.py
+-rw-rw-rw-   0        0        0      910 2024-05-08 02:57:09.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFMaterialGroup.py
+-rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFMaterialMap.py
+-rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFMaterialMapScale.py
+-rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFMaterials.py
+-rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFMesh.py
+-rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFMetadata.py
+-rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFPoints.py
+-rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFReader.py
+-rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFTransform.py
+-rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/SVFUVMap.py
+-rw-rw-rw-   0        0        0     9163 2024-05-17 05:36:10.000000 aps-toolkit-0.6.8/src/aps_toolkit/Token.py
+-rw-rw-rw-   0        0        0     5076 2024-05-08 09:51:14.000000 aps-toolkit-0.6.8/src/aps_toolkit/Webhooks.py
+-rw-rw-rw-   0        0        0      888 2024-05-17 05:24:22.000000 aps-toolkit-0.6.8/src/aps_toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:00:05.084428 aps-toolkit-0.6.8/src/aps_toolkit/units/
+-rw-rw-rw-   0        0        0     1481 2024-05-08 09:45:28.000000 aps-toolkit-0.6.8/src/aps_toolkit/units/DisplayUnits.py
+-rw-rw-rw-   0        0        0        0 2024-05-08 09:41:50.000000 aps-toolkit-0.6.8/src/aps_toolkit/units/__init__.py
+-rw-rw-rw-   0        0        0    38555 2024-05-08 09:41:50.000000 aps-toolkit-0.6.8/src/aps_toolkit/units/units.json
+drwxrwxrwx   0        0        0        0 2024-05-30 06:00:05.082428 aps-toolkit-0.6.8/src/aps_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-30 06:00:04.000000 aps-toolkit-0.6.8/src/aps_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1967 2024-05-30 06:00:04.000000 aps-toolkit-0.6.8/src/aps_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:00:04.000000 aps-toolkit-0.6.8/src/aps_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-30 06:00:04.000000 aps-toolkit-0.6.8/src/aps_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-30 06:00:04.000000 aps-toolkit-0.6.8/src/aps_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 06:00:05.101428 aps-toolkit-0.6.8/src/test/
+-rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.6.8/src/test/__init__.py
+-rw-rw-rw-   0        0        0     1141 2024-05-17 05:25:10.000000 aps-toolkit-0.6.8/src/test/context.py
+-rw-rw-rw-   0        0        0     1381 2024-05-08 09:51:14.000000 aps-toolkit-0.6.8/src/test/test_Webhooks.py
+-rw-rw-rw-   0        0        0     2006 2024-05-08 07:26:15.000000 aps-toolkit-0.6.8/src/test/test_auth.py
+-rw-rw-rw-   0        0        0     1429 2024-05-06 09:51:01.000000 aps-toolkit-0.6.8/src/test/test_auth_colab.py
+-rw-rw-rw-   0        0        0     5896 2024-05-30 05:33:28.000000 aps-toolkit-0.6.8/src/test/test_bim360.py
+-rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.6.8/src/test/test_bucket.py
+-rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.6.8/src/test/test_db_reader.py
+-rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.6.8/src/test/test_derivative.py
+-rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.6.8/src/test/test_fragment.py
+-rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.6.8/src/test/test_geometries.py
+-rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.6.8/src/test/test_image.py
+-rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.6.8/src/test/test_material.py
+-rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.6.8/src/test/test_mesh.py
+-rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.6.8/src/test/test_metadata.py
+-rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.6.8/src/test/test_prop_reader.py
+-rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.6.8/src/test/test_prop_reader_cad.py
+-rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.6.8/src/test/test_prop_reader_navis.py
+-rw-rw-rw-   0        0        0     3516 2024-05-08 09:41:50.000000 aps-toolkit-0.6.8/src/test/test_prop_reader_revit.py
+-rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.6.8/src/test/test_svf_reader.py
+-rw-rw-rw-   0        0        0      808 2024-05-17 05:35:41.000000 aps-toolkit-0.6.8/src/test/test_token.py
```

### Comparing `aps-toolkit-0.6.7/PKG-INFO` & `aps-toolkit-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.6.7
+Version: 0.6.8
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.6.7/setup.py` & `aps-toolkit-0.6.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("Readme.md") as f:
     if f is not None:
         readme = f.read()
 
 setuptools.setup(
     name="aps-toolkit",
-    version="0.6.7",
+    version="0.6.8",
     author="chuong mep",
     author_email="chuongpqvn@gmail.com",
     description="A Toolkit Autodesk Platform Services for Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/chuongmep/aps-toolkit",
     project_urls={
```

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/Auth.py` & `aps-toolkit-0.6.8/src/aps_toolkit/Auth.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/AuthGoogleColab.py` & `aps-toolkit-0.6.8/src/aps_toolkit/AuthGoogleColab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/BIM360.py` & `aps-toolkit-0.6.8/src/aps_toolkit/BIM360.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,32 +210,58 @@
         item_versions = response.json()
         return item_versions['data'][0]['relationships']['derivatives']['data']['id']
 
     def batch_report_projects(self, hub_id: str) -> pd.DataFrame:
         """
         Get batch all projects with general information by hub_id
         :param hub_id:  :class:`str` the unique identifier of a hub
-        :return:  :class:`pandas.DataFrame` all projects with general information
+        :return:  :class:`pandas.DataFrame` all projects with general information : id, name, type
         """
-        df = pd.DataFrame(columns=['project_id', 'project_name', "project_type", 'top_folder_id'])
+        df = pd.DataFrame(columns=['id', 'name', 'type'])
         headers = {'Authorization': 'Bearer ' + self.token.access_token}
         url = f"{self.host}/project/v1/hubs/{hub_id}/projects"
         response = requests.get(url, headers=headers)
         if response.status_code != 200:
             raise Exception(response.content)
         projects = response.json()
         for project in projects['data']:
             project_id = project['id']
             project_name = project['attributes']['name']
-            project_type = project['attributes']['extension']["data"]["projectType"]
-            top_folder = self.get_top_folders(hub_id, project_id)
-            top_folder_id = top_folder["data"][0]["id"]
-            df = pd.concat([df, pd.DataFrame(
-                {'project_id': project_id, 'project_name': project_name, 'project_type': project_type,
-                 'top_folder_id': top_folder_id}, index=[0])], ignore_index=True)
+            type = project['attributes']['extension']["data"]["projectType"]
+            df = pd.concat([df, pd.DataFrame({'id': project_id, 'name': project_name, 'type': type}, index=[0])],
+                           ignore_index=True)
+        df.sort_values(by='name', inplace=True)
+        return df
+
+    def batch_report_top_folders(self, hub_id: str, project_id: str) -> pd.DataFrame:
+        """
+        Get batch all top folders with general information by hub_id and project_id
+        :param hub_id:  :class:`str` the unique identifier of a hub
+        :param project_id:  :class:`str` the unique identifier of a project
+        :return:  :class:`pandas.DataFrame` all top folders with general information : id, name
+        """
+        df = pd.DataFrame(columns=['id'])
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/project/v1/hubs/{hub_id}/projects/{project_id}/topFolders"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        top_folders = response.json()
+        for top_folder in top_folders['data']:
+            top_folder_id = top_folder['id']
+            atts = top_folder['attributes']
+            properties_values = {}
+            for key in atts:
+                if isinstance(atts[key], dict):
+                    continue
+                properties_values[key] = atts[key]
+            properties_values['id'] = top_folder_id
+            df = pd.concat([df, pd.DataFrame(properties_values, index=[0])], ignore_index=True)
+        # drop all columns have null value
+        df.dropna(axis=1, how='all', inplace=True)
         return df
 
     def batch_report_item_versions(self, project_id: str, item_id: str) -> pd.DataFrame:
         """
         Get batch all item versions with general information by project_id and item_id
         :param project_id:  :class:`str` the unique identifier of a project
         :param item_id:  :class:`str` the unique identifier of an item
```

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/Bucket.py` & `aps-toolkit-0.6.8/src/aps_toolkit/Bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/DbReader.py` & `aps-toolkit-0.6.8/src/aps_toolkit/DbReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/Derivative.py` & `aps-toolkit-0.6.8/src/aps_toolkit/Derivative.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,16 @@
             "region": self.region
         }
         # request
         response = requests.get(URL, headers=headers)
         if response.status_code == 404:
             raise Exception(response.content)
         json_response = response.json()
+        if "derivatives" not in json_response:
+            raise Exception("No derivatives found in the manifest.")
         children = json_response['derivatives'][0]["children"]
         manifest_items = []
         image_items = []
         for child in children:
             if child["type"] == "geometry":
                 for c in child["children"]:
                     # check if contains 'mime' and 'application/autodesk-svf
```

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/Fragments.py` & `aps-toolkit-0.6.8/src/aps_toolkit/Fragments.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/InputStream.py` & `aps-toolkit-0.6.8/src/aps_toolkit/InputStream.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/ManifestItem.py` & `aps-toolkit-0.6.8/src/aps_toolkit/ManifestItem.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/MaterialProperties.py` & `aps-toolkit-0.6.8/src/aps_toolkit/MaterialProperties.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/Materials.py` & `aps-toolkit-0.6.8/src/aps_toolkit/Materials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/PackFileReader.py` & `aps-toolkit-0.6.8/src/aps_toolkit/PackFileReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/PathInfo.py` & `aps-toolkit-0.6.8/src/aps_toolkit/PathInfo.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/ProDbReaderCad.py` & `aps-toolkit-0.6.8/src/aps_toolkit/ProDbReaderCad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/ProDbReaderNavis.py` & `aps-toolkit-0.6.8/src/aps_toolkit/ProDbReaderNavis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/ProDbReaderRevit.py` & `aps-toolkit-0.6.8/src/aps_toolkit/ProDbReaderRevit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/PropReader.py` & `aps-toolkit-0.6.8/src/aps_toolkit/PropReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/Resource.py` & `aps-toolkit-0.6.8/src/aps_toolkit/Resource.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFContent.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFContent.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFGeometries.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFGeometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFImage.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFImage.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFLines.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFLines.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFManifestType.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFManifestType.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFMaterialGroup.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFMaterialGroup.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFMaterialMap.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFMaterialMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFMaterialMapScale.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFMaterialMapScale.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFMaterials.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFMaterials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFMesh.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFMesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFMetadata.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFMetadata.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFPoints.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFPoints.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFReader.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFTransform.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFTransform.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/SVFUVMap.py` & `aps-toolkit-0.6.8/src/aps_toolkit/SVFUVMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/Token.py` & `aps-toolkit-0.6.8/src/aps_toolkit/Token.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/Webhooks.py` & `aps-toolkit-0.6.8/src/aps_toolkit/Webhooks.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/__init__.py` & `aps-toolkit-0.6.8/src/aps_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/units/DisplayUnits.py` & `aps-toolkit-0.6.8/src/aps_toolkit/units/DisplayUnits.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit/units/units.json` & `aps-toolkit-0.6.8/src/aps_toolkit/units/units.json`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit.egg-info/PKG-INFO` & `aps-toolkit-0.6.8/src/aps_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.6.7
+Version: 0.6.8
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.6.7/src/aps_toolkit.egg-info/SOURCES.txt` & `aps-toolkit-0.6.8/src/aps_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/context.py` & `aps-toolkit-0.6.8/src/test/context.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_Webhooks.py` & `aps-toolkit-0.6.8/src/test/test_Webhooks.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_auth.py` & `aps-toolkit-0.6.8/src/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_auth_colab.py` & `aps-toolkit-0.6.8/src/test/test_auth_colab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_bim360.py` & `aps-toolkit-0.6.8/src/test/test_bim360.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,19 +61,21 @@
         urn = self.bim360.get_urn_item_version(self.project_id, self.item_id, 2)
         self.assertNotEquals(urn, "")
 
     def test_batch_report_projects(self):
         df = self.bim360.batch_report_projects(self.hub_id)
         self.assertNotEquals(df.empty, True)
 
+    def test_batch_report_top_folders(self):
+        df = self.bim360.batch_report_top_folders(self.hub_id, self.project_id)
+        self.assertNotEquals(df.empty, True)
+
     def test_batch_report_items(self):
         self.bim360.token = Auth().auth3leg()
-        project_id = "b.40f9b774-380b-44d4-a65b-3269178c81ac"
-        folder_id = "urn:adsk.wipemea:fs.folder:co.0LE6VP4_Rraan4-Qce5MGw"
-        df = self.bim360.batch_report_items(project_id, folder_id, ".rvt", True)
+        df = self.bim360.batch_report_items(self.project_id, self.folder_id, ".rvt", True)
         self.assertNotEquals(df.empty, True)
 
     def test_get_item__display_name(self):
         item_name = self.bim360.get_item_display_name(self.project_id, self.item_id)
         self.assertNotEquals(item_name, "")
 
     def test_create_object_storage(self):
```

### Comparing `aps-toolkit-0.6.7/src/test/test_bucket.py` & `aps-toolkit-0.6.8/src/test/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_db_reader.py` & `aps-toolkit-0.6.8/src/test/test_db_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_derivative.py` & `aps-toolkit-0.6.8/src/test/test_derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_fragment.py` & `aps-toolkit-0.6.8/src/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_geometries.py` & `aps-toolkit-0.6.8/src/test/test_geometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_image.py` & `aps-toolkit-0.6.8/src/test/test_image.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_material.py` & `aps-toolkit-0.6.8/src/test/test_material.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_mesh.py` & `aps-toolkit-0.6.8/src/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_prop_reader.py` & `aps-toolkit-0.6.8/src/test/test_prop_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_prop_reader_cad.py` & `aps-toolkit-0.6.8/src/test/test_prop_reader_cad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_prop_reader_navis.py` & `aps-toolkit-0.6.8/src/test/test_prop_reader_navis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_prop_reader_revit.py` & `aps-toolkit-0.6.8/src/test/test_prop_reader_revit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_svf_reader.py` & `aps-toolkit-0.6.8/src/test/test_svf_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.7/src/test/test_token.py` & `aps-toolkit-0.6.8/src/test/test_token.py`

 * *Files identical despite different names*

