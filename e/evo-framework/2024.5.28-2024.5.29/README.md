# Comparing `tmp/evo_framework-2024.5.28.tar.gz` & `tmp/evo_framework-2024.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo_framework-2024.5.28.tar", max compression
+gzip compressed data, was "evo_framework-2024.5.29.tar", max compression
```

## Comparing `evo_framework-2024.5.28.tar` & `evo_framework-2024.5.29.tar`

### file list

```diff
@@ -1,76 +1,75 @@
--rw-r--r--   0        0        0    13525 2024-05-28 16:27:09.302451 evo_framework-2024.5.28/LICENSE.txt
--rw-r--r--   0        0        0      406 2024-05-28 16:35:10.344754 evo_framework-2024.5.28/README.md
--rw-r--r--   0        0        0        0 2024-05-27 18:53:16.952349 evo_framework-2024.5.28/evo/__init__.py
--rwxr-xr-x   0        0        0      830 2024-04-17 13:11:06.786632 evo_framework-2024.5.28/evo/evo_framework/__init__.py
--rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-2024.5.28/evo/evo_framework/control/CObject.py
--rwxr-xr-x   0        0        0       55 2021-12-06 13:42:26.000000 evo_framework-2024.5.28/evo/evo_framework/control/__init__.py
--rw-r--r--   0        0        0      399 2024-05-28 10:42:13.864068 evo_framework-2024.5.28/evo/evo_framework/core/__init__.py
--rwxr-xr-x   0        0        0      172 2024-04-19 18:05:05.984591 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/__init__.py
--rw-r--r--   0        0        0     2136 2024-05-29 22:43:27.679085 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/automation/entity.yaml
--rw-r--r--   0        0        0     5806 2024-05-28 13:29:01.048359 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/control/CApi.py
--rw-r--r--   0        0        0    26330 2024-05-28 13:31:18.108609 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/control/CApiFlow.py
--rw-r--r--   0        0        0      139 2024-04-23 13:31:42.061922 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/control/__init__.py
--rw-r--r--   0        0        0     1834 2024-05-29 23:04:53.266652 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EAction.py
--rw-r--r--   0        0        0     1318 2024-04-19 18:07:44.067267 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EActionTask.py
--rw-r--r--   0        0        0     1701 2024-05-29 23:04:53.276117 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApi.py
--rw-r--r--   0        0        0     1788 2024-05-29 23:04:53.280064 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiAudio.py
--rw-r--r--   0        0        0     3057 2024-05-29 23:08:56.693463 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiConfig.py
--rw-r--r--   0        0        0     1785 2024-05-29 23:04:53.291651 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiFile.py
--rw-r--r--   0        0        0     1793 2024-05-29 23:04:53.294896 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiImage.py
--rw-r--r--   0        0        0     1788 2024-05-29 23:04:53.297767 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiVideo.py
--rwxr-xr-x   0        0        0     2136 2024-04-20 18:47:45.597392 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/ERequest.py
--rwxr-xr-x   0        0        0      703 2024-04-15 20:02:21.126538 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EResponse.py
--rw-r--r--   0        0        0      568 2024-05-29 23:04:53.300310 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiAction.py
--rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
--rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
--rw-r--r--   0        0        0      274 2024-05-28 15:31:41.321728 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiType.py
--rw-r--r--   0        0        0      493 2024-05-29 23:04:53.308461 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiVisibility.py
--rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumLanguage.py
--rwxr-xr-x   0        0        0     1730 2024-05-29 23:05:16.396723 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/__init__.py
--rwxr-xr-x   0        0        0    11450 2024-05-28 12:20:40.146628 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/utility/IuApi.py
--rw-r--r--   0        0        0    14972 2024-04-11 12:54:19.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/utility/IuApiPb.py
--rwxr-xr-x   0        0        0       68 2024-03-22 08:51:24.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/utility/__init__.py
--rwxr-xr-x   0        0        0      223 2024-03-29 21:27:12.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/__init__.py
--rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/entity/IBinary.py
--rwxr-xr-x   0        0        0     9101 2024-04-20 10:22:41.877540 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/IuBinary.py
--rw-r--r--   0        0        0     6662 2024-04-22 18:30:35.211681 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
--rw-r--r--   0        0        0     7728 2024-04-22 18:30:35.215456 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/UBinary.py
--rw-r--r--   0        0        0     1360 2024-04-11 08:07:07.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_boot/control/CBoot.py
--rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_bridge/IBridge.py
--rw-r--r--   0        0        0       79 2024-04-11 08:42:37.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/__init__.py
--rw-r--r--   0        0        0     6217 2024-04-14 09:37:12.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/test_evo_core_binary.py
--rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/utility/IuConvert.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/utility/__init__.py
--rw-r--r--   0        0        0      248 2024-03-29 21:12:01.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/__init__.py
--rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
--rwxr-xr-x   0        0        0     1471 2024-04-20 18:17:27.427816 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
--rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
--rw-r--r--   0        0        0     1344 2024-04-22 10:08:58.482611 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_file/entity/EFileChunk.py
--rw-r--r--   0        0        0      707 2024-04-11 08:07:07.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_foundation/IFoundation.py
--rw-r--r--   0        0        0       67 2024-03-29 21:24:14.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_key/__init__.py
--rw-r--r--   0        0        0      897 2024-04-16 15:31:33.740160 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_key/utility/IuKey.py
--rw-r--r--   0        0        0       67 2024-03-29 18:12:11.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_log/__init__.py
--rw-r--r--   0        0        0     2154 2024-03-17 19:32:16.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_log/utility/IuLog.py
--rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_log/utility/ULogger.py
--rwxr-xr-x   0        0        0      154 2024-04-11 08:09:54.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/__init__.py
--rw-r--r--   0        0        0     2825 2024-04-20 18:51:28.692331 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/control/CSetting.py
--rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/control/__init__.py
--rw-r--r--   0        0        0     1205 2024-04-22 10:09:10.368909 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/entity/ESetting.py
--rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/entity/__init__.py
--rw-r--r--   0        0        0       76 2024-03-29 21:25:40.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_system/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_system/control/__init__.py
--rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_system/utility/IuSystem.py
--rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_system/utility/__init__.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_type/__init__.py
--rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_type/entity/EvoMap.py
--rw-r--r--   0        0        0       70 2024-04-11 08:44:35.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_yaml/__init__.py
--rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_yaml/utility/IuYaml.py
--rwxr-xr-x   0        0        0     9407 2024-05-28 16:14:36.768193 evo_framework-2024.5.28/evo/evo_framework/entity/EObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-2024.5.28/evo/evo_framework/entity/IEObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-2024.5.28/evo/evo_framework/entity/IEvo.py
--rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-2024.5.28/evo/evo_framework/entity/Id.py
--rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-2024.5.28/evo/evo_framework/entity/Time.py
--rwxr-xr-x   0        0        0      185 2024-03-29 18:40:07.000000 evo_framework-2024.5.28/evo/evo_framework/entity/__init__.py
--rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-2024.5.28/evo/evo_framework/utility/__init__.py
--rw-r--r--   0        0        0      556 2024-05-29 22:59:57.712590 evo_framework-2024.5.28/pyproject.toml
--rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 evo_framework-2024.5.28/PKG-INFO
+-rw-r--r--   0        0        0    13525 2024-05-28 16:27:09.302451 evo_framework-2024.5.29/LICENSE.txt
+-rw-r--r--   0        0        0      406 2024-05-28 16:35:10.344754 evo_framework-2024.5.29/README.md
+-rwxr-xr-x   0        0        0      770 2024-05-29 23:15:57.646008 evo_framework-2024.5.29/evo_framework/__init__.py
+-rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-2024.5.29/evo_framework/control/CObject.py
+-rwxr-xr-x   0        0        0       51 2024-05-29 23:15:57.849272 evo_framework-2024.5.29/evo_framework/control/__init__.py
+-rw-r--r--   0        0        0      399 2024-05-28 10:42:13.864068 evo_framework-2024.5.29/evo_framework/core/__init__.py
+-rwxr-xr-x   0        0        0      160 2024-05-29 23:15:57.645990 evo_framework-2024.5.29/evo_framework/core/evo_core_api/__init__.py
+-rw-r--r--   0        0        0     2136 2024-05-29 22:43:27.679085 evo_framework-2024.5.29/evo_framework/core/evo_core_api/automation/entity.yaml
+-rw-r--r--   0        0        0     5770 2024-05-29 23:15:57.847986 evo_framework-2024.5.29/evo_framework/core/evo_core_api/control/CApi.py
+-rw-r--r--   0        0        0    26238 2024-05-29 23:15:57.853079 evo_framework-2024.5.29/evo_framework/core/evo_core_api/control/CApiFlow.py
+-rw-r--r--   0        0        0      131 2024-05-29 23:15:57.840551 evo_framework-2024.5.29/evo_framework/core/evo_core_api/control/__init__.py
+-rw-r--r--   0        0        0     1826 2024-05-29 23:15:57.821619 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EAction.py
+-rw-r--r--   0        0        0     1306 2024-05-29 23:15:57.646050 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EActionTask.py
+-rw-r--r--   0        0        0     1690 2024-05-29 23:15:57.645978 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApi.py
+-rw-r--r--   0        0        0     1780 2024-05-29 23:15:57.646024 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApiAudio.py
+-rw-r--r--   0        0        0     3000 2024-05-29 23:17:42.176322 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApiConfig.py
+-rw-r--r--   0        0        0     1777 2024-05-29 23:15:57.646016 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApiFile.py
+-rw-r--r--   0        0        0     1785 2024-05-29 23:15:57.804481 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApiImage.py
+-rw-r--r--   0        0        0     1780 2024-05-29 23:15:57.826695 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApiVideo.py
+-rwxr-xr-x   0        0        0     2128 2024-05-29 23:15:57.850000 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/ERequest.py
+-rwxr-xr-x   0        0        0      695 2024-05-29 23:15:57.646159 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EResponse.py
+-rw-r--r--   0        0        0      568 2024-05-29 23:04:53.300310 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EnumApiAction.py
+-rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
+-rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
+-rw-r--r--   0        0        0      274 2024-05-28 15:31:41.321728 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EnumApiType.py
+-rw-r--r--   0        0        0      493 2024-05-29 23:04:53.308461 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EnumApiVisibility.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EnumLanguage.py
+-rwxr-xr-x   0        0        0     1502 2024-05-29 23:16:21.970731 evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/__init__.py
+-rwxr-xr-x   0        0        0    11410 2024-05-29 23:15:57.840538 evo_framework-2024.5.29/evo_framework/core/evo_core_api/utility/IuApi.py
+-rw-r--r--   0        0        0    14944 2024-05-29 23:15:57.840524 evo_framework-2024.5.29/evo_framework/core/evo_core_api/utility/IuApiPb.py
+-rwxr-xr-x   0        0        0       64 2024-05-29 23:15:57.840493 evo_framework-2024.5.29/evo_framework/core/evo_core_api/utility/__init__.py
+-rwxr-xr-x   0        0        0      215 2024-05-29 23:15:57.848203 evo_framework-2024.5.29/evo_framework/core/evo_core_binary/__init__.py
+-rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_binary/entity/IBinary.py
+-rwxr-xr-x   0        0        0     9089 2024-05-29 23:15:57.849286 evo_framework-2024.5.29/evo_framework/core/evo_core_binary/utility/IuBinary.py
+-rw-r--r--   0        0        0     6658 2024-05-29 23:15:57.848274 evo_framework-2024.5.29/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
+-rw-r--r--   0        0        0     7700 2024-05-29 23:15:57.848234 evo_framework-2024.5.29/evo_framework/core/evo_core_binary/utility/UBinary.py
+-rw-r--r--   0        0        0     1324 2024-05-29 23:15:57.844638 evo_framework-2024.5.29/evo_framework/core/evo_core_boot/control/CBoot.py
+-rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-2024.5.29/evo_framework/core/evo_core_bridge/IBridge.py
+-rw-r--r--   0        0        0       75 2024-05-29 23:15:57.848167 evo_framework-2024.5.29/evo_framework/core/evo_core_convert/__init__.py
+-rw-r--r--   0        0        0     6217 2024-04-14 09:37:12.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_convert/test_evo_core_binary.py
+-rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_convert/utility/IuConvert.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_convert/utility/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-29 23:15:57.848112 evo_framework-2024.5.29/evo_framework/core/evo_core_crypto/__init__.py
+-rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
+-rwxr-xr-x   0        0        0     1467 2024-05-29 23:15:57.848244 evo_framework-2024.5.29/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
+-rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
+-rw-r--r--   0        0        0     1332 2024-05-29 23:15:57.848017 evo_framework-2024.5.29/evo_framework/core/evo_core_file/entity/EFileChunk.py
+-rw-r--r--   0        0        0      699 2024-05-29 23:15:57.848149 evo_framework-2024.5.29/evo_framework/core/evo_core_foundation/IFoundation.py
+-rw-r--r--   0        0        0       63 2024-05-29 23:15:57.849413 evo_framework-2024.5.29/evo_framework/core/evo_core_key/__init__.py
+-rw-r--r--   0        0        0      893 2024-05-29 23:15:57.844661 evo_framework-2024.5.29/evo_framework/core/evo_core_key/utility/IuKey.py
+-rw-r--r--   0        0        0       63 2024-05-29 23:15:57.848179 evo_framework-2024.5.29/evo_framework/core/evo_core_log/__init__.py
+-rw-r--r--   0        0        0     2150 2024-05-29 23:15:57.848192 evo_framework-2024.5.29/evo_framework/core/evo_core_log/utility/IuLog.py
+-rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_log/utility/ULogger.py
+-rwxr-xr-x   0        0        0      146 2024-05-29 23:15:57.848259 evo_framework-2024.5.29/evo_framework/core/evo_core_setting/__init__.py
+-rw-r--r--   0        0        0     2813 2024-05-29 23:15:57.849237 evo_framework-2024.5.29/evo_framework/core/evo_core_setting/control/CSetting.py
+-rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_setting/control/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-29 23:15:57.849250 evo_framework-2024.5.29/evo_framework/core/evo_core_setting/entity/ESetting.py
+-rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_setting/entity/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-29 23:15:57.848222 evo_framework-2024.5.29/evo_framework/core/evo_core_system/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_system/control/__init__.py
+-rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_system/utility/IuSystem.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_system/utility/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_type/__init__.py
+-rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-2024.5.29/evo_framework/core/evo_core_type/entity/EvoMap.py
+-rw-r--r--   0        0        0       66 2024-05-29 23:15:57.849211 evo_framework-2024.5.29/evo_framework/core/evo_core_yaml/__init__.py
+-rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-2024.5.29/evo_framework/core/evo_core_yaml/utility/IuYaml.py
+-rwxr-xr-x   0        0        0     9395 2024-05-29 23:15:57.849264 evo_framework-2024.5.29/evo_framework/entity/EObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-2024.5.29/evo_framework/entity/IEObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-2024.5.29/evo_framework/entity/IEvo.py
+-rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-2024.5.29/evo_framework/entity/Id.py
+-rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-2024.5.29/evo_framework/entity/Time.py
+-rwxr-xr-x   0        0        0      181 2024-05-29 23:15:57.849324 evo_framework-2024.5.29/evo_framework/entity/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-2024.5.29/evo_framework/utility/__init__.py
+-rw-r--r--   0        0        0      557 2024-05-29 23:20:36.540074 evo_framework-2024.5.29/pyproject.toml
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 evo_framework-2024.5.29/PKG-INFO
```

### Comparing `evo_framework-2024.5.28/LICENSE.txt` & `evo_framework-2024.5.29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/__init__.py` & `evo_framework-2024.5.29/evo_framework/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.control.CObject import CObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_foundation.IFoundation import IFoundation
-from evo.evo_framework.core.evo_core_bridge.IBridge import IBridge
-from evo.evo_framework.core import *
-from evo.evo_framework.core.evo_core_log import *
-from evo.evo_framework.core.evo_core_crypto import *
-from evo.evo_framework.core.evo_core_key import *
-from evo.evo_framework.core.evo_core_system import *
-from evo.evo_framework.core.evo_core_binary import *
-from evo.evo_framework.core.evo_core_setting import *
-from evo.evo_framework.core.evo_core_convert import *
-from evo.evo_framework.core.evo_core_yaml import *
-from evo.evo_framework.core.evo_core_api import *
+from evo_framework.entity.EObject import EObject
+from evo_framework.control.CObject import CObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.core.evo_core_foundation.IFoundation import IFoundation
+from evo_framework.core.evo_core_bridge.IBridge import IBridge
+from evo_framework.core import *
+from evo_framework.core.evo_core_log import *
+from evo_framework.core.evo_core_crypto import *
+from evo_framework.core.evo_core_key import *
+from evo_framework.core.evo_core_system import *
+from evo_framework.core.evo_core_binary import *
+from evo_framework.core.evo_core_setting import *
+from evo_framework.core.evo_core_convert import *
+from evo_framework.core.evo_core_yaml import *
+from evo_framework.core.evo_core_api import *
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/control/CObject.py` & `evo_framework-2024.5.29/evo_framework/control/CObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/automation/entity.yaml` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/automation/entity.yaml`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/control/CApi.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/control/CApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 #                           0 0    0                                                                                                    #
 #                           0      0                                                                                                    #
 #                           00000000                                                                                                    #
 #                                                                                                                                       #
 # CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International       https://github.com/cyborg-ai-git     #
 # =======================================================================================================================================
 
-from evo.evo_framework.core import *
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_log.utility.IuLog import IuLog
-from evo.evo_framework.core.evo_core_key.utility.IuKey import IuKey
-from evo.evo_framework.core.evo_core_api.control.CApiFlow import CApiFlow
-from evo.evo_framework.core.evo_core_api.entity.EApi import EApi
-from evo.evo_framework.core.evo_core_api.entity.EApiItem import EApiItem
-from evo.evo_framework.core.evo_core_api.entity.EnumApiType import EnumApiType
+from evo_framework.core import *
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.core.evo_core_log.utility.IuLog import IuLog
+from evo_framework.core.evo_core_key.utility.IuKey import IuKey
+from evo_framework.core.evo_core_api.control.CApiFlow import CApiFlow
+from evo_framework.core.evo_core_api.entity.EApi import EApi
+from evo_framework.core.evo_core_api.entity.EApiItem import EApiItem
+from evo_framework.core.evo_core_api.entity.EnumApiType import EnumApiType
 
 # ------------------------------------------------------------------------------------------------
 # CActionApi
 # ------------------------------------------------------------------------------------------------
 class CApi():
 
 # ------------------------------------------------------------------------------------------------
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/control/CApiFlow.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/control/CApiFlow.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,37 +19,37 @@
 #                           0 0    0                                                                                                    #
 #                           0      0                                                                                                    #
 #                           00000000                                                                                                    #
 #                                                                                                                                       #
 # CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International       https://github.com/cyborg-ai-git     #
 #========================================================================================================================================
 """
-from evo.evo_framework.core import *
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_log.utility.IuLog import IuLog
-from evo.evo_framework.core.evo_core_api.entity.EApiConfig import EApiConfig
-from evo.evo_framework.core.evo_core_key.utility.IuKey import IuKey
-from evo.evo_framework.core.evo_core_crypto.utility.IuCryptEC import IuCryptEC
-from evo.evo_framework.core.evo_core_crypto.utility.IuCryptHash import IuCryptHash
-from evo.evo_framework.core.evo_core_log.utility.IuLog import IuLog
-from evo.evo_framework.core.evo_core_system.utility.IuSystem import IuSystem
-from evo.evo_framework.core.evo_core_convert.utility.IuConvert import IuConvert
-from evo.evo_framework.core.evo_core_setting.control.CSetting import CSetting
-from evo.evo_framework.core.evo_core_log.utility.IuLog import IuLog
-from evo.evo_framework.core.evo_core_api.entity.EActionTask import EActionTask
-from evo.evo_framework.core.evo_core_api.entity.ERequest import ERequest
-from evo.evo_framework.core.evo_core_api.entity.EResponse import EResponse
-from evo.evo_framework.core.evo_core_api.entity.EApi import EApi
-from evo.evo_framework.core.evo_core_api.entity.EAction import EAction
-from evo.evo_framework.core.evo_core_api.entity.EApiItem import EApiItem
-from evo.evo_framework.core.evo_core_api.entity.EnumApiAction import EnumApiAction
-from evo.evo_framework.core.evo_core_api.entity.EnumApiCrypto import EnumApiCrypto
-from evo.evo_framework.core.evo_core_api.entity.EnumApiType import EnumApiType
-from evo.evo_framework.core.evo_core_api.utility.IuApi import IuApi
+from evo_framework.core import *
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.core.evo_core_log.utility.IuLog import IuLog
+from evo_framework.core.evo_core_api.entity.EApiConfig import EApiConfig
+from evo_framework.core.evo_core_key.utility.IuKey import IuKey
+from evo_framework.core.evo_core_crypto.utility.IuCryptEC import IuCryptEC
+from evo_framework.core.evo_core_crypto.utility.IuCryptHash import IuCryptHash
+from evo_framework.core.evo_core_log.utility.IuLog import IuLog
+from evo_framework.core.evo_core_system.utility.IuSystem import IuSystem
+from evo_framework.core.evo_core_convert.utility.IuConvert import IuConvert
+from evo_framework.core.evo_core_setting.control.CSetting import CSetting
+from evo_framework.core.evo_core_log.utility.IuLog import IuLog
+from evo_framework.core.evo_core_api.entity.EActionTask import EActionTask
+from evo_framework.core.evo_core_api.entity.ERequest import ERequest
+from evo_framework.core.evo_core_api.entity.EResponse import EResponse
+from evo_framework.core.evo_core_api.entity.EApi import EApi
+from evo_framework.core.evo_core_api.entity.EAction import EAction
+from evo_framework.core.evo_core_api.entity.EApiItem import EApiItem
+from evo_framework.core.evo_core_api.entity.EnumApiAction import EnumApiAction
+from evo_framework.core.evo_core_api.entity.EnumApiCrypto import EnumApiCrypto
+from evo_framework.core.evo_core_api.entity.EnumApiType import EnumApiType
+from evo_framework.core.evo_core_api.utility.IuApi import IuApi
 import lz4.frame
 import requests
 from functools import partial
 # ---------------------------------------------------------------------------------------------------------------------------------------
 # CApi
 # ---------------------------------------------------------------------------------------------------------------------------------------
 class CApiFlow():
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EAction.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EAction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 from evo_packages.evo_core_api.entity.EnumApiAction import EnumApiAction
 #========================================================================================================================================
 """EAction
 
 	this is EAction DESCRIPTION
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EActionTask.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EActionTask.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_api.entity.EAction import EAction
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.core.evo_core_api.entity.EAction import EAction
 
 class EActionTask(EObject):
     #annotation
     
     def __init__(self):
         super().__init__()
         self.action:str = ""
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApi.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
 """EApi
 
 	this is EAPI DESCRIPTION
 	
 """
 class EApi(EObject):
 
 	VERSION:str="da9425fde78f3f2dbb9c52ba7a93787960d94e81751ae8594a64f678a80060d3"
 
 	def __init__(self):
 		super().__init__()
 		
-		self.description:str = ""this"
+		self.description:str = None
 		self.isStream:bool = None
 		self.input:str = None
 		self.output:str = None
   
 	def toStream(self, stream):
 		super().toStream(stream)
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiAudio.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApiImage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
-"""EApiAudio
+"""EApiImage
 
-	this is EAPIAudio DESCRIPTION
+	this is EAPiImagection DESCRIPTION
 	
 """
-class EApiAudio(EObject):
+class EApiImage(EObject):
 
 	VERSION:str="3c37d0d7315664187980d10bc9abe5541b93f38ef107473e66bc336fac026f55"
 
 	def __init__(self):
 		super().__init__()
 		
 		self.isUrl:bool = None
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiConfig.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApiConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
-from evo_packages.evo_core_api.entity.EnumApiVisibility import EnumApiVisibility
-from evo_packages.evo_core_api.entity.EApi import EApi
+from evo_framework.core.evo_core_api.entity.EnumApiVisibility import EnumApiVisibility
 from enum import Enum
 #========================================================================================================================================
 
 class EnumApiTunnel(Enum):
     LOCAL = 0
     CYBORGAI = 1
     NGROK = 2
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiFile.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApiFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
 """EApiFile
 
 	this is EApiFile DESCRIPTION
 	
 """
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiImage.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApiAudio.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
-"""EApiImage
+"""EApiAudio
 
-	this is EAPiImagection DESCRIPTION
+	this is EAPIAudio DESCRIPTION
 	
 """
-class EApiImage(EObject):
+class EApiAudio(EObject):
 
 	VERSION:str="3c37d0d7315664187980d10bc9abe5541b93f38ef107473e66bc336fac026f55"
 
 	def __init__(self):
 		super().__init__()
 		
 		self.isUrl:bool = None
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiVideo.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EApiVideo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
 """EApiVideo
 
 	this is EApiVideo DESCRIPTION
 	
 """
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/ERequest.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/ERequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_api.entity.EnumApiCrypto import EnumApiCrypto
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_api.entity.EnumApiCrypto import EnumApiCrypto
 
 class ERequest(EObject):
     def __init__(self):
         super().__init__()
         self.enumCrypto:EnumApiCrypto = EnumApiCrypto.NONE
         self.pk: bytes = None
         self.cipher: bytes = None
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EResponse.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EResponse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_api.entity.ERequest import ERequest
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_api.entity.ERequest import ERequest
 
 class EResponse(ERequest):
     def __init__(self):
         super().__init__()
         self.result = -1
         
     def toStream(self, stream):
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiAction.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/EnumApiAction.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/__init__.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/entity/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-#from evo.evo_framework.core.evo_core_api.entity.evo_core_api_entity_pb2 import ERequestPb as ERequest
-#from evo.evo_framework.core.evo_core_api.entity.evo_core_api_entity_pb2 import EResponsePb as EResponse
-#from evo.evo_framework.core.evo_core_api.entity.evo_core_api_entity_pb2 import EActionPb as EAction
-#from evo.evo_framework.core.evo_core_api.entity.evo_core_api_entity_pb2 import EActionItemPb as EActionItem
-
-from evo.evo_framework.core.evo_core_api.entity.EnumApiCrypto import EnumApiCrypto
-
-from evo.evo_framework.core.evo_core_api.entity.EResponse import EResponse
-from evo.evo_framework.core.evo_core_api.entity.ERequest import ERequest
-
-from evo.evo_framework.core.evo_core_api.entity.EnumApiAction import EnumApiAction
-from evo.evo_framework.core.evo_core_api.entity.EnumApiType import EnumApiType
-from evo.evo_framework.core.evo_core_api.entity.EnumApiVisibility import EnumApiVisibility
-from evo.evo_framework.core.evo_core_api.entity.EApiConfig import EnumApiTunnel
-from evo.evo_framework.core.evo_core_api.entity.EApiConfig import EApiConfig
-
-from evo.evo_framework.core.evo_core_api.entity.EActionTask import EActionTask
-
-from evo.evo_framework.core.evo_core_api.entity.EAction import EAction
-from evo.evo_framework.core.evo_core_api.entity.EActionItem import EActionItem
-from evo.evo_framework.core.evo_core_api.entity.EApi import EApi
-from evo.evo_framework.core.evo_core_api.entity.EApiItem import EApiItem
-
-
-from evo.evo_framework.core.evo_core_api.entity.EApiFile import EApiFile
-from evo.evo_framework.core.evo_core_api.entity.EApiImage import EApiImage
-from evo.evo_framework.core.evo_core_api.entity.EApiVideo import EApiVideo
-from evo.evo_framework.core.evo_core_api.entity.EApiAudio import EApiAudio
+#from evo_framework.core.evo_core_api.entity.evo_core_api_entity_pb2 import ERequestPb as ERequest
+#from evo_framework.core.evo_core_api.entity.evo_core_api_entity_pb2 import EResponsePb as EResponse
+#from evo_framework.core.evo_core_api.entity.evo_core_api_entity_pb2 import EActionPb as EAction
+#from evo_framework.core.evo_core_api.entity.evo_core_api_entity_pb2 import EActionItemPb as EActionItem
+
+from evo_framework.core.evo_core_api.entity.EnumApiCrypto import EnumApiCrypto
+
+from evo_framework.core.evo_core_api.entity.EResponse import EResponse
+from evo_framework.core.evo_core_api.entity.ERequest import ERequest
+
+from evo_framework.core.evo_core_api.entity.EnumApiAction import EnumApiAction
+from evo_framework.core.evo_core_api.entity.EnumApiType import EnumApiType
+from evo_framework.core.evo_core_api.entity.EnumApiVisibility import EnumApiVisibility
+from evo_framework.core.evo_core_api.entity.EApiConfig import EnumApiTunnel
+from evo_framework.core.evo_core_api.entity.EApiConfig import EApiConfig
+
+from evo_framework.core.evo_core_api.entity.EActionTask import EActionTask
+
+from evo_framework.core.evo_core_api.entity.EAction import EAction
+
+from evo_framework.core.evo_core_api.entity.EApi import EApi
+
+from evo_framework.core.evo_core_api.entity.EApiFile import EApiFile
+from evo_framework.core.evo_core_api.entity.EApiImage import EApiImage
+from evo_framework.core.evo_core_api.entity.EApiVideo import EApiVideo
+from evo_framework.core.evo_core_api.entity.EApiAudio import EApiAudio
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/utility/IuApi.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/utility/IuApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 #                           0 0    0                                                                                                    #
 #                           0      0                                                                                                    #
 #                           00000000                                                                                                    #
 #                                                                                                                                       #
 # CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International       https://github.com/cyborg-ai-git     #
 # ========================================================================================================================================
 
-from evo.evo_framework.core import *
+from evo_framework.core import *
 import lz4.frame
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_api.entity import *
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.core.evo_core_api.entity import *
 
-from evo.evo_framework.core.evo_core_crypto import *
-from evo.evo_framework.core.evo_core_log import *
-from evo.evo_framework.core.evo_core_key import *
-from evo.evo_framework.core.evo_core_system import *
-from evo.evo_framework.core.evo_core_binary.utility.IuBinary import IuBinary
+from evo_framework.core.evo_core_crypto import *
+from evo_framework.core.evo_core_log import *
+from evo_framework.core.evo_core_key import *
+from evo_framework.core.evo_core_system import *
+from evo_framework.core.evo_core_binary.utility.IuBinary import IuBinary
 from PIL import Image
 import importlib
 # ---------------------------------------------------------------------------------------------------------------------------------------
 class IuApi(object):
 
  # ---------------------------------------------------------------------------------------------------------------------------------------       
     @staticmethod
@@ -50,15 +50,15 @@
             return eAction      
         except Exception as exception:
             IuLog.doException(__name__,exception)
             raise exception
         
     @staticmethod
     def addCApi(module:str):
-        from evo.evo_framework.core.evo_core_api.control.CApi import CApi
+        from evo_framework.core.evo_core_api.control.CApi import CApi
         
         if not module:
             raise Exception("ERROR_NONE_MODULE")
             
         arrayModule= module.split(".")
         className = arrayModule[-1]
         IuLog.doDebug(__name__, f"{module} {className}")
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/utility/IuApiPb.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_api/utility/IuApiPb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
-from evo.evo_framework.core import *
+from evo_framework.core import *
 import lz4.frame
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_crypto import *
-from evo.evo_framework.core.evo_core_log import *
-from evo.evo_framework.core.evo_core_api.entity import *
-from evo.evo_framework.core.evo_core_key import *
-from evo.evo_framework.core.evo_core_system import *
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_crypto import *
+from evo_framework.core.evo_core_log import *
+from evo_framework.core.evo_core_api.entity import *
+from evo_framework.core.evo_core_key import *
+from evo_framework.core.evo_core_system import *
 
 class IuApiPb(object):
     @staticmethod
     def toBytes(eObjectInput:EObject) -> bytes :
             stream = io.BytesIO()
             eObjectInput.toStream(stream)
             data=bytes(stream.getbuffer())
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/IuBinary.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_binary/utility/IuBinary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import struct
 import io
 
-from  evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_binary.utility.UBinary import UBinary
-from evo.evo_framework.core.evo_core_log.utility.IuLog import IuLog
+from  evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.core.evo_core_binary.utility.UBinary import UBinary
+from evo_framework.core.evo_core_log.utility.IuLog import IuLog
 from PIL import Image
 class IuBinary(object):
    
     #for other languages 
     @staticmethod
     def DoSetEClass(idClassName:str, classPackage:str):
         UBinary.getInstance().DoSetEClass(idClassName, classPackage)
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import struct
 import io
 
-from  evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from  evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 class IuBinaryAsync(object):
 
     @staticmethod
     async def DoWriteString(value: str, stream: io.BytesIO):
         if value == None:
             await IuBinaryAsync.DoWriteInt(-1, stream)
         else:
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/UBinary.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_binary/utility/UBinary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import struct
 import io
-from evo.evo_framework.entity import *
-from evo.evo_framework.core.evo_core_log.utility.IuLog import IuLog
-from  evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.entity import *
+from evo_framework.core.evo_core_log.utility.IuLog import IuLog
+from  evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 class UBinary:  
     __instance = None
 
     def __init__(self):
         if UBinary.__instance != None:
             raise Exception("ERROR_SINGLETON")
         else:
@@ -28,18 +28,18 @@
     def doInit(self):
         try:
             self.offsetInt = 4
             self.offsetLong = 8
             self.offsetFloat = 4
             self.offsetDouble = 8
             '''
-            self.DoSetEClass("ERequest","evo.evo_framework.core.evo_core_api.entity.ERequest")
-            self.DoSetEClass("EResponse","evo.evo_framework.core.evo_core_api.entity.EResponse")
-            self.DoSetEClass("EApiActionItem", "evo.evo_framework.core.evo_core_api.entity.EApiActionItem")
-            self.DoSetEClass("EApiAction", "evo.evo_framework.core.evo_core_api.entity.EApiAction")
+            self.DoSetEClass("ERequest","evo_framework.core.evo_core_api.entity.ERequest")
+            self.DoSetEClass("EResponse","evo_framework.core.evo_core_api.entity.EResponse")
+            self.DoSetEClass("EApiActionItem", "evo_framework.core.evo_core_api.entity.EApiActionItem")
+            self.DoSetEClass("EApiAction", "evo_framework.core.evo_core_api.entity.EApiAction")
             #@TODO:Add from evo_package_shop
             self.DoSetEClass("EShop", "evo.evo_packages.evo_package_shop.entity.EShop")
             self.DoSetEClass("EShopProduct", "evo.evo_packages.evo_package_shop.entity.EShopProduct")
             '''
         except Exception as exception:
             IuLog.doException(__name__,exception)
             raise
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_boot/control/CBoot.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_boot/control/CBoot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 import os
 import asyncio
 import sys
 import platform
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_system.utility.IuSystem import IuSystem
-from evo.evo_framework.core.evo_core_key.utility.IuKey import IuKey
-from evo.evo_framework.core.evo_core_log.utility.IuLog import IuLog
-from evo.evo_framework.core.evo_core_crypto.utility.IuCryptHash import IuCryptHash
-from evo.evo_framework.core.evo_core_crypto.utility.IuCryptEC import IuCryptEC
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_binary.utility.IuBinary import IuBinary
-from evo.evo_framework.core.evo_core_yaml.utility.IuYaml import IuYAml
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_system.utility.IuSystem import IuSystem
+from evo_framework.core.evo_core_key.utility.IuKey import IuKey
+from evo_framework.core.evo_core_log.utility.IuLog import IuLog
+from evo_framework.core.evo_core_crypto.utility.IuCryptHash import IuCryptHash
+from evo_framework.core.evo_core_crypto.utility.IuCryptEC import IuCryptEC
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.core.evo_core_binary.utility.IuBinary import IuBinary
+from evo_framework.core.evo_core_yaml.utility.IuYaml import IuYAml
 # -------------------------------------------------------------------------
 # CBoot
 # -------------------------------------------------------------------------
 class CBoot():
     __instance = None
 
     def __init__(self):
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/test_evo_core_binary.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_convert/test_evo_core_binary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/utility/IuConvert.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_convert/utility/IuConvert.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ecdsa
 from ecdsa.util import sigencode_string, sigdecode_string
-from evo.evo_framework.core.evo_core_convert.utility.IuConvert import IuConvert
+from evo_framework.core.evo_core_convert.utility.IuConvert import IuConvert
 import base64
 import hashlib
 class IuCryptEC:
     @staticmethod
     def generate_key_pair():
         sk = ecdsa.SigningKey.generate(curve=ecdsa.SECP256k1, hashfunc=hashlib.sha256)
         pk = sk.verifying_key
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_file/entity/EFileChunk.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_file/entity/EFileChunk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-from  evo.evo_framework.entity.EObject import EObject
-from  evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_crypto.utility.IuCryptHash import IuCryptHash
+from  evo_framework.entity.EObject import EObject
+from  evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.core.evo_core_crypto.utility.IuCryptHash import IuCryptHash
 class EFileChunk(EObject):
     #annotation
     def __init__(self):
         super().__init__()
         self.chunk:int = 0
         self.chunkTotal:int = 0
         self.extension:str = None
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_foundation/IFoundation.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_foundation/IFoundation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 import asyncio
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.entity.EObject import EObject
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 class IFoundation(ABC):
     @abstractmethod
     async def doSet(self, eObject, isFoundation:bool = True):
         """Implement this method"""
         pass
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_key/utility/IuKey.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_key/utility/IuKey.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime, timezone
 import hashlib
 import time
-from evo.evo_framework.core.evo_core_crypto.utility.IuCryptHash import IuCryptHash
+from evo_framework.core.evo_core_crypto.utility.IuCryptHash import IuCryptHash
 
 class IuKey:
     countNonce = 0
     @staticmethod
     def generateId(input_string:str=None):
         IuKey.countNonce +=1 
         if input_string == None:
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_log/utility/IuLog.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_log/utility/IuLog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from evo.evo_framework.core.evo_core_log.utility.ULogger import ULogger
+from evo_framework.core.evo_core_log.utility.ULogger import ULogger
 import traceback
 class IuLog(object):
     
     @staticmethod
     def doSetLevel(level:str):
         logger = ULogger.getInstance().logger
         logger.setLevel(level)
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_log/utility/ULogger.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_log/utility/ULogger.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/control/CSetting.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_setting/control/CSetting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import json
 import os
 import lz4.frame
-from evo.evo_framework.core.evo_core_setting.entity.ESetting import ESetting
-from evo.evo_framework.core.evo_core_log.utility.IuLog import IuLog
-from evo.evo_framework.core.evo_core_system.utility.IuSystem import IuSystem
+from evo_framework.core.evo_core_setting.entity.ESetting import ESetting
+from evo_framework.core.evo_core_log.utility.IuLog import IuLog
+from evo_framework.core.evo_core_system.utility.IuSystem import IuSystem
 from urllib.parse import unquote
 current_path = os.path.dirname(os.path.abspath(__file__))
 class CSetting:
     __instance = None
 
     @staticmethod
     def getInstance():
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/entity/ESetting.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_setting/entity/ESetting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from  evo.evo_framework.entity.EObject import EObject
+from  evo_framework.entity.EObject import EObject
 
 class ESetting(EObject):
     #annotation
     def __init__(self):
         super().__init__()
         self.isOutput:bool = False
         self.isUrl:bool = False
```

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_system/utility/IuSystem.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_system/utility/IuSystem.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_type/entity/EvoMap.py` & `evo_framework-2024.5.29/evo_framework/core/evo_core_type/entity/EvoMap.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.28/evo/evo_framework/entity/EObject.py` & `evo_framework-2024.5.29/evo_framework/entity/EObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 #                           0 0    0                                                                                                    #
 #                           0      0                                                                                                    #
 #                           00000000                                                                                                    #
 #                                                                                                                                       #
 # CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International       https://github.com/cyborg-ai-git     #
 #========================================================================================================================================
 
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_binary.utility.IuBinary import IuBinary
-from evo.evo_framework.core.evo_core_key.utility.IuKey import IuKey
+from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo_framework.core.evo_core_binary.utility.IuBinary import IuBinary
+from evo_framework.core.evo_core_key.utility.IuKey import IuKey
 import io
 import struct
 
 #cached
 int_packer = struct.Struct('<l')
 long_packer = struct.Struct('<q')
 float_packer = struct.Struct('<f')
```

### Comparing `evo_framework-2024.5.28/pyproject.toml` & `evo_framework-2024.5.29/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "evo-framework"
-version = "2024.5.28"
+version = "2024.5.29"
 description = "evo framework python"
 authors = ["cyborg-ai-git <129898917+cyborg-ai-git@users.noreply.github.com>"]
 readme = "README.md"
-packages = [{include = "evo"}]
+#packages = [{include = "evo"}]
 license = "CC BY-NC-ND 4.0"
 include = ["LICENSE.txt"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 PyYAML = "^6.0.1"
 lz4 = "^4.3.2"
```

### Comparing `evo_framework-2024.5.28/PKG-INFO` & `evo_framework-2024.5.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo-framework
-Version: 2024.5.28
+Version: 2024.5.29
 Summary: evo framework python
 License: CC BY-NC-ND 4.0
 Author: cyborg-ai-git
 Author-email: 129898917+cyborg-ai-git@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

