# Comparing `tmp/openfisca_france_data-3.3.1.tar.gz` & `tmp/openfisca_france_data-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfisca_france_data-3.3.1.tar", last modified: Wed May 22 15:10:32 2024, max compression
+gzip compressed data, was "openfisca_france_data-3.4.0.tar", last modified: Thu May 30 14:29:11 2024, max compression
```

## Comparing `openfisca_france_data-3.3.1.tar` & `openfisca_france_data-3.4.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.008922 openfisca_france_data-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.008922 openfisca_france_data-3.3.1/OpenFisca_France_Data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-22 15:10:31.000000 openfisca_france_data-3.3.1/OpenFisca_France_Data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-22 15:10:31.000000 openfisca_france_data-3.3.1/OpenFisca_France_Data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:10:31.000000 openfisca_france_data-3.3.1/OpenFisca_France_Data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-22 15:10:31.000000 openfisca_france_data-3.3.1/OpenFisca_France_Data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-22 15:10:31.000000 openfisca_france_data-3.3.1/OpenFisca_France_Data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 15:10:31.000000 openfisca_france_data-3.3.1/OpenFisca_France_Data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-22 15:10:32.008922 openfisca_france_data-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.996922 openfisca_france_data-3.3.1/openfisca_france_data/
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.996922 openfisca_france_data-3.3.1/openfisca_france_data/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.988922 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.996922 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.996922 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/ines/
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/ines/ines_2019.json
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/ines/ines_2020.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.996922 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/taxipp/
--rw-r--r--   0 runner    (1001) docker     (127)    12991 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.996922 openfisca_france_data-3.3.1/openfisca_france_data/assets/zone_apl_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/zone_apl_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.996922 openfisca_france_data-3.3.1/openfisca_france_data/assets/zone_apl_data/zone_apl/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/base_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)    22091 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    24951 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.988922 openfisca_france_data-3.3.1/openfisca_france_data/dads/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.996922 openfisca_france_data-3.3.1/openfisca_france_data/dads/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/dads/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.996922 openfisca_france_data-3.3.1/openfisca_france_data/erfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.000922 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/run_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
--rw-r--r--   0 runner    (1001) docker     (127)    26165 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36615 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
--rw-r--r--   0 runner    (1001) docker     (127)    13155 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_08_final.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.000922 openfisca_france_data-3.3.1/openfisca_france_data/erfs/old/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/old/aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/old/datatable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.000922 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/get_survey_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.000922 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15394 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    25444 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
--rw-r--r--   0 runner    (1001) docker     (127)    51170 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
--rw-r--r--   0 runner    (1001) docker     (127)    35145 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/test_case_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.000922 openfisca_france_data-3.3.1/openfisca_france_data/felin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/felin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.000922 openfisca_france_data-3.3.1/openfisca_france_data/felin/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/felin/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.000922 openfisca_france_data-3.3.1/openfisca_france_data/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/model/calage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/model/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/model/id_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/model/survey_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.000922 openfisca_france_data-3.3.1/openfisca_france_data/reforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/inversion_directe_salaires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.004922 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.004922 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/allocations_familiales_imposables.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/cesthra_invalidite.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2015.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2016.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/trannoy_wasmer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.004922 openfisca_france_data-3.3.1/openfisca_france_data/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/scripts/build_input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/smic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/openfisca_france_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-22 15:10:32.008922 openfisca_france_data-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.004922 openfisca_france_data-3.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:31.992922 openfisca_france_data-3.3.1/tests/erfs_fpr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.008922 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_af.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_al.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_create_salaire_de_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_impot_revenu.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_inflation.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_input_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_rebuild_input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_salaire_imposable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:10:32.008922 openfisca_france_data-3.3.1/tests/erfs_fpr/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/unit/test_get_survey_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/erfs_fpr/unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/test_fake_survey_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/test_get_baremes_salarie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/test_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-22 15:10:14.000000 openfisca_france_data-3.3.1/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.011625 openfisca_france_data-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.011625 openfisca_france_data-3.4.0/OpenFisca_France_Data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-30 14:29:10.000000 openfisca_france_data-3.4.0/OpenFisca_France_Data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-30 14:29:10.000000 openfisca_france_data-3.4.0/OpenFisca_France_Data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:29:10.000000 openfisca_france_data-3.4.0/OpenFisca_France_Data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-30 14:29:10.000000 openfisca_france_data-3.4.0/OpenFisca_France_Data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-30 14:29:10.000000 openfisca_france_data-3.4.0/OpenFisca_France_Data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 14:29:10.000000 openfisca_france_data-3.4.0/OpenFisca_France_Data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-30 14:29:11.011625 openfisca_france_data-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.999625 openfisca_france_data-3.4.0/openfisca_france_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.999625 openfisca_france_data-3.4.0/openfisca_france_data/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.995625 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.999625 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.999625 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/ines/
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/ines/ines_2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/ines/ines_2020.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.999625 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/taxipp/
+-rw-r--r--   0 runner    (1001) docker     (127)    12991 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.999625 openfisca_france_data-3.4.0/openfisca_france_data/assets/zone_apl_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/zone_apl_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.999625 openfisca_france_data-3.4.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/base_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23702 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24951 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.995625 openfisca_france_data-3.4.0/openfisca_france_data/dads/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.999625 openfisca_france_data-3.4.0/openfisca_france_data/dads/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/dads/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.999625 openfisca_france_data-3.4.0/openfisca_france_data/erfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.003625 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26165 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36615 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13155 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.003625 openfisca_france_data-3.4.0/openfisca_france_data/erfs/old/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/old/aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/old/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.003625 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.003625 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15394 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25444 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51170 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35145 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/test_case_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.003625 openfisca_france_data-3.4.0/openfisca_france_data/felin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/felin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.003625 openfisca_france_data-3.4.0/openfisca_france_data/felin/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/felin/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.007625 openfisca_france_data-3.4.0/openfisca_france_data/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/model/calage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/model/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/model/id_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/model/survey_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.007625 openfisca_france_data-3.4.0/openfisca_france_data/reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/inversion_directe_salaires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.007625 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.007625 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/allocations_familiales_imposables.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/cesthra_invalidite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2015.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2016.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/trannoy_wasmer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.007625 openfisca_france_data-3.4.0/openfisca_france_data/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/scripts/build_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/smic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/openfisca_france_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-30 14:29:11.015625 openfisca_france_data-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.007625 openfisca_france_data-3.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:10.995625 openfisca_france_data-3.4.0/tests/erfs_fpr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.011625 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_af.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_al.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_impot_revenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_input_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_salaire_imposable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:11.011625 openfisca_france_data-3.4.0/tests/erfs_fpr/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/erfs_fpr/unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/test_fake_survey_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/test_get_baremes_salarie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/test_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-30 14:28:54.000000 openfisca_france_data-3.4.0/tests/test_misc.py
```

### Comparing `openfisca_france_data-3.3.1/CHANGELOG.md` & `openfisca_france_data-3.4.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+### 3.4.0 [#252](https://github.com/openfisca/openfisca-france-data/pull/252)
+
+* New features
+  - Rend l'inversion plus robuste pour permettre de la faire de manière mois par mois
+  - En particulier, donne un seuil d'exonération sur le chômage net dépendant de la période.
+  - Ajoute dans l'inversion la prise en compte de l'indemnité compensatrice de csg
+
 ### 3.3.1 [#256](https://github.com/openfisca/openfisca-france-data/pull/256)
 
 * Technical changes
   - Met à jour la version d'Openfisca France dans les dépendances
 
 
 ### 3.3.0 [#251](https://github.com/openfisca/openfisca-france-data/pull/251)
```

### Comparing `openfisca_france_data-3.3.1/CONTRIBUTING.md` & `openfisca_france_data-3.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/LICENSE` & `openfisca_france_data-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/OpenFisca_France_Data.egg-info/PKG-INFO` & `openfisca_france_data-3.4.0/OpenFisca_France_Data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 3.3.1
+Version: 3.4.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `openfisca_france_data-3.3.1/OpenFisca_France_Data.egg-info/SOURCES.txt` & `openfisca_france_data-3.4.0/OpenFisca_France_Data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/PKG-INFO` & `openfisca_france_data-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 3.3.1
+Version: 3.4.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `openfisca_france_data-3.3.1/README.md` & `openfisca_france_data-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/__init__.py` & `openfisca_france_data-3.4.0/openfisca_france_data/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/aggregates.py` & `openfisca_france_data-3.4.0/openfisca_france_data/aggregates.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json` & `openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json` & `openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json` & `openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json` & `openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json` & `openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json` & `openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/ines/ines_2019.json` & `openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/ines/ines_2019.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/ines/ines_2020.json` & `openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/ines/ines_2020.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx` & `openfisca_france_data-3.4.0/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py` & `openfisca_france_data-3.4.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/base_survey.py` & `openfisca_france_data-3.4.0/openfisca_france_data/base_survey.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/common.py` & `openfisca_france_data-3.4.0/openfisca_france_data/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import numpy as np
 import logging
 
 from openfisca_core import periods
+from openfisca_core.periods.date_unit import DateUnit
 from openfisca_core.taxscales import MarginalRateTaxScale, combine_tax_scales
 from openfisca_core.formula_helpers import switch
 from openfisca_france.model.base import TypesCategorieSalarie, TAUX_DE_PRIME
 from openfisca_france.model.prelevements_obligatoires.prelevements_sociaux.cotisations_sociales.base import (
     cotisations_salarie_by_categorie_salarie,
     )
 from openfisca_france_data.smic import smic_horaire_brut
+from openfisca_france_data import openfisca_france_tax_benefit_system
 
 
 log = logging.getLogger(__name__)
 
 
 def get_baremes_salarie(parameters, categorie_salarie, period, exclude_alsace_moselle = True):
     assert categorie_salarie in [
@@ -54,41 +56,41 @@
     salarie = parameters.cotsoc.cotisations_salarie
     plafond_securite_sociale_mensuel = parameters.prelevements_sociaux.pss.plafond_securite_sociale_mensuel
     parameters_csg_deductible = parameters.prelevements_sociaux.contributions_sociales.csg.activite.deductible
     taux_csg = parameters_csg_deductible.taux
     taux_abattement = parameters_csg_deductible.abattement.rates[0]
     try:
         seuil_abattement = parameters_csg_deductible.abattement.thresholds[1]
-    except IndexError:  # Pour gérer le fait que l'abattement n'a pas toujours était limité à 4 PSS
+    except IndexError:  # Pour gérer le fait que l'abattement n'a pas toujours été limité à 4 PSS
         seuil_abattement = None
     csg_deductible = MarginalRateTaxScale(name = 'csg_deductible')
     csg_deductible.add_bracket(0, taux_csg * (1 - taux_abattement))
     if seuil_abattement is not None:
         csg_deductible.add_bracket(seuil_abattement, taux_csg)
 
     if revenu_type == 'net':  # On ajoute CSG imposable et crds
 
         parameters_csg_imposable = parameters.prelevements_sociaux.contributions_sociales.csg.activite.imposable
         taux_csg = parameters_csg_imposable.taux
         taux_abattement = parameters_csg_imposable.abattement.rates[0]
         try:
             seuil_abattement = parameters_csg_imposable.abattement.thresholds[1]
-        except IndexError:  # Pour gérer le fait que l'abattement n'a pas toujours était limité à 4 PSS
+        except IndexError:  # Pour gérer le fait que l'abattement n'a pas toujours été limité à 4 PSS
             seuil_abattement = None
         csg_imposable = MarginalRateTaxScale(name = 'csg_imposable')
         csg_imposable.add_bracket(0, taux_csg * (1 - taux_abattement))
         if seuil_abattement is not None:
             csg_imposable.add_bracket(seuil_abattement, taux_csg)
 
         parameters_crds = parameters.prelevements_sociaux.contributions_sociales.crds.activite
         taux_csg = parameters_crds.taux
         taux_abattement = parameters_crds.abattement.rates[0]
         try:
             seuil_abattement = parameters_crds.abattement.thresholds[1]
-        except IndexError:  # Pour gérer le fait que l'abattement n'a pas toujours était limité à 4 PSS
+        except IndexError:  # Pour gérer le fait que l'abattement n'a pas toujours été limité à 4 PSS
             seuil_abattement = None
         crds = MarginalRateTaxScale(name = 'crds')
         crds.add_bracket(0, taux_csg * (1 - taux_abattement))
         if seuil_abattement is not None:
             crds.add_bracket(seuil_abattement, taux_csg)
 
     # Check baremes
@@ -117,21 +119,21 @@
     del bareme
 
     # On ajoute la CSG deductible et on proratise par le plafond de la sécurité sociale
     # Pour éviter les divisions 0 /0 dans le switch qui sert à calculer le salaire_pour_inversion_proratise
     whours = parameters.marche_travail.salaire_minimum.smic.nb_heures_travail_mensuel
 
     if period.unit == 'year':
-        plafond_securite_sociale = plafond_securite_sociale_mensuel * 12
-        heures_temps_plein = whours * 12
+        nb_mois = 12
     elif period.unit == 'month':
-        plafond_securite_sociale = plafond_securite_sociale_mensuel * period.size
-        heures_temps_plein = whours * period.size
+        nb_mois = period.size
     else:
         raise
+    plafond_securite_sociale = plafond_securite_sociale_mensuel * nb_mois
+    heures_temps_plein = whours * nb_mois
 
     if revenu_type == 'imposable':
         salaire_pour_inversion = individus.salaire_imposable
     else:
         salaire_pour_inversion = individus.salaire_net
 
     categorie_salarie = individus.categorie_salarie
@@ -147,28 +149,34 @@
             # temps partiel
             1: salaire_pour_inversion / (
                 (heures_remunerees_volume_avoid_warning / heures_temps_plein) * plafond_securite_sociale
                 ),
             }
         )
 
-    def add_agirc_gmp_to_agirc(agirc, parameters):
-        plafond_securite_sociale_annuel = parameters.prelevements_sociaux.pss.plafond_securite_sociale_mensuel * 12
-        salaire_charniere = parameters.prelevements_sociaux.regimes_complementaires_retraite_secteur_prive.gmp.salaire_charniere_annuel / plafond_securite_sociale_annuel
-        cotisation = parameters.prelevements_sociaux.regimes_complementaires_retraite_secteur_prive.gmp.cotisation_forfaitaire_mensuelle.part_salariale * 12
-        n = (cotisation + 1) * 12
-        agirc.add_bracket(n / plafond_securite_sociale_annuel, 0)
+    def add_agirc_gmp_to_agirc(agirc, parameters, period):
+        if period.unit == 'year':
+            nb_mois = 12
+        elif period.unit == 'month':
+            nb_mois = period.size
+        else:
+            raise
+        plafond_securite_sociale = plafond_securite_sociale_mensuel * nb_mois
+        salaire_charniere = parameters.prelevements_sociaux.regimes_complementaires_retraite_secteur_prive.gmp.salaire_charniere_annuel * (nb_mois / 12) / plafond_securite_sociale
+        cotisation = parameters.prelevements_sociaux.regimes_complementaires_retraite_secteur_prive.gmp.cotisation_forfaitaire_mensuelle.part_salariale * nb_mois
+        n = (cotisation + 1) * 12 # pour permettre la mensualisation en cas d'inversion, en évitant un taux 12 fois plus élevé sur une tranche 12 fois plus étroite
+        agirc.add_bracket(n / plafond_securite_sociale, 0)
         agirc.rates[0] = cotisation / n
         agirc.thresholds[2] = salaire_charniere
 
     salaire_de_base = 0.0
     for categorie in ['prive_non_cadre', 'prive_cadre', 'public_non_titulaire']:
         if categorie == 'prive_cadre' and "agirc" in salarie[categorie]._children:
             print("adding GMP")
-            add_agirc_gmp_to_agirc(salarie[categorie].agirc, parameters)
+            add_agirc_gmp_to_agirc(salarie[categorie].agirc, parameters, period)
 
         bareme = combine_tax_scales(salarie[categorie])
         bareme.add_tax_scale(csg_deductible)
         if revenu_type == 'net':
             bareme.add_tax_scale(csg_imposable)
             bareme.add_tax_scale(crds)
 
@@ -205,15 +213,15 @@
             'salaire_de_base'
             ] = np.maximum(salaire_de_base, smic_horaire_brut[year] * heures_remunerees_volume)
 
 
 def create_traitement_indiciaire_brut(individus, period = None, revenu_type = 'imposable',
             tax_benefit_system = None):
     """
-    Calcule le tratement indiciaire brut à partir du salaire imposable ou du salaire net.
+    Calcule le traitement indiciaire brut à partir du salaire imposable ou du salaire net.
     Note : le supplément familial de traitement est imposable. Pas géré
     """
     assert period is not None
     assert revenu_type in ['net', 'imposable']
     assert tax_benefit_system is not None
 
     for variable in ['categorie_salarie', 'contrat_de_travail', 'heures_remunerees_volume']:
@@ -380,47 +388,67 @@
             {
                 # temps plein
                 0: brut_proratise,
                 # temps partiel
                 1: brut_proratise * (heures_remunerees_volume / (heures_temps_plein)),
                 }
             )
-        traitement_indiciaire_brut += (
-            (categorie_salarie == TypesCategorieSalarie[categorie].index) * brut
-            )
+
+        if period.start.year>2017:traitement_indiciaire_brut += (
+                (categorie_salarie == TypesCategorieSalarie[categorie].index) * brut / (1 + 0.0076)
+                ) # Prise en compte de l'indemnité compensatrice de csg, qui sera recalculée. Non prise en compte des exonérations de cotisation sur cette indemnité
+        else:
+            traitement_indiciaire_brut += (
+                (categorie_salarie == TypesCategorieSalarie[categorie].index) * brut
+                )
         if (categorie_salarie == TypesCategorieSalarie[categorie].index).any():
             log.debug("Pour {} : brut = {}".format(TypesCategorieSalarie[categorie].index, brut))
             log.debug('bareme direct: {}'.format(bareme))
 
     individus['traitement_indiciaire_brut'] = traitement_indiciaire_brut
     individus['primes_fonction_publique'] = TAUX_DE_PRIME * traitement_indiciaire_brut
 
 
-def create_revenus_remplacement_bruts(individus, period, tax_benefit_system):
+def create_revenus_remplacement_bruts(individus, period, tax_benefit_system, revenu_type = 'net'):
     assert 'taux_csg_remplacement' in individus
 
     individus.chomage_imposable.fillna(0, inplace = True)
     individus.retraite_imposable.fillna(0, inplace = True)
-    individus.salaire_net.fillna(0, inplace = True)
+    if revenu_type == 'imposable':
+        assert 'salaire_imposable' in individus.columns
+        salaire_pour_inversion = individus.salaire_imposable
+    elif revenu_type == 'net':
+        assert 'salaire_net' in individus.columns
+        salaire_pour_inversion = individus.salaire_net
+    else :
+        raise Exception("revenu_type not implemented")
+    salaire_pour_inversion.fillna(0, inplace = True)
 
     parameters = tax_benefit_system.get_parameters_at_instant(period.start)
     csg = parameters.prelevements_sociaux.contributions_sociales.csg
     csg_deductible_chomage = csg.remplacement.allocations_chomage.deductible
     pss = parameters.prelevements_sociaux.pss.plafond_securite_sociale_annuel
     taux_abattement_csg_chomage = parameters.prelevements_sociaux.contributions_sociales.csg.remplacement.allocations_chomage.deductible.abattement.rates[0]
     seuil_abattement_csg_chomage = parameters.prelevements_sociaux.contributions_sociales.csg.remplacement.allocations_chomage.deductible.abattement.thresholds[1]
     taux_plein = csg_deductible_chomage.taux_plein
     taux_reduit = csg_deductible_chomage.taux_reduit
+    liste_smic_mensuel = []
+    for month in period.get_subperiods(DateUnit.MONTH):
+        smic_horaire_mois = openfisca_france_tax_benefit_system.parameters.marche_travail.salaire_minimum.smic.smic_b_horaire(month)
+        nb_heures_mois = openfisca_france_tax_benefit_system.parameters.marche_travail.salaire_minimum.smic.nb_heures_travail_mensuel(month)
+        smic_mensuel = smic_horaire_mois * nb_heures_mois
+        liste_smic_mensuel.append(smic_mensuel)
+
     seuil_chomage_net_exoneration = (
-        (35 * 52) * smic_horaire_brut[period.start.year]
+        sum(liste_smic_mensuel)
         * (
             (individus.taux_csg_remplacement == 2) / (1 - taux_reduit)
             + (individus.taux_csg_remplacement >= 3) / (1 - taux_plein)
             )
-        ) - individus.salaire_net
+        ) - salaire_pour_inversion # théoriquement, il s'agit du net pour salaire et rpns, mais il n'est pas toujours disponible en pratique
     exonere_csg_chomage = (
         (individus.taux_csg_remplacement < 2)
         | (individus.chomage_imposable <= seuil_chomage_net_exoneration)
         )
     taux_csg_chomage = np.where(
         individus.taux_csg_remplacement < 2,
         0,
```

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/comparator.py` & `openfisca_france_data-3.4.0/openfisca_france_data/comparator.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/config.py` & `openfisca_france_data-3.4.0/openfisca_france_data/config.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py` & `openfisca_france_data-3.4.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,12 +43,12 @@
     create_traitement_indiciaire_brut(individus, period = period, revenu_type = revenu_type, tax_benefit_system = tax_benefit_system)
     created_variables.append('traitement_indiciaire_brut')
     created_variables.append('primes_fonction_publique')
 
     create_taux_csg_remplacement(individus, period, tax_benefit_system)
     created_variables.append('taux_csg_remplacement')
 
-    create_revenus_remplacement_bruts(individus, period, tax_benefit_system)
+    create_revenus_remplacement_bruts(individus, period, tax_benefit_system, revenu_type = revenu_type)
     created_variables.append('chomage_brut')
     created_variables.append('retraite_brute')
 
     return created_variables
```

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/__init__.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/__init__.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/base.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/base.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/run_all.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/run_all.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_03_fip.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_04_famille.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_08_final.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/old/aggregates.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/old/aggregates.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/old/datatable.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/old/datatable.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs/scenario.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs/scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/comparison.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/comparison.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/get_survey_scenario.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/scenario.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/erfs_fpr/test_case_creation.py` & `openfisca_france_data-3.4.0/openfisca_france_data/erfs_fpr/test_case_creation.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py` & `openfisca_france_data-3.4.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/model/base.py` & `openfisca_france_data-3.4.0/openfisca_france_data/model/base.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/model/calage.py` & `openfisca_france_data-3.4.0/openfisca_france_data/model/calage.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/model/common.py` & `openfisca_france_data-3.4.0/openfisca_france_data/model/common.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/model/id_variables.py` & `openfisca_france_data-3.4.0/openfisca_france_data/model/id_variables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/model/survey_variables.py` & `openfisca_france_data-3.4.0/openfisca_france_data/model/survey_variables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/inversion_directe_salaires.py` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/inversion_directe_salaires.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py` & `openfisca_france_data-3.4.0/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/scripts/build_input_data.py` & `openfisca_france_data-3.4.0/openfisca_france_data/scripts/build_input_data.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/smic.py` & `openfisca_france_data-3.4.0/openfisca_france_data/smic.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/surveys.py` & `openfisca_france_data-3.4.0/openfisca_france_data/surveys.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/openfisca_france_data/utils.py` & `openfisca_france_data-3.4.0/openfisca_france_data/utils.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/setup.cfg` & `openfisca_france_data-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/setup.py` & `openfisca_france_data-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name = "OpenFisca-France-Data",
-    version = "3.3.1",
+    version = "3.4.0",
     description = "OpenFisca-France-Data module to work with French survey data",
     long_description = long_description,
     long_description_content_type="text/markdown",
     author = "OpenFisca Team",
     author_email = "contact@openfisca.fr",
     url = "https://github.com/openfisca/openfisca-france-data",
     license = "http://www.fsf.org/licensing/licenses/agpl-3.0.html",
```

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_af.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_af.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_aggregates.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_al.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_al.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_create_salaire_de_base.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_impot_revenu.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_impot_revenu.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_inflation.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_inflation.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_input_variables.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_input_variables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_pivot_table.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_pivot_table.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_rebuild_input_data.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_rebuild_input_data.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_rsa.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_rsa.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/integration/test_salaire_imposable.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/integration/test_salaire_imposable.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/erfs_fpr/unit/test_get_survey_scenario.py` & `openfisca_france_data-3.4.0/tests/erfs_fpr/unit/test_get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/test_aggregate.py` & `openfisca_france_data-3.4.0/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/test_calibration.py` & `openfisca_france_data-3.4.0/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/test_fake_survey_simulation.py` & `openfisca_france_data-3.4.0/tests/test_fake_survey_simulation.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/test_get_baremes_salarie.py` & `openfisca_france_data-3.4.0/tests/test_get_baremes_salarie.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.3.1/tests/test_inversion.py` & `openfisca_france_data-3.4.0/tests/test_inversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 with open(path) as yaml:
     individus = pd.DataFrame.from_dict(load(yaml, Loader=SafeLoader))
 
 # Inverse incomes from net to gross : the tested functions
 
 create_taux_csg_remplacement(individus, period(year), tax_benefit_system)
-create_revenus_remplacement_bruts(individus, period(year), tax_benefit_system)
+create_revenus_remplacement_bruts(individus, period(year), tax_benefit_system, revenu_type = 'net')
 
 # Test against chomage_brut_test
 
 fails_chomage = [i for i in individus.index if abs(individus.loc[i]["chomage_brut"]-individus.loc[i]["chomage_brut_test"])>=margin]
 fails_retraite = [i for i in individus.index if abs(individus.loc[i]["retraite_brute"]-individus.loc[i]["retraite_brute_test"])>=margin]
 
 message = "".join(
```

### Comparing `openfisca_france_data-3.3.1/tests/test_misc.py` & `openfisca_france_data-3.4.0/tests/test_misc.py`

 * *Files identical despite different names*

