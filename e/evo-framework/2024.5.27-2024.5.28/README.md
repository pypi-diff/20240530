# Comparing `tmp/evo_framework-2024.5.27.tar.gz` & `tmp/evo_framework-2024.5.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo_framework-2024.5.27.tar", max compression
+gzip compressed data, was "evo_framework-2024.5.28.tar", max compression
```

## Comparing `evo_framework-2024.5.27.tar` & `evo_framework-2024.5.28.tar`

### file list

```diff
@@ -1,86 +1,76 @@
--rw-r--r--   0        0        0    13525 2024-05-28 16:27:09.302451 evo_framework-2024.5.27/LICENSE.txt
--rw-r--r--   0        0        0      406 2024-05-28 16:35:10.344754 evo_framework-2024.5.27/README.md
--rw-r--r--   0        0        0        0 2024-05-27 18:53:16.952349 evo_framework-2024.5.27/evo/__init__.py
--rwxr-xr-x   0        0        0      830 2024-04-17 13:11:06.786632 evo_framework-2024.5.27/evo/evo_framework/__init__.py
--rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-2024.5.27/evo/evo_framework/control/CObject.py
--rwxr-xr-x   0        0        0       55 2021-12-06 13:42:26.000000 evo_framework-2024.5.27/evo/evo_framework/control/__init__.py
--rw-r--r--   0        0        0      399 2024-05-28 10:42:13.864068 evo_framework-2024.5.27/evo/evo_framework/core/__init__.py
--rwxr-xr-x   0        0        0      172 2024-04-19 18:05:05.984591 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-28 15:55:12.165810 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/automation/entity.yaml
--rw-r--r--   0        0        0     5806 2024-05-28 13:29:01.048359 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/control/CApi.py
--rw-r--r--   0        0        0    26330 2024-05-28 13:31:18.108609 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/control/CApiFlow.py
--rw-r--r--   0        0        0      139 2024-04-23 13:31:42.061922 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/control/__init__.py
--rw-r--r--   0        0        0     1543 2024-05-28 12:49:57.985763 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EAction.py
--rw-r--r--   0        0        0     3400 2024-04-30 07:46:43.021601 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EActionItem.py
--rw-r--r--   0        0        0     1318 2024-04-19 18:07:44.067267 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EActionTask.py
--rw-r--r--   0        0        0     1690 2024-05-28 11:38:21.099639 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApi.py
--rw-r--r--   0        0        0     1673 2024-05-27 13:15:44.727399 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiAudio.py
--rw-r--r--   0        0        0     3451 2024-05-28 15:47:09.443067 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiConfig.py
--rw-r--r--   0        0        0     4429 2024-04-27 00:31:04.310181 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiEntity.py
--rw-r--r--   0        0        0     1672 2024-05-27 13:15:44.726902 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiFile.py
--rw-r--r--   0        0        0     1673 2024-05-27 13:15:44.727081 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiImage.py
--rw-r--r--   0        0        0     1245 2024-05-24 13:13:40.128210 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiItem.py
--rw-r--r--   0        0        0     1673 2024-05-27 13:15:44.727247 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiVideo.py
--rwxr-xr-x   0        0        0     2136 2024-04-20 18:47:45.597392 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/ERequest.py
--rwxr-xr-x   0        0        0      703 2024-04-15 20:02:21.126538 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EResponse.py
--rw-r--r--   0        0        0      176 2024-04-19 16:53:34.484658 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EnumApiAction.py
--rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
--rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
--rw-r--r--   0        0        0      274 2024-05-28 15:31:41.321728 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EnumApiType.py
--rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EnumLanguage.py
--rwxr-xr-x   0        0        0     1723 2024-05-27 13:30:46.260548 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/__init__.py
--rw-r--r--   0        0        0     1612 2024-05-27 13:15:44.729616 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/cs/EApiAudio.cs
--rw-r--r--   0        0        0     1611 2024-05-27 13:15:44.729333 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/cs/EApiFile.cs
--rw-r--r--   0        0        0     1612 2024-05-27 13:15:44.729435 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/cs/EApiImage.cs
--rw-r--r--   0        0        0     1612 2024-05-27 13:15:44.729535 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/cs/EApiVideo.cs
--rw-r--r--   0        0        0     5283 2024-04-25 07:23:54.907302 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/evo_core_api_entity_pb2.py
--rwxr-xr-x   0        0        0      336 2024-04-14 16:10:28.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/proto/build_proto.sh
--rw-r--r--   0        0        0    78867 2024-04-25 07:23:54.933268 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/proto/entity/cs/EvoCoreApiEntity.cs
--rw-r--r--   0        0        0     2814 2024-04-25 07:23:37.891555 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/proto/evo_core_api_entity.proto
--rwxr-xr-x   0        0        0    11450 2024-05-28 12:20:40.146628 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/utility/IuApi.py
--rw-r--r--   0        0        0    14972 2024-04-11 12:54:19.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/utility/IuApiPb.py
--rwxr-xr-x   0        0        0       68 2024-03-22 08:51:24.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/utility/__init__.py
--rwxr-xr-x   0        0        0      223 2024-03-29 21:27:12.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_binary/__init__.py
--rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_binary/entity/IBinary.py
--rwxr-xr-x   0        0        0     9101 2024-04-20 10:22:41.877540 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_binary/utility/IuBinary.py
--rw-r--r--   0        0        0     6662 2024-04-22 18:30:35.211681 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
--rw-r--r--   0        0        0     7728 2024-04-22 18:30:35.215456 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_binary/utility/UBinary.py
--rw-r--r--   0        0        0     1360 2024-04-11 08:07:07.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_boot/control/CBoot.py
--rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_bridge/IBridge.py
--rw-r--r--   0        0        0       79 2024-04-11 08:42:37.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_convert/__init__.py
--rw-r--r--   0        0        0     6217 2024-04-14 09:37:12.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_convert/test_evo_core_binary.py
--rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_convert/utility/IuConvert.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_convert/utility/__init__.py
--rw-r--r--   0        0        0      248 2024-03-29 21:12:01.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_crypto/__init__.py
--rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
--rwxr-xr-x   0        0        0     1471 2024-04-20 18:17:27.427816 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
--rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
--rw-r--r--   0        0        0     1344 2024-04-22 10:08:58.482611 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_file/entity/EFileChunk.py
--rw-r--r--   0        0        0      707 2024-04-11 08:07:07.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_foundation/IFoundation.py
--rw-r--r--   0        0        0       67 2024-03-29 21:24:14.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_key/__init__.py
--rw-r--r--   0        0        0      897 2024-04-16 15:31:33.740160 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_key/utility/IuKey.py
--rw-r--r--   0        0        0       67 2024-03-29 18:12:11.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_log/__init__.py
--rw-r--r--   0        0        0     2154 2024-03-17 19:32:16.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_log/utility/IuLog.py
--rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_log/utility/ULogger.py
--rwxr-xr-x   0        0        0      154 2024-04-11 08:09:54.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_setting/__init__.py
--rw-r--r--   0        0        0     2825 2024-04-20 18:51:28.692331 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_setting/control/CSetting.py
--rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_setting/control/__init__.py
--rw-r--r--   0        0        0     1205 2024-04-22 10:09:10.368909 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_setting/entity/ESetting.py
--rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_setting/entity/__init__.py
--rw-r--r--   0        0        0       76 2024-03-29 21:25:40.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_system/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_system/control/__init__.py
--rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_system/utility/IuSystem.py
--rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_system/utility/__init__.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_type/__init__.py
--rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_type/entity/EvoMap.py
--rw-r--r--   0        0        0       70 2024-04-11 08:44:35.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_yaml/__init__.py
--rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-2024.5.27/evo/evo_framework/core/evo_core_yaml/utility/IuYaml.py
--rwxr-xr-x   0        0        0     9407 2024-05-28 16:14:36.768193 evo_framework-2024.5.27/evo/evo_framework/entity/EObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-2024.5.27/evo/evo_framework/entity/IEObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-2024.5.27/evo/evo_framework/entity/IEvo.py
--rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-2024.5.27/evo/evo_framework/entity/Id.py
--rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-2024.5.27/evo/evo_framework/entity/Time.py
--rwxr-xr-x   0        0        0      185 2024-03-29 18:40:07.000000 evo_framework-2024.5.27/evo/evo_framework/entity/__init__.py
--rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-2024.5.27/evo/evo_framework/utility/__init__.py
--rw-r--r--   0        0        0      556 2024-05-28 16:35:28.603940 evo_framework-2024.5.27/pyproject.toml
--rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 evo_framework-2024.5.27/PKG-INFO
+-rw-r--r--   0        0        0    13525 2024-05-28 16:27:09.302451 evo_framework-2024.5.28/LICENSE.txt
+-rw-r--r--   0        0        0      406 2024-05-28 16:35:10.344754 evo_framework-2024.5.28/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 18:53:16.952349 evo_framework-2024.5.28/evo/__init__.py
+-rwxr-xr-x   0        0        0      830 2024-04-17 13:11:06.786632 evo_framework-2024.5.28/evo/evo_framework/__init__.py
+-rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-2024.5.28/evo/evo_framework/control/CObject.py
+-rwxr-xr-x   0        0        0       55 2021-12-06 13:42:26.000000 evo_framework-2024.5.28/evo/evo_framework/control/__init__.py
+-rw-r--r--   0        0        0      399 2024-05-28 10:42:13.864068 evo_framework-2024.5.28/evo/evo_framework/core/__init__.py
+-rwxr-xr-x   0        0        0      172 2024-04-19 18:05:05.984591 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/__init__.py
+-rw-r--r--   0        0        0     2136 2024-05-29 22:43:27.679085 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/automation/entity.yaml
+-rw-r--r--   0        0        0     5806 2024-05-28 13:29:01.048359 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/control/CApi.py
+-rw-r--r--   0        0        0    26330 2024-05-28 13:31:18.108609 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/control/CApiFlow.py
+-rw-r--r--   0        0        0      139 2024-04-23 13:31:42.061922 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/control/__init__.py
+-rw-r--r--   0        0        0     1834 2024-05-29 23:04:53.266652 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EAction.py
+-rw-r--r--   0        0        0     1318 2024-04-19 18:07:44.067267 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EActionTask.py
+-rw-r--r--   0        0        0     1701 2024-05-29 23:04:53.276117 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApi.py
+-rw-r--r--   0        0        0     1788 2024-05-29 23:04:53.280064 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiAudio.py
+-rw-r--r--   0        0        0     3057 2024-05-29 23:08:56.693463 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiConfig.py
+-rw-r--r--   0        0        0     1785 2024-05-29 23:04:53.291651 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiFile.py
+-rw-r--r--   0        0        0     1793 2024-05-29 23:04:53.294896 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiImage.py
+-rw-r--r--   0        0        0     1788 2024-05-29 23:04:53.297767 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiVideo.py
+-rwxr-xr-x   0        0        0     2136 2024-04-20 18:47:45.597392 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/ERequest.py
+-rwxr-xr-x   0        0        0      703 2024-04-15 20:02:21.126538 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EResponse.py
+-rw-r--r--   0        0        0      568 2024-05-29 23:04:53.300310 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiAction.py
+-rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
+-rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
+-rw-r--r--   0        0        0      274 2024-05-28 15:31:41.321728 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiType.py
+-rw-r--r--   0        0        0      493 2024-05-29 23:04:53.308461 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumApiVisibility.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EnumLanguage.py
+-rwxr-xr-x   0        0        0     1730 2024-05-29 23:05:16.396723 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/__init__.py
+-rwxr-xr-x   0        0        0    11450 2024-05-28 12:20:40.146628 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/utility/IuApi.py
+-rw-r--r--   0        0        0    14972 2024-04-11 12:54:19.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/utility/IuApiPb.py
+-rwxr-xr-x   0        0        0       68 2024-03-22 08:51:24.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/utility/__init__.py
+-rwxr-xr-x   0        0        0      223 2024-03-29 21:27:12.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/__init__.py
+-rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/entity/IBinary.py
+-rwxr-xr-x   0        0        0     9101 2024-04-20 10:22:41.877540 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/IuBinary.py
+-rw-r--r--   0        0        0     6662 2024-04-22 18:30:35.211681 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
+-rw-r--r--   0        0        0     7728 2024-04-22 18:30:35.215456 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/UBinary.py
+-rw-r--r--   0        0        0     1360 2024-04-11 08:07:07.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_boot/control/CBoot.py
+-rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_bridge/IBridge.py
+-rw-r--r--   0        0        0       79 2024-04-11 08:42:37.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/__init__.py
+-rw-r--r--   0        0        0     6217 2024-04-14 09:37:12.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/test_evo_core_binary.py
+-rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/utility/IuConvert.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/utility/__init__.py
+-rw-r--r--   0        0        0      248 2024-03-29 21:12:01.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/__init__.py
+-rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
+-rwxr-xr-x   0        0        0     1471 2024-04-20 18:17:27.427816 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
+-rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
+-rw-r--r--   0        0        0     1344 2024-04-22 10:08:58.482611 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_file/entity/EFileChunk.py
+-rw-r--r--   0        0        0      707 2024-04-11 08:07:07.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_foundation/IFoundation.py
+-rw-r--r--   0        0        0       67 2024-03-29 21:24:14.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_key/__init__.py
+-rw-r--r--   0        0        0      897 2024-04-16 15:31:33.740160 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_key/utility/IuKey.py
+-rw-r--r--   0        0        0       67 2024-03-29 18:12:11.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_log/__init__.py
+-rw-r--r--   0        0        0     2154 2024-03-17 19:32:16.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_log/utility/IuLog.py
+-rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_log/utility/ULogger.py
+-rwxr-xr-x   0        0        0      154 2024-04-11 08:09:54.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/__init__.py
+-rw-r--r--   0        0        0     2825 2024-04-20 18:51:28.692331 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/control/CSetting.py
+-rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/control/__init__.py
+-rw-r--r--   0        0        0     1205 2024-04-22 10:09:10.368909 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/entity/ESetting.py
+-rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/entity/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-29 21:25:40.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_system/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_system/control/__init__.py
+-rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_system/utility/IuSystem.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_system/utility/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_type/__init__.py
+-rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_type/entity/EvoMap.py
+-rw-r--r--   0        0        0       70 2024-04-11 08:44:35.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_yaml/__init__.py
+-rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-2024.5.28/evo/evo_framework/core/evo_core_yaml/utility/IuYaml.py
+-rwxr-xr-x   0        0        0     9407 2024-05-28 16:14:36.768193 evo_framework-2024.5.28/evo/evo_framework/entity/EObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-2024.5.28/evo/evo_framework/entity/IEObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-2024.5.28/evo/evo_framework/entity/IEvo.py
+-rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-2024.5.28/evo/evo_framework/entity/Id.py
+-rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-2024.5.28/evo/evo_framework/entity/Time.py
+-rwxr-xr-x   0        0        0      185 2024-03-29 18:40:07.000000 evo_framework-2024.5.28/evo/evo_framework/entity/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-2024.5.28/evo/evo_framework/utility/__init__.py
+-rw-r--r--   0        0        0      556 2024-05-29 22:59:57.712590 evo_framework-2024.5.28/pyproject.toml
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 evo_framework-2024.5.28/PKG-INFO
```

### Comparing `evo_framework-2024.5.27/LICENSE.txt` & `evo_framework-2024.5.28/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/__init__.py` & `evo_framework-2024.5.28/evo/evo_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/control/CObject.py` & `evo_framework-2024.5.28/evo/evo_framework/control/CObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/automation/entity.yaml` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/automation/entity.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -29,57 +29,64 @@
     COMPLETE
 
   EnumApiVisibility:
     PUBLIC
     PRIVATE
 
 entity:
-  EApi:
-    description: STRING
+  EApi: 
+    _DESCRIPTION_: "this is EAPI DESCRIPTION"
+    description: STRING "this is a description"
     isStream: BOOL     
     input: STRING
     output: STRING
 
   EAction:
+    _DESCRIPTION_: "this is EAction DESCRIPTION"
     enumApiAction: ENUM EnumApiAction .NONE
     action: STRING     
     input: BYTES 
     output: BYTES
 
   EApiConfig:
-        enumApiVisibility: ENUM EnumApiVisibility .PRIVATE
-        publicKey: BYTES
-        label: STRING
-        description: STRING
-        urlLogo: STRING
-        remoteUrl: STRING 
-        remotePort: INT 443
-        os: STRING
-        mapEApi: MAP EApi
+      _DESCRIPTION_: "this is EAction DESCRIPTION"
+      enumApiVisibility: ENUM EnumApiVisibility .PRIVATE
+      publicKey: BYTES
+      label: STRING
+      description: STRING
+      urlLogo: STRING
+      remoteUrl: STRING 
+      remotePort: INT 443
+      os: STRING
+      mapEApi: MAP EApi
 
   EApiFile:
+    _DESCRIPTION_: "this is EApiFile DESCRIPTION"
     isUrl: BOOL
     name : STRING
     ext: STRING
     length : LONG
     data: BYTES
 
   EApiImage:
+    _DESCRIPTION_: "this is EAPiImagection DESCRIPTION"
     isUrl: BOOL
     name : STRING
     ext: STRING
     length : LONG
     data: BYTES
 
   EApiVideo:
+    _DESCRIPTION_: "this is EApiVideo DESCRIPTION"
     isUrl: BOOL
     name : STRING
     ext: STRING
     length : LONG
     data: BYTES
 
   EApiAudio:
+    _DESCRIPTION_: "this is EAPIAudio DESCRIPTION"
     isUrl: BOOL
     name : STRING
     ext: STRING
     length : LONG
     data: BYTES
```

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/control/CApi.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/control/CApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/control/CApiFlow.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/control/CApiFlow.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EActionTask.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EActionTask.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApi.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_file/entity/EFileChunk.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,37 @@
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_api.entity.EApiItem import EApiItem
-from evo.evo_framework.core.evo_core_api.entity.EnumApiType import EnumApiType
-from evo.evo_framework.core.evo_core_log.utility.IuLog import IuLog
-class EApi(EObject):
+
+from  evo.evo_framework.entity.EObject import EObject
+from  evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+from evo.evo_framework.core.evo_core_crypto.utility.IuCryptHash import IuCryptHash
+class EFileChunk(EObject):
     #annotation
-    
     def __init__(self):
         super().__init__()
-        self.description:str = None
-        self.isStream:bool = False       
-        self.input:str = None
-        self.output:str = None
+        self.chunk:int = 0
+        self.chunkTotal:int = 0
+        self.extension:str = None
+        self.length:int = 0   
 
-        #NOT_SERIALIZED
-        self.context = {}
-        self.callback = None
-        self.isEnabled:bool = True
-        
     def toStream(self, stream):
         super().toStream(stream)
-        self._doWriteStr(self.description, stream)
-        self._doWriteBool(self.isStream, stream)
-        self._doWriteStr(self.input, stream)
-        self._doWriteStr(self.output, stream)
-
+        self._doWriteInt(self.chunk, stream)
+        self._doWriteInt(self.chunkTotal, stream)
+        self._doWriteStr(self.extension, stream)
+        self._doWriteInt(self.length, stream)
+ 
     def fromStream(self, stream):
         super().fromStream(stream)
-        self.description = self._doReadStr(stream)
-        self.isStream = self._doReadBool(stream)
-        self.input = self._doReadStr(stream)
-        self.output = self._doReadStr(stream)
-
-    def __str__(self) -> str:
+        self.chunk = self._doReadInt(stream)
+        self.chunkTotal = self._doReadInt(stream)
+        self.extension = self._doReadStr(stream)
+        self.length = self._doReadInt(stream)
+    
+    def toString(self) -> str:
         strReturn = "\n".join([
-                            super().__str__(),        
-                            f"\tisStream:{self.isStream}",
-                            f"\tcontext:{self.context}",
-                            f"\tinput:{self.input}", 
-                            f"\toutput:{self.output}",
-                            f"callback:{self.callback}",                  
+                            super().toString(),
+                            f"chunk:{self.chunk}",
+                            f"chunkTotal:{self.chunkTotal}",
+                            f"extension:{self.extension}",
+                            f"length:{self.length}"
                             ]) 
-        return strReturn
+        return strReturn
+
```

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiAudio.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiFile.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
 from evo.evo_framework.entity.EObject import EObject
 from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
-class EApiAudio(EObject):
-	#annotation
+"""EApiFile
+
+	this is EApiFile DESCRIPTION
 	
+"""
+class EApiFile(EObject):
+
+	VERSION:str="3c37d0d7315664187980d10bc9abe5541b93f38ef107473e66bc336fac026f55"
+
 	def __init__(self):
 		super().__init__()
 		
 		self.isUrl:bool = None
 		self.name:str = None
 		self.ext:str = None
 		self.length:int = None
@@ -34,15 +40,15 @@
 		self.name = self._doReadStr(stream)
 		self.ext = self._doReadStr(stream)
 		self.length = self._doReadInt(stream)
 		self.data = self._doReadBytes(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
-							super().__str__(),
+				super().__str__(),
 							
 				f"\tisUrl:{ self.isUrl  }",
 				f"\tname:{ self.name  }",
 				f"\text:{ self.ext  }",
 				f"\tlength:{ self.length  }",
 				f"\tdata:{ self.data  }",
 							])
```

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiFile.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiVideo.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
 from evo.evo_framework.entity.EObject import EObject
 from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
-class EApiFile(EObject):
-	#annotation
+"""EApiVideo
+
+	this is EApiVideo DESCRIPTION
 	
+"""
+class EApiVideo(EObject):
+
+	VERSION:str="3c37d0d7315664187980d10bc9abe5541b93f38ef107473e66bc336fac026f55"
+
 	def __init__(self):
 		super().__init__()
 		
 		self.isUrl:bool = None
 		self.name:str = None
 		self.ext:str = None
 		self.length:int = None
@@ -34,15 +40,15 @@
 		self.name = self._doReadStr(stream)
 		self.ext = self._doReadStr(stream)
 		self.length = self._doReadInt(stream)
 		self.data = self._doReadBytes(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
-							super().__str__(),
+				super().__str__(),
 							
 				f"\tisUrl:{ self.isUrl  }",
 				f"\tname:{ self.name  }",
 				f"\text:{ self.ext  }",
 				f"\tlength:{ self.length  }",
 				f"\tdata:{ self.data  }",
 							])
```

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiImage.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiAudio.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
 from evo.evo_framework.entity.EObject import EObject
 from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
-class EApiImage(EObject):
-	#annotation
+"""EApiAudio
+
+	this is EAPIAudio DESCRIPTION
 	
+"""
+class EApiAudio(EObject):
+
+	VERSION:str="3c37d0d7315664187980d10bc9abe5541b93f38ef107473e66bc336fac026f55"
+
 	def __init__(self):
 		super().__init__()
 		
 		self.isUrl:bool = None
 		self.name:str = None
 		self.ext:str = None
 		self.length:int = None
@@ -34,15 +40,15 @@
 		self.name = self._doReadStr(stream)
 		self.ext = self._doReadStr(stream)
 		self.length = self._doReadInt(stream)
 		self.data = self._doReadBytes(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
-							super().__str__(),
+				super().__str__(),
 							
 				f"\tisUrl:{ self.isUrl  }",
 				f"\tname:{ self.name  }",
 				f"\text:{ self.ext  }",
 				f"\tlength:{ self.length  }",
 				f"\tdata:{ self.data  }",
 							])
```

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiItem.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/entity/ESetting.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from evo.evo_framework.entity.EObject import EObject
-from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo.evo_framework.core.evo_core_api.entity.EnumApiType import EnumApiType
+from  evo.evo_framework.entity.EObject import EObject
 
-class EApiItem(EObject):
+class ESetting(EObject):
     #annotation
     def __init__(self):
         super().__init__()
-        self.enumApiType:EnumApiType = EnumApiType.STRING
-        self.mapEApiItem = EvoMap()
-        
-        #TODO:ADD TO SERIALIZE  
-        self.eClass = None
-        self.rangeDefault = None
-        self.rangeMin = None
-        self.rangeMax = None
+        self.isOutput:bool = False
+        self.isUrl:bool = False
+        self.typeExt:str = None
+        self.data:bytes =None
           
     def toStream(self, stream):
         super().toStream(stream)
-        self._doWriteInt(self.enumApiType.value, stream)
-        self._doWriteMap(self.mapEApiItem, stream)
-           
+        self._doWriteBool(self.isOutput, stream)
+        self._doWriteBool(self.isUrl, stream)
+        self._doWriteStr(self.typeExt, stream)
+        self._doWriteBytes(self.data, stream)
+      
+        
     def fromStream(self, stream):
         super().fromStream(stream)
-        self.enumApiType = EnumApiType(self._doReadInt(stream))
-        self._doReadMap(EApiItem, stream)
-        
+        self.isOutput = self._doReadBool(stream)
+        self.isUrl = self._doReadBool(stream)
+        self.typeExt = self._doReadStr(stream)
+        self.data = self._doReadBytes(stream)
+       
     def __str__(self) -> str:
         strReturn = "\n".join([
-                            super().__str__(),        
-                            f"enumApiType:{self.enumApiType}",  
-                            f"mapEApiItem:{self.mapEApiItem}",               
+                            super().__str__(),
+                            f"isOutput:{self.isOutput}",
+                            f"isUrl:{self.isUrl}",
+                            f"typeExt:{self.typeExt}",
+                            f"data:{self.data[:100]}",
                             ]) 
-        return strReturn
+        return strReturn
```

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EApiVideo.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EApiImage.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
 from evo.evo_framework.entity.EObject import EObject
 from evo.evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
-class EApiVideo(EObject):
-	#annotation
+"""EApiImage
+
+	this is EAPiImagection DESCRIPTION
 	
+"""
+class EApiImage(EObject):
+
+	VERSION:str="3c37d0d7315664187980d10bc9abe5541b93f38ef107473e66bc336fac026f55"
+
 	def __init__(self):
 		super().__init__()
 		
 		self.isUrl:bool = None
 		self.name:str = None
 		self.ext:str = None
 		self.length:int = None
@@ -34,15 +40,15 @@
 		self.name = self._doReadStr(stream)
 		self.ext = self._doReadStr(stream)
 		self.length = self._doReadInt(stream)
 		self.data = self._doReadBytes(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
-							super().__str__(),
+				super().__str__(),
 							
 				f"\tisUrl:{ self.isUrl  }",
 				f"\tname:{ self.name  }",
 				f"\text:{ self.ext  }",
 				f"\tlength:{ self.length  }",
 				f"\tdata:{ self.data  }",
 							])
```

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/ERequest.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/ERequest.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/EResponse.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/EResponse.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/entity/__init__.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/entity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from evo.evo_framework.core.evo_core_api.entity.EnumApiCrypto import EnumApiCrypto
 
 from evo.evo_framework.core.evo_core_api.entity.EResponse import EResponse
 from evo.evo_framework.core.evo_core_api.entity.ERequest import ERequest
 
 from evo.evo_framework.core.evo_core_api.entity.EnumApiAction import EnumApiAction
 from evo.evo_framework.core.evo_core_api.entity.EnumApiType import EnumApiType
-from evo.evo_framework.core.evo_core_api.entity.EApiConfig import EnumApiVisibility
+from evo.evo_framework.core.evo_core_api.entity.EnumApiVisibility import EnumApiVisibility
 from evo.evo_framework.core.evo_core_api.entity.EApiConfig import EnumApiTunnel
 from evo.evo_framework.core.evo_core_api.entity.EApiConfig import EApiConfig
 
 from evo.evo_framework.core.evo_core_api.entity.EActionTask import EActionTask
 
 from evo.evo_framework.core.evo_core_api.entity.EAction import EAction
 from evo.evo_framework.core.evo_core_api.entity.EActionItem import EActionItem
```

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/utility/IuApi.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/utility/IuApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_api/utility/IuApiPb.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_api/utility/IuApiPb.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_binary/utility/IuBinary.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/IuBinary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_binary/utility/UBinary.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_binary/utility/UBinary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_boot/control/CBoot.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_boot/control/CBoot.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_convert/test_evo_core_binary.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/test_evo_core_binary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_convert/utility/IuConvert.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_convert/utility/IuConvert.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_foundation/IFoundation.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_foundation/IFoundation.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_key/utility/IuKey.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_key/utility/IuKey.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_log/utility/IuLog.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_log/utility/IuLog.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_log/utility/ULogger.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_log/utility/ULogger.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_setting/control/CSetting.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_setting/control/CSetting.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_system/utility/IuSystem.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_system/utility/IuSystem.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/core/evo_core_type/entity/EvoMap.py` & `evo_framework-2024.5.28/evo/evo_framework/core/evo_core_type/entity/EvoMap.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/evo/evo_framework/entity/EObject.py` & `evo_framework-2024.5.28/evo/evo_framework/entity/EObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.27/pyproject.toml` & `evo_framework-2024.5.28/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evo-framework"
-version = "2024.5.27"
+version = "2024.5.28"
 description = "evo framework python"
 authors = ["cyborg-ai-git <129898917+cyborg-ai-git@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "evo"}]
 license = "CC BY-NC-ND 4.0"
 include = ["LICENSE.txt"]
```

### Comparing `evo_framework-2024.5.27/PKG-INFO` & `evo_framework-2024.5.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo-framework
-Version: 2024.5.27
+Version: 2024.5.28
 Summary: evo framework python
 License: CC BY-NC-ND 4.0
 Author: cyborg-ai-git
 Author-email: 129898917+cyborg-ai-git@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

