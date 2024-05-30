# Comparing `tmp/es_aces-0.2.0.tar.gz` & `tmp/es_aces-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "es_aces-0.2.0.tar", last modified: Fri May 24 18:22:10 2024, max compression
+gzip compressed data, was "es_aces-0.2.1.tar", last modified: Thu May 30 01:33:11 2024, max compression
```

## Comparing `es_aces-0.2.0.tar` & `es_aces-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,93 @@
-drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-24 18:22:10.671163 es_aces-0.2.0/
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1085 2024-05-23 23:19:04.000000 es_aces-0.2.0/LICENSE
--rw-r--r--   0 justinxu  (1024) justinxu  (1027)     9722 2024-05-24 18:22:10.671163 es_aces-0.2.0/PKG-INFO
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     8604 2024-05-24 18:05:34.000000 es_aces-0.2.0/README.md
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1076 2024-05-24 17:40:18.000000 es_aces-0.2.0/pyproject.toml
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)       38 2024-05-24 18:22:10.671163 es_aces-0.2.0/setup.cfg
-drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-24 18:22:10.667162 es_aces-0.2.0/src/
-drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-24 18:22:10.671163 es_aces-0.2.0/src/aces/
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)        0 2023-12-12 13:22:32.000000 es_aces-0.2.0/src/aces/__init__.py
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     2343 2024-05-24 17:32:17.000000 es_aces-0.2.0/src/aces/__main__.py
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    95141 2024-05-23 20:43:39.000000 es_aces-0.2.0/src/aces/aggregate.py
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    45355 2024-05-23 22:33:41.000000 es_aces-0.2.0/src/aces/config.py
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     5675 2024-05-23 20:43:39.000000 es_aces-0.2.0/src/aces/constraints.py
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    24206 2024-05-23 20:43:39.000000 es_aces-0.2.0/src/aces/extract_subtree.py
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    14960 2024-05-23 22:33:41.000000 es_aces-0.2.0/src/aces/predicates.py
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1687 2024-05-24 06:48:01.000000 es_aces-0.2.0/src/aces/query.py
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    12547 2024-05-23 20:43:39.000000 es_aces-0.2.0/src/aces/types.py
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1745 2024-05-23 20:43:39.000000 es_aces-0.2.0/src/aces/utils.py
-drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-24 18:22:10.671163 es_aces-0.2.0/src/es_aces.egg-info/
--rw-r--r--   0 justinxu  (1024) justinxu  (1027)     9722 2024-05-24 18:22:10.000000 es_aces-0.2.0/src/es_aces.egg-info/PKG-INFO
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      456 2024-05-24 18:22:10.000000 es_aces-0.2.0/src/es_aces.egg-info/SOURCES.txt
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)        1 2024-05-24 18:22:10.000000 es_aces-0.2.0/src/es_aces.egg-info/dependency_links.txt
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)       48 2024-05-24 18:22:10.000000 es_aces-0.2.0/src/es_aces.egg-info/entry_points.txt
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      213 2024-05-24 18:22:10.000000 es_aces-0.2.0/src/es_aces.egg-info/requires.txt
--rw-rw-r--   0 justinxu  (1024) justinxu  (1027)        5 2024-05-24 18:22:10.000000 es_aces-0.2.0/src/es_aces.egg-info/top_level.txt
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.100053 es_aces-0.2.1/
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.084052 es_aces-0.2.1/.github/
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.084052 es_aces-0.2.1/.github/workflows/
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      448 2024-05-20 01:55:23.000000 es_aces-0.2.1/.github/workflows/code-quality-master.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      887 2024-05-20 01:55:23.000000 es_aces-0.2.1/.github/workflows/code-quality-pr.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      931 2024-05-30 01:20:24.000000 es_aces-0.2.1/.github/workflows/tests.yml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     3342 2024-05-30 01:18:59.000000 es_aces-0.2.1/.gitignore
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     3335 2024-05-09 03:49:20.000000 es_aces-0.2.1/.pre-commit-config.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)        0 2023-12-12 13:22:32.000000 es_aces-0.2.1/.project-root
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      615 2024-05-22 19:01:07.000000 es_aces-0.2.1/.readthedocs.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1085 2024-05-23 23:19:04.000000 es_aces-0.2.1/LICENSE
+-rw-r--r--   0 justinxu  (1024) justinxu  (1027)    18598 2024-05-30 01:33:11.096053 es_aces-0.2.1/PKG-INFO
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    17478 2024-05-29 20:11:51.000000 es_aces-0.2.1/README.md
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.084052 es_aces-0.2.1/docs/
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      638 2024-05-22 19:01:07.000000 es_aces-0.2.1/docs/Makefile
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      764 2024-05-22 19:01:07.000000 es_aces-0.2.1/docs/make.bat
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      139 2024-05-22 19:01:07.000000 es_aces-0.2.1/docs/requirements.txt
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.088052 es_aces-0.2.1/docs/source/
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)   835151 2024-01-17 18:52:57.000000 es_aces-0.2.1/docs/source/TaskSchemaDefinition.svg
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    11599 2024-05-24 17:57:19.000000 es_aces-0.2.1/docs/source/conf.py
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    12321 2024-05-26 07:16:21.000000 es_aces-0.2.1/docs/source/configuration.md
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      217 2024-05-24 18:05:34.000000 es_aces-0.2.1/docs/source/examples.md
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      549 2024-05-26 07:27:35.000000 es_aces-0.2.1/docs/source/index.md
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)       72 2024-05-22 19:01:07.000000 es_aces-0.2.1/docs/source/license.md
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.088052 es_aces-0.2.1/docs/source/notebooks/
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     4522 2024-05-29 09:52:06.000000 es_aces-0.2.1/docs/source/notebooks/tutorial.ipynb
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)       33 2024-05-22 19:01:07.000000 es_aces-0.2.1/docs/source/overview.md
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)        0 2024-05-26 07:27:09.000000 es_aces-0.2.1/docs/source/predicates.md
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1150 2024-05-22 19:01:07.000000 es_aces-0.2.1/docs/source/query-16.ico
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     6403 2024-05-22 19:01:07.000000 es_aces-0.2.1/docs/source/query-512.png
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    16222 2024-05-29 06:40:22.000000 es_aces-0.2.1/docs/source/terminology.md
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     3531 2024-05-29 22:08:47.000000 es_aces-0.2.1/docs/source/usage.md
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1101 2024-05-30 01:18:59.000000 es_aces-0.2.1/pyproject.toml
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.088052 es_aces-0.2.1/sample_configs/
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      979 2024-05-30 00:37:22.000000 es_aces-0.2.1/sample_configs/abnormal-lab.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      696 2024-05-30 00:37:26.000000 es_aces-0.2.1/sample_configs/heart-failture-controls.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      673 2024-05-30 00:37:49.000000 es_aces-0.2.1/sample_configs/heart-failure-cases.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      275 2024-05-30 00:37:49.000000 es_aces-0.2.1/sample_configs/imminent-mortality.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      751 2024-05-30 00:37:49.000000 es_aces-0.2.1/sample_configs/inhospital-mortality.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      613 2024-05-30 00:37:49.000000 es_aces-0.2.1/sample_configs/intervention-weaning.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1122 2024-05-30 00:37:49.000000 es_aces-0.2.1/sample_configs/intubation-onset.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      731 2024-05-30 00:37:49.000000 es_aces-0.2.1/sample_configs/long-length-of-stay.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1607 2024-05-30 00:37:49.000000 es_aces-0.2.1/sample_configs/long-term-incidence.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      435 2024-05-30 00:37:49.000000 es_aces-0.2.1/sample_configs/readmission-risk.yaml
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.088052 es_aces-0.2.1/sample_data/
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.092052 es_aces-0.2.1/sample_data/esgpt_sample/
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.084052 es_aces-0.2.1/sample_data/esgpt_sample/.logs/
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.092052 es_aces-0.2.1/sample_data/esgpt_sample/.logs/.hydra/
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1526 2024-04-19 04:41:45.000000 es_aces-0.2.1/sample_data/esgpt_sample/.logs/.hydra/config.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     3619 2024-04-19 04:41:45.000000 es_aces-0.2.1/sample_data/esgpt_sample/.logs/.hydra/hydra.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)        3 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/.logs/.hydra/overrides.yaml
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.096053 es_aces-0.2.1/sample_data/esgpt_sample/DL_reps/
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)   117564 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/DL_reps/held_out_0.parquet
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)   851949 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/DL_reps/train_0.parquet
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    91192 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/DL_reps/tuning_0.parquet
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     5244 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/E.pkl
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     2175 2024-04-19 04:41:45.000000 es_aces-0.2.1/sample_data/esgpt_sample/config.json
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)   790645 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/dynamic_measurements_df.parquet
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)   429294 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/events_df.parquet
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1530 2024-04-19 04:41:45.000000 es_aces-0.2.1/sample_data/esgpt_sample/hydra_config.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     3337 2024-04-19 04:41:45.000000 es_aces-0.2.1/sample_data/esgpt_sample/inferred_measurement_configs.json
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.096053 es_aces-0.2.1/sample_data/esgpt_sample/inferred_measurement_metadata/
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      181 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/inferred_measurement_metadata/HR.csv
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      183 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/inferred_measurement_metadata/age.csv
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      712 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/inferred_measurement_metadata/lab_name.csv
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      182 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/inferred_measurement_metadata/temp.csv
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1701 2024-04-19 04:41:45.000000 es_aces-0.2.1/sample_data/esgpt_sample/input_schema.json
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     2693 2024-04-14 07:01:46.000000 es_aces-0.2.1/sample_data/esgpt_sample/subjects_df.parquet
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      773 2024-04-19 04:41:45.000000 es_aces-0.2.1/sample_data/esgpt_sample/vocabulary_config.json
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     2444 2024-05-23 20:43:39.000000 es_aces-0.2.1/sample_data/sample_data.csv
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)       38 2024-05-30 01:33:11.100053 es_aces-0.2.1/setup.cfg
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.084052 es_aces-0.2.1/src/
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.096053 es_aces-0.2.1/src/aces/
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)        0 2024-05-29 19:33:49.000000 es_aces-0.2.1/src/aces/__init__.py
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1323 2024-05-30 01:18:59.000000 es_aces-0.2.1/src/aces/__main__.py
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    95141 2024-05-27 19:50:14.000000 es_aces-0.2.1/src/aces/aggregate.py
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    49231 2024-05-30 01:11:42.000000 es_aces-0.2.1/src/aces/config.py
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      731 2024-05-30 01:18:59.000000 es_aces-0.2.1/src/aces/config.yaml
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     5595 2024-05-29 08:34:32.000000 es_aces-0.2.1/src/aces/constraints.py
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    24131 2024-05-29 08:34:38.000000 es_aces-0.2.1/src/aces/extract_subtree.py
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    22685 2024-05-30 01:18:59.000000 es_aces-0.2.1/src/aces/predicates.py
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     3207 2024-05-30 01:11:42.000000 es_aces-0.2.1/src/aces/query.py
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    12546 2024-05-27 19:47:35.000000 es_aces-0.2.1/src/aces/types.py
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     1765 2024-05-30 01:11:42.000000 es_aces-0.2.1/src/aces/utils.py
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.096053 es_aces-0.2.1/src/es_aces.egg-info/
+-rw-r--r--   0 justinxu  (1024) justinxu  (1027)    18598 2024-05-30 01:33:11.000000 es_aces-0.2.1/src/es_aces.egg-info/PKG-INFO
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)     2448 2024-05-30 01:33:11.000000 es_aces-0.2.1/src/es_aces.egg-info/SOURCES.txt
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)        1 2024-05-30 01:33:11.000000 es_aces-0.2.1/src/es_aces.egg-info/dependency_links.txt
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)       48 2024-05-30 01:33:11.000000 es_aces-0.2.1/src/es_aces.egg-info/entry_points.txt
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)      215 2024-05-30 01:33:11.000000 es_aces-0.2.1/src/es_aces.egg-info/requires.txt
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)        5 2024-05-30 01:33:11.000000 es_aces-0.2.1/src/es_aces.egg-info/top_level.txt
+drwxrwxr-x   0 justinxu  (1024) justinxu  (1027)        0 2024-05-30 01:33:11.096053 es_aces-0.2.1/tests/
+-rw-rw-r--   0 justinxu  (1024) justinxu  (1027)    10188 2024-05-30 01:18:59.000000 es_aces-0.2.1/tests/test_e2e.py
```

### Comparing `es_aces-0.2.0/LICENSE` & `es_aces-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `es_aces-0.2.0/pyproject.toml` & `es_aces-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [project]
 name = "es-aces"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Justin Xu", email="justin13601@hotmail.com" },
   { name="Matthew McDermott", email="mattmcdermott8@gmail.com" },
 ]
 description = "Event Stream Automatic Cohort Extraction System (ACES)"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "polars == 0.20.18",
     "bigtree == 0.17.0",
     "ruamel.yaml == 0.18.6",
-    "pandas == 2.2.2",
     "loguru == 0.7.2",
     "hydra-core == 1.3.2",
     "pytimeparse == 1.1.8",
     "networkx == 3.3",
+    "pyarrow == 16.1.0",
 ]
 
 [project.scripts]
 aces-cli = "aces.__main__:main"
 
 [build-system]
-requires = ["setuptools>=61.0", "wheel"]
+requires = ["setuptools>=61.0", "setuptools-scm>=8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
 dev = [
   "pre-commit", "pytest", "pytest-cov", "pytest-subtests", "rootutils"
 ]
 profiling = ["psutil"]
```

### Comparing `es_aces-0.2.0/src/aces/aggregate.py` & `es_aces-0.2.1/src/aces/aggregate.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,85 +79,85 @@
         ...     "is_C": [1, 1, 0, 0, 1, 0],
         ... })
         >>> aggregate_temporal_window(df, TemporalWindowBounds(True, timedelta(days=7), True, None))
         shape: (6, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-08 12:03:00 ┆ 2    ┆ 2    ┆ 2    │
         │ 1          ┆ 1989-12-02 05:17:00 ┆ 1989-12-02 05:17:00 ┆ 1989-12-09 05:17:00 ┆ 1    ┆ 2    ┆ 1    │
         │ 1          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-09 12:03:00 ┆ 1    ┆ 1    ┆ 0    │
         │ 1          ┆ 1989-12-06 11:00:00 ┆ 1989-12-06 11:00:00 ┆ 1989-12-13 11:00:00 ┆ 0    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-01 13:14:00 ┆ 1989-12-01 13:14:00 ┆ 1989-12-08 13:14:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-03 15:17:00 ┆ 1989-12-03 15:17:00 ┆ 1989-12-10 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
         └────────────┴─────────────────────┴─────────────────────┴─────────────────────┴──────┴──────┴──────┘
         >>> aggregate_temporal_window(df, (True, timedelta(days=1), True, timedelta(days=0)))
         shape: (6, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 2    ┆ 1    ┆ 2    │
         │ 1          ┆ 1989-12-02 05:17:00 ┆ 1989-12-02 05:17:00 ┆ 1989-12-03 05:17:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-03 12:03:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-06 11:00:00 ┆ 1989-12-06 11:00:00 ┆ 1989-12-07 11:00:00 ┆ 0    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-01 13:14:00 ┆ 1989-12-01 13:14:00 ┆ 1989-12-02 13:14:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-03 15:17:00 ┆ 1989-12-03 15:17:00 ┆ 1989-12-04 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
         └────────────┴─────────────────────┴─────────────────────┴─────────────────────┴──────┴──────┴──────┘
         >>> aggregate_temporal_window(df, (True, timedelta(days=1), False, timedelta(days=0)))
         shape: (6, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1    ┆ 1    ┆ 2    │
         │ 1          ┆ 1989-12-02 05:17:00 ┆ 1989-12-02 05:17:00 ┆ 1989-12-03 05:17:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-03 12:03:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-06 11:00:00 ┆ 1989-12-06 11:00:00 ┆ 1989-12-07 11:00:00 ┆ 0    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-01 13:14:00 ┆ 1989-12-01 13:14:00 ┆ 1989-12-02 13:14:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-03 15:17:00 ┆ 1989-12-03 15:17:00 ┆ 1989-12-04 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
         └────────────┴─────────────────────┴─────────────────────┴─────────────────────┴──────┴──────┴──────┘
         >>> aggregate_temporal_window(df, (False, timedelta(days=1), False, timedelta(days=0)))
         shape: (6, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-02 05:17:00 ┆ 1989-12-02 05:17:00 ┆ 1989-12-03 05:17:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-03 12:03:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-06 11:00:00 ┆ 1989-12-06 11:00:00 ┆ 1989-12-07 11:00:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-01 13:14:00 ┆ 1989-12-01 13:14:00 ┆ 1989-12-02 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-03 15:17:00 ┆ 1989-12-03 15:17:00 ┆ 1989-12-04 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
         └────────────┴─────────────────────┴─────────────────────┴─────────────────────┴──────┴──────┴──────┘
         >>> aggregate_temporal_window(df, (False, timedelta(days=-1), False, timedelta(days=0)))
         shape: (6, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-11-30 12:03:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-02 05:17:00 ┆ 1989-12-02 05:17:00 ┆ 1989-12-01 05:17:00 ┆ 1    ┆ 0    ┆ 1    │
         │ 1          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-06 11:00:00 ┆ 1989-12-06 11:00:00 ┆ 1989-12-05 11:00:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-01 13:14:00 ┆ 1989-12-01 13:14:00 ┆ 1989-11-30 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-03 15:17:00 ┆ 1989-12-03 15:17:00 ┆ 1989-12-02 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
         └────────────┴─────────────────────┴─────────────────────┴─────────────────────┴──────┴──────┴──────┘
         >>> aggregate_temporal_window(df, (False, timedelta(hours=12), False, timedelta(hours=12)))
         shape: (6, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-02 00:03:00 ┆ 1989-12-02 12:03:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-02 05:17:00 ┆ 1989-12-02 17:17:00 ┆ 1989-12-03 05:17:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-02 12:03:00 ┆ 1989-12-03 00:03:00 ┆ 1989-12-03 12:03:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-06 11:00:00 ┆ 1989-12-06 23:00:00 ┆ 1989-12-07 11:00:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-01 13:14:00 ┆ 1989-12-02 01:14:00 ┆ 1989-12-02 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-03 15:17:00 ┆ 1989-12-04 03:17:00 ┆ 1989-12-04 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
@@ -167,29 +167,29 @@
         >>> # the earliest event in the aggregation window, regardless of whether that is earlier than the
         >>> # timestamp of the row.
         >>> aggregate_temporal_window(df, (False, timedelta(days=-1), True, timedelta(days=1)))
         shape: (6, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-02 05:17:00 ┆ 1989-12-03 05:17:00 ┆ 1989-12-02 05:17:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-02 12:03:00 ┆ 1989-12-03 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-06 11:00:00 ┆ 1989-12-07 11:00:00 ┆ 1989-12-06 11:00:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-01 13:14:00 ┆ 1989-12-02 13:14:00 ┆ 1989-12-01 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-03 15:17:00 ┆ 1989-12-04 15:17:00 ┆ 1989-12-03 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
         └────────────┴─────────────────────┴─────────────────────┴─────────────────────┴──────┴──────┴──────┘
         >>> aggregate_temporal_window(df, (True, timedelta(days=-1), False, timedelta(days=1)))
         shape: (6, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1    ┆ 1    ┆ 2    │
         │ 1          ┆ 1989-12-02 05:17:00 ┆ 1989-12-03 05:17:00 ┆ 1989-12-02 05:17:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-02 12:03:00 ┆ 1989-12-03 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-06 11:00:00 ┆ 1989-12-07 11:00:00 ┆ 1989-12-06 11:00:00 ┆ 0    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-01 13:14:00 ┆ 1989-12-02 13:14:00 ┆ 1989-12-01 13:14:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-03 15:17:00 ┆ 1989-12-04 15:17:00 ┆ 1989-12-03 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
@@ -297,15 +297,15 @@
         ...     "is_C": [0, 1, 0, 0, 0, 1, 0, 1],
         ... })
         >>> aggregate_event_bound_window(df, ToEventWindowBounds(True, "is_C", True, None))
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-06 15:17:00 ┆ 3    ┆ 2    ┆ 1    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-06 15:17:00 ┆ 2    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-06 15:17:00 ┆ 1989-12-06 15:17:00 ┆ 1    ┆ 1    ┆ 1    │
@@ -313,15 +313,15 @@
         │ 2          ┆ 1989-12-10 03:07:00 ┆ 1989-12-10 03:07:00 ┆ 1989-12-10 03:07:00 ┆ 0    ┆ 1    ┆ 1    │
         └────────────┴─────────────────────┴─────────────────────┴─────────────────────┴──────┴──────┴──────┘
         >>> aggregate_event_bound_window(df, ToEventWindowBounds(True, "is_C", False, None))
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-06 15:17:00 ┆ 2    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-06 15:17:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-06 15:17:00 ┆ 1989-12-10 03:07:00 ┆ 1    ┆ 2    ┆ 1    │
@@ -329,15 +329,15 @@
         │ 2          ┆ 1989-12-10 03:07:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         └────────────┴─────────────────────┴─────────────────────┴─────────────────────┴──────┴──────┴──────┘
         >>> aggregate_event_bound_window(df, ToEventWindowBounds(False, "is_C", True, None))
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-06 15:17:00 ┆ 2    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-06 15:17:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-06 15:17:00 ┆ 1989-12-06 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
@@ -345,15 +345,15 @@
         │ 2          ┆ 1989-12-10 03:07:00 ┆ 1989-12-10 03:07:00 ┆ 1989-12-10 03:07:00 ┆ 0    ┆ 0    ┆ 0    │
         └────────────┴─────────────────────┴─────────────────────┴─────────────────────┴──────┴──────┴──────┘
         >>> aggregate_event_bound_window(df, ToEventWindowBounds(True, "is_C", True, timedelta(days=3)))
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-05 12:03:00 ┆ 1989-12-06 15:17:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-07 13:14:00 ┆ 1989-12-10 03:07:00 ┆ 0    ┆ 2    ┆ 1    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-09 15:17:00 ┆ 1989-12-10 03:07:00 ┆ 0    ┆ 1    ┆ 1    │
@@ -493,15 +493,15 @@
         ...     "bound_to_row",
         ...     "both",
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-05 15:17:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-06 15:17:00 ┆ 2    ┆ 1    ┆ 1    │
@@ -514,15 +514,15 @@
         ...     "bound_to_row",
         ...     "none",
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-05 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-06 15:17:00 ┆ 0    ┆ 0    ┆ 0    │
@@ -535,15 +535,15 @@
         ...     "bound_to_row",
         ...     "left",
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-05 15:17:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-06 15:17:00 ┆ 1    ┆ 0    ┆ 0    │
@@ -556,15 +556,15 @@
         ...     "bound_to_row",
         ...     "right",
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-05 15:17:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-06 15:17:00 ┆ 1    ┆ 1    ┆ 1    │
@@ -577,15 +577,15 @@
         ...     "row_to_bound",
         ...     "both",
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-04 13:14:00 ┆ 2    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-06 15:17:00 ┆ 1989-12-10 03:07:00 ┆ 1    ┆ 3    ┆ 2    │
@@ -598,15 +598,15 @@
         ...     "row_to_bound",
         ...     "none",
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-04 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-10 03:07:00 ┆ 1    ┆ 2    ┆ 1    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-06 15:17:00 ┆ 1989-12-10 03:07:00 ┆ 0    ┆ 1    ┆ 0    │
@@ -619,15 +619,15 @@
         ...     "row_to_bound",
         ...     "left",
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-04 13:14:00 ┆ 1    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-10 03:07:00 ┆ 2    ┆ 2    ┆ 1    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-06 15:17:00 ┆ 1989-12-10 03:07:00 ┆ 1    ┆ 2    ┆ 1    │
@@ -640,15 +640,15 @@
         ...     "row_to_bound",
         ...     "right",
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-01 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-02 12:03:00 ┆ 1989-12-04 13:14:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-06 15:17:00 ┆ 1989-12-10 03:07:00 ┆ 0    ┆ 2    ┆ 1    │
@@ -663,15 +663,15 @@
         ...     "both",
         ...     offset = timedelta(days=3),
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-04 12:03:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-06 13:14:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-08 15:17:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-05 12:03:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-07 13:14:00 ┆ 2    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-09 15:17:00 ┆ 2    ┆ 2    ┆ 1    │
@@ -685,15 +685,15 @@
         ...     "left",
         ...     offset = timedelta(days=3),
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-04 12:03:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-06 13:14:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ 1989-12-03 13:14:00 ┆ 1989-12-08 15:17:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-05 12:03:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-07 13:14:00 ┆ 2    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-04 13:14:00 ┆ 1989-12-09 15:17:00 ┆ 2    ┆ 2    ┆ 1    │
@@ -707,15 +707,15 @@
         ...     "none",
         ...     timedelta(days=-3),
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
@@ -729,15 +729,15 @@
         ...     "right",
         ...     offset = timedelta(days=-3),
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
@@ -751,15 +751,15 @@
         ...     "both",
         ...     offset = timedelta(days=3),
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-05 12:03:00 ┆ 1989-12-10 03:07:00 ┆ 1    ┆ 3    ┆ 2    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-07 13:14:00 ┆ 1989-12-10 03:07:00 ┆ 0    ┆ 2    ┆ 1    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-09 15:17:00 ┆ 1989-12-10 03:07:00 ┆ 0    ┆ 1    ┆ 1    │
@@ -773,15 +773,15 @@
         ...     "left",
         ...     offset = timedelta(days=3),
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ null                ┆ null                ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-12-05 12:03:00 ┆ 1989-12-10 03:07:00 ┆ 1    ┆ 2    ┆ 1    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-07 13:14:00 ┆ 1989-12-10 03:07:00 ┆ 0    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-09 15:17:00 ┆ 1989-12-10 03:07:00 ┆ 0    ┆ 0    ┆ 0    │
@@ -795,15 +795,15 @@
         ...     "none",
         ...     offset = timedelta(days=-3),
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-11-28 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ 1989-11-30 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 1    ┆ 0    ┆ 0    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ 1989-12-02 15:17:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-11-29 12:03:00 ┆ 1989-12-04 13:14:00 ┆ 1    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-01 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 1    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-03 15:17:00 ┆ 1989-12-04 13:14:00 ┆ 0    ┆ 0    ┆ 0    │
@@ -817,15 +817,15 @@
         ...     "right",
         ...     offset = timedelta(days=-3),
         ... ).drop("idx")
         shape: (8, 7)
         ┌────────────┬─────────────────────┬─────────────────────┬─────────────────────┬──────┬──────┬──────┐
         │ subject_id ┆ timestamp           ┆ timestamp_at_start  ┆ timestamp_at_end    ┆ is_A ┆ is_B ┆ is_C │
         │ ---        ┆ ---                 ┆ ---                 ┆ ---                 ┆ ---  ┆ ---  ┆ ---  │
-        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ u16  ┆ u16  ┆ u16  │
+        │ i64        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ i64  ┆ i64  ┆ i64  │
         ╞════════════╪═════════════════════╪═════════════════════╪═════════════════════╪══════╪══════╪══════╡
         │ 1          ┆ 1989-12-01 12:03:00 ┆ 1989-11-28 12:03:00 ┆ 1989-12-03 13:14:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-03 13:14:00 ┆ 1989-11-30 13:14:00 ┆ 1989-12-03 13:14:00 ┆ 1    ┆ 1    ┆ 1    │
         │ 1          ┆ 1989-12-05 15:17:00 ┆ 1989-12-02 15:17:00 ┆ 1989-12-03 13:14:00 ┆ 0    ┆ 1    ┆ 1    │
         │ 2          ┆ 1989-12-02 12:03:00 ┆ 1989-11-29 12:03:00 ┆ 1989-12-04 13:14:00 ┆ 2    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-04 13:14:00 ┆ 1989-12-01 13:14:00 ┆ 1989-12-04 13:14:00 ┆ 2    ┆ 1    ┆ 0    │
         │ 2          ┆ 1989-12-06 15:17:00 ┆ 1989-12-03 15:17:00 ┆ 1989-12-04 13:14:00 ┆ 1    ┆ 0    ┆ 0    │
```

### Comparing `es_aces-0.2.0/src/aces/config.py` & `es_aces-0.2.1/src/aces/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,25 +257,39 @@
             Likewise, unreferenced predicates are also left unconstrained. Note that as predicate counts are
             always integral, this specification does not need an additional inclusive/exclusive endpoint
             field, as one can simply increment the bound by one in the appropriate direction to achieve the
             result. Instead, this bound is always interpreted to be inclusive, so a window would satisfy the
             constraint for predicate `name` with constraint `name: (1, 2)` if the count of observations of
             predicate `name` in a window was either 1 or 2. All constraints in the dictionary must be
             satisfied on a window for it to be included.
+        label: A string that specifies the name of a predicate to be used as the label for the task. The
+            predicate count of the window this field is specified in will be extracted as a column in the
+            final result. Hence, there can only be one 'label' per TaskExtractorConfig. If more than one
+            'label' is specified, an error is raised. If the specified 'label' is not a defined predicate,
+            an error is also raised. If no 'label' is specified, there will be not be a 'label' column.
+        index_timestamp: A string that is either 'start' or 'end' and is used to index result rows. If it is
+            defined, there will be an 'index_timestamp' column in the result with its values equal to the
+            'start' or 'end' timestamp of the window in which it was specified. Usually, this will be
+            specified to indicate the time of prediction for the task, which is often the 'end' of the input
+            window. There can only be one 'index_timestamp' per TaskExtractorConfig. If more than one
+            'index_timestamp' is specified, an error is raised. If the specified 'index_timestamp' is not
+            'start' or 'end', an error is also raised. If no 'index_timestamp' is defined, there will be no
+            'index_timestamp' column.
 
     Raises:
         ValueError: If the window is misconfigured in any of a variety of ways; see below for examples.
 
     Examples:
         >>> input_window = WindowConfig(
         ...     start=None,
         ...     end="trigger + 2 days",
         ...     start_inclusive=True,
         ...     end_inclusive=True,
-        ...     has={"_ANY_EVENT": "(5, None)"}
+        ...     has={"_ANY_EVENT": "(5, None)"},
+        ...     index_timestamp="end",
         ... )
         >>> input_window.referenced_event
         ('trigger',)
         >>> # This window does not reference any "true" external predicates, only implicit predicates like
         >>> # start, end, and * events, so this list should be empty.
         >>> sorted(input_window.referenced_predicates)
         []
@@ -414,22 +428,34 @@
         ...     start_inclusive=False,
         ...     end_inclusive=True,
         ...     has={}
         ... )
         Traceback (most recent call last):
             ...
         ValueError: Window boundary cannot contain both '->' and '<-' operators.
+        >>> invalid_window = WindowConfig(
+        ...     start="input.end",
+        ...     end="input.end + 2d",
+        ...     start_inclusive=False,
+        ...     end_inclusive=True,
+        ...     has={"discharge": "(0)", "death": "(None, 0)"}
+        ... ) # doctest: +NORMALIZE_WHITESPACE
+        Traceback (most recent call last):
+            ...
+        ValueError: Invalid constraint format: discharge.
+        Expected format: '(min, max)', but got: '(0)'
     """
 
     start: str | None
     end: str | None
     start_inclusive: bool
     end_inclusive: bool
     has: dict[str, str] = field(default_factory=dict)
     label: str | None = None
+    index_timestamp: str | None = None
 
     @classmethod
     def _check_reference(cls, reference: str):
         """Checks to ensure referenced events are valid."""
 
         err_str = (
             "Window boundary reference must be either a valid alphanumeric/'_' string "
@@ -492,16 +518,21 @@
 
     def __post_init__(self):
         # Parse the has constraints from the string representation to the tuple representation
         if self.has is not None:
             for each_constraint in self.has:
                 elements = self.has[each_constraint].strip("()").split(",")
                 elements = [element.strip() for element in elements]
+                if len(elements) != 2:
+                    raise ValueError(
+                        f"Invalid constraint format: {each_constraint}. "
+                        f"Expected format: '(min, max)', but got: '{self.has[each_constraint]}'"
+                    )
                 self.has[each_constraint] = tuple(
-                    int(element) if element != "None" else None for element in elements
+                    int(element) if element not in ("None", "") else None for element in elements
                 )
 
         if self.start is None and self.end is None:
             raise ValueError("Window cannot progress from the start of the record to the end of the record.")
 
         if self.start is None:
             self._parsed_start = {
@@ -578,15 +609,14 @@
             # `start_inclusive` and `right_inclusive` corresponds to `end_inclusive`.
             left_inclusive = self.start_inclusive
             right_inclusive = self.end_inclusive
         else:
             # If this window references end from start, then the end event window expression will not have
             # any constraints as it will reference an external event, and therefore the inclusive
             # parameters don't matter.
-            # TODO(mmd): This may not be the best API.
             left_inclusive = False
             right_inclusive = False
 
         if self._parsed_start["event_bound"]:
             return ToEventWindowBounds(
                 end_event=self._parsed_start["event_bound"],
                 left_inclusive=left_inclusive,
@@ -603,15 +633,14 @@
 
     @property
     def end_endpoint_expr(self) -> None | ToEventWindowBounds | TemporalWindowBounds:
         if self._start_references_end:
             # If this window references end from start, then the end event window expression will not have
             # any constraints as it will reference an external event, and therefore the inclusive
             # parameters don't matter.
-            # TODO(mmd): This may not be the best API.
             left_inclusive = False
             right_inclusive = False
         else:
             # If end references start, then end will occur after start, so `left_inclusive` corresponds to
             # `start_inclusive` and `right_inclusive` corresponds to `end_inclusive`.
             left_inclusive = self.start_inclusive
             right_inclusive = self.end_inclusive
@@ -660,15 +689,15 @@
     which is ultimately parsed into the expansive, full specification contained in the YAML file referenced
     above.
 
     Args:
         predicates: A dictionary of predicate configurations, stored as either plain or derived predicate
             configuration objects (which are simple dataclasses with utility functions over plain
             dictionaries).
-        trigger_event: The event configuration that triggers the task extraction process. This is a simple
+        trigger: The event configuration that triggers the task extraction process. This is a simple
             dataclass with a single field, the name of the predicate that triggers the task extraction and
             serves as the root of the window tree.
         windows: A dictionary of window configurations. Each window configuration is a simple dataclass with
             that can be materialized to/from a simple, POD dictionary.
 
     Raises:
         ValueError: If any window or predicate names are not composed of alphanumeric or "_" characters.
@@ -677,39 +706,41 @@
         >>> from bigtree import print_tree
         >>> predicates = {
         ...     "admission": PlainPredicateConfig("admission"),
         ...     "discharge": PlainPredicateConfig("discharge"),
         ...     "death": PlainPredicateConfig("death"),
         ...     "death_or_discharge": DerivedPredicateConfig("or(death, discharge)"),
         ... }
-        >>> trigger_event = EventConfig("admission")
+        >>> trigger = EventConfig("admission")
         >>> windows = {
         ...     "input": WindowConfig(
         ...         start=None,
         ...         end="trigger + 24h",
         ...         start_inclusive=True,
         ...         end_inclusive=True,
         ...         has={"_ANY_EVENT": "(32, None)"},
+        ...         index_timestamp="end",
         ...     ),
         ...     "gap": WindowConfig(
         ...         start="input.end",
         ...         end="start + 24h",
         ...         start_inclusive=False,
         ...         end_inclusive=True,
         ...         has={"death_or_discharge": "(None, 0)", "admission": "(None, 0)"},
         ...     ),
         ...     "target": WindowConfig(
         ...         start="gap.end",
         ...         end="start -> death_or_discharge",
         ...         start_inclusive=False,
         ...         end_inclusive=True,
         ...         has={},
+        ...         label="death",
         ...     ),
         ... }
-        >>> config = TaskExtractorConfig(predicates=predicates, trigger_event=trigger_event, windows=windows)
+        >>> config = TaskExtractorConfig(predicates=predicates, trigger=trigger, windows=windows)
         >>> print(config.plain_predicates) # doctest: +NORMALIZE_WHITESPACE
         {'admission': PlainPredicateConfig(code='admission',
                               value_min=None,
                               value_max=None,
                               value_min_inclusive=None,
                               value_max_inclusive=None),
          'discharge': PlainPredicateConfig(code='discharge',
@@ -719,14 +750,18 @@
                               value_max_inclusive=None),
          'death': PlainPredicateConfig(code='death',
                               value_min=None,
                               value_max=None,
                               value_min_inclusive=None,
                               value_max_inclusive=None)}
 
+        >>> print(config.label_window) # doctest: +NORMALIZE_WHITESPACE
+        target
+        >>> print(config.index_timestamp_window) # doctest: +NORMALIZE_WHITESPACE
+        input
         >>> print(config.derived_predicates) # doctest: +NORMALIZE_WHITESPACE
         {'death_or_discharge': DerivedPredicateConfig(expr='or(death, discharge)')}
         >>> print(nx.write_network_text(config.predicates_DAG))
         ╟── death
         ╎   └─╼ death_or_discharge ╾ discharge
         ╙── discharge
             └─╼  ...
@@ -735,16 +770,18 @@
         └── input.end
             ├── input.start
             └── gap.end
                 └── target.end
     """
 
     predicates: dict[str, PlainPredicateConfig | DerivedPredicateConfig]
-    trigger_event: EventConfig
+    trigger: EventConfig
     windows: dict[str, WindowConfig]
+    label_window: str | None = None
+    index_timestamp_window: str | None = None
 
     @classmethod
     def load(cls, config_path: str | Path) -> TaskExtractorConfig:
         """Load a configuration file from the given path and return it as a dict.
 
         Args:
             config_path: The path to which a configuration object will be read from in YAML form.
@@ -762,33 +799,33 @@
         if config_path.suffix == ".yaml":
             yaml = ruamel.yaml.YAML(typ="safe", pure=True)
             loaded_dict = yaml.load(config_path.read_text())
         else:
             raise ValueError(f"Only supports reading from '.yaml' files currently. Got {config_path.suffix}")
 
         predicates = loaded_dict.pop("predicates")
-        trigger_event = loaded_dict.pop("trigger_event")
+        trigger = loaded_dict.pop("trigger")
         windows = loaded_dict.pop("windows")
 
         if loaded_dict:
             raise ValueError(f"Unrecognized keys in configuration file: {', '.join(loaded_dict.keys())}")
 
         logger.info("Parsing predicates...")
         predicates = {
             n: DerivedPredicateConfig(**p) if "expr" in p else PlainPredicateConfig(**p)
             for n, p in predicates.items()
         }
 
         logger.info("Parsing trigger event...")
-        trigger_event = EventConfig(trigger_event)
+        trigger = EventConfig(trigger)
 
         logger.info("Parsing windows...")
         windows = {n: WindowConfig(**w) for n, w in windows.items()}
 
-        return cls(predicates=predicates, trigger_event=trigger_event, windows=windows)
+        return cls(predicates=predicates, trigger=trigger, windows=windows)
 
     def save(self, config_path: str | Path, do_overwrite: bool = False):
         """Load a configuration file from the given path and return it as a dict.
 
         Args:
             config_path: The path to which the calling object will be saved in YAML form.
             do_overwrite: Whether or not to overwrite any existing saved configuration file at that filepath.
@@ -867,17 +904,48 @@
 
         for name in self.windows:
             if re.match(r"^\w+$", name) is None:
                 raise ValueError(
                     f"Window name '{name}' is invalid; must be composed of alphanumeric or '_' characters."
                 )
 
-        if self.trigger_event.predicate not in self.predicates:
+        label_windows = []
+        index_timestamp_windows = []
+        for name, window in self.windows.items():
+            if window.label:
+                if window.label not in self.predicates:
+                    raise ValueError(
+                        f"Label must be one of the defined predicates, got: {window.label} "
+                        f"for window '{name}'"
+                    )
+                label_windows.append(name)
+            if window.index_timestamp:
+                if window.index_timestamp not in ["start", "end"]:
+                    raise ValueError(
+                        f"Index timestamp must be either 'start' or 'end', got: {window.index_timestamp} "
+                        f"for window '{name}'"
+                    )
+                index_timestamp_windows.append(name)
+        if len(label_windows) > 1:
+            raise ValueError(
+                f"Only one window can be labeled, found {len(label_windows)} labeled windows: "
+                f"{', '.join(label_windows)}"
+            )
+        self.label_window = label_windows[0] if label_windows else None
+        if len(index_timestamp_windows) > 1:
+            raise ValueError(
+                f"Only the 'start'/'end' of one window can be used as the index timestamp, "
+                f"found {len(index_timestamp_windows)} windows with index_timestamp: "
+                f"{', '.join(index_timestamp_windows)}"
+            )
+        self.index_timestamp_window = index_timestamp_windows[0] if index_timestamp_windows else None
+
+        if self.trigger.predicate not in self.predicates and self.trigger.predicate != ANY_EVENT_COLUMN:
             raise KeyError(
-                f"Trigger event predicate '{self.trigger_event.predicate}' not found in predicates: "
+                f"Trigger event predicate '{self.trigger.predicate}' not found in predicates: "
                 f"{', '.join(self.predicates.keys())}"
             )
 
         trigger_node = Node("trigger")
 
         window_nodes = {"trigger": trigger_node}
         for name, window in self.windows.items():
```

### Comparing `es_aces-0.2.0/src/aces/constraints.py` & `es_aces-0.2.1/src/aces/constraints.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 
 def check_constraints(
     window_constraints: dict[str, tuple[int | None, int | None]], summary_df: pl.DataFrame
 ) -> pl.DataFrame:
     """Checks the constraints on the counts of predicates in the summary dataframe.
 
-    TODO(mmd): integrate this function into the Window object for ease of use.
-
     Args:
         window_constraints: constraints on counts of predicates that must
             be satsified, organized as a dictionary from predicate column name to the lowerbound and upper
             bound range required for that constraint to be satisfied.
         summary_df: A dataframe containing a row for every possible prospective window to be analyzed. The
             only columns expected are predicate columns within the ``window_constraints`` dictionary.
```

### Comparing `es_aces-0.2.0/src/aces/extract_subtree.py` & `es_aces-0.2.1/src/aces/extract_subtree.py`

 * *Files 10% similar despite different names*

```diff
@@ -185,75 +185,74 @@
         ...         .drop(*drop_cols)
         ...     )
         >>> print_window("gap_summary")
         shape: (1, 6)
         ┌─────────────────────┬─────────────────────┬──────────────┬──────────────┬──────────┬─────────────┐
         │ timestamp_at_start  ┆ timestamp_at_end    ┆ is_admission ┆ is_discharge ┆ is_death ┆ is_covid_dx │
         │ ---                 ┆ ---                 ┆ ---          ┆ ---          ┆ ---      ┆ ---         │
-        │ datetime[μs]        ┆ datetime[μs]        ┆ u16          ┆ u16          ┆ u16      ┆ u16         │
+        │ datetime[μs]        ┆ datetime[μs]        ┆ i64          ┆ i64          ┆ i64      ┆ i64         │
         ╞═════════════════════╪═════════════════════╪══════════════╪══════════════╪══════════╪═════════════╡
         │ 1989-12-06 15:17:00 ┆ 1989-12-08 15:17:00 ┆ 1            ┆ 0            ┆ 0        ┆ 0           │
         └─────────────────────┴─────────────────────┴──────────────┴──────────────┴──────────┴─────────────┘
         >>> print_window("target_summary")
         shape: (1, 6)
         ┌─────────────────────┬─────────────────────┬──────────────┬──────────────┬──────────┬─────────────┐
         │ timestamp_at_start  ┆ timestamp_at_end    ┆ is_admission ┆ is_discharge ┆ is_death ┆ is_covid_dx │
         │ ---                 ┆ ---                 ┆ ---          ┆ ---          ┆ ---      ┆ ---         │
-        │ datetime[μs]        ┆ datetime[μs]        ┆ u16          ┆ u16          ┆ u16      ┆ u16         │
+        │ datetime[μs]        ┆ datetime[μs]        ┆ i64          ┆ i64          ┆ i64      ┆ i64         │
         ╞═════════════════════╪═════════════════════╪══════════════╪══════════════╪══════════╪═════════════╡
         │ 1989-12-08 15:17:00 ┆ 1989-12-10 16:22:00 ┆ 0            ┆ 1            ┆ 1        ┆ 0           │
         └─────────────────────┴─────────────────────┴──────────────┴──────────────┴──────────┴─────────────┘
         >>> print_window("input_start_summary")
         shape: (1, 6)
         ┌─────────────────────┬─────────────────────┬──────────────┬──────────────┬──────────┬─────────────┐
         │ timestamp_at_start  ┆ timestamp_at_end    ┆ is_admission ┆ is_discharge ┆ is_death ┆ is_covid_dx │
         │ ---                 ┆ ---                 ┆ ---          ┆ ---          ┆ ---      ┆ ---         │
-        │ datetime[μs]        ┆ datetime[μs]        ┆ u16          ┆ u16          ┆ u16      ┆ u16         │
+        │ datetime[μs]        ┆ datetime[μs]        ┆ i64          ┆ i64          ┆ i64      ┆ i64         │
         ╞═════════════════════╪═════════════════════╪══════════════╪══════════════╪══════════╪═════════════╡
         │ 1983-12-01 22:02:00 ┆ 1989-12-06 15:17:00 ┆ 2            ┆ 1            ┆ 0        ┆ 0           │
         └─────────────────────┴─────────────────────┴──────────────┴──────────────┴──────────┴─────────────┘
         >>> print_window("input_end_summary")
         shape: (1, 6)
         ┌─────────────────────┬─────────────────────┬──────────────┬──────────────┬──────────┬─────────────┐
         │ timestamp_at_start  ┆ timestamp_at_end    ┆ is_admission ┆ is_discharge ┆ is_death ┆ is_covid_dx │
         │ ---                 ┆ ---                 ┆ ---          ┆ ---          ┆ ---      ┆ ---         │
-        │ datetime[μs]        ┆ datetime[μs]        ┆ u16          ┆ u16          ┆ u16      ┆ u16         │
+        │ datetime[μs]        ┆ datetime[μs]        ┆ i64          ┆ i64          ┆ i64      ┆ i64         │
         ╞═════════════════════╪═════════════════════╪══════════════╪══════════════╪══════════╪═════════════╡
         │ 1989-12-06 15:17:00 ┆ 1989-12-07 15:17:00 ┆ 1            ┆ 0            ┆ 0        ┆ 0           │
         └─────────────────────┴─────────────────────┴──────────────┴──────────────┴──────────┴─────────────┘
         >>> print_window("pre_node_1yr_summary")
         shape: (1, 6)
         ┌─────────────────────┬─────────────────────┬──────────────┬──────────────┬──────────┬─────────────┐
         │ timestamp_at_start  ┆ timestamp_at_end    ┆ is_admission ┆ is_discharge ┆ is_death ┆ is_covid_dx │
         │ ---                 ┆ ---                 ┆ ---          ┆ ---          ┆ ---      ┆ ---         │
-        │ datetime[μs]        ┆ datetime[μs]        ┆ u16          ┆ u16          ┆ u16      ┆ u16         │
+        │ datetime[μs]        ┆ datetime[μs]        ┆ i64          ┆ i64          ┆ i64      ┆ i64         │
         ╞═════════════════════╪═════════════════════╪══════════════╪══════════════╪══════════╪═════════════╡
         │ 1989-12-06 15:17:00 ┆ 1988-12-06 15:17:00 ┆ 0            ┆ 0            ┆ 0        ┆ 0           │
         └─────────────────────┴─────────────────────┴──────────────┴──────────────┴──────────┴─────────────┘
         >>> print_window("pre_node_total_summary")
         shape: (1, 6)
         ┌─────────────────────┬─────────────────────┬──────────────┬──────────────┬──────────┬─────────────┐
         │ timestamp_at_start  ┆ timestamp_at_end    ┆ is_admission ┆ is_discharge ┆ is_death ┆ is_covid_dx │
         │ ---                 ┆ ---                 ┆ ---          ┆ ---          ┆ ---      ┆ ---         │
-        │ datetime[μs]        ┆ datetime[μs]        ┆ u16          ┆ u16          ┆ u16      ┆ u16         │
+        │ datetime[μs]        ┆ datetime[μs]        ┆ i64          ┆ i64          ┆ i64      ┆ i64         │
         ╞═════════════════════╪═════════════════════╪══════════════╪══════════════╪══════════╪═════════════╡
         │ 1983-12-01 22:02:00 ┆ 1988-12-06 15:17:00 ┆ 1            ┆ 1            ┆ 0        ┆ 0           │
         └─────────────────────┴─────────────────────┴──────────────┴──────────────┴──────────┴─────────────┘
     """
     recursive_results = []
     predicate_cols = [c for c in predicates_df.columns if c not in {"subject_id", "timestamp"}]
 
     if not subtree.children:
         return subtree_anchor_realizations
 
     for child in subtree.children:
         logger.info(f"Summarizing subtree rooted at '{child.name}'...")
 
         # Step 1: Summarize the window from the subtree.root to child
-        # TODO(mmd): Make this more object oriented using the dataclasses.
         endpoint_expr = child.endpoint_expr
         if type(endpoint_expr) is tuple:
             endpoint_expr = endpoint_expr + (subtree_root_offset,)
         else:
             endpoint_expr.offset += subtree_root_offset
 
         match endpoint_expr[1]:
```

### Comparing `es_aces-0.2.0/src/aces/types.py` & `es_aces-0.2.1/src/aces/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import dataclasses
 from datetime import timedelta
 
 import polars as pl
 
 # The type used for final aggregate counts of predicates.
-PRED_CNT_TYPE = pl.UInt16
+PRED_CNT_TYPE = pl.Int64
 
 # The key used in the endpoint expression to indicate the window should be aggregated to the record start.
 START_OF_RECORD_KEY = "_RECORD_START"
 END_OF_RECORD_KEY = "_RECORD_END"
 
 # The key used to capture the count of events of any kind that occur in a window.
 ANY_EVENT_COLUMN = "_ANY_EVENT"
```

### Comparing `es_aces-0.2.0/src/aces/utils.py` & `es_aces-0.2.1/src/aces/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,9 +48,10 @@
     finally:
         sys.stdout = old_out  # Restore the original stdout
 
 
 def log_tree(node):
     """Logs the tree structure using logging.info."""
     with capture_output() as captured:
+        print("\n")
         print_tree(node, style="const_bold")  # This will print to the captured StringIO instead of stdout
     logger.info(captured.getvalue())  # Log the captured output
```

