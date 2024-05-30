# Comparing `tmp/cumulus_library_data_metrics-1.0.0.tar.gz` & `tmp/cumulus_library_data_metrics-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library_data_metrics-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library_data_metrics-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library_data_metrics-1.0.0.tar` & `cumulus_library_data_metrics-2.0.0.tar`

### file list

```diff
@@ -1,278 +1,284 @@
--rw-r--r--   0        0        0    11357 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/LICENSE
--rw-r--r--   0        0        0     3362 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/README.md
--rw-r--r--   0        0        0       68 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/__init__.py
--rw-r--r--   0        0        0     3332 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/base.py
--rw-r--r--   0        0        0     1434 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/base.summary.jinja
--rw-r--r--   0        0        0      899 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/README.md
--rw-r--r--   0        0        0     1113 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.jinja
--rw-r--r--   0        0        0      909 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.py
--rw-r--r--   0        0        0      308 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_deceased_count/README.md
--rw-r--r--   0        0        0     1861 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.jinja
--rw-r--r--   0        0        0      550 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.py
--rw-r--r--   0        0        0      265 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resource_count/README.md
--rw-r--r--   0        0        0     1099 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resource_count/c_resource_count.jinja
--rw-r--r--   0        0        0     1068 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resource_count/c_resource_count.py
--rw-r--r--   0        0        0      347 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resources_per_pt/README.md
--rw-r--r--   0        0        0     2545 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.jinja
--rw-r--r--   0        0        0      929 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.py
--rw-r--r--   0        0        0     1057 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/README.md
--rw-r--r--   0        0        0     2083 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/c_term_coverage.jinja
--rw-r--r--   0        0        0     2205 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/c_term_coverage.py
--rw-r--r--   0        0        0     2075 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_us_core_v4_count/README.md
--rw-r--r--   0        0        0     1595 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_us_core_v4_count/c_us_core_v4_count.jinja
--rw-r--r--   0        0        0      433 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_us_core_v4_count/c_us_core_v4_count.py
--rw-r--r--   0        0        0     3647 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/manifest.toml
--rw-r--r--   0        0        0     1078 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/meta/dates.jinja
--rw-r--r--   0        0        0      735 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/meta/meta.py
--rw-r--r--   0        0        0       77 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/meta/version.jinja
--rw-r--r--   0        0        0      904 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/README.md
--rw-r--r--   0        0        0     1234 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.jinja
--rw-r--r--   0        0        0      812 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.py
--rw-r--r--   0        0        0     1420 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_pop/README.md
--rw-r--r--   0        0        0      374 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_pop/q_ref_target_pop.jinja
--rw-r--r--   0        0        0     1531 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_pop/q_ref_target_pop.py
--rw-r--r--   0        0        0     1195 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/README.md
--rw-r--r--   0        0        0      504 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/denominator.jinja
--rw-r--r--   0        0        0      991 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.jinja
--rw-r--r--   0        0        0     2581 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.py
--rw-r--r--   0        0        0      736 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/README.md
--rw-r--r--   0        0        0      947 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/q_term_use.jinja
--rw-r--r--   0        0        0     3235 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/q_term_use.py
--rw-r--r--   0        0        0     3587 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/README.md
--rw-r--r--   0        0        0      738 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.jinja
--rw-r--r--   0        0        0      688 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.py
--rw-r--r--   0        0        0     2509 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/resource_info.py
--rw-r--r--   0        0        0     2046 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/systems.py
--rw-r--r--   0        0        0      105 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/t_us_core_v4/README.md
--rw-r--r--   0        0        0      182 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/t_us_core_v4/mandatory.jinja
--rw-r--r--   0        0        0      225 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/t_us_core_v4/must_support.jinja
--rw-r--r--   0        0        0      815 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/t_us_core_v4/t_us_core_v4.py
--rw-r--r--   0        0        0      345 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/README.md
--rw-r--r--   0        0        0       50 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/__init__.py
--rw-r--r--   0        0        0     2453 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_mandatory.jinja
--rw-r--r--   0        0        0     2666 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_must_support.jinja
--rw-r--r--   0        0        0     2603 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/condition_mandatory.jinja
--rw-r--r--   0        0        0     1414 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/condition_must_support.jinja
--rw-r--r--   0        0        0     1180 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_mandatory.jinja
--rw-r--r--   0        0        0      763 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_must_support.jinja
--rw-r--r--   0        0        0     2129 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_mandatory.jinja
--rw-r--r--   0        0        0     2945 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_must_support.jinja
--rw-r--r--   0        0        0      834 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/encounter_mandatory.jinja
--rw-r--r--   0        0        0     1503 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/encounter_must_support.jinja
--rw-r--r--   0        0        0      954 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/immunization_mandatory.jinja
--rw-r--r--   0        0        0      570 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/immunization_must_support.jinja
--rw-r--r--   0        0        0      356 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medication_mandatory.jinja
--rw-r--r--   0        0        0      129 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medication_must_support.jinja
--rw-r--r--   0        0        0     1322 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_mandatory.jinja
--rw-r--r--   0        0        0     1018 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_must_support.jinja
--rw-r--r--   0        0        0      316 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_blood_pressure_mandatory.jinja
--rw-r--r--   0        0        0     2291 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_mandatory.jinja
--rw-r--r--   0        0        0     1024 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_must_support.jinja
--rw-r--r--   0        0        0     1974 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_smoking_status_mandatory.jinja
--rw-r--r--   0        0        0      190 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_smoking_status_must_support.jinja
--rw-r--r--   0        0        0     3804 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_utils.jinja
--rw-r--r--   0        0        0     4855 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_mandatory.jinja
--rw-r--r--   0        0        0     1032 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_must_support.jinja
--rw-r--r--   0        0        0      619 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_mandatory.jinja
--rw-r--r--   0        0        0     2503 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_must_support.jinja
--rw-r--r--   0        0        0     5242 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_utils.jinja
--rw-r--r--   0        0        0     1004 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/procedure_mandatory.jinja
--rw-r--r--   0        0        0      128 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/procedure_must_support.jinja
--rw-r--r--   0        0        0     3546 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/profiles.py
--rw-r--r--   0        0        0      398 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/slice.jinja
--rw-r--r--   0        0        0     9285 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/utils.jinja
--rw-r--r--   0        0        0     1599 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     9018 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/cubed/expected.csv
--rw-r--r--   0        0        0     3065 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/cubed/patient/0.ndjson
--rw-r--r--   0        0        0      679 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/general/expected.csv
--rw-r--r--   0        0        0     3065 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/general/patient/0.ndjson
--rw-r--r--   0        0        0      122 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/no-ext/expected.csv
--rw-r--r--   0        0        0       33 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/no-ext/patient/0.ndjson
--rw-r--r--   0        0        0      269 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_deceased_count/general/expected.csv
--rw-r--r--   0        0        0      786 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_deceased_count/general/patient/0.ndjson
--rw-r--r--   0        0        0     1334 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0     1978 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/condition/0.ndjson
--rw-r--r--   0        0        0       24 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/device/0.ndjson
--rw-r--r--   0        0        0      494 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0      593 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/documentreference/0.ndjson
--rw-r--r--   0        0        0      603 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/encounter/0.ndjson
--rw-r--r--   0        0        0      417 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_allergyintolerance_month.csv
--rw-r--r--   0        0        0      375 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_allergyintolerance_year.csv
--rw-r--r--   0        0        0      456 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_condition_month.csv
--rw-r--r--   0        0        0      354 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_condition_year.csv
--rw-r--r--   0        0        0       27 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_device_all.csv
--rw-r--r--   0        0        0      200 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_diagnosticreport_month.csv
--rw-r--r--   0        0        0      190 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_diagnosticreport_year.csv
--rw-r--r--   0        0        0      225 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_documentreference_month.csv
--rw-r--r--   0        0        0      215 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_documentreference_year.csv
--rw-r--r--   0        0        0      203 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_encounter_month.csv
--rw-r--r--   0        0        0      193 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_encounter_year.csv
--rw-r--r--   0        0        0      114 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_immunization_month.csv
--rw-r--r--   0        0        0      104 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_immunization_year.csv
--rw-r--r--   0        0        0       27 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_medication_all.csv
--rw-r--r--   0        0        0      144 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_medicationrequest_month.csv
--rw-r--r--   0        0        0      140 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_medicationrequest_year.csv
--rw-r--r--   0        0        0      273 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_observation_month.csv
--rw-r--r--   0        0        0      257 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_observation_year.csv
--rw-r--r--   0        0        0       47 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_patient_all.csv
--rw-r--r--   0        0        0      178 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_procedure_month.csv
--rw-r--r--   0        0        0      147 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_procedure_year.csv
--rw-r--r--   0        0        0      203 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/immunization/0.ndjson
--rw-r--r--   0        0        0       36 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/medication/0.ndjson
--rw-r--r--   0        0        0      342 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0      934 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/observation/0.ndjson
--rw-r--r--   0        0        0       87 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/patient/0.ndjson
--rw-r--r--   0        0        0      310 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/procedure/0.ndjson
--rw-r--r--   0        0        0      118 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/condition/0.ndjson
--rw-r--r--   0        0        0      544 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/expected_summary.csv
--rw-r--r--   0        0        0     1264 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0       36 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/patient/0.ndjson
--rw-r--r--   0        0        0     1082 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0     1408 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/condition/0.ndjson
--rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/device/0.ndjson
--rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/documentreference/0.ndjson
--rw-r--r--   0        0        0      383 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/encounter/0.ndjson
--rw-r--r--   0        0        0      308 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_allergyintolerance_code.csv
--rw-r--r--   0        0        0      368 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_condition_code.csv
--rw-r--r--   0        0        0       73 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_device_type.csv
--rw-r--r--   0        0        0      106 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_diagnosticreport_code.csv
--rw-r--r--   0        0        0      106 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_documentreference_type.csv
--rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_encounter_class.csv
--rw-r--r--   0        0        0      147 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_encounter_type.csv
--rw-r--r--   0        0        0      106 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_immunization_vaccinecode.csv
--rw-r--r--   0        0        0       73 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_medication_code.csv
--rw-r--r--   0        0        0      106 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_medicationrequest_medicationcodeableconcept.csv
--rw-r--r--   0        0        0      281 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_observation_code.csv
--rw-r--r--   0        0        0      308 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_observation_valuecodeableconcept.csv
--rw-r--r--   0        0        0      106 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_procedure_code.csv
--rw-r--r--   0        0        0      112 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/immunization/0.ndjson
--rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/medication/0.ndjson
--rw-r--r--   0        0        0      126 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0     1415 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/observation/0.ndjson
--rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/procedure/0.ndjson
--rw-r--r--   0        0        0      842 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_us_core_v4_count/general/documentreference/0.ndjson
--rw-r--r--   0        0        0      254 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_us_core_v4_count/general/expected_documentreference.csv
--rw-r--r--   0        0        0       68 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/condition/0.ndjson
--rw-r--r--   0        0        0       74 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/encounter/0.ndjson
--rw-r--r--   0        0        0       40 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/expected_date.csv
--rw-r--r--   0        0        0       23 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/expected_version.csv
--rw-r--r--   0        0        0      246 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/observation/0.ndjson
--rw-r--r--   0        0        0       12 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/patient/0.ndjson
--rw-r--r--   0        0        0      269 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/condition/0.ndjson
--rw-r--r--   0        0        0      221 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/encounter/0.ndjson
--rw-r--r--   0        0        0      138 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/expected_condition.csv
--rw-r--r--   0        0        0       44 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/expected_encounter.csv
--rw-r--r--   0        0        0       76 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/expected_procedure.csv
--rw-r--r--   0        0        0      238 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/expected_summary.csv
--rw-r--r--   0        0        0      262 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/procedure/0.ndjson
--rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/condition/0.ndjson
--rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/device/0.ndjson
--rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/documentreference/0.ndjson
--rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/encounter/0.ndjson
--rw-r--r--   0        0        0      451 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/expected_summary.csv
--rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/immunization/0.ndjson
--rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/observation/0.ndjson
--rw-r--r--   0        0        0      198 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/procedure/0.ndjson
--rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/condition/0.ndjson
--rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/device/0.ndjson
--rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0      603 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/documentreference/0.ndjson
--rw-r--r--   0        0        0       51 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/encounter/0.ndjson
--rw-r--r--   0        0        0      122 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/expected_documentreference_encounter.csv
--rw-r--r--   0        0        0      107 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/expected_procedure_encounter.csv
--rw-r--r--   0        0        0      787 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/expected_summary.csv
--rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/immunization/0.ndjson
--rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/observation/0.ndjson
--rw-r--r--   0        0        0       12 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/patient/0.ndjson
--rw-r--r--   0        0        0      890 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/procedure/0.ndjson
--rw-r--r--   0        0        0       77 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0       77 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/condition/0.ndjson
--rw-r--r--   0        0        0       77 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/device/0.ndjson
--rw-r--r--   0        0        0       71 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0       71 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/documentreference/0.ndjson
--rw-r--r--   0        0        0      498 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/expected_summary.csv
--rw-r--r--   0        0        0       89 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/immunization/0.ndjson
--rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/medication/0.ndjson
--rw-r--r--   0        0        0      119 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0      175 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/observation/0.ndjson
--rw-r--r--   0        0        0      452 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/procedure/0.ndjson
--rw-r--r--   0        0        0      178 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_valid_us_core_v4/general/encounter/0.ndjson
--rw-r--r--   0        0        0      155 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_valid_us_core_v4/general/expected_encounter.csv
--rw-r--r--   0        0        0      344 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_valid_us_core_v4/general/expected_summary.csv
--rw-r--r--   0        0        0       18 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/allergy-low-schema/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0      146 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/allergy-low-schema/expected_allergyintolerance_mandatory.csv
--rw-r--r--   0        0        0       90 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/allergy-low-schema/expected_allergyintolerance_must_support.csv
--rw-r--r--   0        0        0       18 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/docref-low-schema/documentreference/0.ndjson
--rw-r--r--   0        0        0      125 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/docref-low-schema/expected_documentreference_mandatory.csv
--rw-r--r--   0        0        0      119 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/docref-low-schema/expected_documentreference_must_support.csv
--rw-r--r--   0        0        0       18 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/encounter-low-schema/encounter/0.ndjson
--rw-r--r--   0        0        0       97 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/encounter-low-schema/expected_encounter_mandatory.csv
--rw-r--r--   0        0        0      145 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/encounter-low-schema/expected_encounter_must_support.csv
--rw-r--r--   0        0        0     2788 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0     2723 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/condition/0.ndjson
--rw-r--r--   0        0        0     1527 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0     1407 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/documentreference/0.ndjson
--rw-r--r--   0        0        0      827 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/encounter/0.ndjson
--rw-r--r--   0        0        0      945 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_allergyintolerance_mandatory.csv
--rw-r--r--   0        0        0     1048 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_condition_mandatory.csv
--rw-r--r--   0        0        0      610 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_diagnosticreport_note_mandatory.csv
--rw-r--r--   0        0        0      763 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_documentreference_mandatory.csv
--rw-r--r--   0        0        0      395 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_encounter_mandatory.csv
--rw-r--r--   0        0        0      377 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_immunization_mandatory.csv
--rw-r--r--   0        0        0       80 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_medication_mandatory.csv
--rw-r--r--   0        0        0      497 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_medicationrequest_mandatory.csv
--rw-r--r--   0        0        0     1682 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_laboratory_mandatory.csv
--rw-r--r--   0        0        0      620 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_smoking_status_mandatory.csv
--rw-r--r--   0        0        0     1238 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_vital_signs_mandatory.csv
--rw-r--r--   0        0        0      164 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_patient_mandatory.csv
--rw-r--r--   0        0        0      510 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_procedure_mandatory.csv
--rw-r--r--   0        0        0      894 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/immunization/0.ndjson
--rw-r--r--   0        0        0      109 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/medication/0.ndjson
--rw-r--r--   0        0        0      937 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/medicationrequest/0.ndjson
--rw-r--r--   0        0        0     6994 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/labs.ndjson
--rw-r--r--   0        0        0     1471 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/smoking.ndjson
--rw-r--r--   0        0        0     3357 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/vitals.ndjson
--rw-r--r--   0        0        0      191 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/patient/0.ndjson
--rw-r--r--   0        0        0     1358 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/procedure/0.ndjson
--rw-r--r--   0        0        0      799 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0      237 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/condition/0.ndjson
--rw-r--r--   0        0        0      210 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0      714 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/documentreference/0.ndjson
--rw-r--r--   0        0        0      598 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/encounter/0.ndjson
--rw-r--r--   0        0        0      371 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_allergyintolerance_must_support.csv
--rw-r--r--   0        0        0      106 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_condition_must_support.csv
--rw-r--r--   0        0        0      195 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_diagnosticreport_note_must_support.csv
--rw-r--r--   0        0        0      441 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_documentreference_must_support.csv
--rw-r--r--   0        0        0      364 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_encounter_must_support.csv
--rw-r--r--   0        0        0      207 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_immunization_must_support.csv
--rw-r--r--   0        0        0       22 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_medication_must_support.csv
--rw-r--r--   0        0        0      236 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_medicationrequest_must_support.csv
--rw-r--r--   0        0        0      141 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_observation_laboratory_must_support.csv
--rw-r--r--   0        0        0       30 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_observation_smoking_status_must_support.csv
--rw-r--r--   0        0        0      173 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_observation_vital_signs_must_support.csv
--rw-r--r--   0        0        0      637 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_patient_must_support.csv
--rw-r--r--   0        0        0       22 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_procedure_must_support.csv
--rw-r--r--   0        0        0      296 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/immunization/0.ndjson
--rw-r--r--   0        0        0       18 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/medication/0.ndjson
--rw-r--r--   0        0        0      313 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/medicationrequest/0.ndjson
--rw-r--r--   0        0        0      901 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/labs.ndjson
--rw-r--r--   0        0        0       18 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/nothing.ndjson
--rw-r--r--   0        0        0       99 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/smoking.ndjson
--rw-r--r--   0        0        0      773 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/vitals.ndjson
--rw-r--r--   0        0        0     1652 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/patient/0.ndjson
--rw-r--r--   0        0        0       18 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/procedure/0.ndjson
--rw-r--r--   0        0        0      165 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/obs-low-schema/expected_observation_laboratory_mandatory.csv
--rw-r--r--   0        0        0       50 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/obs-low-schema/expected_observation_laboratory_must_support.csv
--rw-r--r--   0        0        0      147 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/obs-low-schema/observation/0.ndjson
--rw-r--r--   0        0        0       57 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/patient-low-schema/expected_patient_mandatory.csv
--rw-r--r--   0        0        0      152 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/patient-low-schema/expected_patient_must_support.csv
--rw-r--r--   0        0        0       18 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/patient-low-schema/patient/0.ndjson
--rw-r--r--   0        0        0     6243 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/test_metrics.py
--rw-r--r--   0        0        0     4253 1970-01-01 00:00:00.000000 cumulus_library_data_metrics-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 20:20:05.185731 cumulus_library_data_metrics-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3647 2024-05-29 20:20:05.185731 cumulus_library_data_metrics-2.0.0/README.md
+-rw-r--r--   0        0        0       68 2024-05-29 20:20:05.185731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/__init__.py
+-rw-r--r--   0        0        0     3829 2024-05-29 20:20:05.185731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/base.py
+-rw-r--r--   0        0        0     1430 2024-05-29 20:20:05.185731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/base.summary.jinja
+-rw-r--r--   0        0        0      899 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_pt_count/README.md
+-rw-r--r--   0        0        0     1265 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.jinja
+-rw-r--r--   0        0        0      743 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.py
+-rw-r--r--   0        0        0      308 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_pt_deceased_count/README.md
+-rw-r--r--   0        0        0     1861 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.jinja
+-rw-r--r--   0        0        0      385 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.py
+-rw-r--r--   0        0        0      265 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_resource_count/README.md
+-rw-r--r--   0        0        0     1099 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_resource_count/c_resource_count.jinja
+-rw-r--r--   0        0        0      893 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_resource_count/c_resource_count.py
+-rw-r--r--   0        0        0      347 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_resources_per_pt/README.md
+-rw-r--r--   0        0        0     2545 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.jinja
+-rw-r--r--   0        0        0      749 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.py
+-rw-r--r--   0        0        0      580 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_system_use/README.md
+-rw-r--r--   0        0        0     2080 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_system_use/c_system_use.jinja
+-rw-r--r--   0        0        0     1807 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_system_use/c_system_use.py
+-rw-r--r--   0        0        0     2075 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_us_core_v4_count/README.md
+-rw-r--r--   0        0        0     1595 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_us_core_v4_count/c_us_core_v4_count.jinja
+-rw-r--r--   0        0        0      433 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_us_core_v4_count/c_us_core_v4_count.py
+-rw-r--r--   0        0        0     3606 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/manifest.toml
+-rw-r--r--   0        0        0     1078 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/meta/dates.jinja
+-rw-r--r--   0        0        0      735 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/meta/meta.py
+-rw-r--r--   0        0        0       77 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/meta/version.jinja
+-rw-r--r--   0        0        0      904 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_date_recent/README.md
+-rw-r--r--   0        0        0     1234 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.jinja
+-rw-r--r--   0        0        0      682 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.py
+-rw-r--r--   0        0        0     1420 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_ref_target_pop/README.md
+-rw-r--r--   0        0        0      383 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_ref_target_pop/q_ref_target_pop.jinja
+-rw-r--r--   0        0        0     1383 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_ref_target_pop/q_ref_target_pop.py
+-rw-r--r--   0        0        0     1046 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_ref_target_valid/README.md
+-rw-r--r--   0        0        0     1163 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.jinja
+-rw-r--r--   0        0        0     2320 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.py
+-rw-r--r--   0        0        0      740 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_system_use/README.md
+-rw-r--r--   0        0        0      949 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_system_use/q_system_use.jinja
+-rw-r--r--   0        0        0     2972 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_system_use/q_system_use.py
+-rw-r--r--   0        0        0     3587 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/README.md
+-rw-r--r--   0        0        0      738 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.jinja
+-rw-r--r--   0        0        0      688 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.py
+-rw-r--r--   0        0        0     2831 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/resource_info.py
+-rw-r--r--   0        0        0     2046 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/systems.py
+-rw-r--r--   0        0        0      105 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/t_us_core_v4/README.md
+-rw-r--r--   0        0        0      182 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/t_us_core_v4/mandatory.jinja
+-rw-r--r--   0        0        0      225 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/t_us_core_v4/must_support.jinja
+-rw-r--r--   0        0        0      815 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/t_us_core_v4/t_us_core_v4.py
+-rw-r--r--   0        0        0      345 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/README.md
+-rw-r--r--   0        0        0       50 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/__init__.py
+-rw-r--r--   0        0        0     2453 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_mandatory.jinja
+-rw-r--r--   0        0        0     2666 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_must_support.jinja
+-rw-r--r--   0        0        0     2603 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/condition_mandatory.jinja
+-rw-r--r--   0        0        0     1414 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/condition_must_support.jinja
+-rw-r--r--   0        0        0     1025 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_lab_mandatory.jinja
+-rw-r--r--   0        0        0     1286 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_lab_must_support.jinja
+-rw-r--r--   0        0        0     1039 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_mandatory.jinja
+-rw-r--r--   0        0        0      816 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_must_support.jinja
+-rw-r--r--   0        0        0     1307 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_utils.jinja
+-rw-r--r--   0        0        0     2129 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_mandatory.jinja
+-rw-r--r--   0        0        0     2945 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_must_support.jinja
+-rw-r--r--   0        0        0      834 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/encounter_mandatory.jinja
+-rw-r--r--   0        0        0     1503 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/encounter_must_support.jinja
+-rw-r--r--   0        0        0      954 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/immunization_mandatory.jinja
+-rw-r--r--   0        0        0      570 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/immunization_must_support.jinja
+-rw-r--r--   0        0        0      356 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/medication_mandatory.jinja
+-rw-r--r--   0        0        0      129 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/medication_must_support.jinja
+-rw-r--r--   0        0        0     1322 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_mandatory.jinja
+-rw-r--r--   0        0        0     1018 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_must_support.jinja
+-rw-r--r--   0        0        0      316 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_blood_pressure_mandatory.jinja
+-rw-r--r--   0        0        0     2291 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_mandatory.jinja
+-rw-r--r--   0        0        0     1024 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_must_support.jinja
+-rw-r--r--   0        0        0     1974 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_smoking_status_mandatory.jinja
+-rw-r--r--   0        0        0      190 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_smoking_status_must_support.jinja
+-rw-r--r--   0        0        0     3804 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_utils.jinja
+-rw-r--r--   0        0        0     4855 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_mandatory.jinja
+-rw-r--r--   0        0        0     1032 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_must_support.jinja
+-rw-r--r--   0        0        0      619 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/patient_mandatory.jinja
+-rw-r--r--   0        0        0     2503 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/patient_must_support.jinja
+-rw-r--r--   0        0        0     5242 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/patient_utils.jinja
+-rw-r--r--   0        0        0     1004 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/procedure_mandatory.jinja
+-rw-r--r--   0        0        0      128 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/procedure_must_support.jinja
+-rw-r--r--   0        0        0     3606 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/profiles.py
+-rw-r--r--   0        0        0      660 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/slice.jinja
+-rw-r--r--   0        0        0     9327 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/utils.jinja
+-rw-r--r--   0        0        0     1599 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    20839 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/tests/data/c_pt_count/cubed/expected.csv
+-rw-r--r--   0        0        0     3202 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/tests/data/c_pt_count/cubed/patient/0.ndjson
+-rw-r--r--   0        0        0      819 2024-05-29 20:20:05.189731 cumulus_library_data_metrics-2.0.0/tests/data/c_pt_count/general/expected.csv
+-rw-r--r--   0        0        0     3202 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_pt_count/general/patient/0.ndjson
+-rw-r--r--   0        0        0      137 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_pt_count/no-ext/expected.csv
+-rw-r--r--   0        0        0       33 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_pt_count/no-ext/patient/0.ndjson
+-rw-r--r--   0        0        0      269 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_pt_deceased_count/general/expected.csv
+-rw-r--r--   0        0        0      786 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_pt_deceased_count/general/patient/0.ndjson
+-rw-r--r--   0        0        0     1334 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0     1978 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/condition/0.ndjson
+-rw-r--r--   0        0        0       24 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/device/0.ndjson
+-rw-r--r--   0        0        0      494 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0      695 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0      603 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      417 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_allergyintolerance_month.csv
+-rw-r--r--   0        0        0      375 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_allergyintolerance_year.csv
+-rw-r--r--   0        0        0      456 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_condition_month.csv
+-rw-r--r--   0        0        0      354 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_condition_year.csv
+-rw-r--r--   0        0        0       27 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_device_all.csv
+-rw-r--r--   0        0        0      200 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_diagnosticreport_month.csv
+-rw-r--r--   0        0        0      190 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_diagnosticreport_year.csv
+-rw-r--r--   0        0        0      225 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_documentreference_month.csv
+-rw-r--r--   0        0        0      215 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_documentreference_year.csv
+-rw-r--r--   0        0        0      203 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_encounter_month.csv
+-rw-r--r--   0        0        0      193 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_encounter_year.csv
+-rw-r--r--   0        0        0      114 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_immunization_month.csv
+-rw-r--r--   0        0        0      104 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_immunization_year.csv
+-rw-r--r--   0        0        0       27 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_medication_all.csv
+-rw-r--r--   0        0        0      144 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_medicationrequest_month.csv
+-rw-r--r--   0        0        0      140 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_medicationrequest_year.csv
+-rw-r--r--   0        0        0      273 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_observation_month.csv
+-rw-r--r--   0        0        0      257 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_observation_year.csv
+-rw-r--r--   0        0        0       47 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_patient_all.csv
+-rw-r--r--   0        0        0      178 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_procedure_month.csv
+-rw-r--r--   0        0        0      147 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/expected_procedure_year.csv
+-rw-r--r--   0        0        0      203 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/immunization/0.ndjson
+-rw-r--r--   0        0        0       36 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/medication/0.ndjson
+-rw-r--r--   0        0        0      342 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0      934 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/observation/0.ndjson
+-rw-r--r--   0        0        0       87 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/patient/0.ndjson
+-rw-r--r--   0        0        0      310 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/procedure/0.ndjson
+-rw-r--r--   0        0        0      118 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resources_per_pt/general/condition/0.ndjson
+-rw-r--r--   0        0        0      544 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resources_per_pt/general/expected_summary.csv
+-rw-r--r--   0        0        0     1264 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resources_per_pt/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0       36 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_resources_per_pt/general/patient/0.ndjson
+-rw-r--r--   0        0        0     1082 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0     1408 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/condition/0.ndjson
+-rw-r--r--   0        0        0      105 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/device/0.ndjson
+-rw-r--r--   0        0        0      105 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0      105 2024-05-29 20:20:05.193731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0      383 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      308 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_allergyintolerance_code.csv
+-rw-r--r--   0        0        0      368 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_condition_code.csv
+-rw-r--r--   0        0        0       73 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_device_type.csv
+-rw-r--r--   0        0        0      106 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_diagnosticreport_code.csv
+-rw-r--r--   0        0        0      106 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_documentreference_type.csv
+-rw-r--r--   0        0        0      105 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_encounter_class.csv
+-rw-r--r--   0        0        0      147 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_encounter_type.csv
+-rw-r--r--   0        0        0      106 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_immunization_vaccinecode.csv
+-rw-r--r--   0        0        0       73 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_medication_code.csv
+-rw-r--r--   0        0        0      106 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_medicationrequest_medicationcodeableconcept.csv
+-rw-r--r--   0        0        0      281 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_observation_code.csv
+-rw-r--r--   0        0        0      308 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_observation_valuecodeableconcept.csv
+-rw-r--r--   0        0        0      106 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/expected_procedure_code.csv
+-rw-r--r--   0        0        0      112 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/immunization/0.ndjson
+-rw-r--r--   0        0        0      105 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/medication/0.ndjson
+-rw-r--r--   0        0        0      126 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0     1415 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/observation/0.ndjson
+-rw-r--r--   0        0        0      105 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/procedure/0.ndjson
+-rw-r--r--   0        0        0      842 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_us_core_v4_count/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0      254 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/c_us_core_v4_count/general/expected_documentreference.csv
+-rw-r--r--   0        0        0       68 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/meta/general/condition/0.ndjson
+-rw-r--r--   0        0        0       74 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/meta/general/encounter/0.ndjson
+-rw-r--r--   0        0        0       40 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/meta/general/expected_date.csv
+-rw-r--r--   0        0        0       23 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/meta/general/expected_version.csv
+-rw-r--r--   0        0        0      246 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/meta/general/observation/0.ndjson
+-rw-r--r--   0        0        0       12 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/meta/general/patient/0.ndjson
+-rw-r--r--   0        0        0      269 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_date_recent/general/condition/0.ndjson
+-rw-r--r--   0        0        0      221 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_date_recent/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      222 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_date_recent/general/expected_condition.csv
+-rw-r--r--   0        0        0       60 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_date_recent/general/expected_encounter.csv
+-rw-r--r--   0        0        0       98 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_date_recent/general/expected_procedure.csv
+-rw-r--r--   0        0        0      247 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_date_recent/general/expected_summary.csv
+-rw-r--r--   0        0        0      262 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_date_recent/general/procedure/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/condition/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/device/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      468 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/expected_summary.csv
+-rw-r--r--   0        0        0       55 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/immunization/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/observation/0.ndjson
+-rw-r--r--   0        0        0      198 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_pop/general/procedure/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-29 20:20:05.197731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/condition/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/device/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0      792 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0       51 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      156 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/expected_documentreference_encounter.csv
+-rw-r--r--   0        0        0       47 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/expected_procedure_encounter.csv
+-rw-r--r--   0        0        0      814 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/expected_summary.csv
+-rw-r--r--   0        0        0       98 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/immunization/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/observation/0.ndjson
+-rw-r--r--   0        0        0       12 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/patient/0.ndjson
+-rw-r--r--   0        0        0      890 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/procedure/0.ndjson
+-rw-r--r--   0        0        0       77 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0       77 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/condition/0.ndjson
+-rw-r--r--   0        0        0       77 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/device/0.ndjson
+-rw-r--r--   0        0        0       71 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0       71 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0      511 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/expected_summary.csv
+-rw-r--r--   0        0        0       89 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/immunization/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/medication/0.ndjson
+-rw-r--r--   0        0        0      119 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0      175 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/observation/0.ndjson
+-rw-r--r--   0        0        0      452 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_system_use/general/procedure/0.ndjson
+-rw-r--r--   0        0        0      178 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_valid_us_core_v4/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      155 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_valid_us_core_v4/general/expected_encounter.csv
+-rw-r--r--   0        0        0      397 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/q_valid_us_core_v4/general/expected_summary.csv
+-rw-r--r--   0        0        0       18 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/allergy-low-schema/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0      146 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/allergy-low-schema/expected_allergyintolerance_mandatory.csv
+-rw-r--r--   0        0        0       90 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/allergy-low-schema/expected_allergyintolerance_must_support.csv
+-rw-r--r--   0        0        0       18 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/docref-low-schema/documentreference/0.ndjson
+-rw-r--r--   0        0        0      125 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/docref-low-schema/expected_documentreference_mandatory.csv
+-rw-r--r--   0        0        0      119 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/docref-low-schema/expected_documentreference_must_support.csv
+-rw-r--r--   0        0        0       18 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/encounter-low-schema/encounter/0.ndjson
+-rw-r--r--   0        0        0       97 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/encounter-low-schema/expected_encounter_mandatory.csv
+-rw-r--r--   0        0        0      145 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/encounter-low-schema/expected_encounter_must_support.csv
+-rw-r--r--   0        0        0     2788 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0     2723 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/condition/0.ndjson
+-rw-r--r--   0        0        0      918 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/diagnosticreport/labs.ndjson
+-rw-r--r--   0        0        0     1527 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/diagnosticreport/notes.ndjson
+-rw-r--r--   0        0        0     1407 2024-05-29 20:20:05.201731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/documentreference/0.ndjson
+-rw-r--r--   0        0        0      827 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/encounter/0.ndjson
+-rw-r--r--   0        0        0      945 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_allergyintolerance_mandatory.csv
+-rw-r--r--   0        0        0     1048 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_condition_mandatory.csv
+-rw-r--r--   0        0        0      331 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_diagnosticreport_lab_mandatory.csv
+-rw-r--r--   0        0        0      610 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_diagnosticreport_note_mandatory.csv
+-rw-r--r--   0        0        0      763 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_documentreference_mandatory.csv
+-rw-r--r--   0        0        0      395 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_encounter_mandatory.csv
+-rw-r--r--   0        0        0      377 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_immunization_mandatory.csv
+-rw-r--r--   0        0        0       80 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_medication_mandatory.csv
+-rw-r--r--   0        0        0      497 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_medicationrequest_mandatory.csv
+-rw-r--r--   0        0        0     1682 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_laboratory_mandatory.csv
+-rw-r--r--   0        0        0      620 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_smoking_status_mandatory.csv
+-rw-r--r--   0        0        0     1238 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_vital_signs_mandatory.csv
+-rw-r--r--   0        0        0      164 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_patient_mandatory.csv
+-rw-r--r--   0        0        0      510 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_procedure_mandatory.csv
+-rw-r--r--   0        0        0      894 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/immunization/0.ndjson
+-rw-r--r--   0        0        0      109 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/medication/0.ndjson
+-rw-r--r--   0        0        0      937 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0     6994 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/observation/labs.ndjson
+-rw-r--r--   0        0        0     1471 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/observation/smoking.ndjson
+-rw-r--r--   0        0        0     3357 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/observation/vitals.ndjson
+-rw-r--r--   0        0        0      191 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/patient/0.ndjson
+-rw-r--r--   0        0        0     1358 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/procedure/0.ndjson
+-rw-r--r--   0        0        0      799 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0      237 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/condition/0.ndjson
+-rw-r--r--   0        0        0      971 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/diagnosticreport/labs.ndjson
+-rw-r--r--   0        0        0      210 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/diagnosticreport/notes.ndjson
+-rw-r--r--   0        0        0      714 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/documentreference/0.ndjson
+-rw-r--r--   0        0        0      598 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/encounter/0.ndjson
+-rw-r--r--   0        0        0      371 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_allergyintolerance_must_support.csv
+-rw-r--r--   0        0        0      106 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_condition_must_support.csv
+-rw-r--r--   0        0        0      269 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_diagnosticreport_lab_must_support.csv
+-rw-r--r--   0        0        0      195 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_diagnosticreport_note_must_support.csv
+-rw-r--r--   0        0        0      441 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_documentreference_must_support.csv
+-rw-r--r--   0        0        0      364 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_encounter_must_support.csv
+-rw-r--r--   0        0        0      207 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_immunization_must_support.csv
+-rw-r--r--   0        0        0       22 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_medication_must_support.csv
+-rw-r--r--   0        0        0      236 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_medicationrequest_must_support.csv
+-rw-r--r--   0        0        0      141 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_observation_laboratory_must_support.csv
+-rw-r--r--   0        0        0       30 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_observation_smoking_status_must_support.csv
+-rw-r--r--   0        0        0      173 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_observation_vital_signs_must_support.csv
+-rw-r--r--   0        0        0      637 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_patient_must_support.csv
+-rw-r--r--   0        0        0       22 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_procedure_must_support.csv
+-rw-r--r--   0        0        0      296 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/immunization/0.ndjson
+-rw-r--r--   0        0        0       18 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/medication/0.ndjson
+-rw-r--r--   0        0        0      313 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0      901 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/observation/labs.ndjson
+-rw-r--r--   0        0        0       18 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/observation/nothing.ndjson
+-rw-r--r--   0        0        0       99 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/observation/smoking.ndjson
+-rw-r--r--   0        0        0      773 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/observation/vitals.ndjson
+-rw-r--r--   0        0        0     1652 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/patient/0.ndjson
+-rw-r--r--   0        0        0       18 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/procedure/0.ndjson
+-rw-r--r--   0        0        0      165 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/obs-low-schema/expected_observation_laboratory_mandatory.csv
+-rw-r--r--   0        0        0       50 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/obs-low-schema/expected_observation_laboratory_must_support.csv
+-rw-r--r--   0        0        0      147 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/obs-low-schema/observation/0.ndjson
+-rw-r--r--   0        0        0       57 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/patient-low-schema/expected_patient_mandatory.csv
+-rw-r--r--   0        0        0      152 2024-05-29 20:20:05.205731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/patient-low-schema/expected_patient_must_support.csv
+-rw-r--r--   0        0        0       18 2024-05-29 20:20:05.209731 cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/patient-low-schema/patient/0.ndjson
+-rw-r--r--   0        0        0     6241 2024-05-29 20:20:05.209731 cumulus_library_data_metrics-2.0.0/tests/test_metrics.py
+-rw-r--r--   0        0        0     4538 1970-01-01 00:00:00.000000 cumulus_library_data_metrics-2.0.0/PKG-INFO
```

### Comparing `cumulus_library_data_metrics-1.0.0/LICENSE` & `cumulus_library_data_metrics-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/base.summary.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/base.summary.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 
     union_table AS (
         {%- for entry_key in entries %}
         SELECT
             numerator_table.entry_key AS id,
             numerator,
             denominator,
-            CASE
+            CAST(
+                CASE
                 WHEN denominator = 0 OR numerator = 0
-                THEN '0%'
-                ELSE CONCAT(CAST(CAST(CAST(numerator AS real) / denominator * 100 AS DECIMAL(5, 2)) AS varchar(10)), '%')
-            END AS percentage
+                THEN 0
+                ELSE CAST(numerator AS real) / denominator * 100
+                END
+            AS DECIMAL(5, 2)) AS percentage
         FROM {{ entry_key }}_numerator AS numerator_table
         INNER JOIN {{ entry_key }}_denominator AS denominator_table
         ON numerator_table.entry_key = denominator_table.entry_key
         {%- if not loop.last %}
         UNION
         {%- endif -%}
         {%- endfor %}
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/README.md` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_pt_count/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.jinja`

 * *Files 21% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 simplified AS (
     SELECT
         src.id,
         {{ utils.get_date_string(['src.birthDate'], 'year') }} AS birth_year,
         {{ utils.coalesce_missing('src.gender') }} AS administrative_gender,
         {{ utils.coalesce_missing('src_status.status') }} AS status,
         {{ utils.coalesce_missing('grouped_ethnicity.display') }} AS ethnicity,
-        {{ utils.coalesce_missing('grouped_race.display') }} AS race
-
+        {{ utils.coalesce_missing('grouped_race.display') }} AS race,
+        (
+            deceasedDateTime IS NOT NULL
+            OR (deceasedBoolean IS NOT NULL AND deceasedBoolean)
+        ) AS deceased
     FROM patient AS src
     LEFT JOIN src_status
     ON src.id = src_status.id
     LEFT JOIN grouped_ethnicity
     ON src.id = grouped_ethnicity.id
     LEFT JOIN grouped_race
     ON src.id = grouped_race.id
 )
 
 {% call utils.make_counts('simplified', output_mode) %}
     birth_year,
     administrative_gender,
     ethnicity,
     race,
+    deceased,
     status
 {% endcall %}
 );
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,9 +21,8 @@
                 },
                 "url": {},
             },
         },
     }
 
     def add_metric_queries(self) -> None:
-        # https://github.com/sync-for-science/qualifier/blob/master/metrics.md#c_pt_count-demographics-count-of-patients-by-birth-year-by-gender-by-ethnicity-by-race
         self.queries = [self.render_sql(self.name, src="Patient")]
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,21 @@
-"""Module for generating c_pt_deceased_count tables"""
+"""Module for generating c_resources_per_pt tables"""
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
+from cumulus_library_data_metrics import resource_info
 from cumulus_library_data_metrics.base import MetricMixin
 
 
-class DeceasedCountBuilder(MetricMixin, BaseTableBuilder):
-    name = "c_pt_deceased_count"
+class ResourcesPerPatientBuilder(MetricMixin, BaseTableBuilder):
+    name = "c_resources_per_pt"
 
-    def add_metric_queries(self, *args, **kwargs) -> None:
-        # https://github.com/sync-for-science/qualifier/blob/master/metrics.md#c_pt_deceased_count-demographics-count-of-deceased-patients-by-gender-by-age-at-death
-        self.queries = [self.render_sql(self.name)]
+    def add_metric_queries(self) -> None:
+        # The SQL wants to examine all the resources at once - so we don't do our normal metric
+        # pattern of rendering the template once per resource.
+        self.queries += [
+            self.render_sql(
+                self.name,
+                patient_fields=resource_info.PATIENTS,
+                categories=resource_info.CATEGORIES,
+            ),
+        ]
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resource_count/c_resource_count.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_resource_count/c_resource_count.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/c_term_coverage.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_system_use/c_system_use.jinja`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% import 'utils.jinja' as utils %}
 
-CREATE TABLE data_metrics__count_c_term_coverage_{{ src|lower }}_{{ field|lower }} AS (
+CREATE TABLE data_metrics__count_c_system_use_{{ src|lower }}_{{ field|lower }} AS (
 
 WITH
 src_status AS {{ utils.extract_status(src) }},
 
 {% if category_system %}
 src_categories AS {{ utils.extract_codes(src, 'category', system=category_system, is_array=true) }},
 {% endif %}
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/c_term_coverage.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_system_use/c_system_use.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,27 @@
-"""Module for generating c_term_coverage tables"""
+"""Module for generating c_system_use tables"""
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
 from cumulus_library_data_metrics import systems
 from cumulus_library_data_metrics.base import MetricMixin
 
 # Note that this CUBE is already very large / slow.
 # Please do not add new columns to it.
 # We already had to drop one planned column (has_text) from it due to performance.
 
 
-class TermCoverageBuilder(MetricMixin, BaseTableBuilder):
-    name = "c_term_coverage"
+class SystemUseBuilder(MetricMixin, BaseTableBuilder):
+    name = "c_system_use"
 
     def make_table(self, **kwargs) -> None:
         """Make a single metric table"""
         self.queries.append(self.render_sql(self.name, system_names=systems.NAMES, **kwargs))
 
     def add_metric_queries(self) -> None:
-        # https://github.com/sync-for-science/qualifier/blob/master/metrics.md#c_term_coverage-terminology-count-of-resources-by-terminology-system-by-resource-type-by-category
-        # With some tweaks:
-        # - Also stratify by year
-        # - Don't stratify by has_text -- CUBE was too big, had to drop something
-        # - added Encounter.class
-        # - added Medication.code
         self.make_table(
             src="Observation",
             field="code",
             category_system=systems.OBSERVATION_CATEGORY,
         )
         self.make_table(
             src="Observation",
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_us_core_v4_count/README.md` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_us_core_v4_count/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_us_core_v4_count/c_us_core_v4_count.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/c_us_core_v4_count/c_us_core_v4_count.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/meta/dates.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/meta/dates.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/meta/meta.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/README.md` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_date_recent/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
 Module for generating q_date_recent tables
-
-https://github.com/sync-for-science/qualifier/blob/master/metrics.md#q_date_recent-plausibility-expect-date-to-be-in-recent-past
 """
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
 from cumulus_library_data_metrics.base import MetricMixin
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_pop/README.md` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_ref_target_pop/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_pop/q_ref_target_pop.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,52 @@
-"""Module for generating q_ref_target_pop tables"""
+"""Module for generating q_ref_target_valid tables"""
+
+from typing import ClassVar
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
 from cumulus_library_data_metrics.base import MetricMixin
 
 
-class TargetPopBuilder(MetricMixin, BaseTableBuilder):
-    name = "q_ref_target_pop"
+class TargetValidBuilder(MetricMixin, BaseTableBuilder):
+    name = "q_ref_target_valid"
+
+    uses_fields: ClassVar[dict] = {
+        "DocumentReference": {
+            "context": {
+                "encounter": {},
+            },
+        },
+    }
 
-    def make_table(self, **kwargs) -> str:
+    def make_table(self, **kwargs) -> None:
         """Make a single metric table"""
         summary_key = f"{kwargs['src'].lower()}_{kwargs['dest'].lower()}"
         self.summary_entries[summary_key] = None
 
         self.queries.append(self.render_sql(self.name, **kwargs))
 
     def add_metric_queries(self) -> None:
-        # https://github.com/sync-for-science/qualifier/blob/master/metrics.md#q_ref_target_pop-conformance-expect-reference-target-to-be-populated
         self.make_table(src="AllergyIntolerance", dest="Patient", field="patient")
+        self.make_table(src="AllergyIntolerance", dest="Encounter", field="encounter")
         self.make_table(src="Condition", dest="Patient", field="subject")
+        self.make_table(src="Condition", dest="Encounter", field="encounter")
         self.make_table(src="Device", dest="Patient", field="patient")
         self.make_table(src="DiagnosticReport", dest="Patient", field="subject")
+        self.make_table(src="DiagnosticReport", dest="Encounter", field="encounter")
         self.make_table(src="DocumentReference", dest="Patient", field="subject")
+        self.make_table(
+            src="DocumentReference",
+            dest="Encounter",
+            field="context.encounter",
+            is_array=True,
+        )
         self.make_table(src="Encounter", dest="Patient", field="subject")
         self.make_table(src="Immunization", dest="Patient", field="patient")
+        self.make_table(src="Immunization", dest="Encounter", field="encounter")
         self.make_table(src="MedicationRequest", dest="Patient", field="subject")
+        self.make_table(src="MedicationRequest", dest="Encounter", field="encounter")
         self.make_table(src="Observation", dest="Patient", field="subject")
+        self.make_table(src="Observation", dest="Encounter", field="encounter")
         self.make_table(src="Procedure", dest="Patient", field="subject")
+        self.make_table(src="Procedure", dest="Encounter", field="encounter")
         self.make_summary()
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/README.md` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_ref_target_valid/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 This looks at whether target reference resources actually exist.
 
 For example, "for every `Condition.subject` that points to a patient,
 does that target actual exist in the Patient database?"
 
 ### Numerator (flagged rows)
 
-Any source Reference field which has a `.reference`
+Any source row which has at least one `.reference` field
 that looks like `"TargetResource/xxx"` but the corresponding `xxx` resource
 does not actually exist.
 
 Note that this does not check spec-valid but more complex forms like
 absolute URLs, contained resources, logical references, or display-only references.
-All such forms are not included in the numerator or denominator.
 
 ### Denominator
 
-All fields for the resource in question that have a populated reference to
-the target resource.
+All possible rows for the resource in question.
 
-(e.g. `count(*) from condition where subject.reference like 'Patient/%'`)
+(e.g. `count(*) from condition`)
 
 ### Debugging
 
 Each resource/field combo creates a table full of each row
 that was flagged as an issue.
 
 For example, for `Condition.subject` a table named
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -3,35 +3,43 @@
 CREATE TABLE data_metrics__q_ref_target_valid_{{ src|lower }}_{{ dest|lower }} AS (
 
 {% if field == 'context.encounter' and not schema['context']['encounter'] %}
     SELECT id FROM {{ src }} WHERE 1=0  -- return an empty table
 {% else %}
 
 WITH
-src_status AS {{ utils.extract_status(src) }}
+src_status AS {{ utils.extract_status(src) }},
 
 {%- if is_array %}
-    , flattened AS (
+    flattened AS (
         SELECT id, t.row AS unnested_field
         FROM {{ src }},
             UNNEST({{ field }}) AS t (row)
-    )
+    ),
 {%- set src = 'flattened' %}
 {%- set field = 'unnested_field' %}
 {%- endif %}
 
+grouped_bad_refs AS (
+    SELECT
+        src.id,
+        ARRAY_AGG(src.{{ field }}.reference) AS target
+    FROM {{ src }} AS src
+    LEFT JOIN {{ dest }} AS dest
+    ON SUBSTRING(src.{{ field }}.reference, LENGTH('{{ dest }}/') + 1) = dest.id
+    WHERE
+        REGEXP_LIKE(src.{{ field }}.reference, '^{{ dest }}/')
+        AND dest.id IS NULL
+    GROUP BY src.id
+)
+
 SELECT
     src.id,
     src_status.status,
-    src.{{ field }} AS target
-FROM {{ src }} AS src
+    {{ utils.array_to_string('target') }} AS target
+FROM grouped_bad_refs AS src
 LEFT JOIN src_status
 ON src.id = src_status.id
-LEFT JOIN {{ dest }} AS dest
-ON SUBSTRING(src.{{ field }}.reference, LENGTH('{{ dest }}/') + 1) = dest.id
-WHERE
-    src.{{ field }}.reference LIKE '{{ dest }}/%' -- keep in sync with denominator query
-    AND dest.id IS NULL
 
 {% endif %} -- closing initial "return empty table" check
 
 );
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/README.md` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_system_use/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# q_term_use
+# q_system_use
 
 **Are the recommended coding systems being used?**
 
 ### Numerator (flagged rows)
 
 All resource rows that have codings without a recommended system.
 
@@ -18,11 +18,11 @@
 
 ### Debugging
 
 Each resource/field combo creates a table full of each row
 that was flagged as an issue.
 
 For example, for `Condition.code` a table named
-`data_metrics__q_term_use_condition_code` is created.
+`data_metrics__q_system_use_condition_code` is created.
 
 These tables hold the `id`, `status`, and problem field for each flagged row,
 to aid root cause analysis.
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/q_term_use.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_system_use/q_system_use.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% import 'utils.jinja' as utils %}
 
 {%- set system_list = "('" + systems|join("', '") + "')" %}
 
-CREATE TABLE data_metrics__q_term_use_{{ src|lower }}_{{ field|lower }} AS (
+CREATE TABLE data_metrics__q_system_use_{{ src|lower }}_{{ field|lower }} AS (
 WITH
 src_status AS {{ utils.extract_status(src) }},
 
 -- Look for target systems
 src_has_system AS (
     SELECT
         id,
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/q_term_use.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_system_use/q_system_use.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-"""Module for generating q_term_use tables"""
+"""Module for generating q_system_use tables"""
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
 from cumulus_library_data_metrics import systems
 from cumulus_library_data_metrics.base import MetricMixin
 
 
-class TermUseBuilder(MetricMixin, BaseTableBuilder):
-    name = "q_term_use"
+class SystemUseBuilder(MetricMixin, BaseTableBuilder):
+    name = "q_system_use"
 
     def make_table(self, **kwargs) -> None:
         """Make a single metric table"""
         summary_key = f"{kwargs['src'].lower()}_{kwargs['field'].lower()}"
         self.summary_entries[summary_key] = None
 
         self.queries.append(self.render_sql(self.name, **kwargs))
 
     def add_metric_queries(self) -> None:
-        # https://github.com/sync-for-science/qualifier/blob/master/metrics.md#q_term_use-conformance-expect-common-terminology-systems-to-be-populated
-        # With some differences:
-        # - Allow multiple systems (pulled from US Core v4 profile recommendations)
         self.make_table(
             src="AllergyIntolerance",
             field="code",
             systems=[systems.RXNORM, systems.SNOMED],
         )
         self.make_table(
             src="Condition",
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/README.md` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.py`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/resource_info.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/resource_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,28 +34,42 @@
 }
 
 # Date fields in preference order.
 # This prefers "interaction with health system" dates, then administrative dates like "issued",
 # then best effort start dates like onsetDateTime.
 # See https://github.com/smart-on-fhir/cumulus-library-data-metrics/issues/16 for more.
 DATES = {
-    "AllergyIntolerance": ["recordedDate", "onsetDateTime", "onsetPeriod.start"],
-    "Condition": ["recordedDate", "onsetDateTime", "onsetPeriod.start"],
-    "DiagnosticReport": ["effectiveDateTime", "effectivePeriod.start", "issued"],
-    "DocumentReference": ["context.period.start", "date"],
-    "Encounter": ["period.start"],
+    "AllergyIntolerance": ["recordedDate", "onsetDateTime", "onsetPeriod.start", "onsetPeriod.end"],
+    "Condition": [
+        "recordedDate",
+        "onsetDateTime",
+        "onsetPeriod.start",
+        "onsetPeriod.end",
+        "abatementDateTime",
+        "abatementPeriod.start",
+        "abatementPeriod.end",
+    ],
+    "DiagnosticReport": [
+        "effectiveDateTime",
+        "effectivePeriod.start",
+        "effectivePeriod.end",
+        "issued",
+    ],
+    "DocumentReference": ["context.period.start", "context.period.end", "date"],
+    "Encounter": ["period.start", "period.end"],
     "Immunization": ["occurrenceDateTime", "recorded"],
     "MedicationRequest": ["authoredOn"],
     "Observation": [
         "effectiveDateTime",
         "effectivePeriod.start",
+        "effectivePeriod.end",
         "effectiveInstant",
         "issued",
     ],
-    "Procedure": ["performedDateTime", "performedPeriod.start"],
+    "Procedure": ["performedDateTime", "performedPeriod.start", "performedPeriod.end"],
 }
 
 # Which field to examine for a Patient
 PATIENTS = {
     "AllergyIntolerance": "patient",
     "Condition": "subject",
     "Device": "patient",
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/systems.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/systems.py`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/t_us_core_v4/t_us_core_v4.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/t_us_core_v4/t_us_core_v4.py`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_must_support.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/condition_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/condition_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/condition_must_support.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/condition_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_lab_mandatory.jinja`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,37 @@
--- http://hl7.org/fhir/us/core/STU4/StructureDefinition-us-core-diagnosticreport-note.html
--- There is another lab-report-specific profile,
--- but this is the "base DiagnosticReport" profile that covers the bare minimum.
+-- http://hl7.org/fhir/us/core/STU4/StructureDefinition-us-core-diagnosticreport-lab.html
+-- There is another non-lab-report-specific profile,
+-- but this is the DiagnosticReport profile that covers the LAB rows.
+
+{% import 'us_core_v4/diagnosticreport_utils.jinja' as dr_utils %}
 
 WITH
+tmp_slice AS {% include 'us_core_v4/slice.jinja' %},
 
 tmp_simplified AS (
     SELECT
         id,
-        {{ utils.is_code_valid('status', [
-            'registered',
-            'partial',
-            'preliminary',
-            'final',
-            'amended',
-            'corrected',
-            'appended',
-            'cancelled',
-            'entered-in-error',
-            'unknown',
-        ]) }} AS valid_status,
-        category IS NOT NULL AS valid_category,
+        {{ dr_utils.is_dr_status_valid() }} AS valid_status,
         {{ utils.is_concept_valid('code') }} AS valid_code,
         {{ utils.is_reference_of_type('subject', 'Patient') }} AS valid_subject,
         (
             effectiveDateTime IS NOT NULL
             OR {{ utils.is_period_valid('effectivePeriod') }}
-        ) AS valid_effective
-    FROM {{ src }}
+        ) AS valid_effective,
+        issued IS NOT NULL AS valid_issued
+    FROM tmp_slice
 )
 
 {%
 set fields = [
     'valid_status',
-    'valid_category',
     'valid_code',
     'valid_subject',
     'valid_effective',
+    'valid_issued',
 ]
 %}
 
 SELECT
     id,
     {{ fields|join(", ") }},
     {{ fields|join(" AND ") }} AS valid
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_must_support.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_must_support.jinja`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 -- http://hl7.org/fhir/us/core/STU4/StructureDefinition-us-core-diagnosticreport-note.html
 -- There is another lab-report-specific profile,
 -- but this is the "base DiagnosticReport" profile that covers the bare minimum.
 
 WITH
+tmp_slice AS {% include 'us_core_v4/slice.jinja' %},
 
 tmp_simplified AS (
     SELECT
         id,
         {{ utils.is_reference_of_type('encounter', 'Encounter') }} AS valid_encounter,
         issued IS NOT NULL AS valid_issued,
         performer IS NOT NULL AS valid_performer,
         presentedForm IS NOT NULL as valid_presented_form
-    FROM {{ src }}
+    FROM tmp_slice
 )
 
 {%
 set ns.fields = [
     'valid_encounter',
     'valid_issued',
     'valid_performer',
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_must_support.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/encounter_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/encounter_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/encounter_must_support.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/encounter_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/immunization_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/immunization_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/immunization_must_support.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/immunization_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_must_support.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_must_support.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_smoking_status_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_smoking_status_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_utils.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_utils.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_must_support.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/patient_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_must_support.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/patient_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_utils.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/patient_utils.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/procedure_mandatory.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/procedure_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/profiles.py` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/us_core_v4/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         self.make_table(src="Observation", name="laboratory", category="laboratory")
         self.make_table(src="Observation", name="smoking_status", loinc="72166-2")
         self.make_table(src="Observation", name="vital_signs", category="vital-signs")
 
         # Rest of profiles
         self.make_table(src="AllergyIntolerance")
         self.make_table(src="Condition")
+        self.make_table(src="DiagnosticReport", name="lab")
         self.make_table(src="DiagnosticReport", name="note")
         self.make_table(src="DocumentReference")
         self.make_table(src="Encounter")
         self.make_table(src="Immunization")
         self.make_table(src="Medication")
         self.make_table(src="MedicationRequest")
         self.make_table(src="Patient")
```

### Comparing `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/utils.jinja` & `cumulus_library_data_metrics-2.0.0/cumulus_library_data_metrics/utils.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 {%- endmacro %}
 
 
 -- Extracts a date field from a list of choices and returns a DATE.
 {% macro coalesce_date(fields) -%}
     date(from_iso8601_timestamp(
         COALESCE(
-            {{ fields|join(', ') }}
+            "{{ fields|join('", "')|replace('.', '"."') }}"
         )
     ))
 {%- endmacro %}
 
 -- Extracts a date field from a list of choices, chops it to the period, and returns a string.
 {% macro get_date_string(fields, period) -%}
     {% call coalesce_missing() %}
@@ -170,22 +170,22 @@
     {% if types is string %}
         {% set types = [types] %}
     {% endif %}
     {{ field }} IS NOT NULL
     AND (
         {{ field }}.reference IS NOT NULL AND (
             {% for type in types %}
-            {{ field }}.reference LIKE '{{ type }}/%'
+            REGEXP_LIKE({{ field }}.reference, '^{{ type }}/')
             {%- if not loop.last %}OR{%- endif -%}
             {%- endfor %}
 
             {% if allow_contained %}
             {# Validating the type further would be very hard (unnesting), so we don't here.
                This is only used rarely (MedRequest, where the target must be Medication). #}
-            OR {{ field }}.reference LIKE '#%'
+            OR REGEXP_LIKE({{ field }}.reference, '^#')
             {% endif %}
         )
         -- TODO: Should we allow this form? FHIR spec says yes... but not sure our SQL allows it
         -- OR ({{ field }}.type IS NOT NULL AND {{ field }}.type = {{ type }})
     )
 )
 {%- endmacro %}
```

### Comparing `cumulus_library_data_metrics-1.0.0/pyproject.toml` & `cumulus_library_data_metrics-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/cubed/patient/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_pt_count/cubed/patient/0.ndjson`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-{"id": "all-values", "active": true, "gender": "female", "birthDate": "2000-04-04", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2028-9", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2106-3", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2076-8", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2054-5", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "1002-5", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}, {"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2135-2", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}]}
+{"id": "all-values", "deceasedBoolean": false, "active": true, "gender": "female", "birthDate": "2000-04-04", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2028-9", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2106-3", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2076-8", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2054-5", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "1002-5", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}, {"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2135-2", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}]}
 {"id": "unk-race", "active": true, "gender": "other", "birthDate": "2001-01-02", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race", "extension": [{"url": "ombCategory", "valueCoding": {"code": "UNK", "system": "http://terminology.hl7.org/CodeSystem/v3-NullFlavor"}}]}]}
 {"id": "asku-race", "active": true, "gender": "other", "birthDate": "2001-01-02", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race", "extension": [{"url": "ombCategory", "valueCoding": {"code": "ASKU", "system": "http://terminology.hl7.org/CodeSystem/v3-NullFlavor"}}]}]}
 {"id": "unexpected-race", "active": true, "gender": "other", "birthDate": "2001-01-02", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race", "extension": [{"url": "ombCategory", "valueCoding": {"code": "race", "system": "weird-system"}}]}]}
 {"id": "non-hispanic-ethnicity", "active": true, "gender": "other", "birthDate": "2003-01-02", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2186-5", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}]}
 {"id": "unexpected-ethnicity", "active": true, "gender": "other", "birthDate": "2001-01-02", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "eth", "system": "weird-system"}}]}]}
 {"id": "no-extensions", "active": true, "gender": "other", "birthDate": "2001-01-02"}
 {"id": "no-birthdate", "active": true, "gender": "other", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2135-2", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}]}
 {"id": "no-gender", "active": true, "birthDate": "1990-04-04", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2135-2", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}]}
+{"id": "deceased-bool", "deceasedBoolean": true}
+{"id": "deceased-datetime", "deceasedDateTime": "2022-09-21"}
 {"id": "inactive", "active": false}
 {"id": "nothing"}
```

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/general/expected.csv` & `cumulus_library_data_metrics-2.0.0/tests/data/c_pt_count/general/expected.csv`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-cnt,birth_year,administrative_gender,ethnicity,race,status
-3,2001,other,cumulus__none,cumulus__none,active
-1,cumulus__none,other,Hispanic or Latino,cumulus__none,active
-1,cumulus__none,cumulus__none,cumulus__none,cumulus__none,inactive
-1,cumulus__none,cumulus__none,cumulus__none,cumulus__none,cumulus__none
-1,2003,other,Non Hispanic or Latino,cumulus__none,active
-1,2001,other,cumulus__none,Unknown,active
-1,2001,other,cumulus__none,Asked but no answer,active
-1,2000,female,Hispanic or Latino,American Indian or Alaska Native; Asian; Black or African American; Native Hawaiian or Other Pacific Islander; White,active
-1,1990,cumulus__none,Hispanic or Latino,cumulus__none,active
+cnt,birth_year,administrative_gender,ethnicity,race,deceased,status
+3,2001,other,cumulus__none,cumulus__none,false,active
+2,cumulus__none,cumulus__none,cumulus__none,cumulus__none,true,cumulus__none
+1,cumulus__none,other,Hispanic or Latino,cumulus__none,false,active
+1,cumulus__none,cumulus__none,cumulus__none,cumulus__none,false,inactive
+1,cumulus__none,cumulus__none,cumulus__none,cumulus__none,false,cumulus__none
+1,2003,other,Non Hispanic or Latino,cumulus__none,false,active
+1,2001,other,cumulus__none,Unknown,false,active
+1,2001,other,cumulus__none,Asked but no answer,false,active
+1,2000,female,Hispanic or Latino,American Indian or Alaska Native; Asian; Black or African American; Native Hawaiian or Other Pacific Islander; White,false,active
+1,1990,cumulus__none,Hispanic or Latino,cumulus__none,false,active
```

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/general/patient/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_pt_count/general/patient/0.ndjson`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-{"id": "all-values", "active": true, "gender": "female", "birthDate": "2000-04-04", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2028-9", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2106-3", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2076-8", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2054-5", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "1002-5", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}, {"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2135-2", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}]}
+{"id": "all-values", "deceasedBoolean": false, "active": true, "gender": "female", "birthDate": "2000-04-04", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2028-9", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2106-3", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2076-8", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "2054-5", "system": "urn:oid:2.16.840.1.113883.6.238"}}, {"url": "ombCategory", "valueCoding": {"code": "1002-5", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}, {"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2135-2", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}]}
 {"id": "unk-race", "active": true, "gender": "other", "birthDate": "2001-01-02", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race", "extension": [{"url": "ombCategory", "valueCoding": {"code": "UNK", "system": "http://terminology.hl7.org/CodeSystem/v3-NullFlavor"}}]}]}
 {"id": "asku-race", "active": true, "gender": "other", "birthDate": "2001-01-02", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race", "extension": [{"url": "ombCategory", "valueCoding": {"code": "ASKU", "system": "http://terminology.hl7.org/CodeSystem/v3-NullFlavor"}}]}]}
 {"id": "unexpected-race", "active": true, "gender": "other", "birthDate": "2001-01-02", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race", "extension": [{"url": "ombCategory", "valueCoding": {"code": "race", "system": "weird-system"}}]}]}
 {"id": "non-hispanic-ethnicity", "active": true, "gender": "other", "birthDate": "2003-01-02", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2186-5", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}]}
 {"id": "unexpected-ethnicity", "active": true, "gender": "other", "birthDate": "2001-01-02", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "eth", "system": "weird-system"}}]}]}
 {"id": "no-extensions", "active": true, "gender": "other", "birthDate": "2001-01-02"}
 {"id": "no-birthdate", "active": true, "gender": "other", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2135-2", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}]}
 {"id": "no-gender", "active": true, "birthDate": "1990-04-04", "extension": [{"url": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity", "extension": [{"url": "ombCategory", "valueCoding": {"code": "2135-2", "system": "urn:oid:2.16.840.1.113883.6.238"}}]}]}
+{"id": "deceased-bool", "deceasedBoolean": true}
+{"id": "deceased-datetime", "deceasedDateTime": "2022-09-21"}
 {"id": "inactive", "active": false}
 {"id": "nothing"}
```

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_pt_deceased_count/general/patient/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_pt_deceased_count/general/patient/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/allergyintolerance/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/allergyintolerance/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/condition/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/condition/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/encounter/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/encounter/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/observation/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_resource_count/general/observation/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/expected_summary.csv` & `cumulus_library_data_metrics-2.0.0/tests/data/c_resources_per_pt/general/expected_summary.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/medicationrequest/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_resources_per_pt/general/medicationrequest/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/allergyintolerance/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/allergyintolerance/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/condition/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/condition/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/observation/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_system_use/general/observation/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/c_us_core_v4_count/general/documentreference/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/c_us_core_v4_count/general/documentreference/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/documentreference/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/documentreference/0.ndjson`

 * *Files 7% similar despite different names*

```diff
@@ -1,5 +1,6 @@
 {"id": "valid", "subject": {"reference": "Patient/A"}, "context": {"encounter": [{"reference": "Encounter/A"}]}}
 {"id": "bad-encounter", "subject": {"reference": "Patient/A"}, "context": {"encounter": [{"reference": "Encounter/Nope"}]}}
 {"id": "bad-second-encounter-in-list", "subject": {"reference": "Patient/A"}, "context": {"encounter": [{"reference": "Encounter/A"}, {"reference": "Encounter/Nope"}]}}
+{"id": "bad-multiple-encounters", "status": "current", "subject": {"reference": "Patient/A"}, "context": {"encounter": [{"reference": "Encounter/Nope2"}, {"reference": "Encounter/Nope"}]}}
 {"id": "missing-encounter-field", "subject": {"reference": "Patient/A"}, "context": {"facilityType": {"text": "A nice one"}}}
 {"id": "missing-context-field", "subject": {"reference": "Patient/A"}}
```

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/procedure/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/q_ref_target_valid/general/procedure/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/allergyintolerance/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/allergyintolerance/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/condition/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/condition/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/diagnosticreport/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/diagnosticreport/notes.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/documentreference/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/documentreference/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/encounter/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/encounter/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_allergyintolerance_mandatory.csv` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_allergyintolerance_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_condition_mandatory.csv` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_condition_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_diagnosticreport_note_mandatory.csv` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_diagnosticreport_note_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_documentreference_mandatory.csv` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_documentreference_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_laboratory_mandatory.csv` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_laboratory_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_smoking_status_mandatory.csv` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_smoking_status_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_vital_signs_mandatory.csv` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_vital_signs_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/immunization/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/immunization/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/medicationrequest/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/medicationrequest/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/labs.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/observation/labs.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/smoking.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/observation/smoking.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/vitals.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/observation/vitals.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/procedure/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/mandatory/procedure/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/allergyintolerance/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/allergyintolerance/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/documentreference/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/documentreference/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/encounter/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/encounter/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_patient_must_support.csv` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/expected_patient_must_support.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/labs.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/observation/labs.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/vitals.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/observation/vitals.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/patient/0.ndjson` & `cumulus_library_data_metrics-2.0.0/tests/data/t_us_core_v4/must-support/patient/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-1.0.0/tests/test_metrics.py` & `cumulus_library_data_metrics-2.0.0/tests/test_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,32 +44,32 @@
 
     def test_c_resource_count(self):
         self.run_study("c_resource_count", prefix="count_")
 
     def test_c_resources_per_pt(self):
         self.run_study("c_resources_per_pt")
 
-    def test_c_term_coverage(self):
-        self.run_study("c_term_coverage", prefix="count_")
+    def test_c_system_use(self):
+        self.run_study("c_system_use", prefix="count_")
 
     def test_c_us_core_v4_count(self):
         # Just spot checks one resource - the main logic is tested in t_us_core_v4
         self.run_study("c_us_core_v4_count", prefix="count_")
 
     def test_q_date_recent(self):
         self.run_study("q_date_recent")
 
     def test_q_ref_target_pop(self):
         self.run_study("q_ref_target_pop")
 
     def test_q_ref_target_valid(self):
         self.run_study("q_ref_target_valid")
 
-    def test_q_term_use(self):
-        self.run_study("q_term_use")
+    def test_q_system_use(self):
+        self.run_study("q_system_use")
 
     def test_q_valid_us_core_v4(self):
         # Just spot checks one resource & the summary - the main logic is tested in t_us_core_v4
         self.run_study("q_valid_us_core_v4")
 
     @ddt.data(
         "mandatory",
```

