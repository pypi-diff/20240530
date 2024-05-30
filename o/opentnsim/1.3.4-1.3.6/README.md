# Comparing `tmp/opentnsim-1.3.4.tar.gz` & `tmp/opentnsim-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentnsim-1.3.4.tar", last modified: Thu Jun  1 07:49:15 2023, max compression
+gzip compressed data, was "opentnsim-1.3.6.tar", last modified: Wed May 15 11:52:55 2024, max compression
```

## Comparing `opentnsim-1.3.4.tar` & `opentnsim-1.3.6.tar`

### file list

```diff
@@ -1,100 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.607651 opentnsim-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-01 07:49:02.000000 opentnsim-1.3.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-01 07:49:02.000000 opentnsim-1.3.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 07:49:02.000000 opentnsim-1.3.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-01 07:49:02.000000 opentnsim-1.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-01 07:49:02.000000 opentnsim-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-01 07:49:15.607651 opentnsim-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-01 07:49:02.000000 opentnsim-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.591651 opentnsim-1.3.4/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-01 07:49:02.000000 opentnsim-1.3.4/data/Correctionfactors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-01 07:49:02.000000 opentnsim-1.3.4/data/KarpovSmoothCurves.csv
--rw-r--r--   0 runner    (1001) docker     (123)   212529 2023-06-01 07:49:02.000000 opentnsim-1.3.4/data/ais.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.595651 opentnsim-1.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/OpenTNSim.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.595651 opentnsim-1.3.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   785084 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/_static/book.png
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/opentnsim.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/version-conventions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.595651 opentnsim-1.3.4/opentnsim/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20866 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    80195 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/fis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/graph_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    69590 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.595651 opentnsim-1.3.4/opentnsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 07:49:03.000000 opentnsim-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-01 07:49:15.607651 opentnsim-1.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2716 2023-06-01 07:49:03.000000 opentnsim-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.603651 opentnsim-1.3.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.603651 opentnsim-1.3.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2888448 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/data/ect-bctn.json
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_limiting_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_limiting_depth_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_uniform_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_uniform_depth_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_varying_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_varying_depth_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_resistance_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_resistance_components_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_squat.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_squat_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_total_power.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_total_power_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_Van_Dorsser_et_al_2020_draught_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_Van_Dorsser_et_al_2020_draught_payload_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_basic_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_fis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_single_vessel_with_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_single_vessel_without_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_without_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.607651 opentnsim-1.3.4/tests/vessels/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/vessels/vessels.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:52:55.430453 opentnsim-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-15 11:52:48.000000 opentnsim-1.3.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-15 11:52:48.000000 opentnsim-1.3.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-15 11:52:48.000000 opentnsim-1.3.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-15 11:52:48.000000 opentnsim-1.3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-15 11:52:48.000000 opentnsim-1.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-15 11:52:55.430453 opentnsim-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-15 11:52:48.000000 opentnsim-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:52:55.410453 opentnsim-1.3.6/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-15 11:52:48.000000 opentnsim-1.3.6/data/Correctionfactors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-15 11:52:48.000000 opentnsim-1.3.6/data/KarpovSmoothCurves.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   212529 2024-05-15 11:52:48.000000 opentnsim-1.3.6/data/ais.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:52:55.410453 opentnsim-1.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-15 11:52:48.000000 opentnsim-1.3.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-15 11:52:48.000000 opentnsim-1.3.6/docs/OpenTNSim.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:52:55.410453 opentnsim-1.3.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   785084 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/_static/book.png
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/opentnsim.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-15 11:52:49.000000 opentnsim-1.3.6/docs/version-conventions.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:52:55.414453 opentnsim-1.3.6/opentnsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21562 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80195 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/fis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/graph_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123133 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13353 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14357 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14991 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71970 2024-05-15 11:52:50.000000 opentnsim-1.3.6/opentnsim/vessel_traffic_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:52:55.430453 opentnsim-1.3.6/opentnsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-15 11:52:55.000000 opentnsim-1.3.6/opentnsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-15 11:52:55.000000 opentnsim-1.3.6/opentnsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:52:55.000000 opentnsim-1.3.6/opentnsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 11:52:55.000000 opentnsim-1.3.6/opentnsim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:52:55.000000 opentnsim-1.3.6/opentnsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-15 11:52:55.000000 opentnsim-1.3.6/opentnsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 11:52:55.000000 opentnsim-1.3.6/opentnsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 11:52:50.000000 opentnsim-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-15 11:52:55.430453 opentnsim-1.3.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2736 2024-05-15 11:52:50.000000 opentnsim-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:52:55.426453 opentnsim-1.3.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:52:55.426453 opentnsim-1.3.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  2888448 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/data/ect-bctn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_limiting_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_limiting_depth_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_uniform_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_uniform_depth_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_varying_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_varying_depth_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_resistance_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_resistance_components_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_squat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_squat_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_total_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_total_power_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_Van_Dorsser_et_al_2020_draught_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_Van_Dorsser_et_al_2020_draught_payload_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_basic_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_fis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_single_vessel_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_single_vessel_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10320 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:52:55.430453 opentnsim-1.3.6/tests/vessels/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-15 11:52:50.000000 opentnsim-1.3.6/tests/vessels/vessels.csv
```

### Comparing `opentnsim-1.3.4/AUTHORS.rst` & `opentnsim-1.3.6/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/CONTRIBUTING.rst` & `opentnsim-1.3.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/HISTORY.rst` & `opentnsim-1.3.6/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/LICENSE.txt` & `opentnsim-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/PKG-INFO` & `opentnsim-1.3.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: opentnsim
-Version: 1.3.4
-Summary: The OpenTNSim package aims to facilitate the analysis of network performance for different network configurations, fleet compositions and traffic rules.
-Home-page: https://github.com/TUDelft-CITG/OpenTNSim
-Author: Mark van Koningsveld
-Author-email: m.vankoningsveld@tudelft.nl
-License: mit
-Keywords: OpenTNSim
-Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
-
 [![Documentation](https://img.shields.io/badge/sphinx-documentation-informational.svg)](https://opentnsim.readthedocs.io/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/TUDelft-CITG/Transport-Network-Analysis/blob/master/LICENSE.txt)
 [![DOI](https://zenodo.org/badge/145843547.svg)](https://zenodo.org/badge/latestdoi/145843547)
 
 [![TUDelft-CITG](https://circleci.com/gh/TUDelft-CITG/OpenTNSim.svg?style=shield&circle-token=59b1f167ed771129459d86e822fd2faaae8f4a34)](https://circleci.com/gh/TUDelft-CITG/OpenTNSim)
 [![Coverage](https://artifact-getter.herokuapp.com/get_coverage_badge?circle_url=https://circleci.com/gh/TUDelft-CITG/OpenTNSim&circle_token=727b95b70301407d3c0af44e1af2039fd9486f6f=str)](https://artifact-getter.herokuapp.com/get_coverage_report?circle_url=https://circleci.com/gh/TUDelft-CITG/OpenTNSim&circle_token=727b95b70301407d3c0af44e1af2039fd9486f6f)
```

#### html2text {}

```diff
@@ -1,22 +1,14 @@
-Metadata-Version: 2.1 Name: opentnsim Version: 1.3.4 Summary: The OpenTNSim
-package aims to facilitate the analysis of network performance for different
-network configurations, fleet compositions and traffic rules. Home-page: https:
-//github.com/TUDelft-CITG/OpenTNSim Author: Mark van Koningsveld Author-email:
-m.vankoningsveld@tudelft.nl License: mit Keywords: OpenTNSim Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
-:: Developers Classifier: Natural Language :: English Classifier: Programming
-Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
-testing License-File: LICENSE.txt License-File: AUTHORS.rst [![Documentation]
-(https://img.shields.io/badge/sphinx-documentation-informational.svg)](https://
-opentnsim.readthedocs.io/) [![License: MIT](https://img.shields.io/badge/
-License-MIT-informational.svg)](https://github.com/TUDelft-CITG/Transport-
-Network-Analysis/blob/master/LICENSE.txt) [![DOI](https://zenodo.org/badge/
-145843547.svg)](https://zenodo.org/badge/latestdoi/145843547) [![TUDelft-CITG]
-(https://circleci.com/gh/TUDelft-CITG/OpenTNSim.svg?style=shield&circle-
+[![Documentation](https://img.shields.io/badge/sphinx-documentation-
+informational.svg)](https://opentnsim.readthedocs.io/) [![License: MIT](https:/
+/img.shields.io/badge/License-MIT-informational.svg)](https://github.com/
+TUDelft-CITG/Transport-Network-Analysis/blob/master/LICENSE.txt) [![DOI](https:
+//zenodo.org/badge/145843547.svg)](https://zenodo.org/badge/latestdoi/
+145843547) [![TUDelft-CITG](https://circleci.com/gh/TUDelft-CITG/
+OpenTNSim.svg?style=shield&circle-
 token=59b1f167ed771129459d86e822fd2faaae8f4a34)](https://circleci.com/gh/
 TUDelft-CITG/OpenTNSim) [![Coverage](https://artifact-getter.herokuapp.com/
 get_coverage_badge?circle_url=https://circleci.com/gh/TUDelft-CITG/
 OpenTNSim&circle_token=727b95b70301407d3c0af44e1af2039fd9486f6f=str)](https://
 artifact-getter.herokuapp.com/get_coverage_report?circle_url=https://
 circleci.com/gh/TUDelft-CITG/
 OpenTNSim&circle_token=727b95b70301407d3c0af44e1af2039fd9486f6f) # OpenTNSim
```

### Comparing `opentnsim-1.3.4/data/Correctionfactors.csv` & `opentnsim-1.3.6/data/Correctionfactors.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/data/KarpovSmoothCurves.csv` & `opentnsim-1.3.6/data/KarpovSmoothCurves.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/data/ais.csv` & `opentnsim-1.3.6/data/ais.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/docs/Makefile` & `opentnsim-1.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/docs/OpenTNSim.png` & `opentnsim-1.3.6/docs/OpenTNSim.png`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/docs/_static/book.png` & `opentnsim-1.3.6/docs/_static/book.png`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/docs/conf.py` & `opentnsim-1.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/docs/index.rst` & `opentnsim-1.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/docs/installation.rst` & `opentnsim-1.3.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/docs/opentnsim.rst` & `opentnsim-1.3.6/docs/opentnsim.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/docs/version-conventions.rst` & `opentnsim-1.3.6/docs/version-conventions.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/opentnsim/cli.py` & `opentnsim-1.3.6/opentnsim/cli.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/opentnsim/core.py` & `opentnsim-1.3.6/opentnsim/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,16 +159,14 @@
     - T_e: draught unloaded
     - T_f: draught loaded
     - renewable_fuel_mass: renewable fuel mass on board [kg]
     - renewable_fuel_volume: renewable fuel volume on board [m3]
     - renewable_fuel_required_space: renewable fuel required storage space (consider packaging factor) on board  [m3]
     """
 
-    # TODO: add blockage factor S to vessel properties
-
     def __init__(
         self,
         type,
         B,
         L,
         h_min=None,
         T=None,
@@ -315,21 +313,35 @@
         self.route = route
         # start at start of route
         self.position_on_route = 0
         self.complete_path = complete_path
 
     @property
     def graph(self):
+        """
+        Return the graph of the underlying environment.
+
+        If it's multigraph cast to corresponding type
+        If you want the multidigraph use the HasMultiGraph mixin
+
+        """
+        graph = None
         if hasattr(self.env, "graph"):
-            return self.env.graph
+            graph = self.env.graph
         elif hasattr(self.env, "FG"):
-            return self.env.FG
+            graph = self.env.FG
         else:
             raise ValueError("Routable expects .graph to be present on env")
 
+        if isinstance(graph, nx.MultiDiGraph):
+            return nx.DiGraph(graph)
+        elif isinstance(graph, nx.MultiGraph):
+            return nx.Graph(graph)
+        return graph
+
 
 @deprecated.deprecated(reason="Use Routable instead of Routeable")
 class Routeable(Routable):
     """Old name for Mixin class: renamed to Routable."""
 
 
 class Movable(Locatable, Routable, Log):
@@ -343,14 +355,15 @@
     """
 
     def __init__(self, v: float, *args, **kwargs):
         """Initialization"""
         self.v = v
         super().__init__(*args, **kwargs)
         self.on_pass_edge_functions = []
+        self.on_pass_node_functions = []
         self.wgs84 = pyproj.Geod(ellps="WGS84")
 
     def move(self, destination: Union[Locatable, Geometry, str] = None, engine_order: float = 1.0, duration: float = None):
         """determine distance between origin and destination, and
         yield the time it takes to travel it
         Assumption is that self.path is in the right order - vessel moves from route[0] to route[-1].
         """
@@ -385,17 +398,23 @@
             self.log_entry("Sailing to start", self.env.now, self.distance, dest)
 
         # Move over the path and log every step
         for i, edge in enumerate(zip(self.route[:-1], self.route[1:])):
             # name it a, b here, to avoid confusion with destination argument
             a, b = edge
 
+            node = a
+
+            yield from self.pass_node(node)
+
+            # we are now at the node
+            self.node = node
+
             # update to current position
             self.geometry = nx.get_node_attributes(self.graph, "geometry")[a]
-            self.node = a
             self.position_on_route = i
 
             # are we already at destination?
             if destination is not None:
                 # for geometry we need to use the shapely equivalent
                 if isinstance(destination, Geometry) and destination.equals(self.geometry):
                     break
@@ -414,14 +433,19 @@
         logger.debug("  distance: " + "%4.2f" % self.distance + " m")
         if self.current_speed is not None:
             logger.debug("  sailing:  " + "%4.2f" % self.current_speed + " m/s")
             logger.debug("  duration: " + "%4.2f" % ((self.distance / self.current_speed) / 3600) + " hrs")
         else:
             logger.debug("  current_speed:  not set")
 
+    def pass_node(self, node):
+        # call all on_pass_node_functions
+        for on_pass_node_function in self.on_pass_node_functions:
+            yield from on_pass_node_function(node)
+
     def pass_edge(self, origin, destination):
         edge = self.graph.edges[origin, destination]
         orig = nx.get_node_attributes(self.graph, "geometry")[origin]
         dest = nx.get_node_attributes(self.graph, "geometry")[destination]
 
         for on_pass_edge_function in self.on_pass_edge_functions:
             yield from on_pass_edge_function(origin, destination)
```

### Comparing `opentnsim-1.3.4/opentnsim/energy.py` & `opentnsim-1.3.6/opentnsim/energy.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/opentnsim/fis.py` & `opentnsim-1.3.6/opentnsim/fis.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/opentnsim/graph_module.py` & `opentnsim-1.3.6/opentnsim/graph_module.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/opentnsim/model.py` & `opentnsim-1.3.6/opentnsim/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Vessel generator."""
 
 # package(s) related to time, space and id
 import json
 import logging
 import uuid
+import numbers
 
 # you need these dependencies (you can get these from anaconda)
 # package(s) related to the simulation
 import simpy
 import networkx as nx
 
 # spatial libraries
@@ -27,28 +28,26 @@
 
 class VesselGenerator:
     """
     A class to generate vessels from a database
     """
 
     def __init__(self, vessel_type, vessel_database, loaded=None, random_seed=3):
-        """ Initialization """
+        """Initialization"""
 
         self.vessel_type = vessel_type
         self.vessel_database = vessel_database
         self.loaded = loaded
 
         random.seed(random_seed)
 
     def generate(self, environment, vessel_name, scenario=None):
-        """ Generate a vessel """
+        """Generate a vessel"""
 
-        vessel_info = self.vessel_database.sample(
-            n=1, random_state=int(1000 * random.random())
-        )
+        vessel_info = self.vessel_database.sample(n=1, random_state=int(1000 * random.random()))
         vessel_data = {}
 
         vessel_data["env"] = environment
         vessel_data["name"] = vessel_name
 
         if scenario:
             vessel_info = vessel_info[vessel_info["scenario"] == scenario]
@@ -66,100 +65,90 @@
                 vessel_data["level"] = vessel_data["capacity"]
             else:
                 vessel_data["level"] = 0
 
         vessel_data["route"] = None
         vessel_data["geometry"] = None
 
+        # add a unique id to the id, so that our ships are unique even when resampled
+        vessel_data["id"] = f'{vessel_data["id"]}-{uuid.uuid4()}'
+
         return self.vessel_type(**vessel_data)
 
     def arrival_process(
         self,
         environment,
         origin,
         destination,
         arrival_distribution,
         scenario,
         arrival_process,
     ):
-        """ 
+        """
         Make arrival process
-        
+
         environment:            simpy environment
         arrival_distribution:   specify the distribution from which vessels are generated, int or list
         arrival_process:        process of arrivals
         """
 
         # Create an array with inter-arrival times -- average number of seconds between arrivals
-        if type(arrival_distribution) == int or type(arrival_distribution) == float:
+        if isinstance(arrival_distribution, numbers.Number):
             self.inter_arrival_times = [3600 / arrival_distribution] * 24
 
-        elif type(arrival_distribution) == list and len(arrival_distribution) == 24:
+        elif isinstance(arrival_distribution, list) and len(arrival_distribution) == 24:
             self.inter_arrival_times = [3600 / n for n in arrival_distribution]
 
-        elif type(arrival_distribution) == list:
-            raise ValueError(
-                "List should contain an average number of vessels per hour for an entire day: 24 entries."
-            )
+        elif isinstance(arrival_distribution, list):
+            raise ValueError("List should contain an average number of vessels per hour for an entire day: 24 entries.")
 
         else:
-            raise ValueError(
-                "Specify an arrival distribution: type Integer or type List."
-            )
+            raise ValueError("Specify an arrival distribution: type Integer or type List.")
 
         while True:
-
             # Check simulation time
-            inter_arrival = self.inter_arrival_times[
-                datetime.datetime.fromtimestamp(environment.now).hour
-            ]
+            inter_arrival = self.inter_arrival_times[datetime.datetime.fromtimestamp(environment.now).hour]
 
             # In the case of a Markovian arrival process
             if arrival_process == "Markovian":
-
                 # Make a timestep based on the poisson process
                 yield environment.timeout(random.expovariate(1 / inter_arrival))
 
             elif arrival_process == "Uniform":
-
                 # Make a timestep based on uniform arrivals
                 yield environment.timeout(inter_arrival)
 
             else:
                 raise ValueError(
                     "No other arrival processes are yet defined. You can add them to transport_network_analysis/vessel_generator.py."
                 )
 
             # Create a vessel
             vessel = self.generate(environment, "Vessel", scenario)
             vessel.env = environment
             vessel.route = nx.dijkstra_path(environment.FG, origin, destination)
-            vessel.geometry = nx.get_node_attributes(environment.FG, "geometry")[
-                vessel.route[0]
-            ]
-            
+            vessel.geometry = nx.get_node_attributes(environment.FG, "geometry")[vessel.route[0]]
+
             environment.vessels.append(vessel)
             # Move on path
             environment.process(vessel.move())
 
 
 class Simulation(core.Identifiable):
     """
     A class to generate vessels from a database
     """
 
     def __init__(self, simulation_start, graph, scenario=None):
-        """ 
-        Initialization 
-        
+        """
+        Initialization
+
         scenario: scenario with vessels - should be coupled to the database
         """
-        self.environment = simpy.Environment(
-            initial_time=time.mktime(simulation_start.timetuple())
-        )
+        self.environment = simpy.Environment(initial_time=time.mktime(simulation_start.timetuple()))
         self.environment.FG = graph
         self.environment.routes = pd.DataFrame.from_dict(
             {
                 "Origin": [],
                 "Destination": [],
                 "Width": [],
                 "Height": [],
@@ -171,44 +160,44 @@
 
         self.environment.vessels = []
 
     def add_vessels(
         self,
         origin,
         destination,
-        vessel = None,
-        vessel_generator = None,
+        vessel=None,
+        vessel_generator=None,
         arrival_distribution=1,
         arrival_process="Markovian",
     ):
-        """ 
+        """
         Make arrival process
-        
+
         environment:            simpy environment
         arrival_distribution:   specify the distribution from which vessels are generated, int or list
         arrival_process:        process of arrivals
         """
-        
+
         if vessel_generator == None:
             self.environment.vessels.append(vessel)
             self.environment.process(vessel.move())
-            
+
         else:
             self.environment.process(
                 vessel_generator.arrival_process(
                     self.environment,
                     origin,
                     destination,
                     arrival_distribution,
                     self.scenario,
                     arrival_process,
                 )
             )
 
     def run(self, duration=24 * 60 * 60):
-        """ 
-        Run the simulation 
-        
+        """
+        Run the simulation
+
         duration:               specify the duration of the simulation in seconds
         """
 
         self.environment.run(until=self.environment.now + duration)
```

### Comparing `opentnsim-1.3.4/opentnsim/plot.py` & `opentnsim-1.3.6/opentnsim/plot.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/opentnsim/strategy.py` & `opentnsim-1.3.6/opentnsim/strategy.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/opentnsim/utils.py` & `opentnsim-1.3.6/opentnsim/utils.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/opentnsim.egg-info/SOURCES.txt` & `opentnsim-1.3.6/opentnsim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,19 @@
 opentnsim/cli.py
 opentnsim/core.py
 opentnsim/energy.py
 opentnsim/fis.py
 opentnsim/graph_module.py
 opentnsim/lock.py
 opentnsim/model.py
+opentnsim/output.py
 opentnsim/plot.py
 opentnsim/strategy.py
 opentnsim/utils.py
+opentnsim/vessel_traffic_service.py
 opentnsim.egg-info/PKG-INFO
 opentnsim.egg-info/SOURCES.txt
 opentnsim.egg-info/dependency_links.txt
 opentnsim.egg-info/entry_points.txt
 opentnsim.egg-info/not-zip-safe
 opentnsim.egg-info/requires.txt
 opentnsim.egg-info/top_level.txt
@@ -72,14 +74,16 @@
 tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv
 tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py
 tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv
 tests/test_Van_Dorsser_et_al_2020_draught_payload.py
 tests/test_Van_Dorsser_et_al_2020_draught_payload_expected.csv
 tests/test_basic_simulation.py
 tests/test_fis.py
+tests/test_lock.py
+tests/test_output.py
 tests/test_single_vessel_with_pre-conversion.py
 tests/test_single_vessel_without_pre-conversion.py
 tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py
 tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py
 tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py
 tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py
 tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py
```

### Comparing `opentnsim-1.3.4/setup.cfg` & `opentnsim-1.3.6/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 [options.extras_require]
 testing = 
 	geopandas
 	pytest
 	pytest-cov
 	pytest-timeout
+	sphinx
 
 [options.entry_points]
 
 [tool:pytest]
 addopts = 
 	--cov --cov-report term-missing --cov-report html
 	--verbose
```

### Comparing `opentnsim-1.3.4/setup.py` & `opentnsim-1.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     "Flask>=1.0",
     "Flask-cors",
     "sphinx_rtd_theme",
     "Dill",
     # deprecate old functions
     "Deprecated",
     "tqdm",
+    "xarray",
 ]
 
 setup_requirements = [
     "pytest-runner",
 ]
 
 tests_require = [
@@ -71,18 +72,19 @@
     "geopandas",
     "momepy",
     "folium",
     "colorcet",
     "notebook==6.4",
     "nbconvert==6.4",
     "jupyter",
-    "jupyter-book==0.13.1",
+    "jupyter-book",
     "ipywidgets==7.7",
     "jsonschema==3.0",
     "jupyterlab_widgets==3",
+    "sphinx",
 ]
 
 with open("README.md", "r") as des:
     long_description = des.read()
 
 setup(
     author="Mark van Koningsveld",
@@ -107,10 +109,10 @@
     name="opentnsim",
     packages=find_packages(include=["opentnsim"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=tests_require,
     extras_require={"testing": tests_require},
     url="https://github.com/TUDelft-CITG/OpenTNSim",
-    version="1.3.4",
+    version="1.3.6",
     zip_safe=False,
 )
```

### Comparing `opentnsim-1.3.4/tests/data/ect-bctn.json` & `opentnsim-1.3.6/tests/data/ect-bctn.json`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_limiting_depth.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_limiting_depth.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_limiting_depth_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_limiting_depth_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_uniform_depth.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_uniform_depth.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_uniform_depth_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_uniform_depth_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_varying_depth.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_varying_depth.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_varying_depth_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_power2v_varying_depth_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_resistance_components.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_resistance_components.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_resistance_components_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_resistance_components_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_squat.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_squat.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_total_power.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_total_power.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv` & `opentnsim-1.3.6/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_Van_Dorsser_et_al_2020_draught_payload.py` & `opentnsim-1.3.6/tests/test_Van_Dorsser_et_al_2020_draught_payload.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_basic_simulation.py` & `opentnsim-1.3.6/tests/test_basic_simulation.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_single_vessel_with_pre-conversion.py` & `opentnsim-1.3.6/tests/test_single_vessel_with_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_single_vessel_without_pre-conversion.py` & `opentnsim-1.3.6/tests/test_single_vessel_without_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py` & `opentnsim-1.3.6/tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py` & `opentnsim-1.3.6/tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py` & `opentnsim-1.3.6/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py` & `opentnsim-1.3.6/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py` & `opentnsim-1.3.6/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_without_pre-conversion.py` & `opentnsim-1.3.6/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_without_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/test_utils.py` & `opentnsim-1.3.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/utils.py` & `opentnsim-1.3.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.3.4/tests/vessels/vessels.csv` & `opentnsim-1.3.6/tests/vessels/vessels.csv`

 * *Files identical despite different names*

