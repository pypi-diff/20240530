# Comparing `tmp/basiclibrary_py-0.6.8.tar.gz` & `tmp/basiclibrary_py-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basiclibrary_py-0.6.8.tar", max compression
+gzip compressed data, was "basiclibrary_py-0.6.9.tar", max compression
```

## Comparing `basiclibrary_py-0.6.8.tar` & `basiclibrary_py-0.6.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0       53 2022-04-20 11:29:01.695732 basiclibrary_py-0.6.8/BasicLibrary/.env.default
--rw-r--r--   0        0        0     1063 2024-01-01 07:19:21.112114 basiclibrary_py-0.6.8/BasicLibrary/.README.md
--rw-r--r--   0        0        0      869 2023-12-05 01:01:36.070344 basiclibrary_py-0.6.8/BasicLibrary/__init__.py
--rw-r--r--   0        0        0     1304 2022-04-20 11:29:46.959488 basiclibrary_py-0.6.8/BasicLibrary/__projectConfig.ini
--rw-r--r--   0        0        0      560 2022-04-20 11:30:48.364663 basiclibrary_py-0.6.8/BasicLibrary/__projectHelper.py
--rw-r--r--   0        0        0      172 2021-11-07 07:17:04.320910 basiclibrary_py-0.6.8/BasicLibrary/biz/__init__.py
--rw-r--r--   0        0        0      172 2021-11-07 07:17:04.320910 basiclibrary_py-0.6.8/BasicLibrary/biz/adobe/__init__.py
--rw-r--r--   0        0        0     6384 2024-03-18 12:15:32.701281 basiclibrary_py-0.6.8/BasicLibrary/biz/adobe/photoShopHelper.py
--rw-r--r--   0        0        0      172 2021-11-07 07:17:04.320910 basiclibrary_py-0.6.8/BasicLibrary/biz/stock/__init__.py
--rw-r--r--   0        0        0     2559 2024-03-14 02:26:18.940531 basiclibrary_py-0.6.8/BasicLibrary/biz/stock/stockHelper.py
--rw-r--r--   0        0        0     3298 2024-03-22 11:25:11.486202 basiclibrary_py-0.6.8/BasicLibrary/configHelper.py
--rw-r--r--   0        0        0      174 2022-03-10 00:57:41.847394 basiclibrary_py-0.6.8/BasicLibrary/data/__init__.py
--rw-r--r--   0        0        0     2235 2024-01-21 14:28:51.444098 basiclibrary_py-0.6.8/BasicLibrary/data/base64Helper.py
--rw-r--r--   0        0        0     1553 2024-01-01 10:44:54.125605 basiclibrary_py-0.6.8/BasicLibrary/data/chineseData.py
--rw-r--r--   0        0        0     1818 2024-02-04 08:59:41.959219 basiclibrary_py-0.6.8/BasicLibrary/data/collectionHelper.py
--rw-r--r--   0        0        0     9312 2024-03-07 05:22:07.118494 basiclibrary_py-0.6.8/BasicLibrary/data/dateTimeHelper.py
--rw-r--r--   0        0        0     5434 2024-03-19 02:00:59.587312 basiclibrary_py-0.6.8/BasicLibrary/data/dateTimePlaceHolderHelper.py
--rw-r--r--   0        0        0     1876 2024-03-08 00:08:37.845960 basiclibrary_py-0.6.8/BasicLibrary/data/dictHelper.py
--rw-r--r--   0        0        0      482 2023-10-29 10:06:49.585275 basiclibrary_py-0.6.8/BasicLibrary/data/enumBase.py
--rw-r--r--   0        0        0      429 2023-10-29 05:13:15.019355 basiclibrary_py-0.6.8/BasicLibrary/data/enumHelper.py
--rw-r--r--   0        0        0        0 2021-04-24 11:00:12.466000 basiclibrary_py-0.6.8/BasicLibrary/data/htmlHelper.py
--rw-r--r--   0        0        0     6478 2024-03-14 02:16:19.043598 basiclibrary_py-0.6.8/BasicLibrary/data/listHelper.py
--rw-r--r--   0        0        0     1340 2023-12-17 07:56:12.197269 basiclibrary_py-0.6.8/BasicLibrary/data/numberHelper.py
--rw-r--r--   0        0        0     3474 2023-12-17 07:56:12.294709 basiclibrary_py-0.6.8/BasicLibrary/data/objectHelper.py
--rw-r--r--   0        0        0     3227 2024-03-15 01:21:43.361361 basiclibrary_py-0.6.8/BasicLibrary/data/pandasHelper.py
--rw-r--r--   0        0        0     1262 2024-01-01 00:18:18.746359 basiclibrary_py-0.6.8/BasicLibrary/data/randomHelper.py
--rw-r--r--   0        0        0      811 2023-12-17 07:58:42.455096 basiclibrary_py-0.6.8/BasicLibrary/data/reflectHelper.py
--rw-r--r--   0        0        0     1952 2023-12-17 07:58:42.306782 basiclibrary_py-0.6.8/BasicLibrary/data/regexHelper.py
--rw-r--r--   0        0        0        2 2021-03-21 10:02:22.227000 basiclibrary_py-0.6.8/BasicLibrary/data/setHelper.py
--rw-r--r--   0        0        0    11384 2024-03-19 02:13:01.276702 basiclibrary_py-0.6.8/BasicLibrary/data/stringHelper.py
--rw-r--r--   0        0        0      317 2023-06-13 12:00:42.965651 basiclibrary_py-0.6.8/BasicLibrary/data/typeEnum.py
--rw-r--r--   0        0        0      384 2024-03-11 08:21:52.844961 basiclibrary_py-0.6.8/BasicLibrary/data/typeHelper.py
--rw-r--r--   0        0        0      117 2022-04-20 11:22:18.330540 basiclibrary_py-0.6.8/BasicLibrary/dataBase/.README.md
--rw-r--r--   0        0        0      218 2022-04-20 11:22:18.274626 basiclibrary_py-0.6.8/BasicLibrary/dataBase/__init__.py
--rw-r--r--   0        0        0     4855 2023-12-17 08:07:39.547566 basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseClient.py
--rw-r--r--   0        0        0     2187 2022-04-20 11:23:22.877729 basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseDDL.py
--rw-r--r--   0        0        0      345 2022-04-20 11:23:51.740994 basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseEnum.py
--rw-r--r--   0        0        0     6920 2023-12-17 08:07:39.601794 basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseHelper.py
--rw-r--r--   0        0        0     5468 2023-06-06 09:46:34.292073 basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseMate.py
--rw-r--r--   0        0        0     1184 2023-12-17 08:07:39.389051 basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseUnitTest.py
--rw-r--r--   0        0        0      164 2022-04-20 11:17:08.876036 basiclibrary_py-0.6.8/BasicLibrary/dataBase/MongoDB/__init__.py
--rw-r--r--   0        0        0     1501 2023-06-06 09:46:34.424073 basiclibrary_py-0.6.8/BasicLibrary/dataBase/MongoDB/ddl.py
--rw-r--r--   0        0        0     2829 2023-06-06 09:46:32.432228 basiclibrary_py-0.6.8/BasicLibrary/dataBase/MongoDB/helper.py
--rw-r--r--   0        0        0    10551 2023-06-06 09:46:34.371074 basiclibrary_py-0.6.8/BasicLibrary/dataBase/MongoDB/mate.py
--rw-r--r--   0        0        0      164 2022-04-20 11:18:12.573529 basiclibrary_py-0.6.8/BasicLibrary/dataBase/MySql/__init__.py
--rw-r--r--   0        0        0     4642 2023-06-06 09:46:32.256228 basiclibrary_py-0.6.8/BasicLibrary/dataBase/MySql/ddl.py
--rw-r--r--   0        0        0    12613 2023-06-06 09:46:33.878072 basiclibrary_py-0.6.8/BasicLibrary/dataBase/MySql/mate.py
--rw-r--r--   0        0        0     3368 2023-06-06 09:46:33.288072 basiclibrary_py-0.6.8/BasicLibrary/dataBase/MySql/pool.py
--rw-r--r--   0        0        0     1416 2023-10-29 10:17:06.615653 basiclibrary_py-0.6.8/BasicLibrary/enums.py
--rw-r--r--   0        0        0      164 2022-04-20 11:24:39.998992 basiclibrary_py-0.6.8/BasicLibrary/environment/__init__.py
--rw-r--r--   0        0        0     1792 2024-02-07 09:16:12.011979 basiclibrary_py-0.6.8/BasicLibrary/environment/consoleHelper.py
--rw-r--r--   0        0        0     1840 2024-02-08 08:18:20.145848 basiclibrary_py-0.6.8/BasicLibrary/environment/dynamicImporter.py
--rw-r--r--   0        0        0     1534 2024-03-07 23:59:26.745695 basiclibrary_py-0.6.8/BasicLibrary/environment/envHelper.py
--rw-r--r--   0        0        0      871 2023-11-28 04:19:44.496618 basiclibrary_py-0.6.8/BasicLibrary/environment/inspectHelper.py
--rw-r--r--   0        0        0      257 2022-04-20 11:25:32.285848 basiclibrary_py-0.6.8/BasicLibrary/io/.README.md
--rw-r--r--   0        0        0      164 2022-04-20 11:24:39.959993 basiclibrary_py-0.6.8/BasicLibrary/io/__init__.py
--rw-r--r--   0        0        0      513 2023-12-22 01:58:17.778023 basiclibrary_py-0.6.8/BasicLibrary/io/_util.py
--rw-r--r--   0        0        0     6674 2024-03-19 02:32:44.881905 basiclibrary_py-0.6.8/BasicLibrary/io/dirHelper.py
--rw-r--r--   0        0        0    14148 2024-03-14 02:12:35.144386 basiclibrary_py-0.6.8/BasicLibrary/io/fileHelper.py
--rw-r--r--   0        0        0     2028 2024-01-23 02:40:36.256785 basiclibrary_py-0.6.8/BasicLibrary/io/fileShadowUsing.py
--rw-r--r--   0        0        0     3003 2024-03-14 01:23:35.768121 basiclibrary_py-0.6.8/BasicLibrary/io/imageHelper.py
--rw-r--r--   0        0        0      650 2024-01-11 02:48:40.389344 basiclibrary_py-0.6.8/BasicLibrary/io/ioEnums.py
--rw-r--r--   0        0        0     1914 2024-01-23 02:40:36.131143 basiclibrary_py-0.6.8/BasicLibrary/io/ioHelper.py
--rw-r--r--   0        0        0     3036 2024-03-14 01:59:35.020362 basiclibrary_py-0.6.8/BasicLibrary/io/pathHelper.py
--rw-r--r--   0        0        0      186 2022-04-20 11:26:05.648500 basiclibrary_py-0.6.8/BasicLibrary/model/__init__.py
--rw-r--r--   0        0        0     1365 2024-01-23 02:42:35.556378 basiclibrary_py-0.6.8/BasicLibrary/model/container.py
--rw-r--r--   0        0        0     2246 2024-01-23 02:43:18.797533 basiclibrary_py-0.6.8/BasicLibrary/model/dataCompare.py
--rw-r--r--   0        0        0     1099 2022-04-20 11:26:29.999355 basiclibrary_py-0.6.8/BasicLibrary/model/kvPair.py
--rw-r--r--   0        0        0     1294 2024-01-23 02:08:08.731306 basiclibrary_py-0.6.8/BasicLibrary/model/returnResult.py
--rw-r--r--   0        0        0      342 2022-04-20 11:26:30.136355 basiclibrary_py-0.6.8/BasicLibrary/model/stopWatcher.py
--rw-r--r--   0        0        0      579 2022-04-20 11:26:59.149767 basiclibrary_py-0.6.8/BasicLibrary/office/.README.md
--rw-r--r--   0        0        0      164 2022-04-20 11:26:38.013071 basiclibrary_py-0.6.8/BasicLibrary/office/__init__.py
--rw-r--r--   0        0        0     6634 2023-06-06 09:46:31.715228 basiclibrary_py-0.6.8/BasicLibrary/office/excelBookMate.py
--rw-r--r--   0        0        0     2560 2023-12-11 13:04:35.845636 basiclibrary_py-0.6.8/BasicLibrary/office/excelHelper.py
--rw-r--r--   0        0        0     3375 2023-06-07 11:44:09.970141 basiclibrary_py-0.6.8/BasicLibrary/office/excelMisc.py
--rw-r--r--   0        0        0      786 2023-06-16 03:30:23.970591 basiclibrary_py-0.6.8/BasicLibrary/office/excelShadowUsing.py
--rw-r--r--   0        0        0    11261 2023-12-11 12:41:18.840106 basiclibrary_py-0.6.8/BasicLibrary/office/excelSheetMate.py
--rw-r--r--   0        0        0      163 2022-04-20 11:27:42.609162 basiclibrary_py-0.6.8/BasicLibrary/pattern/__init__.py
--rw-r--r--   0        0        0      560 2024-01-23 02:45:07.082985 basiclibrary_py-0.6.8/BasicLibrary/pattern/singleton.py
--rw-r--r--   0        0        0      689 2024-03-19 03:44:40.152725 basiclibrary_py-0.6.8/BasicLibrary/projectHelper.py
--rw-r--r--   0        0        0      164 2022-04-20 11:28:12.466235 basiclibrary_py-0.6.8/BasicLibrary/syntax/__init__.py
--rw-r--r--   0        0        0     1664 2022-04-20 11:28:39.899931 basiclibrary_py-0.6.8/BasicLibrary/syntax/switch.py
--rw-r--r--   0        0        0      164 2022-04-20 11:28:40.026934 basiclibrary_py-0.6.8/BasicLibrary/web/__init__.py
--rw-r--r--   0        0        0     7972 2021-11-09 12:40:32.982432 basiclibrary_py-0.6.8/BasicLibrary/web/beautifulSoupHelper.py
--rw-r--r--   0        0        0     1790 2022-04-20 11:28:54.662749 basiclibrary_py-0.6.8/BasicLibrary/web/requestHelper.py
--rw-r--r--   0        0        0      467 2024-03-22 11:33:10.507883 basiclibrary_py-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     3469 2024-03-08 11:01:21.965314 basiclibrary_py-0.6.8/README.md
--rw-r--r--   0        0        0     3952 1970-01-01 00:00:00.000000 basiclibrary_py-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0       53 2022-04-20 11:29:01.695732 basiclibrary_py-0.6.9/BasicLibrary/.env.default
+-rw-r--r--   0        0        0     1063 2024-01-01 07:19:21.112114 basiclibrary_py-0.6.9/BasicLibrary/.README.md
+-rw-r--r--   0        0        0      869 2023-12-05 01:01:36.070344 basiclibrary_py-0.6.9/BasicLibrary/__init__.py
+-rw-r--r--   0        0        0     1304 2022-04-20 11:29:46.959488 basiclibrary_py-0.6.9/BasicLibrary/__projectConfig.ini
+-rw-r--r--   0        0        0      560 2022-04-20 11:30:48.364663 basiclibrary_py-0.6.9/BasicLibrary/__projectHelper.py
+-rw-r--r--   0        0        0      172 2021-11-07 07:17:04.320910 basiclibrary_py-0.6.9/BasicLibrary/biz/__init__.py
+-rw-r--r--   0        0        0      172 2021-11-07 07:17:04.320910 basiclibrary_py-0.6.9/BasicLibrary/biz/adobe/__init__.py
+-rw-r--r--   0        0        0     6384 2024-03-18 12:15:32.701281 basiclibrary_py-0.6.9/BasicLibrary/biz/adobe/photoShopHelper.py
+-rw-r--r--   0        0        0      172 2021-11-07 07:17:04.320910 basiclibrary_py-0.6.9/BasicLibrary/biz/stock/__init__.py
+-rw-r--r--   0        0        0     2559 2024-03-14 02:26:18.940531 basiclibrary_py-0.6.9/BasicLibrary/biz/stock/stockHelper.py
+-rw-r--r--   0        0        0     3298 2024-03-22 11:25:11.486202 basiclibrary_py-0.6.9/BasicLibrary/configHelper.py
+-rw-r--r--   0        0        0      174 2022-03-10 00:57:41.847394 basiclibrary_py-0.6.9/BasicLibrary/data/__init__.py
+-rw-r--r--   0        0        0     2235 2024-01-21 14:28:51.444098 basiclibrary_py-0.6.9/BasicLibrary/data/base64Helper.py
+-rw-r--r--   0        0        0     1553 2024-01-01 10:44:54.125605 basiclibrary_py-0.6.9/BasicLibrary/data/chineseData.py
+-rw-r--r--   0        0        0     1818 2024-02-04 08:59:41.959219 basiclibrary_py-0.6.9/BasicLibrary/data/collectionHelper.py
+-rw-r--r--   0        0        0     9312 2024-03-07 05:22:07.118494 basiclibrary_py-0.6.9/BasicLibrary/data/dateTimeHelper.py
+-rw-r--r--   0        0        0     5434 2024-03-19 02:00:59.587312 basiclibrary_py-0.6.9/BasicLibrary/data/dateTimePlaceHolderHelper.py
+-rw-r--r--   0        0        0     1876 2024-03-08 00:08:37.845960 basiclibrary_py-0.6.9/BasicLibrary/data/dictHelper.py
+-rw-r--r--   0        0        0      482 2023-10-29 10:06:49.585275 basiclibrary_py-0.6.9/BasicLibrary/data/enumBase.py
+-rw-r--r--   0        0        0      429 2023-10-29 05:13:15.019355 basiclibrary_py-0.6.9/BasicLibrary/data/enumHelper.py
+-rw-r--r--   0        0        0        0 2021-04-24 11:00:12.466000 basiclibrary_py-0.6.9/BasicLibrary/data/htmlHelper.py
+-rw-r--r--   0        0        0     6478 2024-03-14 02:16:19.043598 basiclibrary_py-0.6.9/BasicLibrary/data/listHelper.py
+-rw-r--r--   0        0        0     1340 2023-12-17 07:56:12.197269 basiclibrary_py-0.6.9/BasicLibrary/data/numberHelper.py
+-rw-r--r--   0        0        0     3474 2023-12-17 07:56:12.294709 basiclibrary_py-0.6.9/BasicLibrary/data/objectHelper.py
+-rw-r--r--   0        0        0     3227 2024-03-15 01:21:43.361361 basiclibrary_py-0.6.9/BasicLibrary/data/pandasHelper.py
+-rw-r--r--   0        0        0     1262 2024-01-01 00:18:18.746359 basiclibrary_py-0.6.9/BasicLibrary/data/randomHelper.py
+-rw-r--r--   0        0        0      811 2023-12-17 07:58:42.455096 basiclibrary_py-0.6.9/BasicLibrary/data/reflectHelper.py
+-rw-r--r--   0        0        0     1952 2023-12-17 07:58:42.306782 basiclibrary_py-0.6.9/BasicLibrary/data/regexHelper.py
+-rw-r--r--   0        0        0        2 2021-03-21 10:02:22.227000 basiclibrary_py-0.6.9/BasicLibrary/data/setHelper.py
+-rw-r--r--   0        0        0    11384 2024-03-19 02:13:01.276702 basiclibrary_py-0.6.9/BasicLibrary/data/stringHelper.py
+-rw-r--r--   0        0        0      317 2023-06-13 12:00:42.965651 basiclibrary_py-0.6.9/BasicLibrary/data/typeEnum.py
+-rw-r--r--   0        0        0      384 2024-03-11 08:21:52.844961 basiclibrary_py-0.6.9/BasicLibrary/data/typeHelper.py
+-rw-r--r--   0        0        0      117 2022-04-20 11:22:18.330540 basiclibrary_py-0.6.9/BasicLibrary/dataBase/.README.md
+-rw-r--r--   0        0        0      218 2022-04-20 11:22:18.274626 basiclibrary_py-0.6.9/BasicLibrary/dataBase/__init__.py
+-rw-r--r--   0        0        0     4855 2023-12-17 08:07:39.547566 basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseClient.py
+-rw-r--r--   0        0        0     2187 2022-04-20 11:23:22.877729 basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseDDL.py
+-rw-r--r--   0        0        0      345 2022-04-20 11:23:51.740994 basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseEnum.py
+-rw-r--r--   0        0        0     6920 2023-12-17 08:07:39.601794 basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseHelper.py
+-rw-r--r--   0        0        0     5468 2023-06-06 09:46:34.292073 basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseMate.py
+-rw-r--r--   0        0        0     1184 2023-12-17 08:07:39.389051 basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseUnitTest.py
+-rw-r--r--   0        0        0      164 2022-04-20 11:17:08.876036 basiclibrary_py-0.6.9/BasicLibrary/dataBase/MongoDB/__init__.py
+-rw-r--r--   0        0        0     1501 2023-06-06 09:46:34.424073 basiclibrary_py-0.6.9/BasicLibrary/dataBase/MongoDB/ddl.py
+-rw-r--r--   0        0        0     2829 2023-06-06 09:46:32.432228 basiclibrary_py-0.6.9/BasicLibrary/dataBase/MongoDB/helper.py
+-rw-r--r--   0        0        0    10551 2023-06-06 09:46:34.371074 basiclibrary_py-0.6.9/BasicLibrary/dataBase/MongoDB/mate.py
+-rw-r--r--   0        0        0      164 2022-04-20 11:18:12.573529 basiclibrary_py-0.6.9/BasicLibrary/dataBase/MySql/__init__.py
+-rw-r--r--   0        0        0     4642 2023-06-06 09:46:32.256228 basiclibrary_py-0.6.9/BasicLibrary/dataBase/MySql/ddl.py
+-rw-r--r--   0        0        0    12613 2023-06-06 09:46:33.878072 basiclibrary_py-0.6.9/BasicLibrary/dataBase/MySql/mate.py
+-rw-r--r--   0        0        0     3368 2023-06-06 09:46:33.288072 basiclibrary_py-0.6.9/BasicLibrary/dataBase/MySql/pool.py
+-rw-r--r--   0        0        0     1416 2023-10-29 10:17:06.615653 basiclibrary_py-0.6.9/BasicLibrary/enums.py
+-rw-r--r--   0        0        0      164 2022-04-20 11:24:39.998992 basiclibrary_py-0.6.9/BasicLibrary/environment/__init__.py
+-rw-r--r--   0        0        0     1792 2024-02-07 09:16:12.011979 basiclibrary_py-0.6.9/BasicLibrary/environment/consoleHelper.py
+-rw-r--r--   0        0        0     1840 2024-02-08 08:18:20.145848 basiclibrary_py-0.6.9/BasicLibrary/environment/dynamicImporter.py
+-rw-r--r--   0        0        0     1534 2024-03-07 23:59:26.745695 basiclibrary_py-0.6.9/BasicLibrary/environment/envHelper.py
+-rw-r--r--   0        0        0      871 2023-11-28 04:19:44.496618 basiclibrary_py-0.6.9/BasicLibrary/environment/inspectHelper.py
+-rw-r--r--   0        0        0      257 2022-04-20 11:25:32.285848 basiclibrary_py-0.6.9/BasicLibrary/io/.README.md
+-rw-r--r--   0        0        0      164 2022-04-20 11:24:39.959993 basiclibrary_py-0.6.9/BasicLibrary/io/__init__.py
+-rw-r--r--   0        0        0      513 2023-12-22 01:58:17.778023 basiclibrary_py-0.6.9/BasicLibrary/io/_util.py
+-rw-r--r--   0        0        0     6674 2024-03-19 02:32:44.881905 basiclibrary_py-0.6.9/BasicLibrary/io/dirHelper.py
+-rw-r--r--   0        0        0    14148 2024-03-14 02:12:35.144386 basiclibrary_py-0.6.9/BasicLibrary/io/fileHelper.py
+-rw-r--r--   0        0        0     2028 2024-01-23 02:40:36.256785 basiclibrary_py-0.6.9/BasicLibrary/io/fileShadowUsing.py
+-rw-r--r--   0        0        0     3003 2024-03-14 01:23:35.768121 basiclibrary_py-0.6.9/BasicLibrary/io/imageHelper.py
+-rw-r--r--   0        0        0      650 2024-01-11 02:48:40.389344 basiclibrary_py-0.6.9/BasicLibrary/io/ioEnums.py
+-rw-r--r--   0        0        0     1914 2024-01-23 02:40:36.131143 basiclibrary_py-0.6.9/BasicLibrary/io/ioHelper.py
+-rw-r--r--   0        0        0     3036 2024-03-14 01:59:35.020362 basiclibrary_py-0.6.9/BasicLibrary/io/pathHelper.py
+-rw-r--r--   0        0        0      186 2022-04-20 11:26:05.648500 basiclibrary_py-0.6.9/BasicLibrary/model/__init__.py
+-rw-r--r--   0        0        0     1365 2024-01-23 02:42:35.556378 basiclibrary_py-0.6.9/BasicLibrary/model/container.py
+-rw-r--r--   0        0        0     2246 2024-01-23 02:43:18.797533 basiclibrary_py-0.6.9/BasicLibrary/model/dataCompare.py
+-rw-r--r--   0        0        0     1099 2022-04-20 11:26:29.999355 basiclibrary_py-0.6.9/BasicLibrary/model/kvPair.py
+-rw-r--r--   0        0        0     1294 2024-01-23 02:08:08.731306 basiclibrary_py-0.6.9/BasicLibrary/model/returnResult.py
+-rw-r--r--   0        0        0      342 2022-04-20 11:26:30.136355 basiclibrary_py-0.6.9/BasicLibrary/model/stopWatcher.py
+-rw-r--r--   0        0        0      579 2022-04-20 11:26:59.149767 basiclibrary_py-0.6.9/BasicLibrary/office/.README.md
+-rw-r--r--   0        0        0      164 2022-04-20 11:26:38.013071 basiclibrary_py-0.6.9/BasicLibrary/office/__init__.py
+-rw-r--r--   0        0        0     6634 2023-06-06 09:46:31.715228 basiclibrary_py-0.6.9/BasicLibrary/office/excelBookMate.py
+-rw-r--r--   0        0        0     2560 2023-12-11 13:04:35.845636 basiclibrary_py-0.6.9/BasicLibrary/office/excelHelper.py
+-rw-r--r--   0        0        0     3375 2023-06-07 11:44:09.970141 basiclibrary_py-0.6.9/BasicLibrary/office/excelMisc.py
+-rw-r--r--   0        0        0      786 2023-06-16 03:30:23.970591 basiclibrary_py-0.6.9/BasicLibrary/office/excelShadowUsing.py
+-rw-r--r--   0        0        0    11261 2023-12-11 12:41:18.840106 basiclibrary_py-0.6.9/BasicLibrary/office/excelSheetMate.py
+-rw-r--r--   0        0        0      163 2022-04-20 11:27:42.609162 basiclibrary_py-0.6.9/BasicLibrary/pattern/__init__.py
+-rw-r--r--   0        0        0      560 2024-01-23 02:45:07.082985 basiclibrary_py-0.6.9/BasicLibrary/pattern/singleton.py
+-rw-r--r--   0        0        0      689 2024-03-19 03:44:40.152725 basiclibrary_py-0.6.9/BasicLibrary/projectHelper.py
+-rw-r--r--   0        0        0      164 2022-04-20 11:28:12.466235 basiclibrary_py-0.6.9/BasicLibrary/syntax/__init__.py
+-rw-r--r--   0        0        0     1664 2022-04-20 11:28:39.899931 basiclibrary_py-0.6.9/BasicLibrary/syntax/switch.py
+-rw-r--r--   0        0        0      164 2022-04-20 11:28:40.026934 basiclibrary_py-0.6.9/BasicLibrary/web/__init__.py
+-rw-r--r--   0        0        0     7972 2021-11-09 12:40:32.982432 basiclibrary_py-0.6.9/BasicLibrary/web/beautifulSoupHelper.py
+-rw-r--r--   0        0        0     1790 2022-04-20 11:28:54.662749 basiclibrary_py-0.6.9/BasicLibrary/web/requestHelper.py
+-rw-r--r--   0        0        0      478 2024-03-22 11:40:13.726590 basiclibrary_py-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     3469 2024-03-08 11:01:21.965314 basiclibrary_py-0.6.9/README.md
+-rw-r--r--   0        0        0     3959 1970-01-01 00:00:00.000000 basiclibrary_py-0.6.9/PKG-INFO
```

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/.README.md` & `basiclibrary_py-0.6.9/BasicLibrary/.README.md`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/__init__.py` & `basiclibrary_py-0.6.9/BasicLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/__projectConfig.ini` & `basiclibrary_py-0.6.9/BasicLibrary/__projectConfig.ini`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/__projectHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/__projectHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/biz/adobe/photoShopHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/biz/adobe/photoShopHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/biz/stock/stockHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/biz/stock/stockHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/configHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/configHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/base64Helper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/base64Helper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/chineseData.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/chineseData.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/collectionHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/collectionHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/dateTimeHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/dateTimeHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/dateTimePlaceHolderHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/dateTimePlaceHolderHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/dictHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/dictHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/listHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/listHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/numberHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/numberHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/objectHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/objectHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/pandasHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/pandasHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/randomHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/randomHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/reflectHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/reflectHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/regexHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/regexHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/data/stringHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/data/stringHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseClient.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseClient.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseDDL.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseDDL.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseMate.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseMate.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/databaseUnitTest.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/databaseUnitTest.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/MongoDB/ddl.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/MongoDB/ddl.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/MongoDB/helper.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/MongoDB/helper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/MongoDB/mate.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/MongoDB/mate.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/MySql/ddl.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/MySql/ddl.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/MySql/mate.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/MySql/mate.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/dataBase/MySql/pool.py` & `basiclibrary_py-0.6.9/BasicLibrary/dataBase/MySql/pool.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/enums.py` & `basiclibrary_py-0.6.9/BasicLibrary/enums.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/environment/consoleHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/environment/consoleHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/environment/dynamicImporter.py` & `basiclibrary_py-0.6.9/BasicLibrary/environment/dynamicImporter.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/environment/envHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/environment/envHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/environment/inspectHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/environment/inspectHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/io/_util.py` & `basiclibrary_py-0.6.9/BasicLibrary/io/_util.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/io/dirHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/io/dirHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/io/fileHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/io/fileHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/io/fileShadowUsing.py` & `basiclibrary_py-0.6.9/BasicLibrary/io/fileShadowUsing.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/io/imageHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/io/imageHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/io/ioEnums.py` & `basiclibrary_py-0.6.9/BasicLibrary/io/ioEnums.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/io/ioHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/io/ioHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/io/pathHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/io/pathHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/model/container.py` & `basiclibrary_py-0.6.9/BasicLibrary/model/container.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/model/dataCompare.py` & `basiclibrary_py-0.6.9/BasicLibrary/model/dataCompare.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/model/kvPair.py` & `basiclibrary_py-0.6.9/BasicLibrary/model/kvPair.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/model/returnResult.py` & `basiclibrary_py-0.6.9/BasicLibrary/model/returnResult.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/office/.README.md` & `basiclibrary_py-0.6.9/BasicLibrary/office/.README.md`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/office/excelBookMate.py` & `basiclibrary_py-0.6.9/BasicLibrary/office/excelBookMate.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/office/excelHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/office/excelHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/office/excelMisc.py` & `basiclibrary_py-0.6.9/BasicLibrary/office/excelMisc.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/office/excelShadowUsing.py` & `basiclibrary_py-0.6.9/BasicLibrary/office/excelShadowUsing.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/office/excelSheetMate.py` & `basiclibrary_py-0.6.9/BasicLibrary/office/excelSheetMate.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/pattern/singleton.py` & `basiclibrary_py-0.6.9/BasicLibrary/pattern/singleton.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/projectHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/projectHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/syntax/switch.py` & `basiclibrary_py-0.6.9/BasicLibrary/syntax/switch.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/web/beautifulSoupHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/web/beautifulSoupHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/BasicLibrary/web/requestHelper.py` & `basiclibrary_py-0.6.9/BasicLibrary/web/requestHelper.py`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/README.md` & `basiclibrary_py-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `basiclibrary_py-0.6.8/PKG-INFO` & `basiclibrary_py-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.6.8
+Version: 0.6.9
 Summary: 
 Author: 解大劦
 Author-email: 9727005@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
-Requires-Dist: dotenv (>=0.0.5,<0.0.6)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: sxtwl (>=2.0.6,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 企业级的Python类库
 
 ```
 @emailto: 9727005@qq.com
```

