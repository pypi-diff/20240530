# Comparing `tmp/opengamedata_core-0.0.4.tar.gz` & `tmp/opengamedata_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata_core-0.0.4.tar", last modified: Wed May 15 23:03:09 2024, max compression
+gzip compressed data, was "opengamedata_core-0.0.5.tar", last modified: Fri May 17 03:40:41 2024, max compression
```

## Comparing `opengamedata_core-0.0.4.tar` & `opengamedata_core-0.0.5.tar`

### file list

```diff
@@ -1,547 +1,546 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.345651 opengamedata_core-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-15 23:03:09.345651 opengamedata_core-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 23:03:09.345651 opengamedata_core-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.257650 opengamedata_core-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.257650 opengamedata_core-0.0.4/src/ogd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.257650 opengamedata_core-0.0.4/src/ogd/core/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.257650 opengamedata_core-0.0.4/src/ogd/core/exec/
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/exec/Commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/exec/Generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/exec/Parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.245650 opengamedata_core-0.0.4/src/ogd/core/games/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.245650 opengamedata_core-0.0.4/src/ogd/core/games/AQUALAB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.257650 opengamedata_core-0.0.4/src/ogd/core/games/AQUALAB/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/games/AQUALAB/features/AppVersions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/games/AQUALAB/features/PlayLocations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.245650 opengamedata_core-0.0.4/src/ogd/core/games/JOURNALISM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.257650 opengamedata_core-0.0.4/src/ogd/core/games/JOURNALISM/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/games/JOURNALISM/features/FailureAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/games/JOURNALISM/features/FinalAttributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.257650 opengamedata_core-0.0.4/src/ogd/core/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/Generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/GeneratorLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.261650 opengamedata_core-0.0.4/src/ogd/core/generators/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/detectors/Detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/detectors/DetectorEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.261650 opengamedata_core-0.0.4/src/ogd/core/generators/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/extractors/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/extractors/Feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/extractors/PerCountFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/extractors/PerLevelFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/extractors/SessionFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.261650 opengamedata_core-0.0.4/src/ogd/core/generators/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/legacy/LegacyDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/legacy/LegacyFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/legacy/LegacyLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.261650 opengamedata_core-0.0.4/src/ogd/core/generators/registries/
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/registries/DetectorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/registries/ExtractorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/registries/GeneratorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/generators/registries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.265650 opengamedata_core-0.0.4/src/ogd/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/BQFirebaseInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/BigQueryCodingInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/BigQueryInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/CSVInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/CodingInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/DataInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/Interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/MySQLInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.265650 opengamedata_core-0.0.4/src/ogd/core/interfaces/outerfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/outerfaces/DataOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/outerfaces/DebugOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    33757 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/interfaces/outerfaces/TSVOuterface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.265650 opengamedata_core-0.0.4/src/ogd/core/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/managers/EventManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/managers/ExportManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/managers/FeatureManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/managers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.269650 opengamedata_core-0.0.4/src/ogd/core/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/processors/ClassroomDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/processors/DetectorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/processors/EventProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/processors/ExtractorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/processors/GeneratorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/processors/PlayerProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/processors/PopulationProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/processors/Processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/processors/SessionProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.269650 opengamedata_core-0.0.4/src/ogd/core/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/requests/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/requests/RequestResult.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.269650 opengamedata_core-0.0.4/src/ogd/core/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/ExportMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/ExtractionMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/FeatureData.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/IDMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/IterationMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/Schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.269650 opengamedata_core-0.0.4/src/ogd/core/schemas/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/configs/ConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/configs/GameSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/configs/IndexingSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/configs/LegacyConfigSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.273650 opengamedata_core-0.0.4/src/ogd/core/schemas/configs/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.273650 opengamedata_core-0.0.4/src/ogd/core/schemas/games/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/AggregateSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/DataElementSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/DetectorMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/DetectorSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/EventSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/ExtractorSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/FeatureMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/FeatureSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    26726 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/GameSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/GameStateSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/PerCountSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.277650 opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/BIGQUERY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/FIREBASE.json
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.277650 opengamedata_core-0.0.4/src/ogd/core/schemas/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/tables/ColumnMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/tables/ColumnSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    23084 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/schemas/tables/TableSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.277650 opengamedata_core-0.0.4/src/ogd/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/utils/Readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/utils/SemanticVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/core/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.277650 opengamedata_core-0.0.4/src/ogd/games/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.245650 opengamedata_core-0.0.4/src/ogd/games/ALL_YOU_CAN_ET/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.277650 opengamedata_core-0.0.4/src/ogd/games/ALL_YOU_CAN_ET/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.277650 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/
--rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/AqualabLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)   278275 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.281650 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/HintAndLeave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/Idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/TwoHints.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/ActiveJobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/ActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/AppVersions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/AverageSessionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/EchoSessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/EventList.py
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobArgumentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobCompletionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobExperimentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobLocationChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobModeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobPriorAttempt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobPriorComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobStartCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobTasksCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobTriesInArgument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobsAttempted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/ModelExportCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/ModelInterveneCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/ModelPredictCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/PerJobFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/PlayLocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/PlayerSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/PopulationSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/RegionJobCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/RegionName.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SwitchJobsCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SyncCompletionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TankRulesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalArcticTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalBayouTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalCoralTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalKelpTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalModelingTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    32600 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/BACTERIA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/BACTERIA/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/BALLOON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/BALLOON/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/BALLOON/schemas/BALLOON.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/BLOOM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/BLOOM/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/BLOOM/schemas/BLOOM.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/CENSIO_SLIDE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/CENSIO_SLIDE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/CENSIO_STACK/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/CENSIO_STACK/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/CRUSH_STATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/CRUSH_STATION/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/CRYSTAL/
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/CRYSTAL/CrystalLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/CRYSTAL/features/
--rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/CRYSTAL/features/CrystalExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/CRYSTAL/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/CRYSTAL/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/CYCLE_CARBON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/CYCLE_CARBON/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/CYCLE_NITROGEN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/CYCLE_NITROGEN/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/CYCLE_WATER/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/CYCLE_WATER/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/CYCLE_WATER/schemas/CYCLE_WATER.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/EARTHQUAKE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/EARTHQUAKE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/EARTHQUAKE/schemas/EARTHQUAKE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.249650 opengamedata_core-0.0.4/src/ogd/games/GWAKKAMOLE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.293650 opengamedata_core-0.0.4/src/ogd/games/GWAKKAMOLE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.297650 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/DBExport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/IcecubeLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.297650 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/HeadsetOnCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/PerSceneFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/SceneDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/SceneFailureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/SceneFailures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/ScenesEncountered.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/Session_Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.297650 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.297650 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/JournalismLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.305651 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/AttributeView.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/FailureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/GameComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/LevelCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/LevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/PlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/PlayerAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/QuitLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/QuitNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/QuitType.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SessionPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SnippetReplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SnippetsCollected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryAlignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryEditorTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryScore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TextClickCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TopAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TotalFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TotalLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/UserPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/WorstAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.305651 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    45415 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.305651 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/JowilderLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/Jowilder_Enumerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.309651 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/ActiveStateTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/Clicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/EventCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/FirstInteraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/GameScript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/GameVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/Hovers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/IdleState.py
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/Interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/InteractionName.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/LastInteraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/MeaningfulActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/NotebookUses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/QuestionAnswers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/SessionStart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/SurveyItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/SurveyTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/UsedContinue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/UsedSaveCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/UserEnabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/get_jowilder_all_items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.309651 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    35912 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.313650 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/LakelandLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.317651 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/DeathCountModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/DeathPredModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/DeathThresholdModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/FeatSeqPercent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/FeatVelocity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/FeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/LAKELAND_models.json
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/LakelandEnumerators.json
--rw-r--r--   0 runner    (1001) docker     (127)    69732 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/LakelandExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/LinearModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/LogisticModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/MapSummaryModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/NthEventModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/PlayingTimeModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/PopulationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/SequenceModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/SingleFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/TownCompositionFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/TownCompositionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/WAVES_models.json
--rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json
--rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json
--rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json
--rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.317651 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   115553 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.317651 opengamedata_core-0.0.4/src/ogd/games/MAGNET/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/MAGNET/MagnetLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.321651 opengamedata_core-0.0.4/src/ogd/games/MAGNET/features/
--rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/MAGNET/features/MagnetExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/MAGNET/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.321651 opengamedata_core-0.0.4/src/ogd/games/MAGNET/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/MAGNET/schemas/MAGNET.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.253650 opengamedata_core-0.0.4/src/ogd/games/MASHOPOLIS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.321651 opengamedata_core-0.0.4/src/ogd/games/MASHOPOLIS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.321651 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/PenguinsLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.321651 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/detectors/RegionEnter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/detectors/RegionExit.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.325651 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/ActivityCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/ActivityDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/EatFishCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/EggLostCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/EggRecoverTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/GazeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/GazeDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/PerRegionFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/PickupRockCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/RegionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/RegionEnterCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/RegionsEncountered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/RingChimesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/SnowBallDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/WaddlePerRegion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.325651 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    28356 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.325651 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.325651 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.325651 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.325651 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.329651 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/EventList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.329651 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.329651 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/ThermoVRLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.329651 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.333651 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/LabCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/LeftHandMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/PhasesReached.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/PlayMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/RightHandMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/TaskCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/ToolNudgeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/ToolSliderTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.333651 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    51378 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.333651 opengamedata_core-0.0.4/src/ogd/games/TRANSFORMATION_QUEST/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.333651 opengamedata_core-0.0.4/src/ogd/games/TRANSFORMATION_QUEST/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    25177 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.333651 opengamedata_core-0.0.4/src/ogd/games/WAVES/
--rw-r--r--   0 runner    (1001) docker     (127)    37332 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/WaveLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.341651 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/AverageFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/AverageLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/AverageSliderMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/BeginCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/ClosenessIntercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/ClosenessR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/ClosenessSlope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/Completed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/FirstMoveType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/MenuButtonCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OverallSliderAverageRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentOffsetMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentWavelengthMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PersistentSessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/QuestionAnswered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/QuestionCorrect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/RangeIntercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/RangeR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/RangeSlope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/SequenceLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/SliderAverageRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/SucceedCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TimeToAnswerMS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalArrowMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalResets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalSkips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalSliderMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.341651 opengamedata_core-0.0.4/src/ogd/games/WAVES/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WAVES/schemas/WAVES.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.257650 opengamedata_core-0.0.4/src/ogd/games/WEATHER_STATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.341651 opengamedata_core-0.0.4/src/ogd/games/WEATHER_STATION/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    34344 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.257650 opengamedata_core-0.0.4/src/ogd/games/WIND/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.341651 opengamedata_core-0.0.4/src/ogd/games/WIND/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/WIND/schemas/WIND.json.template
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:02:24.000000 opengamedata_core-0.0.4/src/ogd/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.345651 opengamedata_core-0.0.4/src/opengamedata_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-15 23:03:09.000000 opengamedata_core-0.0.4/src/opengamedata_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21737 2024-05-15 23:03:09.000000 opengamedata_core-0.0.4/src/opengamedata_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:03:09.000000 opengamedata_core-0.0.4/src/opengamedata_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 23:03:09.000000 opengamedata_core-0.0.4/src/opengamedata_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:09.345651 opengamedata_core-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-15 23:02:25.000000 opengamedata_core-0.0.4/tests/test_lakeland_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.268148 opengamedata_core-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/exec/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/exec/Generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/exec/Parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.260148 opengamedata_core-0.0.5/src/ogd/core/games/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.260148 opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/features/AppVersions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/features/PlayLocations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.260148 opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/features/FailureAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/features/FinalAttributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/Generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/GeneratorLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/generators/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/detectors/Detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/detectors/DetectorEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.276148 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/Extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/Feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/PerCountFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/PerLevelFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/SessionFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.276148 opengamedata_core-0.0.5/src/ogd/core/generators/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.276148 opengamedata_core-0.0.5/src/ogd/core/generators/registries/
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/registries/DetectorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/registries/ExtractorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/registries/GeneratorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/registries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.280148 opengamedata_core-0.0.5/src/ogd/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/BQFirebaseInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/BigQueryCodingInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/BigQueryInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/CSVInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/CodingInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/DataInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/Interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/MySQLInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.280148 opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DataOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DebugOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33757 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/TSVOuterface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.280148 opengamedata_core-0.0.5/src/ogd/core/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/managers/EventManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/managers/ExportManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/managers/FeatureManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/managers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.284148 opengamedata_core-0.0.5/src/ogd/core/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/ClassroomDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/DetectorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/EventProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/ExtractorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/GeneratorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/PlayerProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/PopulationProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/Processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/SessionProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.284148 opengamedata_core-0.0.5/src/ogd/core/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/requests/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/requests/RequestResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.284148 opengamedata_core-0.0.5/src/ogd/core/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/ExportMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/ExtractionMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/FeatureData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/IDMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/IterationMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/Schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.284148 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/ConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/GameSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/IndexingSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/LegacyConfigSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.284148 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.288148 opengamedata_core-0.0.5/src/ogd/core/schemas/games/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/AggregateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/DataElementSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/DetectorMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/DetectorSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/EventSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/ExtractorSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/FeatureMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/FeatureSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26726 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/GameSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/GameStateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/PerCountSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.288148 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/BIGQUERY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/FIREBASE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.292148 opengamedata_core-0.0.5/src/ogd/core/schemas/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/tables/ColumnMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/tables/ColumnSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23084 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/tables/TableSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.292148 opengamedata_core-0.0.5/src/ogd/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/Readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/SemanticVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.292148 opengamedata_core-0.0.5/src/ogd/games/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.260148 opengamedata_core-0.0.5/src/ogd/games/ALL_YOU_CAN_ET/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.292148 opengamedata_core-0.0.5/src/ogd/games/ALL_YOU_CAN_ET/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.292148 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/AqualabLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278275 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.296148 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/HintAndLeave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/Idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/TwoHints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ActiveJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/AppVersions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/AverageSessionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/EchoSessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobArgumentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobCompletionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobExperimentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobLocationChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobModeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPriorAttempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPriorComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobStartCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobTasksCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobTriesInArgument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobsAttempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelExportCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelInterveneCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelPredictCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PerJobFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PlayerSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PopulationSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/RegionJobCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/RegionName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SwitchJobsCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SyncCompletionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TankRulesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalArcticTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalBayouTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalCoralTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalKelpTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalModelingTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    32117 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.260148 opengamedata_core-0.0.5/src/ogd/games/BACTERIA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/BACTERIA/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/BALLOON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/BALLOON/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/BALLOON/schemas/BALLOON.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/BLOOM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/BLOOM/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/BLOOM/schemas/BLOOM.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CENSIO_SLIDE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CENSIO_SLIDE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CENSIO_STACK/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CENSIO_STACK/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CRUSH_STATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CRUSH_STATION/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/CrystalLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/features/
+-rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/features/CrystalExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_CARBON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_CARBON/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_NITROGEN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_NITROGEN/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_WATER/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_WATER/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CYCLE_WATER/schemas/CYCLE_WATER.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/EARTHQUAKE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/EARTHQUAKE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/EARTHQUAKE/schemas/EARTHQUAKE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/GWAKKAMOLE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/GWAKKAMOLE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.312148 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/DBExport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/IcecubeLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.312148 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/HeadsetOnCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/PerSceneFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneFailureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneFailures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ScenesEncountered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/Session_Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.312148 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.312148 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/JournalismLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.320148 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/AttributeView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/FailureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/GameComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/PlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/PlayerAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SessionPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetReplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetsCollected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryEditorTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryScore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TextClickCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TotalFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TotalLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/UserPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/WorstAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.320148 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    45415 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.324148 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/JowilderLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/Jowilder_Enumerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.328148 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/ActiveStateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Clicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/EventCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/FirstInteraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/GameScript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/GameVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Hovers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/IdleState.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/LastInteraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/MeaningfulActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/NotebookUses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/QuestionAnswers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SessionStart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SurveyItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SurveyTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UsedContinue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UsedSaveCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UserEnabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/get_jowilder_all_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.328148 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    35912 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.328148 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/LakelandLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathCountModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathPredModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathThresholdModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatSeqPercent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatVelocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LAKELAND_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LakelandEnumerators.json
+-rw-r--r--   0 runner    (1001) docker     (127)    69732 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LakelandExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LinearModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LogisticModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/MapSummaryModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/NthEventModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/PlayingTimeModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/PopulationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SequenceModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SingleFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TownCompositionFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TownCompositionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   115553 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/MAGNET/
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/MAGNET/MagnetLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/MAGNET/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/MAGNET/features/MagnetExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/MAGNET/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/MAGNET/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/MAGNET/schemas/MAGNET.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.268148 opengamedata_core-0.0.5/src/ogd/games/MASHOPOLIS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/MASHOPOLIS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/PenguinsLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/detectors/RegionEnter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/detectors/RegionExit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.340147 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/ActivityCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/ActivityDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EatFishCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EggLostCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EggRecoverTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/GazeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/GazeDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PerRegionFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PickupRockCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionEnterCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionsEncountered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RingChimesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/SnowBallDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/WaddlePerRegion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.340147 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    28356 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.340147 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.344147 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.344147 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.344147 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/ThermoVRLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/LabCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/LeftHandMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/PhasesReached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/PlayMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/RightHandMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/TaskCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/ToolNudgeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/ToolSliderTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    51378 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    25177 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/WAVES/
+-rw-r--r--   0 runner    (1001) docker     (127)    37332 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/WaveLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageSliderMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/BeginCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessIntercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessSlope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/Completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/FirstMoveType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/MenuButtonCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallSliderAverageRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentOffsetMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentWavelengthMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PersistentSessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/QuestionAnswered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/QuestionCorrect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeIntercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeSlope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SequenceLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SliderAverageRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SucceedCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TimeToAnswerMS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalArrowMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalResets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalSkips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalSliderMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/src/ogd/games/WAVES/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/schemas/WAVES.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.268148 opengamedata_core-0.0.5/src/ogd/games/WEATHER_STATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/src/ogd/games/WEATHER_STATION/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    34344 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.268148 opengamedata_core-0.0.5/src/ogd/games/WIND/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/src/ogd/games/WIND/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WIND/schemas/WIND.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/src/opengamedata_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-17 03:40:41.000000 opengamedata_core-0.0.5/src/opengamedata_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21689 2024-05-17 03:40:41.000000 opengamedata_core-0.0.5/src/opengamedata_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:40:41.000000 opengamedata_core-0.0.5/src/opengamedata_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 03:40:41.000000 opengamedata_core-0.0.5/src/opengamedata_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-17 03:39:53.000000 opengamedata_core-0.0.5/tests/test_lakeland_models.py
```

### Comparing `opengamedata_core-0.0.4/LICENSE` & `opengamedata_core-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/PKG-INFO` & `opengamedata_core-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for retrieving and processing event-based video game data. Additional authors: Nick Spevacek, Renee Li, John McCloskey, Zach Studdiford, Glenn Palmer, Haishuo Chen, Daus, Ameya Kshirsagar, Yunqing Xiao, Erik Harpstead, Manuel Jesus Gomez Moratilla
 Author-email: Luke Swanson <superscription58@gmail.com>, David Gagnon <djgagnon@wisc.edu>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-core
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-core/issues
 Project-URL: Documentation, https://opengamedata-doc.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_core-0.0.4/README.md` & `opengamedata_core-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/pyproject.toml` & `opengamedata_core-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/exec/Commands.py` & `opengamedata_core-0.0.5/src/ogd/core/exec/Commands.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/exec/Generators.py` & `opengamedata_core-0.0.5/src/ogd/core/exec/Generators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/exec/Parsers.py` & `opengamedata_core-0.0.5/src/ogd/core/exec/Parsers.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/games/AQUALAB/features/AppVersions.py` & `opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/features/AppVersions.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/games/AQUALAB/features/PlayLocations.py` & `opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/features/PlayLocations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/games/JOURNALISM/features/FailureAttributes.py` & `opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/features/FailureAttributes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/games/JOURNALISM/features/FinalAttributes.py` & `opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/features/FinalAttributes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/Generator.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/Generator.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/GeneratorLoader.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/GeneratorLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/detectors/Detector.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/detectors/Detector.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/detectors/DetectorEvent.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/detectors/DetectorEvent.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/extractors/Extractor.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/extractors/Extractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/extractors/Feature.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/extractors/Feature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/extractors/PerCountFeature.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/extractors/PerCountFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/extractors/PerLevelFeature.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/extractors/PerLevelFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/extractors/SessionFeature.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/extractors/SessionFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/legacy/LegacyDetector.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyDetector.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/legacy/LegacyFeature.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/legacy/LegacyLoader.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/registries/DetectorRegistry.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/registries/DetectorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/registries/ExtractorRegistry.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/registries/ExtractorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/generators/registries/GeneratorRegistry.py` & `opengamedata_core-0.0.5/src/ogd/core/generators/registries/GeneratorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/BQFirebaseInterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/BQFirebaseInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/BigQueryCodingInterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/BigQueryCodingInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/BigQueryInterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/BigQueryInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/CSVInterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/CSVInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/CodingInterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/CodingInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/DataInterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/DataInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/Interface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/MySQLInterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/MySQLInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/outerfaces/DataOuterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DataOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/outerfaces/DebugOuterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DebugOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/interfaces/outerfaces/TSVOuterface.py` & `opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/TSVOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/managers/EventManager.py` & `opengamedata_core-0.0.5/src/ogd/core/managers/EventManager.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/managers/ExportManager.py` & `opengamedata_core-0.0.5/src/ogd/core/managers/ExportManager.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/managers/FeatureManager.py` & `opengamedata_core-0.0.5/src/ogd/core/managers/FeatureManager.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/processors/ClassroomDetector.py` & `opengamedata_core-0.0.5/src/ogd/core/processors/ClassroomDetector.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/processors/DetectorProcessor.py` & `opengamedata_core-0.0.5/src/ogd/core/processors/DetectorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/processors/EventProcessor.py` & `opengamedata_core-0.0.5/src/ogd/core/processors/EventProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/processors/ExtractorProcessor.py` & `opengamedata_core-0.0.5/src/ogd/core/processors/ExtractorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/processors/GeneratorProcessor.py` & `opengamedata_core-0.0.5/src/ogd/core/processors/GeneratorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/processors/PlayerProcessor.py` & `opengamedata_core-0.0.5/src/ogd/core/processors/PlayerProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/processors/PopulationProcessor.py` & `opengamedata_core-0.0.5/src/ogd/core/processors/PopulationProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/processors/Processor.py` & `opengamedata_core-0.0.5/src/ogd/core/processors/Processor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/processors/SessionProcessor.py` & `opengamedata_core-0.0.5/src/ogd/core/processors/SessionProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/requests/Request.py` & `opengamedata_core-0.0.5/src/ogd/core/requests/Request.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/requests/RequestResult.py` & `opengamedata_core-0.0.5/src/ogd/core/requests/RequestResult.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/Event.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/Event.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/FeatureData.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/FeatureData.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/Schema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/Schema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/configs/ConfigSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/ConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/configs/GameSourceSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/GameSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/configs/IndexingSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/IndexingSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/configs/LegacyConfigSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/LegacyConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/AggregateSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/AggregateSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/DataElementSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/DataElementSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/DetectorMapSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/DetectorMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/DetectorSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/DetectorSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/EventSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/EventSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/ExtractorSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/ExtractorSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/FeatureMapSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/FeatureMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/FeatureSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/FeatureSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/GameSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/GameSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/GameStateSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/GameStateSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/games/PerCountSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/games/PerCountSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/BIGQUERY.json` & `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/BIGQUERY.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json` & `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/FIREBASE.json` & `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/FIREBASE.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json` & `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json` & `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json` & `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json` & `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json` & `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/tables/ColumnMapSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/tables/ColumnMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/tables/ColumnSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/tables/ColumnSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/schemas/tables/TableSchema.py` & `opengamedata_core-0.0.5/src/ogd/core/schemas/tables/TableSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/utils/Logger.py` & `opengamedata_core-0.0.5/src/ogd/core/utils/Logger.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/utils/Readme.py` & `opengamedata_core-0.0.5/src/ogd/core/utils/Readme.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/core/utils/SemanticVersion.py` & `opengamedata_core-0.0.5/src/ogd/core/utils/SemanticVersion.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,16 @@
             return True
         return False
 
 
     @staticmethod
     def FromString(semver:str, verbose:bool=True) -> 'SemanticVersion':
         pieces = re.split('\.|-', semver)
-        Logger.Log(f"Pieces: {pieces}", logging.DEBUG)
+        if verbose:
+            Logger.Log(f"Pieces: {pieces}", logging.DEBUG)
 
         return SemanticVersion._parseMajor(semver=semver, pieces=pieces, verbose=verbose)
 
     @staticmethod
     def _parseMajor(semver:str, pieces:List[str], verbose:bool) -> 'SemanticVersion':
         ret_val : 'SemanticVersion'
```

### Comparing `opengamedata_core-0.0.4/src/ogd/core/utils/utils.py` & `opengamedata_core-0.0.5/src/ogd/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template` & `opengamedata_core-0.0.5/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/AqualabLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/AqualabLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/DBExport.json` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/HintAndLeave.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/HintAndLeave.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/Idle.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/Idle.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/detectors/TwoHints.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/TwoHints.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/ActiveJobs.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ActiveJobs.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/ActiveTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ActiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/AppVersions.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/AppVersions.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/AverageSessionTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/AverageSessionTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/EchoSessionID.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/EchoSessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/EventList.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/EventList.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobActiveTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobActiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobArgumentation.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobArgumentation.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobCompletionTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobCompletionTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobDiveTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobExperimentation.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobExperimentation.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobGuideCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobGuideCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobHelpCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobHelpCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobLocationChanges.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobLocationChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobModeling.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobModeling.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobPlayTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobPriorAttempt.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPriorAttempt.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobPriorComplete.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPriorComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobStartCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobStartCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobTasksCompleted.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobTasksCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobTriesInArgument.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobTriesInArgument.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobsAttempted.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobsAttempted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/JobsCompleted.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/ModelExportCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelExportCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/ModelInterveneCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelInterveneCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/ModelPredictCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelPredictCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/PerJobFeature.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PerJobFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/PlayerSummary.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PlayerSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/PopulationSummary.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PopulationSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/RegionJobCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/RegionJobCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/RegionName.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/RegionName.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionGuideCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionGuideCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionHelpCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionHelpCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionID.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SwitchJobsCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SwitchJobsCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/SyncCompletionTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SyncCompletionTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TankRulesCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TankRulesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalArcticTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalArcticTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalBayouTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalBayouTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalCoralTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalCoralTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalDiveTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalGuideCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalGuideCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalHelpCount.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalHelpCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalKelpTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalKelpTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalModelingTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalModelingTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/TotalPlayTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/features/__init__.py` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     "JobStartCount",
     "JobTasksCompleted",
     "JobTriesInArgument",
     "ModelExportCount",
     "ModelInterveneCount",
     "ModelPredictCount",
     "PlayerSummary",
-    "PlayLocations",
     "PopulationSummary",
     "RegionJobCount",
     "RegionName",
     "SessionDiveSitesCount",
     "SessionDuration",
     "SessionGuideCount",
     "SessionHelpCount",
@@ -52,15 +51,14 @@
     "TotalHelpCount",
     "TotalKelpTime",
     "TotalModelingTime",
     "TotalPlayTime",
     "UserAvgActiveTime",
     "UserAvgSessionDuration",
     "UserTotalSessionDuration",
-    "PlayLocations",
     "AppVersions"
 ]
 
 from . import ActiveJobs
 from . import ActiveTime
 from . import AppVersions
 from . import AverageSessionTime
@@ -84,15 +82,14 @@
 from . import JobStartCount
 from . import JobTasksCompleted
 from . import JobTriesInArgument
 from . import ModelExportCount
 from . import ModelInterveneCount
 from . import ModelPredictCount
 from . import PlayerSummary
-from . import PlayLocations
 from . import PopulationSummary
 from . import RegionJobCount
 from . import RegionName
 from . import SessionDiveSitesCount
 from . import SessionDuration
 from . import SessionGuideCount
 from . import SessionHelpCount
@@ -113,9 +110,8 @@
 from . import TotalHelpCount
 from . import TotalKelpTime
 from . import TotalModelingTime
 from . import TotalPlayTime
 from . import UserAvgActiveTime
 from . import UserAvgSessionDuration
 from . import UserTotalSessionDuration
-from . import PlayLocations
 from . import AppVersions
```

### Comparing `opengamedata_core-0.0.4/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template` & `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -778,32 +778,32 @@
             },
             "JobsCompleted": {
                 "enabled": true,
                 "type": "JobsCompleted",
                 "description": "List of completed jobs for a player",
                 "return_type": "list[str]"
             },
+            "PlayerSummary": {
+                "enabled": false,
+                "type": "PlayerSummary",
+                "description": "Summary of player statistics (active session time, jobs completed, number of sessions)",
+                "return_type": "dict"
+            },
             "PlayLocations": {
                 "enabled": false,
                 "type": "PlayLocations",
                 "description": "An indicator of whether play happened during normal school hours or not",
                 "return_type": "List[bool]",
                 "subfeatures": {
                     "LocalTime": {
                         "description": "The actual local time when each session started",
                         "return_type": "datetime"
                     }
                 }
             },
-            "PlayerSummary": {
-                "enabled": false,
-                "type": "PlayerSummary",
-                "description": "Summary of player statistics (active session time, jobs completed, number of sessions)",
-                "return_type": "dict"
-            },
             "PopulationSummary": {
                 "enabled": false,
                 "type": "PopulationSummary",
                 "description": "Summary of population statistics (active session time, average jobs completed count, average session count)",
                 "return_type": "dict"
             },
             "SessionDiveSitesCount": {
```

### Comparing `opengamedata_core-0.0.4/src/ogd/games/BLOOM/schemas/BLOOM.json.template` & `opengamedata_core-0.0.5/src/ogd/games/BLOOM/schemas/BLOOM.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template` & `opengamedata_core-0.0.5/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template` & `opengamedata_core-0.0.5/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template` & `opengamedata_core-0.0.5/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/CRYSTAL/CrystalLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/CrystalLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/CRYSTAL/features/CrystalExtractor.py` & `opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/features/CrystalExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template` & `opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template` & `opengamedata_core-0.0.5/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/DBExport.json` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/DBExport.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/DBExport.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/IcecubeLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/IcecubeLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/HeadsetOnCount.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/HeadsetOnCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/PerSceneFeature.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/PerSceneFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/SceneDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/SceneFailureCount.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneFailureCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/SceneFailures.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneFailures.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/ScenesEncountered.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ScenesEncountered.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/SessionDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/Session_Language.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/Session_Language.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/features/__init__.py` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template` & `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/JournalismLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/JournalismLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/AttributeView.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/AttributeView.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/FailureCount.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/FailureCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/GameComplete.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/GameComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/LevelCompleted.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/LevelTime.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/PlayTime.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/PlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/PlayerAttributes.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/PlayerAttributes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/QuitLevel.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/QuitNode.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitNode.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/QuitType.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitType.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SessionPlayTime.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SessionPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SnippetReplace.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetReplace.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SnippetsCollected.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetsCollected.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryAlignment.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryAlignment.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryEditorTime.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryEditorTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryScore.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryScore.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TextClickCount.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TextClickCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TopAttribute.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TotalFails.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TotalFails.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/TotalLevelTime.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TotalLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/UserPlayTime.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/UserPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/WorstAttribute.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/WorstAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/features/__init__.py` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template` & `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/JowilderLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/JowilderLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/Jowilder_Enumerators.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/Jowilder_Enumerators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/ActiveStateTime.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/ActiveStateTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/Clicks.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Clicks.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/EventCount.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/EventCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/FirstInteraction.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/FirstInteraction.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/GameScript.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/GameScript.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/GameVersion.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/GameVersion.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/Hovers.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Hovers.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/IdleState.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/IdleState.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/Interaction.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Interaction.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/InteractionName.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionName.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/LastInteraction.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/LastInteraction.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/MeaningfulActions.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/MeaningfulActions.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/NotebookUses.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/NotebookUses.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/QuestionAnswers.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/QuestionAnswers.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/SessionDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/SessionStart.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SessionStart.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/SurveyItem.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SurveyItem.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/SurveyTime.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SurveyTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/UsedContinue.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UsedContinue.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/UsedSaveCode.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UsedSaveCode.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/UserEnabled.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UserEnabled.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/features/__init__.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/get_jowilder_all_items.py` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/get_jowilder_all_items.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template` & `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/LakelandLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/LakelandLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/DeathCountModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathCountModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/DeathPredModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathPredModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/DeathThresholdModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathThresholdModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/FeatSeqPercent.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatSeqPercent.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/FeatVelocity.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatVelocity.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/FeatureModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatureModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/LAKELAND_models.json` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LAKELAND_models.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/LakelandEnumerators.json` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LakelandEnumerators.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/LakelandExtractor.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LakelandExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/LinearModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LinearModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/LogisticModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LogisticModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/MapSummaryModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/MapSummaryModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/Model.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/Model.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/PopulationModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/PopulationModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/SequenceModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SequenceModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/SingleFeatureModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SingleFeatureModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/TownCompositionModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TownCompositionModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/WAVES_models.json` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template` & `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/MAGNET/MagnetLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/MAGNET/MagnetLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/MAGNET/features/MagnetExtractor.py` & `opengamedata_core-0.0.5/src/ogd/games/MAGNET/features/MagnetExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/MAGNET/schemas/MAGNET.json.template` & `opengamedata_core-0.0.5/src/ogd/games/MAGNET/schemas/MAGNET.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template` & `opengamedata_core-0.0.5/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/DBExport.json` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/PenguinsLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/PenguinsLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/detectors/RegionEnter.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/detectors/RegionEnter.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/detectors/RegionExit.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/detectors/RegionExit.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/ActivityCompleted.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/ActivityCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/ActivityDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/ActivityDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/EatFishCount.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EatFishCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/EggLostCount.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EggLostCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/EggRecoverTime.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EggRecoverTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/GazeCount.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/GazeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/GazeDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/GazeDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/PerRegionFeature.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PerRegionFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/PickupRockCount.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PickupRockCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/RegionDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/RegionEnterCount.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionEnterCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/RegionsEncountered.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionsEncountered.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/RingChimesCount.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RingChimesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/SessionDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/SnowBallDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/SnowBallDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/WaddlePerRegion.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/WaddlePerRegion.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/features/__init__.py` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template` & `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py` & `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py` & `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py` & `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py` & `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/features/SessionID.py` & `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template` & `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/EventList.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/EventList.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/SessionDuration.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/SessionID.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/features/__init__.py` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template` & `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/THERMOVR/ThermoVRLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/ThermoVRLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/LeftHandMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/LeftHandMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/PhasesReached.py` & `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/PhasesReached.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/PlayMode.py` & `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/PlayMode.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/RightHandMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/RightHandMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/TaskCompleteCount.py` & `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/TaskCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/ToolNudgeCount.py` & `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/ToolNudgeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/THERMOVR/features/ToolSliderTime.py` & `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/ToolSliderTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template` & `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json` & `opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template` & `opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/WaveLoader.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/WaveLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/AverageFails.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageFails.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/AverageLevelTime.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/AverageSliderMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageSliderMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/BeginCount.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/BeginCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/ClosenessIntercept.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessIntercept.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/ClosenessR2.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessR2.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/ClosenessSlope.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessSlope.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/Completed.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/Completed.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/FirstMoveType.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/FirstMoveType.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/MenuButtonCount.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/MenuButtonCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OverallSliderAverageRange.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallSliderAverageRange.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentOffsetMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentOffsetMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PercentWavelengthMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentWavelengthMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/PersistentSessionID.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PersistentSessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/QuestionAnswered.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/QuestionAnswered.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/QuestionCorrect.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/QuestionCorrect.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/RangeIntercept.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeIntercept.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/RangeR2.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeR2.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/RangeSlope.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeSlope.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/SequenceLevel.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SequenceLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/SessionID.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/SliderAverageRange.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SliderAverageRange.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/SucceedCount.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SucceedCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TimeToAnswerMS.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TimeToAnswerMS.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalArrowMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalArrowMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalFails.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalFails.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalLevelTime.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalResets.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalResets.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalSkips.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalSkips.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/TotalSliderMoves.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalSliderMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/features/__init__.py` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WAVES/schemas/WAVES.json.template` & `opengamedata_core-0.0.5/src/ogd/games/WAVES/schemas/WAVES.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template` & `opengamedata_core-0.0.5/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.4/src/opengamedata_core.egg-info/PKG-INFO` & `opengamedata_core-0.0.5/src/opengamedata_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for retrieving and processing event-based video game data. Additional authors: Nick Spevacek, Renee Li, John McCloskey, Zach Studdiford, Glenn Palmer, Haishuo Chen, Daus, Ameya Kshirsagar, Yunqing Xiao, Erik Harpstead, Manuel Jesus Gomez Moratilla
 Author-email: Luke Swanson <superscription58@gmail.com>, David Gagnon <djgagnon@wisc.edu>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-core
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-core/issues
 Project-URL: Documentation, https://opengamedata-doc.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_core-0.0.4/src/opengamedata_core.egg-info/SOURCES.txt` & `opengamedata_core-0.0.5/src/opengamedata_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,14 @@
 src/ogd/games/AQUALAB/features/JobTriesInArgument.py
 src/ogd/games/AQUALAB/features/JobsAttempted.py
 src/ogd/games/AQUALAB/features/JobsCompleted.py
 src/ogd/games/AQUALAB/features/ModelExportCount.py
 src/ogd/games/AQUALAB/features/ModelInterveneCount.py
 src/ogd/games/AQUALAB/features/ModelPredictCount.py
 src/ogd/games/AQUALAB/features/PerJobFeature.py
-src/ogd/games/AQUALAB/features/PlayLocations.py
 src/ogd/games/AQUALAB/features/PlayerSummary.py
 src/ogd/games/AQUALAB/features/PopulationSummary.py
 src/ogd/games/AQUALAB/features/RegionJobCount.py
 src/ogd/games/AQUALAB/features/RegionName.py
 src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
 src/ogd/games/AQUALAB/features/SessionDuration.py
 src/ogd/games/AQUALAB/features/SessionGuideCount.py
```

### Comparing `opengamedata_core-0.0.4/tests/test_lakeland_models.py` & `opengamedata_core-0.0.5/tests/test_lakeland_models.py`

 * *Files identical despite different names*

